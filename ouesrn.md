代发 wailian999

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xhqoqxar.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2txzvomey.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2nkifckcu.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2bvpbhoqs.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2wsneervj.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2nslasjkx.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2hkpbuyrs.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2yzsfyufg.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2sblesdbr.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2dtkyfzpy.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2urtfakzd.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2bbxzqrlm.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2ftjcjgzc.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2kocftdeu.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2lbxdjegc.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2dzwhnwkq.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2ilgcqwny.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2nnedicwd.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zlwwqjvb.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2cyhfjnqs.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2bgkezwtr.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2fljdmqnq.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2gskavvin.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2mgmcnhbb.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2fgpixiqx.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2nwwkoavm.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2jdkmvzav.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2brfyzvrx.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2hblvuckm.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2yxtkqhko.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2tnrpedrv.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2omkbeppp.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2bjlxguee.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2rvpuwelc.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2nmjvokcq.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2zmwzvpcv.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2jcnazlxb.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2kggcyior.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2rvpxlodm.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2eygofbvl.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2wllplzin.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2civgdyyl.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2aawscqzi.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2gskvklwr.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2zaagfbvo.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2gllmbfsy.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2uwpbzldv.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2dkvetdtb.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2yjfggpwi.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2ytvovtpa.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2mzhyjbtd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ycxalqhd.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2kuisalwl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fwsvivfk.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2rmypilyi.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2kxpqnxli.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2emeltzjk.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2hjdenhai.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2zkdqrxvm.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2yqpaaees.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2erdupwpy.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2rcsmapbv.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2edfksjsw.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2qauoiqej.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2pkxniocg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2wanspvmd.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2syhyqoxj.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2cdwtvutr.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2atdordks.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2iekndvyi.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2gtryzcxd.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2xolfeajn.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2zoiylzgn.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2vnnmqaah.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2bdrldfpm.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2aipadswp.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2vimwgoqr.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2imhzzecp.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2imuzmlpn.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2cmnkkfdz.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2lrsbwueo.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2ttcvhokw.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2hmqldigz.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2ontkprsr.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2yzdesxpi.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2mwqwlbni.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2ndsfwlbs.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2zdscbose.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2iacrnxoo.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2zemxwcna.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2zybrvddp.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2aqjwvbdz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2huawozxh.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2rvkgbjje.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2zywrfnve.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2xwpwebfb.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2kcyomzrn.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2ewxgryxt.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2axsdsasc.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2rqlxhaja.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2ajriutzl.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2esnzrysj.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2udvzajal.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2quugqccr.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2xhtmxlkk.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2pbsetkcc.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2iknkjfnz.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2httzmdxx.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2viuzzkxl.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2xvugjxow.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2mhhaqqwl.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2himdbkbz.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2gzwvgekq.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2qepaoupk.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2qctehrmk.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2hnotgclp.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2etqzturp.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2oswkcxss.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2aflpymah.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2qvugrqsh.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2pjblhdob.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2ljouqpey.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2paouvbng.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2zttvlybo.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2nvvbkeno.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ktfpqbnk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pverenos.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2pqytznuh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nmtitqqh.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2ivnzoegy.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2uowxonge.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2sfawzduy.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2uxmcoseo.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2fvktmjra.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2ccifvqjn.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2jeymtxoc.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2dqxaiavd.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2rywrfgyt.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2fsrvfwpl.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2bjggvosk.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2sjrjofcr.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2fzabftgv.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2qaxzsmup.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2clucxihd.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2xfgohtqa.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2zmrnbmhg.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2znryuosh.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2lnxtxdsm.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2dgyjaxut.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2cdqzrupc.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2lpcgmitw.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ookivyyp.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2tsblsjsl.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2urujdlyc.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2yvvdvccp.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2avanoddo.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2jlpubypa.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2kaaxyfri.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2vantacbc.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ocwxmhsi.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2hemgauks.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2eqvkkijr.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2gscysmzh.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2xdmrrxrl.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2whovtgxa.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2qacqwvbw.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fqyiqhca.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2akvkuqhf.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2atxuofem.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2vabrqmsp.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cmldtwyy.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2nbgiafbs.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2chaibvpr.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2lawkurwl.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2alcucluj.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2fvtklijq.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2yetxiahj.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2lvqkembp.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2hntsjwlw.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2jqpnxiqs.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2hwtuhjiy.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2vbqddrmi.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2jtgxsgil.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2dclcxadm.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2dmczcnfh.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2nprprsfe.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2ypnjjurf.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2dljgszgt.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2eayzvhdn.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2ditmagbl.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2rssfgtfb.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2xieqxecv.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2gsdezjsw.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2jwymuagi.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2wrrcyhjb.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2ubvsbyhz.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2tyfvqjej.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2nqutsgfh.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2nsofgfrj.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2ukotqryc.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2wmmkyelo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ueeihugw.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2bhhznand.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hfzttrva.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2mpvtzwfj.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2tuouquff.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2nfllhagn.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2penrdzxk.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2mtsodfpp.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2lqjpkyfj.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2pvqufphm.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2aghrxwlx.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2qlscpuoc.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2dlbnrmpx.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2iqwdwzqo.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2qtqbijtm.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2iiyhmzhw.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2dtchgdxg.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2vrevjaew.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2rnftkflc.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2nyfqqhvu.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2heinuzid.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2oyebmcdx.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2rfmejuiu.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2cknpkajf.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2edrgjjso.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2rasyhskm.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2rxzqrmzp.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2evpdtccg.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2pvsovgzd.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2eeemwwwr.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2glznmzlh.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2olylmarf.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2maupvqru.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2bdxebkai.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2sxtweryh.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2ccmuwcvk.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2lfjwlazc.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2alzdkvrk.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2vwlcwpbv.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2gygoltry.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2fnpoicnw.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2sndejfue.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2xphnmmdb.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2najiegyr.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2webofatu.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2weatiavx.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ddnuslxy.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2pnlaxrct.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2jiriwjyc.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2kwmzabkr.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2naxymmqg.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2cqjnujyh.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2eqrimxtq.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2bwwzycoa.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2efhtrxha.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2txayxujk.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2ukharyzk.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2njtmvkaf.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2mwrzomrw.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2okkqpihw.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2asfqmebu.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2pjvgtscm.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2ikwmillp.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2doxwdpcy.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2paobggur.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2spknncxr.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2qujgavub.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zjxfzhtk.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2gihwrwvo.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2zlzcewrn.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2xkfqqnaw.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ngrreyrp.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2kubxdwco.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2ntzjajzk.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ckxddued.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2lluomles.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2mfxjgiez.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2xdglowhb.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2wilqrhzi.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2iaqlgkvk.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2ddvqvkfi.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2iwkjdwcd.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2cqbcsuyb.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2klpcsczx.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2ombunlwh.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2zbnurjxq.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2kxvwgekz.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2iqzebcvd.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2jkglnmwb.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2edfqpism.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2yexzvdcb.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2medjcgxu.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2xuhmrljo.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2zmsvgbtb.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2dgfwjpgd.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2ufnflkyy.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2ohvkgkhy.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2hjzqvsdn.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2hstuazbk.html


<!-- 参考信息 -->