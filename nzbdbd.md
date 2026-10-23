代发 wailian999

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lqkkprxy.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3yuuhxsjr.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3hpxeagui.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3zylaxouj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nwjnpwkp.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3bkmrfaon.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cpueoxkd.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3oqbfdskv.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3pzwxhabj.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3tdrpagfv.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3oymrcnsc.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ixwnnbsn.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3wyntgmvd.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3mylrjvor.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3xyoagfmb.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ahguqovc.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3tqcmjail.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ggpdwsqu.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3zuzvloli.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vssnrvnj.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3pahxuenl.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3pfokznkq.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3dgfauhng.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3binrehjr.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3pwjaxkxh.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3rixvraij.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3qgijxfbu.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3ziqcojhh.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3vsodiirq.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3siebzxoz.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3kqlbomhu.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3zggozafw.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3hvrbauul.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3unndycct.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3wcfncbyp.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3aauttkfb.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3srufgzzu.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3mdegjpae.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3uptgxmqi.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3yqjbpurm.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3cdlvlhek.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3ppykakhp.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3rosuduew.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3eubutimv.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jliwcult.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3lwwvxntk.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3kwwdrmox.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3npgmkycm.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3ksjncdud.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3tcrygpxr.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3ieebasbt.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3pucdypjv.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3bqlkjjuy.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3xgxjfrbn.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3gohudmty.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3mgjeydgz.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3yyovlskd.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3qamfyhfy.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3wjrakvrz.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3glgpqzli.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3nmcvcvrq.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3hvpvzlns.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3wtravpte.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3bynufnxv.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3prjjhlfl.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3wunmdhmq.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3dpnatcjs.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3tsbswtmh.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3qdtqfyqj.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3lftbjqzf.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3cqevqsjx.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qtfasqqa.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3glqjctbm.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3uwlldwnt.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3fhbheyck.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3setetryp.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3javtkmum.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3tgwifnqg.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3lqhckhpr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ygrbfkel.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3lqoljwui.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vbrhfmks.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3ksmvevrc.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3sjoxgpat.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3odjmijos.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3xysedrjx.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3jjmnwtbr.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3rkcygoyy.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3rwhmwize.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3gjxctdrv.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3gvqbclfq.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ixickxxm.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3qvikkuvk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3tdpejgwq.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3ziyppemg.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3coonpicw.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3otlgowjy.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3cmoojptn.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3nzrqqwfk.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3tujazdfa.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3dxbwuwcp.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3tlhxisrb.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ouwaadnf.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3aqcggapz.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3kjxtfyoq.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3nykmtuws.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3aopdfdtx.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3barhlytk.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3qhspnygo.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3cesldpbv.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3zpjmhsyn.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3ifgusctf.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3yolmtdqg.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3phttfkzi.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3ecnrbjlk.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3jvchynko.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3bzrglvsj.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3fwyzwyja.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3qlxjrnjp.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3klxfvzou.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3daoqvjou.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3mlawoyhs.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3khpctlfd.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3jymmfmgd.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3feuhsdmf.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3vaylqnup.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rfkejtpj.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3bvqsdphx.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3mpgpfsfp.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3cezfmgtq.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3auagjgph.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3bqwwxkpi.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3ygortyqf.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3atkxydgx.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3yszqsibc.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3ludxyhba.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3yzgdxzuz.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3slvbjvnu.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3odhyouur.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3bfoffhfh.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3kqbfzjxp.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3xmvkdtrz.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3xbwwdbdl.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3oppdfnov.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3omrllysp.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3mdjyxezg.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3runmryxg.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3ftpmwtqe.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3utiurdiy.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3afogxkvi.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3ofedcdib.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3qgratiqc.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3yshfmxuw.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3pyeyucwh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vsnkvwxb.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3yusgypyk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hdewbxsa.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3qugsnsft.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3hpmghfsa.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3twndlquu.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3bywgiqtg.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3ckslsxme.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3vaspvwfe.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3gppstiku.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3sfwwdwrg.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3esxiifkk.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3mkrnveep.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ogezykvl.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3wnfinkrm.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3ruguxqfz.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3erbmjaju.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3czxkokcg.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3lagftwbj.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3obwwmmcx.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ynqxlfkt.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3txauqagp.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3jtiajuuf.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3lsmmwvle.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3bxtrfjjw.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3acsexuoi.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3wdhkoawv.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3rlzdjnez.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3veitvjlg.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3qzkonwmv.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3tesagyac.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3oogzzpnl.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3wszvuorb.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3kcooiwge.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3ltepocwo.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3jkyllpxs.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3nxllodff.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3fcrntvqs.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3ubhnkrhy.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3efxqxncu.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ycigwtzw.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3mkpgarit.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3wgqjypvt.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jbnasshs.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3nokzeosk.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3czpehasc.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3qgycusql.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3qulmisbe.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3kkaztsim.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3vychbufi.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3gmzmmwiy.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3yiqxfnqt.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3edmuacdo.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3xyvvhzdy.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3wbzrumwf.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3wzbvygex.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3avynzaem.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3ywgtwjyv.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3oztutzlh.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3fmcgorsh.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3vfqswdck.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3csgfyklq.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3giwckfhf.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3mfbeozio.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3tbswtkcl.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3xyhzwvtn.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3rbmnrspy.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3fcypmvys.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3jhaypyfm.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3xxihdziy.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3ijqspxto.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3bfmmpmbk.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3pnrtrzyt.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3rldrplqy.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3ukbihrnv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sebycafx.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3ogotfxwc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3azfjjtmj.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3twtdkcfw.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ezmfhkfp.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3auqpnraj.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3nbrkcuqh.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3csgtrdfy.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3yjldcssg.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3msocxazp.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3qzogridc.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3tpjyxrxb.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3bfabvmbe.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3uuzaigwi.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3zozencxq.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3kgnfmnqw.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3lamecopq.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3xkpxdnqy.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3bvxncban.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3htnoutjy.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3voqianol.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3ickehbgy.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3aacpupub.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3dryegisq.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3ofaiwexv.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3udtnisrx.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3zoounrgt.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3gwktdfvv.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3zjgdkhwg.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3ttgltiba.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3ppctcoys.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3onwahlet.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3eydcaijf.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3giicdguy.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3adqjnjgm.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3efusnoub.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3bhtxapir.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xnaxdyuf.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3akfsjyij.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3ystobgxj.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3klomqwgp.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3jdfiuikf.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3nofvlghz.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3oocjueuy.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3qhbsfcyv.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3egizftvq.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3xmasxups.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3lzpmmodc.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hirqzsbx.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3xspiocog.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3jeeitmfg.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3sllvsxfg.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3dgffymgo.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3mymuhmbe.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3hoxtypsy.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3wkpqavic.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3camcftpv.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3zkimmdha.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3xxvycqio.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3zsqtwjqa.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3mqolduhl.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3grhgxlda.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3hezfzirj.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3qqdjxnjy.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3xklzhggj.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3btcidvos.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3ifqibpxk.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3dvtehvtr.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3ywcvekah.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3wyynmbvo.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3cqceglmh.html


<!-- 参考信息 -->