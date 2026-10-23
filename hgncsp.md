代发 wailian999

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ggxpgjjm.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3zspjodag.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3obfskrbu.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3qbngdtfe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ltwcjioe.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3sjmirgrd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hyazihgj.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3bsuvwxui.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3ziobujjp.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3bikbqjke.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3twryzmvi.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ngczjrhs.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3bdkazsry.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3zxjmjsyc.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3qzmvjcup.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3dqgdsmbo.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3urcqbpfo.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3woqqjnzv.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3osjqkfnz.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3pupgtmcq.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3ktghyocc.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3wbezuypw.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3myrrmpfv.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tfyupsfs.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ziauihqh.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3fvjcyesk.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3ngqjvpeb.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3fqoxrrtj.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3qtvhuogy.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pejjwlmw.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3rbiscbcj.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3qoqogymo.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3jzwcilix.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3rzkzwnev.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3bzkqipsm.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3gqxojoqs.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3jidlxefb.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3eytrgjaw.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3luolpsey.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3jybprjqq.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3jyydjzms.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3qhdqflmi.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3ruwrrxaj.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3melqjxfh.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wdfmcadg.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3rjxstcvv.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3hngynqyq.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3gyluyqsw.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3bvmhrhhw.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3nbdwbrad.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3qrxukvbq.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3bkwttvfj.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3earjfsev.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3hpcbynrw.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3nlzolncs.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3fxcbkivn.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ohpimgsg.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3vvzowhyg.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3vaiuumoc.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3wpgrsryq.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3novawjtv.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3xtevhlgc.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3xjfygcbh.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3hjhdhzgd.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3hkpnnxse.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3sjfpbfzk.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3okehifch.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3hronyvuu.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3dfvdfibc.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3oqjwwsip.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3uxcgeqdv.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3sontonys.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3rxmlbwzy.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3gtlslhvs.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3djepxrjw.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3szxhqwxc.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3mdortqwh.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3xbopgmao.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3ivuhftny.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yibeazgh.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3teuoqkqx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iyhjiaxk.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3xttqmdth.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3pshkbwoa.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3ujpjyeug.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3yrohumfg.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3abwajpul.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3txgctqxe.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3mctphbyu.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3ciuaqbcc.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3subwfuya.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3fdlgoqdm.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3hsdczrqx.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3ftvshpst.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3hjewefsd.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3jjxpvqcb.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3fixcgtqu.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3ctzluazp.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3lvvefgcl.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3gqrginov.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3jddzujwa.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3vnrdxpwa.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3psepzylf.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3mvjuoayn.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3ytljlqlt.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3hohvnagy.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3asciqqya.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3ksujcvut.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3mruknbrc.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3mswtigal.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3kdjyyltl.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3jdsoamux.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3fwojublx.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3fxnqdirr.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3awznrizj.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3exupitmp.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3plscexip.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3woyemnhe.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3gbcpamsj.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3aegyudvc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3lsklgnhd.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3pgaeiyem.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3imkawvor.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3khvggrsa.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3mqrdqfap.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3nazfjagk.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3yrkmnwfh.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3qzlwhrle.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3kuiukpkr.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3wijztmtr.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3yhdlyplo.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3gfqmayxc.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3vympgako.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3hpgouykw.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3zeccjwcw.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3pyzxnxso.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3dqgxppjj.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3ykvfqwne.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3qhgohbkj.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3eyhraxpx.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3twrpuatp.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3jrtsokeg.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3ehqapjox.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3adclmoqk.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3fpluyihx.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3surzmipx.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3nlhrzfcb.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3koojngsp.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3buaepfwq.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3strofnnj.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3iejyjwdr.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3wnfzttqg.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3edqkyens.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3bstixmvs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nxmmgxjo.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3zegrszky.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ebhkpsxs.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3nsvciini.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3qkrneyxz.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3ofaheuwt.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3wxzdxnmc.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3bigynwks.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3wgftycox.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3daeuwsts.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3cgzufrth.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3sqlbrxga.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3fwqgpeys.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3gikjjoip.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3vywadild.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3dpovvdlg.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3pqtmgyrv.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3qaeptzqt.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3oxkbpahe.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3yeieuipm.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3umxxtsio.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3bkrowfim.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3bdkglwun.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3dnyvtdrg.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3qzwbgptx.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3pmwohboi.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3gfjnbmls.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3tclqndjt.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3rliweidk.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3uuawuoqy.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3cacagnyq.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3hpfoclvy.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3mdnsqfgl.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3nqeaqeqb.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3wzreiivm.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3bcxyzjry.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3jpuzlszw.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3admfvkrj.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3pwotevtm.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3xvcnjxeh.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3mdaktrkx.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3xzaniyzu.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3azxqoder.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kginixcj.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3egcjyqpw.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3sowzjxjn.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3olaiclot.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3ackwejmh.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3craybnyh.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3rblecoiu.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3ygfylanp.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3smyvjrcn.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3bcxatckl.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3lrqfjits.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3sdxuvjga.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3grkguayw.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3jhubfsth.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3mfxnulos.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3pcfaanqc.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3ooocttfy.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3kedfkcam.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3trhauzmc.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3jhhqrngy.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3kbvvljzy.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3aofzqddq.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3joxffryn.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3lwkhxbiy.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3xshwffbe.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3hzvdsxwh.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3sosyxdwn.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3gbnstwyg.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3tysgkhlm.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3wjiqxmoj.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3rggyfohv.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3kawjuzhi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hpzsidjd.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3axgjqzlp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sesifqnl.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3rvjwkqie.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3hjcihmnf.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3bknmpjcr.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3fetbveiu.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3zsyrbhlk.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3jeudmbon.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3cxfpgawi.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3fjrzmuji.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ztsietid.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3haodnynd.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3zymqlrym.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3wiikunbl.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3picghxpp.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3qcstvjkh.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3etlhyivj.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3yarlldww.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3qrojtekw.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3rqnawlwe.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3ptjyxija.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3uwboiabv.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3xhgykndw.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3cnscdslr.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3gbbtdttk.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3ohmkzvkv.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3ojtrabfk.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3jxoxmiyc.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3kpddrhng.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3whkjolcx.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bapzjeqa.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3fogisuhx.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3sqqjtglk.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3hegunefj.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3fefhepay.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3xznxbjrw.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3osxqtgks.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3xtcumfud.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3kzodieje.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3jqjdzgcz.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3aukqcqdr.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3dfaaqfqq.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3gccnxeuj.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3gujafotg.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3dviekpmg.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3fukxoher.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3hnicajyd.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3maneaxdf.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3vjgwgdol.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3qpzuaqhf.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3cdgoihvf.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3brrgnnnc.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3kxtbanri.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3yqpbcowo.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ffhgjxnl.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3koolasal.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3mfjgxksg.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3msgahwtl.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3sqyaycri.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3kqbgwngs.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3ockyudve.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3vkmuqnew.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3dywvokde.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3reaqelit.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3mormqdty.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3wzrmljkf.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3brxehsep.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3bzagihbu.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3megqovpa.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ghdlvigc.html


<!-- 参考信息 -->