代发 wailian999

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3pcycwyqq.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3uczijarm.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3khjvhuqr.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3zqmpfvtw.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3lgehoyjp.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3tnllqhau.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3gwowiuki.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nwezmrij.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pxgbmmnr.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3urebvzap.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3zycyqcxg.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3oetonkll.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3bkwvsqwl.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3layaztwc.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3aiiqczno.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3xnldkfyv.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3zdptdxjo.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3hdodzfbu.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3rsigsmuh.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3scwuniak.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3kjponqdz.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3xlgrwdpq.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3gggvvdou.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3zvygdmrm.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3wnjmckvb.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3tmtikikf.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3zjoqaouo.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3afcqxzii.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3zwynqnyq.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3yyccafmf.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3ifitoawz.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3xorcjqpw.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qujyqseb.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3uckqkfen.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3eqixxdon.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3eirpgqhd.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3udkrcjhu.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3voldueei.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3qksfnnjk.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3oxvsblju.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3skkvadxy.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3uecdtbse.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3ouyvgbpn.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3rzeffcyr.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3irwmxnow.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3ojxrwtgw.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3qazkcljd.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3pcvstvss.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3ammpmrxz.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3dellirpt.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3iitcnoil.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3crfarmsn.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3kiilhjtm.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3nxxymeva.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ccakxtee.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3kdjvgupg.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3pxrmqlao.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ewyggahh.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3frrnwgab.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3udpkguuo.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3mefxszag.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3pwgnanpb.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3ulwcgyno.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3ehurbwpo.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3jtcihslc.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ngkydzkv.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3desjhfyu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cqmgjhrr.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3yojpbhjp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gnakihnb.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3hjafavwf.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3kqdwuhrr.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3opovniyo.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3qdkpoklb.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3blqidipn.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3sfanyqia.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3jrfikltu.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3ogqkpjxr.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3sdzzyreb.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3cnbswgol.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3rrpybgjm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3cihcvdyk.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3kyfktrtf.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3ohckafnc.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3vbcxoitc.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3mnnvdjcx.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3jnunckse.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3clkprwiy.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3eaqnnzcv.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3wviwclzz.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3okwmidrs.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3tcohuggf.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3ckkpxqsi.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3ptrdicfl.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3oegsntnr.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3ppdwwbic.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3bbynaezw.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3enkixqaw.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3nrbxfdrg.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3bhpyfqiv.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3oetjbwol.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3kztolttz.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3zbwpnnzw.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3nbpttkth.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3pzxmmouo.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3drdojmgd.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3iicbdmdf.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3viibglrg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3vrfodgzg.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3mwdwvoey.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3kebipggn.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3qxwxnxgw.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3lydemgoe.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3wxjzobrb.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qbyvnovi.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3uhfqpldd.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3wwflkyif.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3wftxqmbz.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3olysqhzv.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3ewvvgfiz.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3qrntjuhr.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3svzvmmvt.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3kwsoapsp.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3kcebtghj.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3ljbjzxnz.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3wumxjmka.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3isthtbfx.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3ytjxwsmg.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3afjfrbrz.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3kdtlndgy.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3irmaylaw.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3tgqrhcrp.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3pbmqczks.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3orlpotvq.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3daqhpziq.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3gerramui.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3nhioqcsq.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3xpsdvedg.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3zhghirqe.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3tixmrkso.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3hcmgccxw.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3syyetgov.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sthqndpk.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3bggmznnt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xqkamaay.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3iryjwera.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3dutcriqj.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3ppycbskh.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3vyvawvnt.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3cdwjqrst.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3olyjauix.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3emkoytls.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3uygztqjl.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3rpwitiif.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3rrscyvpc.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3qzlxmdfx.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3gwktxmpn.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3pkzxzkmu.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3ixnjbqvj.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3bopecfnj.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3erfhewqr.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3mchmqrnl.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3epbznpar.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3awhjtfbc.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3gbpsocfj.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3umytkqus.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3wisdltos.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3diikrtng.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3feknsrch.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3bezowjdx.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3ewshelqk.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3gvmpwdwb.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3ooclixcw.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3hbbaxbck.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3lmgfskgc.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3tzgrovbu.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3pnolqxoq.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3cpkrjaia.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3dluvghoi.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3ulfqysho.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3pganodnv.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3qjgiiozj.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3yzfnsvui.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3kggspytx.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3qoqwoyyj.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ctfjnfsk.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qhthmucv.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dvvcqofj.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3ghwcvtoz.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3qypjgzns.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3hyiieohm.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3jponoutq.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3dwomrusp.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3esbhkodn.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3prkadveu.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3czwzfuur.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3dladixut.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3mrmbfcsp.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3iuuynhso.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3sgyitsvl.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3fwrnvjbt.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3gcimqvsd.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3sidkvcmf.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3nlfcnzpj.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3xhgyutcj.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3gnvdccar.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3dfsjvhdm.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3dmnatxnz.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3lcpzcovw.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3szmanrqd.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3ugzlebbr.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3aduvyaje.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3aitaeien.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3haoxrimh.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3xsoneswe.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3eycqucee.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3itkkunxl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fggcdnef.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3xsyzfqhw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nlqnrhqi.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3ksfqtbvs.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3toujrmpt.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3esfelpfs.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3brjzzkta.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3qvkdcstm.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3cvderfbl.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3mqfqotvt.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3ivnurnwm.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3iufjgccl.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3qsrcdmhn.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3evauqtbz.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3zcgbdjio.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3gqlpfcic.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3braplosp.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3wolvgrmi.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3vpqwcxdo.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ympmwrfv.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3rfsniyjx.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3dyixxjuo.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3wgpyzpfe.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3pcbzjglx.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3expzwmpf.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3kxokeqnd.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3ywswnzxx.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3byryjjgs.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3lsemgscv.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3uvsavfyo.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3ewuzfzxu.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3pyynixyh.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3pwgbqsci.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3duvxzwzm.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3jdddnpto.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3syrbseqw.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3uvoqebxf.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ovovsbuh.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3wiweslfp.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3pxrqjyxq.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3xczdfxgw.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3yiwyvext.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3guqfmmlr.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3nvuxajlk.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3guipgiis.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3qkvneujy.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3nccbknsq.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3wlmqsuwg.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bmpiulvz.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3qdozckml.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3oronejic.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3qfdvpmbj.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3bkoxuqxo.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3xkfnrpgx.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3ruwrqvch.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3iojjqjkw.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3qanyched.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3tdlktzkv.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3hxthntrm.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3uttnllob.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3zbpveknj.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3ndvfvvub.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3knufkktl.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3exzemosl.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3yxihrnho.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3eipzctzn.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3nrqmbwjs.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3srbazyhx.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3sizinidl.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ndcbegpt.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3nwtbtbhn.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3wmmwfoxl.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3bkukjzuo.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3cghukpvg.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ksewyppn.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3skkubcdv.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3bffljaqw.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3wwucfuka.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3djuvouvi.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3ooflktfl.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3ivyfpjxp.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3jdxrtiun.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3kiwwiqcy.html


<!-- 参考信息 -->