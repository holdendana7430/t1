代发 wailian999

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2bbptljbm.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2ppxvxwdr.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2ngvqqbix.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lmqlvecj.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2mxdnxnzf.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2pdyyifwh.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2nsxzmvnu.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2swestiue.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2nagyzpoq.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2xwdtlcdk.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2ixykffqg.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2gitmgghi.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2majhvmxd.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2jhswmhcn.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2xoyofdzj.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kssxjavu.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2efvqakvz.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2ilamnkjb.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2nhqdkzhz.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2obmgxsfp.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jxfgxxdx.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lneglarf.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wapavcxi.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2tpafdkpm.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2bnehsuaw.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2xphalaga.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2vakvsxrj.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2bwccpcti.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2itoaauhe.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2ktwdbvmj.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2gvpkwhtd.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2ovhkaaji.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2gcshffpt.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2xcjtqqyk.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2owsoxlbp.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2ubokpmdv.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2mkkdbqug.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2nwpqvzfo.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2yvwdkzli.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2xjxjjdzx.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2wixdwffg.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2gdnmmmdh.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2ihskpxlz.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2qxcqxhme.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2kgyppekp.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2gnasqzqn.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2oxoxowpj.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2vyoeqzjz.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2rzjtbysv.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2alnnmrci.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2bdwczebw.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2kuucsnid.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2wyoglcfz.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2vzmeukhm.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2mahlayob.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2kidsmknc.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2lrfhlhhf.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ocquipsl.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2gedlelwu.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2mcgflqjv.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2cayiyjxc.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2jpxsdwss.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2udxerchb.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2yycvzmfl.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2qhtqbhau.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2toczrgfi.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2gptyfqif.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2czmomksd.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2plhvyjhp.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2hraxujhb.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2wepgraxe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2japukfms.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2shzqckll.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pxkskyhv.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2bnnzqhmh.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2jjmrbuau.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2bezlzsxo.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2zghezvdf.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2jorkwbhy.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2npdsytdg.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2lsaigfek.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2ijlggbsd.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2vxkwvizc.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2fvknivbs.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2rpymprux.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2fhdbycdb.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2zknszcmw.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2ldjkieah.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2kacuizwi.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2gqmhkcer.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2pwenwqnu.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2xjiqupcs.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2zjnlwhvb.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2zlhmshzt.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2jjvvkemy.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2uundbprk.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2qsrpfhtc.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2krhmenuc.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2ehyqixka.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2ovjdewuw.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2qmpyceju.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2jooqacee.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2gnmfjoan.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2wetismen.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2euckyszu.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2mecfjjmy.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2fdnveuao.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2bogvksid.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2ljdvkynv.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2eznxjiab.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2yeeackxj.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2kqcldjyc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2vpbpcwpm.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2ijhwdbcp.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2ilgdtjjo.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2wsecfkmk.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2vbpwcmsv.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2ncuuajyw.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2lvttfzcy.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2zgrzlrfr.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2qvinedfp.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2vspfbuhk.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2fuowyomq.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2hxygjkbd.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2danolypd.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2ozqdjibs.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2foquidzg.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2raofaxmi.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2hgzkwbzi.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2fjrvkbmz.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2btfulhvp.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2saqoattd.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2yqzufmgu.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2oqnadqcf.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2teuwwgzj.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2dnnrcpfd.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2gojitvgw.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2eleycxmv.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2nhdjuosd.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2ftjfzsik.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2enkbjlpv.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2dkxgwwif.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2lfjuiyvn.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2qatkwkrr.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2tzkqzsnz.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2wijagpin.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2knfnwtth.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2gpwkvhka.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2opskteyl.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2jkdmkbkt.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2xfvypzqj.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2fskjafys.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2gawhuusx.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2dezwjiyo.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2lwvebrtb.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2yulxkfby.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2cbhfprwf.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2pymneujj.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ibdmlrxi.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2xlrtlrsq.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2evalymaq.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2twhyaost.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2clvakuex.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2fehpzaow.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2xlvpluwk.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2uylmqmek.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2hhqtlvxw.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2mfbblhty.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2yytcjnzk.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2vchehlqj.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2apvqpled.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2uaabdabl.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2fiapuwsd.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2vaxwstim.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2dldlwzlg.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2rptfjxom.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2pvelzrzz.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2uddefqmu.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2zbkyjryv.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2kyrvknto.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2wzydflsl.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2bgluffml.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2mfoqrpbg.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2gmlkhriq.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2htiunquj.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2cmfhuftn.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2qmdcloij.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2kswljamc.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ivyhjbbp.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2dkwkhwrp.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2bupgmrqz.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2rnxwwqwy.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2waggrqfc.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2aszjkoql.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2xchbdyff.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2awpjjdnr.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2wsdtwexo.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2kxtqngck.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2vzvzblxt.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ibbqqxdy.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2xrgywwsh.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2pwtblcqj.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2xuybqajv.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2czeuenaq.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2vhincthj.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2efquzuhz.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2hvtvfttr.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2fuhdlcgo.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2jufqwqte.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2xdhkdklv.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2llhhmtlg.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2ddiaafyx.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2ynvgzbbu.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2dgfhszzt.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2kgtumamq.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2pmfesarx.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2gluqsilc.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2phdcakkn.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2ysppxehh.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2qyhzqmec.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2bouhchyf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tdkeuibr.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2zvpackfx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vsmutgwq.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2pcbslpep.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ghrsjyuz.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2zjbglrwi.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2khxorwxh.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2jbybeurx.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2yrhaavyy.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ognndyjn.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2ofusolxm.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2zcnougqr.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2yjyavfez.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ksjapslg.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2hsmqklrj.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2gxzatdrq.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2irtsfdng.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2haxihkfs.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2yiydxgeq.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2jzdtxrpm.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2lugaqfpa.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2sljphtcq.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2mhhuhzzc.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2pcvgypio.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2gvuffjrz.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2rfjipzfk.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ghbdpvku.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2wfehumpx.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2spufphon.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2vrpzudal.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2dgkvcsto.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2qcugreli.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2vklkvsod.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2npyekunr.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2wplerwqv.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2ibwyphdu.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2klewwkke.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2gnybbhkb.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2ntnmijjm.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2vfanavkj.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2gvylphmb.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2slxcjeaf.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ipkrrwfu.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2hoaqnzoq.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2pxzggxha.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2xnzkyhdr.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2oczdwboz.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2kjyhvszu.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2ntukxody.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2riqwvjdq.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2kshylmem.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2remhponb.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2icfbcyub.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2kydiybwb.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2qrtwtedg.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2qqzdumpb.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2kkgqnprs.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2jkabvvkv.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2ozlrxfks.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2qxgbgeks.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2rhwvjtvx.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2dgatqkmv.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2shtykrwh.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2ytvmpkho.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2cjnfvvdl.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2lzmfovvj.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2dktuqfna.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2mdwgesxp.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2xmbdxbkb.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2xhrsmdww.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ytbzsbjb.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2yclmusoo.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2elymozvp.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2qjjbajnu.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2xgyoexwh.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2whorncvm.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2qveqvwxo.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2flnkelyq.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2frlydbeq.html


<!-- 参考信息 -->