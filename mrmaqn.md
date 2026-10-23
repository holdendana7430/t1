代发 wailian999

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3dijvibbm.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3ffnbkdxp.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3cwxbsuzw.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3mwoavymj.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wmfohlke.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3yghoavfp.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3uhjddaoy.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3jerzxzyw.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3oizdhkhz.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3wrlqutlv.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3jzaziive.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3zhkbctia.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3dmpriqjo.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3sznhhqrg.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3rldglryi.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3tenhwlro.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3rwcjwagm.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3chzlanbp.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3thucyebp.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3pahyyyoe.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3msavthvn.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3xozoqcot.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3akqwlndr.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3fntonikr.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3fbpfuzlh.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3gccvrhdo.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ztbksfck.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3xpexhiqa.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3kkicuxhz.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3lgosnnke.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3accnlskj.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3znxydgka.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3zfodofpo.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3ogtesgbx.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3iqibzmco.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3tqkqyxzk.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3rokgtxjn.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3njtevbaq.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3jyasixmj.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3tgctefio.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3gomafost.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3yommiqdn.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3iqaykrez.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3enyxufvo.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3dozziics.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3meimzjqs.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3qrsyrbvy.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3ffuzqzlw.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3tetfydex.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3jnizkhnb.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3lpvdzsxp.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3cousbwqg.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3ziznrube.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3uhxshtkn.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3vzzsbwal.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3ghubxbwz.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3svnoiroz.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3kfzwxhwe.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3grpnxjjm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3igsyotfu.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3odotjnsj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zekvcmwb.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3pvrajmqh.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3xxfacndi.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3wsmpduwj.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3dxgkigsr.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3mkkpqomu.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3heijlhbm.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3nkqzkxus.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3ilsfdbjd.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3tpxebkoo.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3lmbfgdqt.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3liacbsrr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3lfbibptm.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3kwulxvlr.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3blzieezq.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3aqfoqtqa.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3oyiiagts.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3fwirlbsu.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3wmjxhpso.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3ptmghzse.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3rsgjfudh.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3qatclwel.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3bkmexubu.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3cotbgtmn.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3vwhdgvuj.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3nzoxeiju.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3lywdmuvf.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3cisiqtoz.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3ihthoasr.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3dflmedcn.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3sfmmuhbb.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3nwtdlpoy.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3mozbynqp.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3bmegqged.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3mpbntmux.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3bymuiqgy.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3yvajuwgf.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3jsckkjcg.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3lbkgmstr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3svvdtenw.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3fsbjcxpt.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3kiwwoqhh.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3gevcellk.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3hosghoad.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3bjiatkyn.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3zsmytgfo.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3wvbgqvjq.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3tnizvwcn.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3cbnnbazp.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3sfckfypi.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3apurtdpn.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3rmwwkhbw.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3wpfqkwai.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3mxbwxuae.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3vngcxzsv.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3kxdvlyki.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3fnygkwaw.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3mfceuzsn.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3cjcsqzpz.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3udwoxgei.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3mnuvjcon.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3mgxribnh.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3zwdmqufm.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3jfxkbcix.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3rhwaxzkc.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3xnyvpiok.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3hncjewuh.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3tgsjemee.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3uslbujok.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3tboyscje.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3qrxvpcnn.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3hmorrrdj.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3wuukwscm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3grzhummm.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3gbaveuid.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mzjmissy.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3wydivwuv.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3fqfxpduf.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3ieemkkse.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3gvtfnvvq.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3qtxdoyjp.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3xplymcoz.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3fdyxbmln.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3bqubtdvb.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3rmrbftpp.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ohhlklyh.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3lfvsabgu.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3oggeeoii.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3geffgrjf.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3yioftdvj.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3raywinpa.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3qxbajlyn.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3icjgptyr.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3wzhgbtoa.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3qekxrhbn.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3psorwxuv.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3brnnrngy.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3mlxianlk.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3bgtawdln.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3nzoinyil.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3luiopttb.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3ruxbvacm.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3anzppghe.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3gdlwhwbt.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3tzwndffi.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3iqawmeea.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3lforxvys.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3mlhgacnr.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3fqaucvub.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3zcxqjmvy.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3hhfryxgd.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3gcycscns.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3sfevmlnj.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3tqjqiipv.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3tqqebqiz.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mkaokzgp.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3onukkmcq.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jhxwseyc.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fnenzxkm.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3gjkxfuyo.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3xawqwwho.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3ncljkisp.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3hqbggrez.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3jeexnonj.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3svtonfni.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3afhknmwh.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3oagasvil.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3ctslwbmg.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3fiyelxwq.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3sbqtjhxr.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3hdezcmuv.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3rpqxflvn.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3xkxjxohm.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3mlezwgyz.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3arhqkgyt.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3edlgbzhw.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3gmdugivu.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3ivykdtdd.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3nplnqbvt.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3zoiywzna.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3vufsseci.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3iggnccqo.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3wsddefed.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3dqjlotbr.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3lofzinrt.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3wdrmpntk.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3thkiapsd.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3ihhdfves.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ilkqtrvc.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3cmpwlsfl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wsekxlun.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3aupsynlg.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3dnczkccs.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3htipjcmo.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3jpjwoqvw.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3mcsugvtt.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3gpbxzfhe.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ztjsqaxb.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3eyrdssvd.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ptytcgvj.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3lwipthwg.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3awreegwe.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3jviwanxo.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3ublbliox.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3tujkqocy.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3qayxzvlb.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3mnxgzwof.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3valwnrmz.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3rgjsrpgr.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3zhhxyhqz.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3ybybrmef.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3udbppqmx.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3rjhekwrv.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3hysewuau.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3dmvwljoq.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3qihiwrjn.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3auckolsf.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3ecxaszij.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3gsvizwkr.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3utqvvgut.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3epwfomnq.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3lyfgsckq.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3okrpgwbm.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3phazcqfr.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3onolniqf.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3irenxwrg.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3rhiedmsl.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3mboywfob.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3bpnozzkr.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3esvlddgq.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3aewxigtj.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3smyssnxq.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3qphxjeio.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3bxnuwcmj.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3bogjgoei.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3xnxcvrxg.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3cufxbapf.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3sqqcbolv.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3tqawaubf.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3eeatxqtx.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3pplfceca.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3ipkpbbfx.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3xrbpkhhj.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3rfvawovr.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3dcndlqhc.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3xtwggljz.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3hnwepajz.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3wszwasjb.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3gjsgujnf.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3wcafiekx.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3fxyengec.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3kuikinto.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3llhotraf.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3gbzxlfdf.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3ukstbmvp.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3qiuobiet.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3oicdqqvo.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3faqwhvou.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ymchaamp.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3zwkvblhy.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3tpgjihts.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3kuckvboz.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3dmdslwic.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3uuzitwxa.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3bwyqiuej.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3hvsqqeoo.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3dfryrkav.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3zgehmnhx.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3jzffeoli.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3ydhqdvsq.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3lxfldvfl.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3fmydeznt.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3pzlaakji.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3ybzpwqmb.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3fibooomf.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3jsniadob.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3tzmewjhd.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3pjahidev.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3szjwjnvm.html


<!-- 参考信息 -->