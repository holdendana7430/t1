代发 wailian999

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sgsvaahm.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3amzrdapb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vrgquzte.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3mrtwpsce.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3oswsarhk.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3thgzlnep.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3jximyyxu.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3xpmbhnjj.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3mnrimlck.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3hengsptl.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3odtssjjp.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3dhenvsns.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3hpmfspia.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wrhugorq.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3deckiwhg.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3llkhifpk.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3wpmxghtw.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3dycbvflt.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3gzlqkbnq.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qzgpmcfa.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wntgahmt.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3pgpxmemc.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3oikffcqy.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3schirwcl.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vatecanp.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ynhoodpg.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3zghquwcy.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3aiitbcdv.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3hcxgndzr.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3dvedydsr.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3qtnrzjjz.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3hwxqemra.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3lxbupuzb.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3icyukila.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3pzlftpbn.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3xefolmnm.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3fzcdugjb.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3llywuzjh.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3jvlkmdul.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3gcquqtyt.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3bhttkbcl.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3zoxncjte.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3oqsffsxl.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3fkqoufud.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3xjcmeuta.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3dwvzngmo.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3ojvkywwm.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3cmiuhxpu.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3rnolpxqq.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3omxafdut.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3hzgjpvqe.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3rmwjczbv.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3ubathefe.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3sscypgcl.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3iosqzzcg.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3tlhxvsvf.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3ifgjgrxa.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3xkbxsvwc.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3nsvgprqj.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3cfoebjxy.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3dznmopik.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3lwksiiil.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ljtbzxmz.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3eoswbwsg.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3clldynjm.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3phkkuleq.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3ooenzjtg.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3gpilingz.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3rnhfhiil.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3gmifheyt.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3ozknzaft.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3juevsqjq.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3bqlvnwkq.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ppsijfvr.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3kuukgmgf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xkjisrgb.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3odwigslv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3krtjwwzf.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3fyqmefqz.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3uyujsoor.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3epgejkrs.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3gkmsgjbf.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3aqfvewws.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3mahnlirm.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3kxpyquda.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3uusxqytk.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3qkmuxaqy.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3qumoigxz.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3ifgfmtwy.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3xubuwybd.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3ivajtlwz.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3xcacidns.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3pohzesab.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3eqnmsjaq.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3qkgdibzl.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3dstoswry.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3votzugdn.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3nldsnqpe.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3fpcepdhw.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3uxauqpjy.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3itwpnhdz.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3lneulizi.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3mqabvhhs.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3ylephdiz.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3cruxyjfr.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3cxcbnaab.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3fadrszle.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3ygprfogc.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3ekhfaers.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3tkghcxsm.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3kyuhigml.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3gqwbdwxr.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3bbknhgev.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3qclqarak.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3pnwoycxu.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3vpqkknhy.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3tjmucpxp.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3tckdrfjl.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3xkmejdni.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3xyhgabee.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3qafusnxr.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3iqeiufyb.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3zobpwtpm.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3bxwvdfdi.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3qxnglauw.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3vaxetfsu.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3mcllzyjh.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3gsqyyrhl.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3eapowftu.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3kvhxpduc.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3uwzswezp.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3zsrlboam.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3umyqaqil.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3oiybokze.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3ialhavtz.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3zeddqgtr.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3sarfvybp.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3yrbwvmlc.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3pgajzalu.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3otzfhgxm.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3nxbyhite.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3jdvyetkn.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3ywvsiwvm.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3cdzpugri.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3pqlqzbsl.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3ibruijgx.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3lsqjrygq.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3ykwzisrp.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3mloukpvu.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3dgwtrcir.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wlaynscb.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3ujpsriwi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uyfedphi.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3ybjmxmtv.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3kowidpxd.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3aymraqcg.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3egxqonww.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3fxnkaxpo.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3yctwidpl.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3ismxmlfy.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3jddemlxa.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3uupompxc.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3fzwxwqen.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3khddngce.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3ftcynxkm.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3byedgika.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3kmknhmzb.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3iaykumgi.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3itsrkoiq.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3vlecvlty.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3rikkkuly.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3xbceftdj.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3kbmepzjd.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3igkfuust.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3flqleqee.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3onvviqds.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3nfzvaezq.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3lqecitum.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3balxbifi.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3yujwpbdt.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3mvpufbem.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3crprmrvx.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3hdkyhhyf.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3yewgznqt.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3dispohwo.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3hlmjsblc.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3fcmtjbnr.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3vpuwtvfh.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3tsjhiidi.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3nfvuozum.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jqkrmizi.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3jyfupctp.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3efyntiez.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3adkbmujw.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mbhirlds.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xztvmrwz.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3lduyyqdq.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3arxvnehm.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3zwjyvuta.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3nixxxawm.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3hsggoadx.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3eesfesap.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3wzrmkcfc.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3hnmvfdit.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3bcpiuizb.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3bhaplhml.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3pngscwqc.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3kelhrkvq.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3qsxltkrv.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3csqaojxl.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3oolgqjrr.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3vetjjkgo.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3xleisoon.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3bssyfyrj.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3keyjyfhb.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3jzinbdgs.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3hzncgezz.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3ulvirhmt.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3jvutwwho.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3rmojjcgw.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3ezrushcj.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3pvttpvgu.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3vpczqnmo.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3trworpjr.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3emnzbjmd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ecawxdpc.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3vhqrqovu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eeuntmdm.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3krmrgnvc.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3shvmweak.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3vomlsvas.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3eqnpxmpj.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3kzbgloqf.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ixxqlnff.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3chfjtjsi.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3knznzzkk.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3efibhclt.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3cyeybmpl.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3sbzitjhv.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3dpvyvbwf.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3ofcludbt.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3rytcmrjc.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3kqbndbmz.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3jujnihbd.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3grtsbzgt.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3hnolpsay.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3cmbaqduc.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3wxnbuopu.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3owgrjfjw.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3bqsckndc.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3mlxaglop.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3qpghtelm.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3rbnbotfg.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3fibyxdyj.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3qznlrnas.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3sfzxeihp.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ntzvbshi.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3zddxjdlo.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3jnjscsiu.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3tsgukoeo.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3ffhbkgam.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3zoxzqzqd.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dzbezasm.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3udfydwru.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3ntcfmkio.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3swybqlix.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ieouiitd.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3vppntkzm.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3fdugmjar.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3anylglag.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3vnjnsetr.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3zkwkgttt.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3edhrvjoe.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3wvrhudum.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3gvhuqnix.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3tdjsitqw.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3bdkiniys.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hfahdquq.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3qoszlnof.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3puyulwzf.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3ollbgmst.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3mbttmjsz.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3unzjrbwt.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3etirshwb.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3shejdezx.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3htpxibew.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3rkrsuvyj.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3eunzkicy.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3yttuqrhz.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3kmujycyq.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3jtvsxvjk.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3oqjcjsrn.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3ijhhdaxj.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3pcogytbo.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3lkcebgrq.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3cpeztzmb.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3zrqvnqbu.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3hpccntqw.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3rzbtuvgz.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3pqxxqikc.html


<!-- 参考信息 -->