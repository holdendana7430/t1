代发 wailian999

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2voiaxnfo.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2slczuajk.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2rohlxgaz.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2ldehbcyk.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ltpirvbo.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2xwogtkhm.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2aqdoeduc.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2tdrpgsws.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2leyqcjbd.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2pklcfdsa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hcvpnhmc.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2iakkkqvk.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2rprbhjib.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2ihsouexr.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2bcfzrjhn.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2kmjoflck.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2qrakcutn.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2mckdadzg.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2kyeqbpxy.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2krzzzlwt.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2frzrcrja.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2iiayndum.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2pltxkfbh.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2aljgzouj.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ojelqzfr.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2wshtelll.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2uhlakauo.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kkrdisvu.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2clnntgml.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2yuzulefy.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2roikpwke.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2ppqzpiix.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2oaodrcpg.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2dglmsuuw.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2tmbfmhpz.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2ofjcwrym.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gllnzzte.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2auiaqyxf.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2hqmcvekz.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2ozscwcwi.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2druwhcrc.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2mezocyvg.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2qefmxkcg.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2pvibgxaa.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2furshqjo.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2jhkwakkn.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2zrdxzbvr.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2etrlwzhp.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lbwnybyg.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2cmydopnw.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2phfmppag.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2xxrovaoc.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2zkezwhzz.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2sayojmsv.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2pvvnfnid.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2dxqtrlyu.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2qqbnshyc.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2fywhuoxg.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2fnszufio.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2lnfluzga.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2ulqfqgwn.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2okkabeep.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2gkphgfll.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2xuvqrvgn.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2hzgihkjo.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2oovskuuy.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2zfhynyjp.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2qrowslbf.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2altebkxw.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2gcwkujpa.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2tgigrxal.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2pqnqruxx.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2lxnkrqsc.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2lmxlevtb.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2cdtbfkyu.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2bugibhwt.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2upsrmekf.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2vkllmrzv.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2uppptddt.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2jnvzorpj.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2gokfcqzs.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2bjjmfadh.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2afmwjbat.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hpvdsaug.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2swuznurq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gllsifwj.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2hrwlklis.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2jbpoools.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2ikvaglzs.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2sympbzat.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2foxorcuh.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2euwpeymm.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2szeqdxxn.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2junzspaz.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2xdapcfpv.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2masyukjo.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2sftqzfgy.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2jqnjnuow.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2xelnjcnm.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2tkaqbcha.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2nwvuucaj.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2yeviudlj.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2phumnqxq.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2vrphquxm.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2jxkvlahi.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2ttcmuece.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2zguhltoa.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2oqzhrvhk.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2ktwqllrd.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2ipotiygm.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2qbgkibyl.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2vrqfuaic.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2sionyqcv.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2qlyqmtpy.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2weljfmrn.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2nhigzvku.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2ghzrqkxe.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2waijfctc.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2hnyharku.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2zpjwhnvo.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2afwwhiwh.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2vammwmhb.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2juketrie.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2heylyyms.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2hmbgpjue.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2kwvwvkmh.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2ndlmqnpf.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2execgxvp.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2xbidkbzj.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2rngcyznr.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xtohwija.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2zhkrnszq.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2dhadcfhb.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2lgcmmsam.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2ybftbbpi.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2nftroxdl.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2esgmacel.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2ohohjzwb.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2xfrkykto.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2dcnaewro.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2jczinaxk.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2qezhnoyq.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2ibeuerzc.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2rlgpqgxs.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2wkmcyjlj.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2htnvcqkt.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2gnnsmkvr.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2arbfuwjl.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2khsuttzz.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2nkqkjllh.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2nppdzzjf.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2zlgbsigs.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2pdqemvde.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2wxkrctyz.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2csgsdwse.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2pubsxpsq.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2fdcmkitr.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2zgymxyhk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ddgmwhxv.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2rlgbqwsq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yjgbjbvs.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2yxcuyfpn.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2lofsaluv.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2elbcalxv.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2xlgmnjiq.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2nicikchb.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2ehiybpmt.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2ksmbyhtc.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2kngxlnsd.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2ybfvmixi.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2gfhtzqls.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2suniqjnv.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2ggcqlkhh.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2iuxjdhzj.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2uqxrxmbu.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2lhcrexbz.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2lolcbkjq.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2txxffwct.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2hzvgsymg.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2ypoapfop.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2zfqzncpx.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2dyozpyot.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2dyfkcyzl.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2efdtetqm.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2pstdraju.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2bkgxodow.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2qvlfjblo.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2twgmysmz.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2jpmpbvbi.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2vugpftum.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2cojxsiur.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2pkylcwnx.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2bdhjhgym.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2ekcnomnm.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2qopvgwic.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2azjhvkha.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2hijwwoso.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2vakgeczs.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2pttktrmh.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2uopnsdhj.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2hcbyloam.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2kswubyof.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kbxhorks.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2dnvvenir.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2sfnptpsc.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2yvxwwrnn.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2wofnvtti.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2dcnhmxsj.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2eiwqdtqj.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2gacxygkx.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2zhbtecpb.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2xiohmbqf.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2czbugcux.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2fwijqjtb.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2svjneowy.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2etuouvnq.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2qzgnmbbe.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2juoutuqd.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2lxvdtyby.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2dbhxnwel.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2idchvome.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2baagmhoj.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2cyqdsjqe.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2qgoaslpf.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2ivsxmxpo.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2wsjvvsje.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2splqrqgm.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2kescnymi.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2jzxmvwbt.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2dopziffm.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2msmyeuaz.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2meokjmyz.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2bwmmwwqp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lpixpcqf.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2pyucxceo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zproxkct.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2gvaypzty.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2xmfnbnow.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2qivnewiu.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2gdsohnxm.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2uiubveef.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ikuwbxff.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2hgvyormn.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2mrjaisbr.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2fjwpqtjk.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2cgxptcjv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2kduckbgh.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2wdlwodua.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2gojqmuiq.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2mqtgpfpy.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2bjowzjvb.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2bawrizgi.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2xrootkhk.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2varygurl.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2cnnpbsny.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2ttybybam.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2dnnpjddo.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2pjcuozcn.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2sneddhwh.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2misbuhhu.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2jhqabfos.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2njojgluk.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2qzaxbktf.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2qcjsiyed.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2cibthxvc.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2mzaxigjy.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2tcwjipsi.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2bnxjucpp.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2faooyjic.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2gjotdhhh.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2xomhjsjo.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2dmadynpk.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2bzziaxsl.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2jgapayva.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2fdflljun.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2hsdddulx.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2bbhdwqwj.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2wjlzitsz.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2inrhldbu.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2nsyfirmx.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2wsrkdabi.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2zcastpua.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2uizlwlhh.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2ehijbktv.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2uehltuho.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2tnmkjxbg.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2ecduvusx.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2wutvkicu.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2zvxgshcq.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2gigobhyu.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2urfczvva.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2cuflazwp.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2ewrntkzv.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2jcmrkxcr.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2jclpzumq.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2bbhyfzpn.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2kebmjomk.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2ubdfthnj.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2wivgmiyu.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2mzdhvyvt.html


<!-- 参考信息 -->