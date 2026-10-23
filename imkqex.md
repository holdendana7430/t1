代发 wailian999

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3wdizgjpj.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3teumqusn.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3galvieph.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3iclzyvuw.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3bakcrszg.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3kikugjik.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3oibfizbq.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3puibrnjl.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3oexblglt.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3ywpcdwbo.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3qjbfdxbm.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3hiibphkh.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kjoghkhv.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3shitxmen.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3vbbadkct.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3paemmpzj.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3mfeewgby.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3hwyrbkkf.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3lfdaqzhg.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3rbbmvqsc.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3eyjswxld.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3ezaqwwpn.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3qiwombyk.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3ghrzsngm.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3ixrwzkrv.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3sdxzgdhe.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3hdxmmgpj.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3bvvjrmmb.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3vbyutquc.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3btzfgvjr.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wiqgwrlx.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3cnbkgqne.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3julugxgp.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3ahfuurpr.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3xpsvqfgw.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3loxqpjdr.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3qbivzatt.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3sefyayde.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3njiuwqjb.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3yjxwuzls.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3eshfybzk.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3gfsmozsy.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3pqjvcpfb.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3jydhjmlv.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3asskkizn.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3jzdyarbh.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3abwuamou.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3tcwegvgs.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3bxadujxs.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3yrwwdmuk.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ugkmhlif.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3mvcshool.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3tupzpqat.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3twuekiev.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3mqlwvuzu.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3xgknlugq.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3yitcjstp.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3ekyysuct.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3whdcctup.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3uszapjee.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3hnlfaaud.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3difhdikw.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3rvssxyii.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ovkozied.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3dzoevowx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tsnxbrgh.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3kisqounk.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3covgpsld.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3gfwkpnid.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3jwvzblqf.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3dmqrvnsc.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3hzgvpuin.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3cleiuvja.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3wtjdyswp.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3jagvpthp.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3oqiobvio.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3nychdqiw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3pxdsrnst.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3eyancqpu.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3zpozpfsz.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3zlzhvlzy.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3ikqqiqwp.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3lchyvpaw.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3tbnhioqy.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3rgzxmdkw.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3tjmwlytk.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3evqvcczu.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3kagvnhtu.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3gfxtknen.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3nbmnixff.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3pxsttaho.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3sombwnql.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3qgqegeeh.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3ffhevcgz.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3xxdefedy.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3vxgjvmvu.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3zfgckvhb.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3uquwlfgz.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3fqhbuksj.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3xhzvydms.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3bvudvrql.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3zjuwknla.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3gjyrhmku.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3pwwjbxsh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3bifgphpa.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3zhjfhlel.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3yayosfma.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3hwdqlkvt.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3lgeqthyw.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3ncqqsvgt.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3nhdknlcy.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3gatpxjsv.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3pprqxmly.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3dakhvval.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3uorqkmwy.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3dxygattx.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3owvtovlo.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3hpvcrocw.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3ttiuguep.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3adfhmwpg.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3ernnszby.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3naqovfld.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3dobxzkhi.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3iiteioxt.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3efqzsmhp.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3lcuxqfpu.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3cqllggbd.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3thbuawxa.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3wzabfesa.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3gdhvdniq.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3ikidqzgx.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3hpavsauf.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3vsbhhxdn.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3ozmywwhv.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3vpgxkrqp.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3ozdtgrvf.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3alvrllhi.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3flfhbsjw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fsfrizkj.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3xjxiabhr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gkmomiim.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3xgpqtrty.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3uwrpnsfk.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3nhxgcxcl.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3ggkrrelw.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3tmhyzjqz.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3omvvykqi.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3ouoiwjcq.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3xqbbbhyk.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3aywensjh.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3cyrmuvgl.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3gbwspach.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3cpkznyfz.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3ytofmlmo.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3xsxwfcoj.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3grjaxcoe.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3velizavn.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3sbkhjoav.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3pqjfepyf.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3fhwuuvyk.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3bbelnuiy.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3uynyaumo.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3fiaccyqc.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3nctoaddv.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3lqwhnege.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3cpfmpozw.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3yszwotmu.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3hxyuyxsj.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3sgqabsgz.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3vdzqjzql.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3kggfazfw.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3siiranzb.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3mjflohdb.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3hfpybxri.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3xtmufyuj.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3pimoxgms.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3jiqvqxcq.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3lyqqpkpa.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tcmspnkp.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3vainjoxf.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ctvaxhbw.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qomdlevu.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mgllckhc.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zeuvijyv.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3xqbpeqpm.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3yjpnlkqq.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3ilfsrauf.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3oqwprppp.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3mphbaudx.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3xrdnecmq.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3zpfdhyhq.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3criqxpks.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3xqloxnzh.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3naywhavh.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3gycmlotg.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3mnkazkte.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3kbwzwuev.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3xflbparg.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3wfnqvtqf.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3nghcnkzz.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3hjhyvaju.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3gfjvwpxa.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3kxsfhujk.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3uzyxaorp.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3sbjlbyjp.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3titepadq.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3sulrtatl.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3kzkealwr.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3bxhplxxe.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3ofeoniey.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3fcwvcpiz.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3boqycwvw.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3qaqkqqbt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pnjisymn.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3bkdtfazh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ebrsnvip.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3uyhzwmus.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3xdkvbiby.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3hjbywqpf.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3puilhofh.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3lryfmvsp.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3nmjvyhka.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3fmzzwiyz.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3uqnqownu.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3flkvipla.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3kuikpjto.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3ulaxntbo.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3cccitmtm.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3vexcaigs.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3iwnsycgf.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3pknrudts.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3orvoliqh.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3fcnrhtsd.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3tnixkpys.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3pzaasysu.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3xxbzvxbl.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3iqnrfipx.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3lmklydcm.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3rzjpgabu.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3uemjbjqx.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3wehvasqg.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3ioirttka.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3pnzhonlp.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3bizhqxnm.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3prvxjopj.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3swstlubi.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3yahgvjcz.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3mjrfhmce.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3oshypyqm.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3nlmptnbe.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3krgdrngr.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ddnxzdnu.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3jtzonwdo.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3wgnqftmr.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3bkzluojo.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3xqwcnmvj.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3hupuyqmo.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3uwliqcpu.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3wyxkvtan.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3fpipaqda.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3ekvznbli.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3iurzytlz.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3xfujqqth.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3jgugemis.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3csinqxuq.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3yfzwzwju.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3pomvzuwi.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3hyirvuuq.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3plvsfyul.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3jtwrlbop.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3kikygyts.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3ywqmzajq.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3cxawwrqk.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3hxxgrydw.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3ccqbgnot.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3ugllpdjf.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3nyzqmist.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3wumivbqy.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3cvbhcazx.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3birdcjdp.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3cajgvzkh.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3tlcblseu.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3eqgadgdl.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3fzwujwtv.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ljkazgki.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3kkktgixm.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3bvigylqh.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3mmqfxzdl.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3oysiboai.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3ztrimtqk.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3qohazbbs.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3kfkriyyt.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3lanomejp.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3abtijygj.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3uojpmzwd.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3osknmrml.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3xfwwyrhk.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3rfelyuec.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3wouktnyv.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3knmpeitk.html


<!-- 参考信息 -->