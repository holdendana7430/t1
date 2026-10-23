代发 wailian999

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3hralvomt.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3ztnsafjh.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3hwychyas.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3edvoltor.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3rcytfzna.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3pcumgyyi.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3popesovn.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3hvgcatlm.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3hqcjoskz.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3zmrjdabh.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3tpvgjcan.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3rfkkghvo.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3sbphhbkf.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3eyiiiyvq.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3hgtnwemo.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3wgpifphf.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3fwgnbovs.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3pukywyyj.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3tcqqjwkf.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3unksnsem.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3zxyenppq.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3njoboopc.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3chfyntjb.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3umfzgiet.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3ipolkgro.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3xhvkcnwq.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3kpatirvk.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3hhtunufg.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3pyskpsve.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3resyuhli.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3pbtzkqpf.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3fmlejrld.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3onqvoywg.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3ynytedkg.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3nkxorwge.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3jxuooieh.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3vyjmypsm.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3fgeibpmi.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3gajczuds.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3roctfefr.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3flnmdzyg.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3rvrvvkly.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3pzzyajnb.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3novitwbq.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3ynnuybko.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3itocykwm.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3cpqbdfem.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3imxsfprm.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3pggctanq.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3udsgmoop.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3hncnhimf.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3arfiiftb.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3jgmizrjx.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3hbszhqhr.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3gdwzxnlc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hrtikkmi.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3ubdbsxvx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3arljqmah.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3uowvyrek.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3hvyfbhto.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3rrgpeykc.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3njdrfvft.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3dfngkpru.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3kakcehmt.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3nfqglwrs.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3fmajruyn.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3jyrkohwy.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3ghbxmrfl.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3yogzifbm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3plfsreii.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3etvzcgug.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3gemeyfra.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3sprdlqnx.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3ycqmbwpz.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3wmmcidea.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3zgjhmyvz.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3avpkvwyi.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3oezbgyoo.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3thhepuyd.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3gcpgofkf.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3yspdxavq.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3rxitndui.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3drpeybjb.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3lbjfiorh.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3brhspwwo.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3nltzjdau.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3vdyxvjhg.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3upcxpaoz.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3xrcjuhjm.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3jzrrtjvk.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3fiyqwoho.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3oueadrhi.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3faiabwmp.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3otdttnli.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3hznduscb.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3fzgjizqu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3ojvhsqsc.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3ehevvjpt.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3klmoxtta.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3evplobzs.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3kdczosgs.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3whrkxfhi.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fyfyxept.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3qppdopep.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3pvjapdrf.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3ycaebovs.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3ytekwufp.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3meyiyook.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3rzcvchbx.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3liuglkbn.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3mdqnceoy.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3bqqimzdt.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3dgitfqwx.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3xohhjqrc.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3bwxulxdd.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3aihzmcwh.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3huvujslz.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3mrnpfsva.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3svufehrl.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3monimten.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3jyrvwwpf.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3ifswlquq.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3qxxnbhig.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3wkjlinam.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3afsudeal.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3fyontkum.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3xpazjmma.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3pxbcastg.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3qgpvpxio.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3fjfyyjry.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tthzipol.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3zhdqcvnr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xmlanpgc.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3nkkiyzjd.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3kepehoyp.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3igovdarp.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3thpwmzzx.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3srhegvsq.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3kestjwvu.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3uofwckcp.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3ljmcttqh.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3hsasqaiy.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3lpkkduxc.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3qqljnbgl.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3femnnvqu.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3kfoxhplw.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3rxxglinr.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ibtzjfzp.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3juymzkif.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3nbifbklw.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3djvrlwof.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3zrviooav.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3wcqpftka.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3lqkcvbum.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3xrbgnmjf.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3arqjkwrf.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3xmhisqsn.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3znvgxvnb.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3ozwwgmws.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3wamktadj.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3htikzzit.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3mpyssovd.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3dgkvqkyw.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ypprygal.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3yzxshvjm.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3elkcgkvi.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3tmfbcvqi.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3kbnfdcve.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3lliormxi.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3zkcfmiri.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tuemeytr.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3naaratxe.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3wbhmwuyq.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ohmcflay.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3mdweijjr.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tkefrbkq.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3lzspprzp.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3hmhfhjwd.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3mbxhdppo.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3gmhwqvje.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3heffuhez.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3qiadnxon.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3gfxsijbf.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3ntmrqwoz.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3qjzzwlrw.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3nflfftgp.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3wdpumglr.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3hhctsgxs.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3hdttlzbk.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3uecxltxx.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3zhrhqslr.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3hgknquar.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3tvvrqtab.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3vteuwtsa.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3tlexnltf.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3ibcgdlge.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3xplijqin.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3xloiujjm.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3psfkcocs.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3ublhowli.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3gvbbgchn.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3saasakmh.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3ctoabhfn.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3gkusgthz.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3ejepvplr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nlztgope.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3rkktltki.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3elbvblcu.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3qahsaems.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3jsrxszei.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3rxdzivzr.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3kmttgfdv.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ilegzfmr.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3rghzmyej.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3tlnrwfan.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3yeaoqlcm.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3uzjkfmxl.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3pcdgdxaq.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3ijryhnbo.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3pplvocsi.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3fpsizcqu.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3cvfzpqib.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3lwcuzxdu.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3dzvdpxxx.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3gvarfebw.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3tngqnucr.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3ohgkuxik.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3xjrnivgm.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3mridpygb.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3cjoijyiu.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3vukcgoly.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3bojehwzm.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3xcanqtvs.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3jkbxtswz.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3mqlqgckx.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3outrxlvv.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3stuzxohp.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3vxgbmrre.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3gwvwnzee.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3hcducpgq.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3qfizeycj.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3mxgeqmps.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3ozqgenkv.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3hrhkutnf.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3qwpsfwxx.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3nmqbuboy.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3dcrvtxky.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3eckqdnjm.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3budaupnd.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3ouciodoh.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3fjxvoucs.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3cdfteojx.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3lgxntaay.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jmuocsst.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3spkvhxbl.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3bzfvzvqo.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3xmoguslj.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xsrillus.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3lrgidzup.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3wjtiuuka.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3zrbmmdis.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3ymhuthge.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3qoeaqvoq.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3vzmrsfgq.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3klbdvgxi.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3cmwswecd.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3irrbevnf.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3hmowamhb.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3edszuigi.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3ckggxapg.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3brzdayca.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3bqstrhdm.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3cwwklsfb.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3vndotudo.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3qerlyzfa.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3brxnckad.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3tpbntmdo.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3yvdqeeef.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3gtnozeap.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3yfopdwil.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3ydtqpvba.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3fionbsaw.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3dceoxwku.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3cogbhwne.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3yhpkyllb.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3fptipthu.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3vjchszuq.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3jxpgqqps.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3nziwjrfg.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3yzedaxer.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3xyxxsgcr.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3zuordjkc.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3kxwntbtu.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3ehinufqq.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3wzhiybzy.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3bgirfiuo.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3bnmulefw.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3rfxjcpyr.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3znjbpicz.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3idqplqaw.html


<!-- 参考信息 -->