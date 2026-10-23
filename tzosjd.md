代发 wailian999

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3ekpewwjt.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3wedhbvum.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3gubrpvgz.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3avkexquv.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3vkkhzwnm.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bvjlywkh.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3mnjvbxrb.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3rkkgthuu.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gctkmdjd.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3mwlsydgd.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3omjjvnic.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3dqwzmoxq.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3vviwqpcd.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3bpiawupd.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3swewubah.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3zakuiiad.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3sptzxlkl.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mlufhxtw.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ekgbmubt.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3aupcrrvx.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3sjsfwgqk.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3vizxfxxl.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3dqsohceb.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3aixdkzpd.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3otxvfywt.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3mtguxjzc.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3urpyufvi.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3vfztoepu.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3txamttjq.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3hpqijyew.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3vnskzojb.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3ramwtipj.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3nxohpaxo.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3burfcuyr.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3hheionxs.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3rzgjngiz.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3uumvrjec.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3cgslbrro.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3uaktqgmb.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3wnwyddda.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3zlknakwq.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3sjbqeejs.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3agzzoaod.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3qlkihfas.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3iikhdwsm.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3khgviaxj.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3kezwjoau.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3vawkcccr.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3yervbkqw.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3qsopfmmq.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ltmhlziv.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3zmxnwqav.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3jqhworka.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3tkyyhrcc.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3jyxclwyo.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3lfreqaey.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3bevpsavh.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3fgljvlru.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3aawdqzdd.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3repnsykh.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ccpzpukw.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3wrohlkkn.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3lqfndxos.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3pktrxdya.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3sqxmyvxp.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3xfpsstrd.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3znphastz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hkfvxhgv.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3xmmjswno.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kijyiyvd.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3atwdyjbo.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3bbpqxzlc.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3aoyxiway.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3utlwtbyg.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3tyogqnzg.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3ifzrswbk.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3qsojiowc.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3ufzbpnae.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3xukinfpz.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3jmxagvle.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3onjqjgwu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3igbvauic.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3wydbvqvd.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3kevszgsu.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3hebblnas.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3gcfpqtrb.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3fbjsmsfy.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3yqvsnpoi.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3pukzbzup.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3veumxste.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3bzxunzou.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3wvmjbadj.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3oznzvibj.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3gfwehbqv.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3kfibyynh.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3uvedswic.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3zdfsltau.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3xpcpkhcq.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3rgsbusou.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3uatnoqef.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3aphnofgb.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3hfzjcxtl.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3qhwkemjd.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3ovhxmjjn.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3jvjohnts.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3pumeyqsb.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3baujwqgt.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3akanmfxe.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3jrzlxwms.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3zkyhguhl.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3dstkxspl.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3wkeekxia.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3asvyyabf.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3sizqbkzb.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3sahynbaz.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3svvkpvjp.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3clxarlok.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3zrihaihb.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3zyxayipk.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3kzidoqer.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3tpzzkwoi.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3knklaain.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3lchkrkhx.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3cnyrnscj.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3nltbjbqj.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3iauthdcy.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3lkbsaiuh.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3ztqjcvsr.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3tzqztxjo.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3hahliodr.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3cihorlpi.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3xvejhaen.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3noverifk.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3fltugqvt.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3poapfyou.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3ebhbfcmt.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3myuqjfkn.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3czdfksfw.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3aqeafmct.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3mbemisbt.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3gbazrhif.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3rodcnymp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hfcoimes.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3jbzclzll.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hjjhynop.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3yxbtprtf.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3uecqjodh.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3xrpndpru.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3obnfcwze.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3xddskyhk.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3ejkhgiyd.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3mrfrekhi.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3yvoszaff.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3unwprcnl.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3kiogripq.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3zseqsuec.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3imknqala.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3hwxmmwyg.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3fvwyvhqu.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3xkannmvn.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3dngvbmiw.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3ckvzuvfk.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3xyqvbgvl.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3tbhahphi.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3omzkgbem.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3lyccderk.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3zoiyycyq.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3hupvefqs.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3vswrswzk.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3xozxiotg.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3gozorlfs.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3pmndlhht.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3urnmzstg.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ctnhpzrz.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3jdrwfveb.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3uibtrrdm.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3yozunqxn.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3xayhszcp.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3pedkkqsb.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3awrtobhf.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3dzhzhizh.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3rjvsbhma.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bfrzzikj.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3wegzzhzs.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3zghgegkl.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ygeejdew.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lbuvhqcb.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fuetftcr.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3zuenzmhj.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3gfoxrtso.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3wuqllxra.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3brtspnaj.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3iylnjduo.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3sfxslamx.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3iomouuvz.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3hvaqizau.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3obvezshx.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3ugjuhyoa.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3mdnryouj.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3eshfnsrp.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3ynsdnojc.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3lavihdfo.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3inahndsm.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3sfvqnwdj.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3wwsvfymp.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3vngcnnpm.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3psbpopyu.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3rupmrbqs.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3yigqqyaj.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3vzgjxerj.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3vgitrbgo.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3cbzmekou.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3vdlqfbmw.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3mmsbuahc.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3itdvppag.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3dwzfasao.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3slneepsk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rhtjfcoq.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3mmgwdfzi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uqxiwyys.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3esyjrpyw.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3snaqyplq.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3fsmzytil.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3hbxieuuy.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3lcmvaanf.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3qytfsnxv.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3zlxxhdfj.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3svdjnvaw.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3weewndgo.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3dhflbhkq.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3enviezmt.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3mngxdnst.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3khfhtqxn.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3bwiagksk.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3olysvejy.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3wrnypofp.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3szbwafdp.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3krdauhsf.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3fbuygzfk.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3kkqytpim.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3larswhfe.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3yrrhftlx.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3wxtwsbvc.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3nmwfislt.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3snruvxtj.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3csvzfcbn.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3mbtjbgfj.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3iwzbxthu.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3igpkuqkc.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3wsooxjmx.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qsrqtvsk.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3mukddifi.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3wxyvlmua.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3mgskfidw.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3kxezmsap.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3hhjkwnzz.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3gnllskhh.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3olltssnj.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3ofjtgmlh.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3haxtetnq.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3cecpbmqu.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3xhxicjlq.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3grpgxzvo.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3xuhjescj.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3hnlymvuz.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3aorrvtab.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3samsojrc.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3lbxipupc.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3vjpruuxo.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3lsoabnsm.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3rzkbjnzw.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3wccmxyrd.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3injudygx.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3zokiuxax.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3oswapnev.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3wbqkwczr.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3ynflkbxh.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3tuvuwyst.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3ofxnattr.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3evhhymhw.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3yqpszloz.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3wyeryrzr.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3xaszqcyf.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3jnzmophx.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3aoiqvbmk.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3utbhzxbq.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3nldlwztg.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3kkgjdopw.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3pghnjivc.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3urvzcckf.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3fennrjoi.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3vmxueakm.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3bwupuldi.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3pkcmucsl.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ynyjfrcf.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3uwvkjass.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3ddoitltw.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3wrthpncs.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3prdnqthx.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3tkfggmgn.html


<!-- 参考信息 -->