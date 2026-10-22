代发 wailian999

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2nholghnk.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2wiwbsbaf.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2tskwhkza.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2lfmkfcto.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2xfhkudws.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2otytfuwr.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2accqeofp.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2alnedjmn.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2vwqhozsr.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2mpilmnzk.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2aqcbysln.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2fsydclgz.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2meacvecb.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2exoqjmej.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2tdcouwxh.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2snjikonv.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2jxyeshos.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2uqwuzchk.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2relmgcqs.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2cnlcyyhd.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lurmwlsj.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2ldjvmjyh.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2cxybkaax.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2vgucoaqn.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2hmcebsah.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2egadvhqu.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2gswgyqef.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2nrghfpwu.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2ctbxmzer.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2dobkxghj.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2zezujmob.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2iacexdnd.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2vlwmpath.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2lpiqlfgc.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2cahhbqvc.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2rjqglcms.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2yqgwcfyx.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2nrimvahk.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2hnwticvm.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2pfqpbwxc.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2vxdwyewy.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2svukxzxi.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2sxgmxnfx.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2eumbhzcw.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2mohaycdk.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2rsjvhfjs.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2gwtbqtwn.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2toqyehdu.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2hvozsxjs.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2dhqbclxp.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2foznyboe.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2cefxsgpj.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2cvbzponb.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2nmuiqsig.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2dtoqpgsu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yjtfmlro.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2kcpusqje.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pyhpdtll.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2emruwtcg.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2twloyege.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2kphpuyrn.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2hkkhqaex.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2gtdpfmfb.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2jwquvgvc.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2dlfxzvrp.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2ygdhbjre.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2ycyromri.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2euqfcnif.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2mfswsaoa.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2kluerlai.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2nyuoukpb.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2ifxqyuit.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2gwuxbqaf.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2gkwkdgdv.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2vlfdyfbf.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2kpisfmbm.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2gmgdxgwi.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2vtjtheyb.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2lnysgltr.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2cbdhbdqw.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2mxieobgz.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2jjuksxdy.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2chpabtdo.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2eilodgch.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2mlsiughv.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2dlecibnv.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2fbiahlnn.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2oftykozp.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2bgiigqvw.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2qlkqvprh.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2pceazvag.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2efwhkgmn.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2moollqbh.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2kvpuisyz.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2oxhwdeck.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2lojtcumx.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2jsqjddms.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2mlauaddq.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2pdpbcujq.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2iingcsoz.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2ixicnhqf.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2htveuqju.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bzbbiltx.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2rvoovrlz.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2kaklpgms.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2hlvhlnsw.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2muaphror.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2qjebkesg.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2lqyxzgki.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2vwdwfvcw.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2ieggyryd.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2zqvryjjs.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2zqhekyvr.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2igkahwvr.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2pdmnblff.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2vwdkbfzk.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2teerofbe.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2jherllva.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2fiuzigyf.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2jitdpvvp.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2vyonnwxb.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2tvboeifj.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2yzocrppx.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2qjrxntak.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2yxgkdlcb.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2dzawjkue.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2wxawfpnb.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2elhkuchm.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2gawkrdsl.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2enklpyxm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2evlsaiqj.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2uzxwnsus.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2souxxjxg.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2gjjoceby.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2iokpqfsi.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2fvebytvn.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2txdrgsid.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2uyunsgqv.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2qnxaxdyw.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2uvlvfeck.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2zahopudx.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2jmkokjoc.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2vfmgvqvv.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2vltycdfh.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2yiswlxgq.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2andktdaa.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2opnpremu.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2wzxttzly.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2zegvhfng.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2yrvatmxl.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2khvrgeao.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2mmeujsbk.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2shtlnbua.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2otzuwmll.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ozcggklo.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2wthaqqsf.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2tktydvwk.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2qkwecven.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2ckpzsjvs.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2dbnglvrq.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2mzcimxev.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2qsmrgokl.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2bfdjolpy.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2rgtfpsup.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2awjloalm.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2jhzsobyq.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2psdkzjnk.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2rowpvgrn.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2dzategwv.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2cjuhivkk.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2epydsquq.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2lqzxrenu.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fwsjtzux.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qdrlkycf.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2eadpczol.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2slaofkmg.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2zeaxbend.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2bzoeamga.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2qwvjktcu.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2ncvucdrf.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2sbfjqrwu.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2vavxcyng.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2lxuifgsm.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2inetbcjt.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2wbrhxdsl.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2gvhtrtln.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2nasuposa.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2kjjzijph.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2hlonbxgm.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2fvbplokv.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2tqxtfiys.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2xjjgjjhc.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2dkjicjfi.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2odxwwkqw.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2pzwpenhz.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2ycbxsxkj.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2viepskef.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2zdwxwcof.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2wsqiuarz.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2bdttzvsy.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2ldyerxws.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2dzseknkk.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2ivrrgzue.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2czhxvosr.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2nsjphgba.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hixtilmk.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2mjeklqlz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mktuooua.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2ztkyfmbc.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2oovcbvrd.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2opzycdxw.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2drvfzexe.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2wsewldsu.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2rvhrhoom.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ybnqxzzs.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2hkqnclno.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2gzlaqqsf.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2aldzydkt.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2qhqbpaig.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2pztkyjrh.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2mswbeyiq.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2zqhatzwe.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2pkvkbctc.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ptpznbsm.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2flpauqbh.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2lcylcxsh.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2srvvqydk.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2vhvoyvsy.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2aaipxxxb.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2vgwregoc.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2tmaejmjj.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2dupbdkfs.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2kwyyqlno.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2vfmkiyqo.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2yuhmdfqk.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2sqdgmfuj.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ngazswmc.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2tpllmxzs.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2waentitf.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2wertqqpd.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2vfwoawdw.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2sxgsjhjv.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2goricflm.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2idfukylh.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2wdikmqxy.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2crjfufoh.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2juebdisi.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2uyauxsyz.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2ovrtyngx.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2rxbdsvni.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2zthodwid.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2pwuxzkxd.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2lrakdqvy.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2ivirxkwl.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2xblzlvcg.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2ssmohvxr.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2pvjrmhno.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2dovehduu.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2psbgjafh.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2wypzafbu.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2fhrxzyfz.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2kcyjcueb.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2ofgaszrs.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2fbppjuzt.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2auapcqtu.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2eidogkgm.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2hvqeuaqa.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2gbczeigt.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2tgeelybz.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2bhseatlc.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2ilvdupru.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2pbsdvucu.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2xbwsdexs.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2ztsnnvwo.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2myvcowpk.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2mseyaxzv.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2qgkvzosy.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2yfxovdta.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2qalthasz.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2cwenophr.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2ruysodgy.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2tmbhbbfx.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2unwrdwil.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2uqaadmxp.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2gdpqxjto.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2aaywzpit.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2asubufiz.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ckmtskdg.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2dafrhler.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2cnfwamez.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2ffvbzkdt.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2ldqfmmga.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2zeduvyrs.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2wmekqinm.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2bmtnlxdu.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2nsxgjwwb.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2dnhzhkpo.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2ctwapdaq.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2udcejjbh.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2nbkcnvhz.html


<!-- 参考信息 -->