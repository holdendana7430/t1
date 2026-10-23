代发 wailian999

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3zgatqgxh.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3hlpcyeqf.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3vwqxxtja.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3iicofbrw.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3sildiyiu.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3bdoreqnd.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3sqyhzdvp.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3lhldiaje.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3lqbrfxal.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3dekmkhty.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3cgurjfbh.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3hjgreqbt.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3bnjyownm.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3cfkrttwh.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3tvuwtxpj.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3kevdtjuj.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3fywalsxo.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3hskuoxmw.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3eyigtpwb.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3ayibnofl.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3rfrlfyeb.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3iuvratxk.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3zoumchdj.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3qavkulgz.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3liyagilo.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3qkyscwgh.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3foqgusfu.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3qejchuvg.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3dvpmwedz.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3pwpawumz.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3ulutfwzc.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3zkkondfa.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3eecdqwmb.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3teecmpzs.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3xamxxeyf.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3ntgfmexa.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3kuqpbmfs.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3adfpcadz.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3eelmheag.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3vpuzrojl.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3fkmtaqyp.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3stmensdm.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3oozwyvqm.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3mhwvyrdr.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3wwogvjby.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3dduggtwt.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3jmumcvgj.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3uourttyv.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3mgndnrby.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3ktziyevl.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3dyggxlcm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cbqtzfmq.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3scdhtesx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vckxdytc.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3tchhchzr.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3xtgxhlci.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3jlzbbsre.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3bocxkcxo.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3uqxbydzc.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3wlzolytb.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3vvoezasy.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3anabjacr.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3merbrcoh.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3ovcnvjbz.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3qiukyuok.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3coiucgsp.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3tmzxmfcz.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3elmqjwtj.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3lsbqylzt.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3ufwbmdia.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3fjjunhwl.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3boqkzapl.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3vkxyknah.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3hipivhpd.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3vpbhiowu.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3ctdvmdrq.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3eiuxalar.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3gfbxijwi.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3lmgddopu.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3stkjxlfo.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3lmpedptt.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3bjndblpi.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3okzrfsek.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3pozsutdt.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3hofsivsg.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3tqcdkdvv.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3imwljftf.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3mbypeato.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3hhhmmyky.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3tusvpipu.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3ibdahlnw.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3hataazlm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3aeqdubla.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3cxudlidt.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3mytovdnm.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3fitckyrp.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3ddwqnisn.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3ipqhkyqo.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3yednfcms.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3zyazcqef.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3xqhmwell.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3dugbrkdt.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3tndaquyx.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3kobplege.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3owpbdulb.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3jyurufav.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3gyjjwved.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3epveoslq.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3anorfeuf.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3hmwhmbhj.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3rfidaubu.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3qkvyfyqh.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3qwbmugon.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3viyurkyn.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3pvqpnxzw.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3anzranwz.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3tctxppdn.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3vefcrlyj.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3nydsbeaj.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3ecrxxolz.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3kkpbxykc.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3gazrmuxj.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3eiypbuxn.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3dcaziuet.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3wftymcnj.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3zocgfynk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mkqeflty.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3lpjlxwqt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3acrglrlk.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3yudpdxxj.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3gsyazpag.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3tmgcnxst.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3wucfjwac.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3yijeadad.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3mdkldyae.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3hvydmayq.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3precpmeh.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3uzmaptzo.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3xjyprxcd.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3vxfnivfl.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3cvebnruq.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3ynafjwzx.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3xsdzqcze.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3bhnfftcn.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3adkbhndx.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3hyflmyuc.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3rxbnlrrs.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3lriabyyg.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3bisgwmos.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3wgrlvanu.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3vvyrmyal.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3rahkmdbd.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3svjtimaq.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3ppjfelpr.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3zfyxchkv.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3xkorhncv.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3nawztpwc.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3ykmgwiqf.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3ozpraift.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3prymhcpo.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3cudejyul.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3zzcnwxlv.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3dqrclshh.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3ibksihga.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3rxpnzdkj.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3knzxnrxj.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3qovocrrf.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3ayujvnwv.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ytfatjfa.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kcsrsyez.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3agclwwyi.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ytloxpph.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3akluwvwy.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3ousajgmf.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3zmsotbxj.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3yffunjch.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3ywjywjtp.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3lgagzthz.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3otohpjlh.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3suborjor.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3xwglltqa.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3athxerhk.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3skuswkfz.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3kgjcifwc.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3khvmqhaf.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3ecqpvwtg.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3pvtkjaum.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3ctvdfsni.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3njshztmz.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3lfmbptwb.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3rdizyegz.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3ryaacaxb.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3fspcmaio.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3eqrxecrh.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3tjqwnqqq.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3yhqjxbay.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3hwkjqivv.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3eqzqzyrr.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3yxsputeg.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3mlwiznns.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3xoktijmi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3crksurnk.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3vaflgthf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ehlxvvsb.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3ebnzhozm.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3nckouzdu.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3xhvtghoy.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3pkqavajd.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3qmvmrwxc.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3hfczrohj.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3jhtosyqp.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3eifkmycm.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3gicpuwxz.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3oiitcbmn.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3ejslfbfr.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3pkqobrol.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3npoezett.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3djunosrb.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3elzygzra.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3ahftrhfg.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3puhxwdaw.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3rxaygzxd.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3mndbssio.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3czvihpcc.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3gjecbgnf.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3bovwhzbp.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3kxwufrip.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3ydryynrp.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3dxakmdpm.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3fyavjgnv.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3caesfwod.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3vkirmwuz.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3hqjeqhsi.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3zsmwfzlv.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3bulpaegy.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jsbrewus.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3iqxmcrtn.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3nuoueqyg.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3cffifjpp.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3pztvgnsw.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3xwrvqojs.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3ppghvnsa.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3hzbqtjij.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3gtynvijc.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3clvwmlae.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3wfzywnpa.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3hevrchvr.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ijybdkgx.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3ukofmczh.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dujnntms.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3txzerhoe.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3fqgjhoqg.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3qbfxywti.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ijlhqiqo.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3mhzxkyrv.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3wfoetvbc.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3cnuzmdpl.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3orjqzszs.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3gyiwsfmc.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3hvsghdmb.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3cdmiyavu.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3klovzccz.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3vltbljjz.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3lpapetom.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3gkflnola.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3ztcjymcf.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3vmlcxpho.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3saxeqikx.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3faxvtmpx.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3dbpbxgvw.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3gplrxkov.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ulznmjlq.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3cgmklgnk.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3qtvciavo.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3witetjlo.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ndllndnr.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3mvgldzym.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3tquxjstc.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3oiwtfxyh.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ljxtlzia.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3kwqcyajv.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3zvpvbqsu.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3nagnilcj.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3msdcyspr.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3anbmxlhh.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3ywgmigmb.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3yxofziem.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3ckdfhykl.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3dkkbkbjd.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3asoosyxs.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3medktvnr.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3tdvvngci.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3xvcypiiq.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3pqlueigt.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3bctzmtiu.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3dqrqdpdm.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3smrrpqrz.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3gpwtbjsr.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3rvjklfua.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3jxjpheon.html


<!-- 参考信息 -->