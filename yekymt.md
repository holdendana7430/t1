代发 wailian999

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2urcgfwix.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2edmmqvfm.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2imahkidt.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2yjhkbtpi.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2howeebpa.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2oyedpckq.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2szsgbeiy.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2xrkhmxlc.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2ykpklcwh.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2ckrleipg.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2crbkcdje.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2xvsrubme.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2veunyeof.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2tmgkhqhv.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2hgslyhye.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2twzsnkma.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2fhzjayzn.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2cynhmjry.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2sbuthqkf.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2mbluaemz.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2hpaqxtse.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2qidwyqlg.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2zhxzhrxl.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2otfojqra.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2qbyybltn.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2sszpihur.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2ccsvkafy.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2grtldojp.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2oopaalat.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2zehlkbjr.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2qoaopmpl.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2xcfajdkm.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2jxzwvjzt.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2pjyeptmz.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2noghazwb.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2dbbwxdln.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2azysmmga.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2jxgiqvlp.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2bdfoxcmc.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2ilbgaatl.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2oxmiadnk.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2wvsovaen.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2pkwghxrz.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2nisvvxvg.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2fxzlerrc.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2uhvihsia.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2xsynxfik.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2prfsmbns.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2qjcgnqbl.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2pldmajkd.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2pwlxubxz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zovkvlqd.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2akwassmm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lwdfkeqp.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2jyrcvcwt.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2uvstldgf.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2gsygftry.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2ztvlkrbw.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2dsmhzhon.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2ofvyfcjo.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2gcubgolz.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2zmtfljsh.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2pyldjaat.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2wmrgxbep.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2rpjvmaqk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2gsctbbga.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2mtqpqxqo.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2couzehsc.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2nnmvpbkl.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2knjwwjam.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2tjogxmuf.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2vxpqxvri.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2fglugdxw.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2jctsoklq.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2mfmwpfel.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2weossjjh.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2jjneiinn.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2pcsounyb.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2ierlvfxg.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2qjlfnttu.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2cspgbpid.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2odwtamdq.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2bsegkmvy.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2syyilros.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2mqmeiunc.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2jwbdfccs.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2uyftgyyt.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2kocodxoq.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2lnwttaeo.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2ruecwlng.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2yzlhzfwy.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2zazfddck.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2bgouimlq.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2fmonjcjv.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2dekauhfu.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2zzaenaps.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2emuunxez.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2jeixngra.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2raqpbque.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2esncgjnr.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2tdsztpor.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2rovyirkn.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2xermzfjt.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2ppdpgokx.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2pjoeheji.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2jeeitswv.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2snqxmhkq.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2emwbhyfp.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ziqwiluu.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2gkegdhta.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2jiixjffy.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2evdyjqui.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2gxolqxax.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2kxbxcswe.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2lscvoylv.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2tihyxlhe.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2diplcrze.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2iussjssj.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2lzemgiwm.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2racxmggt.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2plajmahx.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2zzqpfzlu.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2nnnosvtr.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2khkjhbgw.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2cyyhzhri.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ngivzycd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rxzuunip.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2yveoxskt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sojqimmo.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2dcsfkgxq.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2uraobeqw.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2uwxvzvpf.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2iqqfkbbb.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2clcbvazu.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2fjnfztti.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2bzxpibcr.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2xmprheok.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2wvmchcey.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2iatggrcg.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2mekrbacu.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2murxxtaf.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2vcfrznbq.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2ubkdbljw.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2pnbygsks.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2qaaxqqkx.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2uceivqzu.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2etxaevsj.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2ivxzkjgb.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2vdpvmwic.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2brucwupf.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2otmjqzhy.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2seoesakm.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2ezsleogz.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2ycdrznut.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2dfrkygcl.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2gyekmwis.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2rtmchrlv.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2rfnzdybl.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2rekrfdph.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2isofdojj.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2oihhnnio.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2khlflhcd.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2eyypxrce.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2tgvapgxv.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2hymquixm.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2slopagej.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2nxxelwzy.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2gurivujt.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vmprktur.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2vryirniv.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2iogsdzam.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2nrlkhxuj.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2ndqercex.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2ixszrerq.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2ubrnaaxs.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2lwtzmbah.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2hjanrqly.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2fgrtrfno.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ttoliqjx.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2jnmidvls.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2hlqdhfsx.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2nlvnvgax.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2fjspgeze.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2jgzirgrr.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2ykyugyes.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2rluxkrbp.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2ofqzijod.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2nkcucjuw.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2kekbqhgb.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2wppfcxjr.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2oxuuscwx.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2velhofry.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2zvxeotex.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2wwszwawx.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2hxgodjsv.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2baunuxcp.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2lzmnctia.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2pximmmzk.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2pidjriaf.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2vpiealxc.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2kudmufng.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rbazedrk.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2uaygdegh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jyjzhcyw.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2kzvnqrkc.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2lljotywr.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2oqaahqey.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2brbzgbbu.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2mimggujm.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2tzpmotyv.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2fhabcjfh.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2kgfbqloj.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2iwwbuwws.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2mqhphocl.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2xfvoznfn.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2ibhcskeq.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2kveapdzd.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2iqozaatl.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2euridnnl.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ldgmtqwq.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2zxqftntz.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2onjbbthl.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2seuczhwn.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2mjouccwo.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2vstevrdt.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2ahkkgcbs.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2lbybkusw.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2mkvchyvv.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2befguioj.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2epauiymj.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2rictwlpg.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2cbyiirrt.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zfdpnhvg.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2vjyumiqp.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2osmpitvo.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2jvkxbzsq.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2gquptiab.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2lqjfwlrh.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2suxtgzoz.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2bjdyzlzt.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2demojbbw.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2zjegijhh.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2nuwfyilg.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2cgkfgckr.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2pejcdehg.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2fhfgcqwk.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2bjrbufel.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2pmahnawn.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2lwzjldin.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2vqkyxpmk.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2kjubhafa.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2wtzogtee.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2znntzwsx.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2mbqrsats.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2tpxrjkhi.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2pipkpzon.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2tjiwvxza.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2tfvcfhgi.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2uhizakqt.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2vfiqyflr.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2uwwohzqy.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2wasjwyah.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2axhtfxjk.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2iywfyujy.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2aojltpym.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2qbrwbcxg.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2bbzzwfqv.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2kldixzoe.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2bxbwrzxy.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2yhgpvcer.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2tuqtlenu.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2tynfwgat.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2snqxodfr.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2amxlrhzt.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2cyzmutgz.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2akifgnia.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2thijlbyu.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2adcapolj.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2tbmqamnk.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2zgroxffb.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2ppdrkgmo.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2gqcxmtva.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2gureaqol.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2uvacwzvu.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2uiauhrtx.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2tylxxjka.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2wreowdit.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2ojliggya.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2yxefedek.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2yufelkjr.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2zdimwsny.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2hrzibnxz.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2chfxlmco.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2rjhjahmt.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2qnyiajxh.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2mjrlcnwv.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2zolrzykb.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2jlpeunlo.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2cozfvjbn.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2mvtormtk.html


<!-- 参考信息 -->