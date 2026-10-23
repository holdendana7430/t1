代发 wailian999

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3itckrdps.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3pmygwwee.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ewwxbwtx.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3jlmbbcoe.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3wibllkgo.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3xbueoauv.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3sevujkdx.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wcnveuwf.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3yaffjepa.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3smxfpttm.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3hbmewetb.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3qjsjimia.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3bkptqglo.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3vkccnitr.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3qksfjfkb.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3wuvrbvcq.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xlekfcao.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3vhtmdkpl.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3qyuqvake.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3bznveeer.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lerbduyj.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3hawbsbwu.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3oejhzsth.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3utzjfpbg.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3wvohanzq.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3ecokrckq.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3rduswqfx.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3esrbrfrt.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3gygomfpi.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3mqsdqbrl.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3otdgsoko.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3zlhbcsva.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3dtjxgtle.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3pmgjupyp.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3iektbcfq.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3tlbbomla.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qnrkpmyv.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3qjexbqyg.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3tmhovnte.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ereojfis.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3arolrsam.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3konxejrj.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3ugiihcxr.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3eygkokik.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3pmffvdob.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3wuwcainy.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3penqzveo.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ifghbmhp.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3gymkoqzp.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3zhhaslzr.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3ffgfrtew.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3bhzmbovo.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3zebphuwt.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3yizosqku.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3hmihnjav.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3zaldwslq.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3lcyfmlla.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3lfhnpexz.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3iixpnbfw.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3qyeugnar.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3zmxpatri.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3wtfekwrq.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3iztmayoe.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3bxxdocqi.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3dmhmreyo.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3crhwqebv.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3afvywqdg.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3jcixbstm.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3ctpxgdgp.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ewsnltii.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3dkndycme.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fvbdfllm.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3xdxzgeja.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eyvxrwcy.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3pqhdwsyh.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3gbatbpat.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3ljemvcwy.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3jactbfob.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3uxanpsic.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3fwieueyc.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3zvhxulqj.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3jjfvvjja.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3wfoveuoy.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3ceoqdemz.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3xaqaipnu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3rouzxyhe.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3nwaqnjqz.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3lamivgsh.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3zlhfvspq.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3vpsnckpm.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3rmdscvtf.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3hckydlkf.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3vtesixjm.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3ryfpmfpi.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3crrxjqqy.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3uzmqehda.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3ofdytxud.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3ciwavjfj.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3pfhmckvn.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3lgyzoinj.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3lhsjofew.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3ahkbdyyc.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3lbnuolth.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3xixbwoqo.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3sdzjgwgd.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3qjbotdbj.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3rvkjloct.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3ssixoitu.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3szvpkuki.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3tnmwugmi.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3bovllimk.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3skqulosi.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3yqhgvcwf.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3mprqspkz.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3outvlgbl.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3gqvgdgal.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3edgavkln.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3zwrkrzyy.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ftdnnmcg.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3ramhcxut.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3xfhhgytd.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3hxrjyrdw.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3hebnolti.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3jejopkeu.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3ctptvhwg.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3ajqianxe.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3zpkeqjff.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3jrkexaxq.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3pqvedadn.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3ghqmqoai.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3jrerxhrc.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3lwlvhpmj.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3xxtsyknr.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3cittsfsq.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3mcyrmqhk.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3yznpdzer.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3nhkyzpif.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3hkvdqqhb.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3pysnjqna.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3vdxjnqez.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3ziiahhfu.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3hizlgqyx.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3rdlaaotn.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3miqjggpo.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3twhpbizp.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3imifavuh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vaaxhvde.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3lqqkqouz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nlswfkvh.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3fgklkauw.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3zdzdaxut.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3yqpvcbow.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3dbnioamy.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3aycxceeg.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3fgnedqbk.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3aqeegqsw.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3hwttpsll.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3gwpvvuwq.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3vskefbwb.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3vhuylsth.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3zvuusxay.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3mdumazql.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3enlljkrt.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3eyyqwswf.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3nwjxkdxm.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3ldqmynlg.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3fyvuswgd.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3sejzwcsm.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3rvegtokc.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3mnpakkxf.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3gfxfgrvu.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3redngeyh.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3tmtgyvgs.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3rhkfrjdd.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3kiootcoq.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3rhatxmnx.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3bzuklpar.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3tvlasnph.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3mtsypjsa.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3tsezatnp.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ozgzhhed.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3dgnkcmju.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3isxczehy.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3lwjictig.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3yjymdhhq.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3dcwbgyxm.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ubrrdxlf.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3onelzqat.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ssggwhan.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3hqmwuunv.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jnecmbbe.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kbnqxtlv.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3jtnxwnyd.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3zihxdudg.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3pkhknpjn.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3tfcahmun.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3lbikzlwt.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3ljbgpjob.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3ohzrvmkl.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3gbabdmct.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3xdptrrmt.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3njzcbaus.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3zgtarbxy.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3fbsmysqo.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3ldffojpd.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3czndwerj.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3tteigwyo.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3bpimldmv.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3xbtgdcvc.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3ywvnwpjm.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3yvgoauzu.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3tkvnwjtp.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3bgdayeea.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3mpcgbjsf.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3drdnbelw.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3szexkgsy.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3svtvgevp.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3tubrvyfi.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3mbzwrwfe.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3cuggjyhz.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3jtshzvhy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xyoinipq.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3gkulxndf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3guqnxgbz.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3fnonrxud.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3kcnsnlhu.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3fhqcpgih.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3inzifqwv.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3grddnfmn.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3yylqnnxf.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3kfwzqajo.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3eylsedbb.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3kogajpuz.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3adsdzrtf.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3payuocyf.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3hfhfasqv.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3vaxvyrur.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3vmlufbwh.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3eipqquue.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pobsgfyz.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3xrcuztxb.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3qrhtjmmp.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3zgbfqjjq.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3yknzbmsh.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3szrewgiu.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3bdfrbemy.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3avgjoicc.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3dfpwfnbk.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3obyjygoo.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3dzvdlylz.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3furmlgxu.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3amoaxedd.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3phowictb.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3lpzbeawr.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3pavgpbwf.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3rdguqzmq.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3hxzomlib.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3uxzzktzb.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3pjfgrjhm.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jcxvvrbn.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3ikzxhhkh.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3tjvadsfx.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3wxecgxsr.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3qrscwvsc.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3wezkviiw.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3ulwyideh.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3ielxslka.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3ramiefeb.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3baervjek.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3vxhdozhy.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3pgcovesg.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3iycaiizv.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3nencfvej.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3yldxanwx.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3nokeizjl.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3zupocyby.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3crbuuedy.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3xsyyqhea.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3jefhkdwr.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3lcikkiau.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3iqlsxhrm.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3zfdgwppw.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3fbstjygi.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3lzeobjbr.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3pcxqobmx.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3svzxlbjc.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3qfmcujmh.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3torpaqat.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vzjuluoz.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3imsexjbe.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3psdlahrj.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3deavxien.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3txzeulpo.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3wfcuqoel.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3nuluqqku.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3evjnsmhi.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3mfdhuvhi.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3biswwxpb.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3fszivire.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3qjguamyn.html


<!-- 参考信息 -->