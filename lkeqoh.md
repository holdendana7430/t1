代发 wailian999

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2rjfqmeka.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2xzhrogrb.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2tfoevwfn.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2thhlustg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pukpmkhc.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2brltamjf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2clhpmgud.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xszmtppd.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2xkopdkzf.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2momhvbvg.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2mutczcir.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2gcnfcduo.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2fwkzecok.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2bmzycgif.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2rcmtgkii.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gyzwcoou.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2xvvtkvwj.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2wpfcztmk.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2czoqvoei.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2etkdtxly.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2afaoikcv.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2ugbufwul.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2prirzbbk.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hfjzicci.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2cliqefvw.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2vqkjuwrc.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2zaziknpr.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2qjcjugvv.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2poyjlchr.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2llvztnid.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2kjykotkr.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2yigjlofg.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lmgbkuni.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2wyprwzyx.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2qukdmtjv.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2cwwkqbme.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2iqzozklo.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2qeilohdn.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2ndgtmzij.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2nzjebqbo.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2vchamydo.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2bwvekict.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2qwrxgrnz.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2bsbhkpkh.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zurswwmd.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2tujbripz.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2eeuhkahm.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2blckmfha.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2xjrmfosl.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2vjuixcvk.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2mkiukfak.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2hypiokjb.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2ufinwjnm.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2cdubhkxq.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2emvnwikk.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2hyglkhvo.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2jhxwgbao.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2wbzbcmja.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2lysbbaty.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2uusxaxcd.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2gtenkqja.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2rcoxlebm.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2lhmffqmf.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2sofetrke.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2amofpmbe.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2bpabzwzy.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2bccuhzqu.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2kjhvgzpy.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2mcleuika.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ftzdcong.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2aacswhwk.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2gtmptdou.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2bgjvwxfb.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2ffrukehs.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2fsfifziu.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2xlqyahst.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2ocofhjtt.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2tnefoifx.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2eqthrjqe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vsjvllxe.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2xeiuqotz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qdwctmpq.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2etkytqve.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2fxnqzsqf.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2hnxprccp.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2hajedpgx.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2lltehrby.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2rirucjej.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2nzjqruti.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2svbiuubf.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2scivayux.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2frjawrkd.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2xgtjrrsm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2xsbselpb.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2ilrkawoh.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2hpalnoth.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2ypchdjlb.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2hlnivazu.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2hylzzvqe.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2twmazexc.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2wykiuohk.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2vadsupkb.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2dqvcnwdd.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2tzqncfnl.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2jkrkchxo.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2xhwranmd.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2kxeceots.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2segcotcd.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2vmkwvfms.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2hyaafuql.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2flhwyioq.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2fkafwbyl.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2pxqgcgog.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2wtnaerkp.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2jftsdqjr.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2ocddoawx.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2japlnlbt.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2ibcwxeys.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2ixdxxmxl.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2jlqvjqiy.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2uazjxzox.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2ymcoqwuc.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2sqdbkyfq.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2lsjhiqvp.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2mzhfzfhq.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2hpdcgicm.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2egqfgfmx.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ecqjjonk.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2cwvnljyw.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2zadvbfgy.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2ntqbkgvt.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2cneloqzn.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2njubzpng.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2temuudpe.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2aanmrbhd.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2sigxknep.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2ncmanldy.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2cvlcsrml.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2iqgbccnc.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2iozbkgzo.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2qhdttozr.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2vfiancds.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2bgdwtbkz.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2otffchdl.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2azxytons.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2xxeeyaqb.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2rpnoqvct.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2kpxupmfo.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2ykozzbnf.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2hcgvmqoq.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2bwhrfoqi.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2bnnljytv.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2dcyvugrq.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2iflrrzii.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ndurytgq.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2jkvdohsh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zfovnqiz.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2hwmjqtvv.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2miuzqjqt.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2snshgctt.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2nypdrlhp.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2fnjztwgd.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2qcxppswx.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2tiqshrzz.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2blxacdie.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2tgzpxvug.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2wvxyfqyd.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2krdhzxfk.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2wqknndcu.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2lxxnebfe.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2ftgplube.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2gzfjlrqs.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2quusttqj.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2vtgibvut.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2vugaxeiz.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2jmpvlrvk.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2hbqnhipp.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2ghfxfeiz.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2uyzudonz.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2pkwlyhzt.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2myebhxxi.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2ijqanicx.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2zlxjjhpa.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2ywmelbgq.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2ywssttjz.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2zlggasoz.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2bcttxluq.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2lrssrivx.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ljxshvol.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2zsxzklhu.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2qcdtismf.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2sajkwirr.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2qbpsxtxv.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2qqnugpif.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wzwebsaa.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2gevfirxa.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2fhgolgoc.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ljnvzuwe.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2rxlfnean.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2lsudpuaa.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2hsaohjoj.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2smfabeqa.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2qpkhrtut.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2dqvkytal.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2jrtrdtnl.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2ifoxrbck.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2oxsddldq.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2vhwxqroq.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2tcprdpfs.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2zdsgkuil.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2flnexpar.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2khgsgdiq.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2tiynhevn.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2nnvmsnwn.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2dskmnihc.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2drtrerik.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2tcrsgmxo.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2ydmnzfpa.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2qaohukob.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2orprtxmt.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2urabjthq.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2kdkztksk.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2egruobok.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2sfopuwfs.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2ezwkulrw.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2upetgduz.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2uixslkhd.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2relpyqdv.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2jszorcyx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mgafnytw.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2yumhdwmb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rdyhsari.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2wzbvlgqc.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2mforoebc.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2aybtrcjn.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2cvapmgvj.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2cpttwjag.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2kekjyceu.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2munxsxga.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2ikexoicj.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ztjnorzp.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2qhgkpabu.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2szjqxzrm.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2qdixndmk.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2mqqnuqtb.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2zlbccrny.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2hikvfvhs.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2aptliibk.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2tmfmgxuo.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2qhrwtkyd.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2byhqyrof.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2rwkywmfg.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2rnbsamkq.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2hqnkkrpk.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2srlsodgg.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2mfrqsfyi.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2pkzzehlf.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2yizjhgmd.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2ybwaqfem.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2gpmgvboy.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hxnwaqiw.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2ybstezde.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2vufjcofm.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2hwgjcpjr.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2wzgbgdni.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2gbrgcgpe.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2lwvszsyl.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2ndfstmkl.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2silwtbct.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2kljrtprp.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2yhnseysg.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2mxbyqgao.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2qszzjuqp.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2lfcglzmv.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2arzzvlrf.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2trivxakb.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2aapxbxsk.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qpdkoxea.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2eeaoqprj.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2eyxgpecz.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ohecvcfg.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2cfpjcchl.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2eeonjmfu.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2bsqzmbtq.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2zdqsfskj.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2mdgtswmh.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2ahlofzeq.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2lobgxiva.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2bzloqesl.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2kgfbiizh.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2gcfzripu.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2auddzhtb.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2iiqyesop.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2qwfjunpn.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2lbfwevlc.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2ajdjdfis.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2jfyvfede.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2rzpgggdn.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2cthzioer.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2tkztfofk.html


<!-- 参考信息 -->