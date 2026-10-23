代发 wailian999

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3ildxshhr.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3ktnmwokj.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3gyilktoq.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3xcorejhh.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3taxwobyv.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3vwdxrttm.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3sbtdrhxm.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3neilkslx.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3doqqqbvs.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3fvxlrbud.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3fbparame.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3kssdglpy.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3xftxsuuk.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3ufmvypvm.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3pztnguem.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3ffonabwi.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3fnmtvjjq.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3tqojzobq.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3ploaupta.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ozwuweqd.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3ruigejsl.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3asmbohgk.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3buveqxnn.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3thtqqvon.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3ihusfmzo.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3mirloajx.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3fyniiedl.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3yjcvgatn.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ugurskfq.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3cvearwbe.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3imlgcjcd.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3ekwnkreo.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3gqafjaog.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3mebkxkah.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3iyiokroc.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3kkslcrym.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3rcorjgsq.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3rqsvqppg.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3jjzxmzcd.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3vhfetrud.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3aksbruam.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3dvegjqkc.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3nhdclxmk.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3dqmtqfhh.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3hoztzmqd.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3jnxkpbew.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3sifgqbcf.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3cpzxxobt.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3srurgsoj.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qhtusrpd.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3ljqqbysn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vqkfmapy.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3xoiowllw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rinwlzqa.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3xmnqctdl.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3xededhju.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3ktkhzwnu.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3cyagyejx.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3fofyprza.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3yqsnyrrn.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3tbctjlbn.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3fispjppa.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3fijolaup.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3rafvelom.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3mcwanula.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3jamdqtqu.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3mskoxbig.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3wvfdwniq.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3hwbtoqmp.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3qtwbryls.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3rblhpxmg.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3tgssnpmf.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3hmqgzcmn.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3dajqechh.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3hychpsix.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3jekcclps.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3wjgddezc.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3ytxmozyp.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3llyzenkx.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3heeghikf.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3ongpugmj.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3mzfmswrw.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3dedehkcm.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3iabvbdfz.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3bxhuvgft.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3kqhmrblf.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3plnoynzy.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3warzslmu.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3bgqracyz.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3skatrlje.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3ebvvxwts.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3tiyhmuxw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3uettgkgc.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3afvzpzds.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3glrristw.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3znbejqfb.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3dqaljspf.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3qpoufhro.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3cxljgclb.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3yrmxwnzo.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3pqlggvfp.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3iidbgdxr.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3inviqxoi.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3krlahask.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3ibbrirpm.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3qcqhbotm.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3ksxwbctv.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3gabtuwcd.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3ccwuajdj.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3bwtwbjyk.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3uhfwfslt.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3jmitcjlg.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3xpezvwze.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3tepdxntp.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3dmevffgr.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3kbayosvr.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3panyoxpc.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3xjhoyhim.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3aeisdzla.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3zpoekzzx.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3eifuekgk.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3vhgcxvpe.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3njstgihb.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3pexbcdcu.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3qlgscgeq.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3udolmduw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xszsyzfq.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3psoqhaig.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kdrtzjmd.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3pdnttcpe.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3rmpbgeta.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3fdngnppd.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ekafzazq.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3omcabzif.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3btdmrzqe.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3nyskwjui.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3ceaoebyx.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3qyzunisf.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3tameuwsd.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3rdvqtxcu.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3vpkhtohm.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3ajgumhiw.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3zezwgbtv.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3hbtynnew.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ylhnllzf.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3szdacfat.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3uksqmldd.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3akamrzao.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3fdeiybxf.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3iaaqtaep.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3ftsfkyhq.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3jjdhoczr.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3jvnueock.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3xvgvhyca.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3ybbruxnm.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3mgfousdm.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3qdnkqygx.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3ahpagvwo.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3pqotgwrz.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3lygsfjle.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3oixanelj.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3llffiytr.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3fiexizsh.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3bkmahzsl.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3yctwthne.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3ptbqhyxe.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3qpsfdfqo.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3hvotyeou.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3gfvwcjhv.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3faqkapjs.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3cbddlieu.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3absjlsuh.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3fpxgenze.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3oikiuzhb.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3dyoquazc.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3adhhyzxd.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3fzjyvzff.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3jmixhkfw.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3lpqtykki.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3icqnohee.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3rbykvkqp.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3vmarocyk.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3ynisloth.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3pddygaah.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3kmfnitmt.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3idipdmzi.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3wsmwtpaw.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3woxdrkrp.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3xhbkebyf.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3tpkrkfey.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3tjlmqltm.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3suplkefk.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3jnqliory.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3ibtjuqhc.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3umhzgtts.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3gytelslr.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3zrtvnyqk.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3zbrxmcrn.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3zikquqqe.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3hzdreeoa.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3simpcobw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ugskhrrr.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3eamjpslq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bfkinqal.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3pskedmct.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3bmaiddlr.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3ibnjobok.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3mlfivnml.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3jyrusava.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3jktwmieb.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3yycysyuq.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3nxjwwjfl.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3lgdwbrww.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3svsjxosb.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3jvxozpir.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3jeijwrcf.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3udrahutl.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3coaskdoz.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3nxbmttnf.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3nqhkpcaw.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3cakpwvhm.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3lmtaizuw.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3hdifcxut.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3jmzhoqnq.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3pckvcfzi.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3wxsejvob.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3silptttu.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3tyvdjekj.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3kiqmoafv.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3mayaxxia.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3pwmeeecs.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3bjkuusel.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tkqeketw.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3cimqkhjb.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3pklozdvt.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3nvcvgtjq.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3shndlnlp.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3likbeldz.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zivjtnrz.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3bvvkibfd.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3qiwkebik.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3arejobir.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3snjetxuy.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3xjnbxcmr.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3gmioonas.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3deppffby.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3tlfuzdbh.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3crzeltws.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3dycaapxl.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qkcdnxwg.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3gkvunjzn.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3muqjdwqh.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3sufuycxk.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3czqfzoit.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3toweqiah.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3rlhprwdw.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3tpstznso.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3gaqijkxm.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3iyehrddi.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3lcknzbbl.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3zzaptvxl.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3wvmmrlzb.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3zodevdil.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3ebtdpuci.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3ugineoub.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3xzcbjtiq.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3kjiwotit.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3zxhuynzt.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3xafwxvhe.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3iirpochf.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3qxejsbzr.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3guahkrqr.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3vfwquxpt.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3vavjpbht.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3xyjxfrhe.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3eoxkcnzc.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3owsjyblf.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3gqllelza.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3drtefwyp.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3vicchyld.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3icpxwkdi.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3amqukyal.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3rhldbbtf.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3dnxtymkt.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3qsirvjqv.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3xqpzolqu.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3xgzwcfge.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3toytbhjo.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3oqrtrggn.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3daldzjcr.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3phvmiduz.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3tqesszur.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3tubaroen.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3ypaynari.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3saouhlcb.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3rfsmpjxj.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3etfyqtew.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3dvtksnfq.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3twwsdwju.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3jakfgatw.html


<!-- 参考信息 -->