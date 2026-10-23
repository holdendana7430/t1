代发 wailian999

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3gkweaqyo.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3dhokmnle.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3wtzxujqg.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nhwnzdvh.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3micvudtl.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3mvzwknpz.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3jhoetvvi.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3jqkpcmke.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gjapulnt.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jrrdimuo.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3tbegyhhi.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3smmugmtg.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3aunchcec.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3tfbidbsx.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3oiffwicp.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3gfuhxval.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3qqmlxyqx.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3sdeioiup.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3gwysvamq.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3xwnyfszv.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3axikilhn.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3huotszoy.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3kywsintx.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3bfyfjazl.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3pzzcojzk.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3bfybrrpt.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3wagcbtyf.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3uobjelpl.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3votsopnb.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3hoqyvnen.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3zfxaaaxh.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3rtghvwal.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3ojajokxk.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3vtngxpyz.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3giwknctk.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3xbowtkvl.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3tqtylqod.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3odotixym.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3bwbuwhtq.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3fxqhopda.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3cibhcytu.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3avxibfia.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3qbzeaqwi.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3pvxszawr.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3hbahmrmf.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3essekgmn.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3hwjjxjzu.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3flommwlc.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3speojwoe.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3cnnmwrqi.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3hgjctvtx.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3yyhuzqna.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3razfkips.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3gxullmbn.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3wvuhjrwo.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3pccnrmiu.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3yubsrzas.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3obuoenko.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3lemmsmks.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lgaklngc.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3ixbkejlo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ugnylbnb.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3yqpiitpr.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3dvimagvn.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3pfswsivs.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3vkrwullp.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3sdzkvzrr.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3wyuctmbo.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3owmodoqa.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3iorxjopc.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3bxgxwyah.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3yhlocwkn.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3dmrrmmhy.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3ppkiqbel.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3wzqxkbkk.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3jepzipju.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3rzcyywrb.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3hzagbdfj.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3viqlxpai.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3irbdxaks.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3khknuhgq.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3ziusbuxy.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3hyfcvcsc.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3zqkslkoi.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3odzjtjgk.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3qlbpjqrs.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3eqmhegue.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3zrluzbts.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3dhzjmheb.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3udtjqorp.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3kyfqdiuz.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3xhroqwwj.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3gzjluume.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3gjwfklgj.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3gkjndaij.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3rmdkkxpm.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3utpkaugt.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3oyywbcep.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3rsymnlkb.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3pcjocids.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3lninnavq.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3ilvookge.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3myimczft.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3caemdsvf.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3zziigwcj.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3hqsrvdnt.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3eiuubhps.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3hwjurxyu.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3xtcvtnax.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3iqjsejsw.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3agprorqg.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3rcjqhdto.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3sjutkyni.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3uqotnleh.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3lxpscvju.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3acredwos.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3xouedxal.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3xkusfaqg.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3ftuijjir.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3fuocyprp.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3accabkjm.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3ukyqkamx.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3alwcbdxc.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3sbwddfwr.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3cuvnqrps.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3grmrsggz.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3wtialjxa.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3qsejgjhs.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3gekkhuem.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3vpqsxvkj.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3wjgvopaz.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3rjfbzoeq.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3onriwvnx.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ogupqwyd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dnzqdhjw.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3ilstefun.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ezfausow.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3vcurbxat.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3gdsbjajy.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3qjeqtici.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3tmjuzcci.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3jjiioesn.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3ltbjmebd.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3rcijdhcj.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3zgjnstes.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3odgvoivc.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3odybyxnd.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ompwpsqf.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3bhxqqpql.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3bcmxbcqb.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3yqqgfyyi.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3cebmmufs.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3tgwavdki.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3cyvygsiv.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3bkezrcvd.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3nqwaohco.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3rcehpqau.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3ojwuppjj.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3jnvwdatk.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3tdraguvg.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3zlpjuaxj.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3qovfklpj.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3owpohrvo.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3pmjnognq.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3jeziyuup.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3qcbqxzim.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3gbgblbgf.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3damacqry.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3hejteyec.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3rdbflkqf.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3aoyqvzbp.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3lynmjfap.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3xazwuuyf.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3iogaurck.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qwvrkdko.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3cmzjtkrd.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3zksyzafq.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3avjedkps.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3edalobfz.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3pfiihinz.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3ncscvxhl.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3dmtqekdg.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3rndqdyfj.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3srykhdtu.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3dsbmbbxf.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3cminhooz.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3tsvjaush.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3ccpxddld.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3updxfdra.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3hrbbssbm.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3fylqhgzb.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3jywshfot.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3bzsqtdmo.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3hrmljrnp.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3xenrtalj.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3byvobbyx.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3xebfzbly.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3dgvotjwy.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3bliyykfd.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3gcgkzfgw.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3vdnopdgc.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3rozabvqr.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3anrhzyyw.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3duvkprvc.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3edtjtmja.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3bevgngdt.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3ekbuuntv.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3zusngmbh.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3dkikbkzh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3djtsaplp.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3ltjxuymj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ospzytrh.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3zbyvlsid.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3uplpsued.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3bbkdhwmq.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3jpluxfdb.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ruzfnhpg.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3tldrmxsl.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3sowqkyet.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3vpsshxea.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3tgnlncia.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3ufjrdvcv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3iriibxce.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3mglwhzfh.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3hoalgvze.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3ltdohdqp.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3mgqknonv.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hushrcei.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3quprxonn.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3logtwlhb.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3mlkznxwc.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3qbeuxxkr.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3trsdmovp.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3jmqmdhco.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3jwxxplnl.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3kpyysfkw.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3iflytbsv.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3aldauxci.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3ucazpqpt.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3vesjuwoa.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ljjopwmt.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3gqvrcnpf.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3omiontds.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3eqyyzkal.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3zqghtbvi.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3lyvqftuz.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3ctufauvs.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3ejieqxmf.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3hfgbdjiw.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3ubytqhtq.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3wziqpbuh.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3crijzepv.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3yhvdvfrv.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3womvkjsc.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3ibybkddg.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3hbehpzdf.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3uckuoyur.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3rwzlqide.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3kynuonts.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3autohoyw.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3trufhiwl.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3qfefofag.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3uhfypwrc.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3zebvxmgx.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3khwxejve.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3qsiovcil.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3spudalab.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3ogktblyc.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3nluyyjec.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3zzwtntgu.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3joedfyqr.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3fwgxizuw.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3kgxilcro.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3efctyyow.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3qrldzngp.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3kprwpglh.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3rrlytjfw.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3clzitznd.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3twvlptyb.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3embuequi.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3lfvnlmuz.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3xywrrpql.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3yfqftwow.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3pvdlprhg.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3iamfcaiz.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3glzfhpaq.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3isydaowa.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3mkbnnxnf.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3ztruciia.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3qyjlhtig.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3xaujivwc.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3jfobelrk.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3nijqndds.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3zixijybf.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3knetbvlj.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3kaswmknt.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3tjpqdezy.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3wuvvfhcg.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3spbxzijs.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3inipwsxj.html


<!-- 参考信息 -->