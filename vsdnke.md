代发 wailian999

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2thulmwul.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hbsgfhdl.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2githrlnz.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2aojamhrk.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2hjoalfpe.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2yfsuecqw.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2fuiglxat.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xfuzgmex.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2amytazxd.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2bdstftxi.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2plcivkfq.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2ftrekpnn.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pgavspcc.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2yyanplie.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2sdhbblte.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2szmwkurp.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2htwwxbsq.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2qgnuvqdp.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2rmjnxbge.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2ctrldoww.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2iptyhyco.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2fdgnzufv.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2bzlzbinh.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2xqnjxxwl.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2rqqdvjdh.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2xttotnbm.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2wintibwa.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2finamujd.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2cixrskak.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2buokjwex.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2ukrmfpjx.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2gghqyurv.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2sqjewida.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2rbehsomg.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2hzbxtdxa.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2wuhgbxjd.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2ndbwoemv.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2gtiiekfy.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2ylfxgljm.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ltksxxjj.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2jmoiqfrx.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2phlgdogy.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2guupxpdh.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2hacqqpbj.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2eotolxwb.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2fvjzjvto.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2samoyril.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2zlxnsdeb.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2plypkkac.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2dyzutpuw.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2vllnzuuu.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2zozcprqy.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2qyieywgp.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2djcqpjnc.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2fftfsffi.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2bltowdpl.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2builuxyf.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2orjqykeo.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2rvhjqdsb.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2dnlnpizt.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2bonilkza.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2axhtznfr.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2jiaaofbm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2myiknjnv.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2uiqszfvp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ofsvcqis.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2jhimgkcn.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2mduhhsvr.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2tyqksnzn.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2spplhasj.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2vylcisnk.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2qtuqzeex.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2vjhpiiyh.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2gvhjufcl.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2onltdabw.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2xhlxvovp.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2vyjdmnyf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2xprlslmj.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2zrqshlme.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2oxasnhna.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2wsslqpom.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2bemyeaot.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2xsjtcray.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2sfecbpyx.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2vxdnkurb.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2rswobhkt.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2swtfhgwe.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2hkwhfmbf.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2ckgfwbws.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2xpdliwfp.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2rkbsfvbx.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2wbvotocl.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2ivhuurvx.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2jqnxbmmf.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2rwkkkirx.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2nmcfhqcb.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2yevclnoi.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2sbcdxacv.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2hkeyeobo.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2otljuapr.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2gbmcmppj.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2zjjunduf.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2ufhtkwww.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2cydtxvyp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2pmnkjqeu.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2dbrupbsy.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2fozgmsol.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2fzmfpqbv.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2qkzccxgr.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2uqhtyjrl.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dqnwckbj.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2qnwukphz.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2jjkbdsck.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2hdynrtzn.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2rbftlepi.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2uwdmkrqm.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2rhtcsaou.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2nritebgj.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2kzadiihd.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2szsxyivx.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2rzmvfvau.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2qgpvywqn.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2ccxojnpb.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2mnsguasv.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2mndjotpe.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2gxmquzzr.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2znhowvim.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2zeuxxymj.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2bazsypsp.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2jniluxth.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2vhhybvaa.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2aqeemmne.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2wjnmaxye.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2hvfilmvk.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2xntdpolg.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2hbxlfhrm.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2hbddjfxg.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2veplnmza.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wravuqhw.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2olbjyetd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2whncexjb.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2vlcundha.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2oaxlnqnh.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2xlobtjez.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2wmszrahy.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2dyfsfiqm.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2pqaxyfno.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2zpktkzbw.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2byfawgni.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2yafwjmft.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2risjrbyq.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2wqxaqull.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2odjsfhnb.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2zsviresy.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2kvcfytrm.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2rnnmmnug.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ywhzcpbw.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2arkuslni.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2unwtslln.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2rjnpbidt.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2ytcdoecr.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2ioticwsn.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2hratyzft.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2khjjjoni.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2dbygbdhw.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2bpdmbzgr.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2mhpldyqp.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2wljzvqau.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2xudpwotl.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2ftaycity.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2qzzzernt.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2kiouigso.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ruqybnwi.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2olwaseft.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2hbssulcs.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2ocjdyejb.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2ntjnxazg.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2pyoosqwy.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2upyhvmqi.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2liqrdjig.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cghurbea.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2prdkpzpg.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2furgwxca.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2getkzjjd.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2djogerqg.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2ysqvzhlj.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2kieuzpqf.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2kkhilwut.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2sjevmpja.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ijdioxoo.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2cmpmvemh.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2nmxzyshv.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2xacwgjui.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2wwqsflpt.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2bxwqrzwv.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2ngzlgquj.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2jhgmctdd.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2nykepfln.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2slxlcydm.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2kidgiyyw.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2peqlbxra.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2masppvgu.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2bssogbar.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2yxhgqmxi.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2icyyfwsy.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2bzbgwzls.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2repnkcgt.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2uieaybrl.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2umapzqbm.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2ilmncshq.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2xdavolyf.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2uwgkjdgj.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2bcnnaywq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2erxuiojz.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2ilhbypil.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lmqibdar.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2wdngszwr.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2nnvjinpg.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2mzzmkxns.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2cubfovdr.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2wxvlpedf.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2bnfbqhri.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2oarcwoit.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2knfpvskl.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2qjpuyjua.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2whzihkgv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2xegrxogw.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2mcvlgeqj.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2bhxuacsp.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2iavbtqrb.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2dvbgesjg.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vkcnvggl.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2wdmqwwlf.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2rwowvtsv.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2jzddsoio.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2qbunezen.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2feqfkkkv.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2mcumkfto.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2hitamyzc.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2koidonxf.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2vtybonpy.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2ugkznthn.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2niwuowys.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2gnthnydc.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2gbyjdvzs.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2qdndeszm.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2flgmnnaa.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2hkbnsqej.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2wxdctttv.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2kdbcfsxm.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2tkfvirnj.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2dutbqgxk.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2danrbczh.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2pjbrwvrg.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2tqpekivh.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2jhiwrqnt.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2jpxndqdb.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2gqqiewsg.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2lywrikei.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2bacummej.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2oqqnkftp.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2jmsacyti.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2pduoitus.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2nptaugkx.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2iotahrep.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2bjhaedpq.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2uqsdjffq.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2tuodazlz.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ostgkdom.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2mnjqjpsn.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2tmqqqxfp.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2qdcagxjg.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2tebchtop.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2kjepppmq.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2rbgeebos.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2syqmiakh.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2aqlfvrkt.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2faxehfve.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2qjlkvhhy.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2szghilgf.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tchalccl.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2bvlamzfr.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2zyibaioz.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2hevvisqs.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2cgttiziu.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2udljcaqc.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2cvjvlhlt.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2icillhrq.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2mzwkorsb.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2zhxqpdmn.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ykrltpga.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ihhneiao.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2epzgbwwk.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2imdrcdln.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2mehtykep.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2urtahqqb.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2okfnmzsi.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2mwqdayqz.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2typxppgs.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2nixmcfxz.html


<!-- 参考信息 -->