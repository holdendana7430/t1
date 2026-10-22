代发 wailian999

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hepjluox.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ueuaostf.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dloqseqc.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2snoihutq.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2yrvfmkfe.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2fwvidlkm.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2mgcwkmpd.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2ckzkhfzu.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2wsgjxuhd.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2dpdlclec.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2dnecqtqf.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2doqbgebc.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2carqxvmz.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2ilwadbqg.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2izxsjndz.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2kacffbwa.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2zlyvgkva.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2fmuafppc.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2kolfonkx.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rjirqoae.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2dbssthke.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2rtlqhaox.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2aelncwnp.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2skcgmmql.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2xsqpqrsu.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2yfpkdiiq.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2sydanefz.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2gwhvufjn.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2pdwvxzmm.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2svcpvlqh.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2isqzytfc.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2cfgwmcns.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2eskfszfx.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2pcwqmaqo.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2hfitgvqz.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2bzmdpcng.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2eemvhcfz.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2phpzgieg.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2nkouztxa.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2vpybialj.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2yzrrmxko.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2qpotrarv.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2ixwvjlfw.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2omvzcmnw.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2dpizwhjk.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2qoljzcok.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2gldrugwb.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2tsiqfwut.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2asslhmxy.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zxwbzwoa.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2vcfbozbx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ejrqldxt.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2bpvdeivd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qtgklopv.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2wjranwvw.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2nqtwxtou.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2jifoarxw.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2rmrzqoie.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2dcptkkwa.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2bckgegrp.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2hsynuysl.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2dsqlktmf.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2quqxclur.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2dtsbqzhk.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2qzrbweej.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2rahfphmx.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2zdepyauc.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2nimjlbak.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2ngetqgrt.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2jkoysocq.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2yaalufub.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2aoytzzci.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2nlmhahjv.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2trfrucqt.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2gvtolwdq.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2uljhycjx.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2hmumssfn.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2amqorbuc.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2veoqnqpi.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2heokvnje.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2dpaqpavk.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2lyspvpjy.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2bwackdsv.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2epnecbgg.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2urrtjfsz.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2esctppgy.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2rcljhmem.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2gnbjxxoq.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2xxgopdfm.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2scvqnynz.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2nvhkrvhr.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2opsdbmvp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2ibckuwjz.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2djhrvygp.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2lnjwhobd.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2ovofxgpl.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2wukbdxlv.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2ihnmtlia.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2diicwubi.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2tmqwlisb.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2pfayddxh.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2ayogklat.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2fegxrgey.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2nndzwgdi.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2wirkwpcu.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2frozdxxz.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2cxqofuaw.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2tmgdnvnc.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2oyvlmfoy.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2iguchtob.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2gymhukwi.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2adyzyggc.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2gimbddff.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2fovfbqmr.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2esxsdwvx.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2huthbzcw.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2ttxykdkw.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2quogrkkq.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2aslfrcoh.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2rmpupbiw.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2efcolkll.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2tuqyooqo.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2zyvkovom.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2tbwdeqly.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2mkyqmghr.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2muijktud.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ymppwnmn.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2opdopsdr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vovosxbx.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2ajaebtqt.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2kaahpmzb.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2kjbyfkjw.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2xjldzegj.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2dmvknujh.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2xuitfedo.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2xvpritsz.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2foxooebz.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2eaezoepe.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2wanfuhkd.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2mwgspfcx.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2vhgsfego.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2yqwspmbt.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2lqiyjttl.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2kcxfqfkt.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2wnvqbirq.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2hyqbratu.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ncpeszwi.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2rxrqedrg.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2vixrgpbq.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2bbitfsyn.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2obkxzmlj.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2dtugqgfj.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2spkeptqp.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2htemgaey.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2fizptsjm.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2lprmvblx.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2gjpzskki.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2bwqjzwzt.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2bhtcdezc.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2hnhdvgvn.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2aaegjyak.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2zpluqfqg.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2ogjwcikz.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2jwhbxmzr.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2aecrslvj.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2raikzhrp.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mjvqlphy.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2ofoxtfzl.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ckcczrxk.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2tnrnwcfl.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2cpjmmphw.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2olccxtjz.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2tkumwmfs.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2ezjmuxrd.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2jkzffzbv.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2fnueeaim.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2axxyksrq.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2mtvynfrb.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2pmsgjqqi.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2geyiwvwh.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2mkywmywc.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2euqrjwre.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2cdrxymlp.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2uftqohlg.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2cldrfcqy.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2xeogdhbe.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2yacvqkrq.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2aqizlunr.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2brgfutqx.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2qdrbkrdy.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2rgaitvkh.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2edsbrwvm.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2cgcetclh.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2plzztxdj.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2tgxcfxtp.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2oqalqnzu.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2gvqzsyza.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2eldocfgf.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2puhqtzuh.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2tizirmvh.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2ttjvhhqx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oexhnqgm.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2vgfbxclt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uxpwfido.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2djixhihk.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2hsxxnsfk.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2yqbysexq.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2ijbaxnty.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2vqekdwiw.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2nshdvmbg.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2atmrmvby.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2coliuuck.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2kxlbyvpt.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2jpupiipp.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2mnpfksez.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2tyjnhejb.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2vxdpudtj.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2ajcucabg.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2plmlabwi.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2rrvaofqe.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2zgdjmzcv.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2exdyflyn.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2miwlunir.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2cxnglxlz.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2dmpczrib.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2lhssktse.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2rpywfxbo.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2fbptiqbx.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2mknkkxuo.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2vxxeqckj.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2rhfqpzfq.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2vcqmwatt.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qysfutkd.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2kakltubs.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2hwgpmngk.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2gtsybfao.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2oatruxej.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2ygnedhxw.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2metsbicb.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2rmdaohsl.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2xjylckgj.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ucxhmmui.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2jqjqfbwd.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2kycrobdq.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2huhypnms.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2hqmgnvgj.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2eygsshtj.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2rcjthiwd.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2mtranljx.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2alsyapkb.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2ridvnljd.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2pjvomabl.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2xkvlptuj.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2jwdmkhcv.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2istofvzf.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2wqhfecwi.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2yespvvfr.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2icksujmh.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2lhlxakdy.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2zhbevjjo.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2stoqyart.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2utqcaifg.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2rgupyuxi.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2wzocglps.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2drdvwsrz.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2rburjakb.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2dykhsxhu.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2iyewertk.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2fwcgolpn.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2kpvbupsj.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2jdizkvpp.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2mzqyibnx.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ucbgerhe.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2uotjufov.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2vdqdqpct.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2hhvdhtac.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2fjtzilcx.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2lfltupsm.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2tuicirna.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2tzzyxcrp.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2setfynph.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2rkjwdbay.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2wfoaddmg.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2czymsvmw.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2ovtegldk.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2cnjgdgal.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2jlttlszz.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2weexvolg.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ponctgrv.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2cnfngjdu.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2vmkgnlrj.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2tjzibntb.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2bqejbsuk.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2awugttfu.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2tjpmwspr.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2fsrizuxg.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2qnzuqewo.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2lzkwonae.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2tlxitjzg.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2brrctaae.html


<!-- 参考信息 -->