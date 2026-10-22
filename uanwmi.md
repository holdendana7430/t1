代发 wailian999

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2shxlianw.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2swzlamks.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2kiotvjau.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qjijpnhl.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2megwqlgr.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2mrbevtdh.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2lngntjed.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2kobcqpzy.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2fqikowvk.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2jjhcyzei.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2vvfsdjwp.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2zipegnfs.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2krcajkbb.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2onxnyzzc.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2eignbbuc.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2wdyhamrr.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2vkodtsaz.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2ibuabzov.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2tgellfzv.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2wczcdxrf.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2qmntaels.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2drnycrhg.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2aaqyrwbp.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2vezxpnrb.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2smoybaea.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2vrukpkzw.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2qvrjyuna.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2clbsdhew.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2cepcjyrj.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2kwuoxkjs.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qmwvbtku.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jhkvitkp.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2glhoqbnw.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2warhfscc.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2hgzvmbck.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2vevjpxlt.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2cjwvggfa.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2kwglcjud.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2mjuhlhiw.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2xxfzwrdw.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2pnaiiiqq.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2gamnobnm.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2ninywjsl.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2swczokgt.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2lsvlvipx.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2chsgscae.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2nqsxdyvg.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2ujzhygfk.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2kiviuekl.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2uhkisjpr.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2qkifbjrf.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2grsatqqf.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2nfbapecp.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2kcrmosdk.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2lwsnasss.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2vavthvth.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2wxmmefmk.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2ognyuptk.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2acuswcdv.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2qujpbaxb.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2xziorrqp.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2kdqoghzr.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2qeetcyvk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hkzcoabl.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2merpcydz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gfxqxfhb.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2kpjjhzjr.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2jzpvyqtg.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2wbyboglq.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2bxgmvraf.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2rbkpdusb.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2afngnmwl.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2xphqfcss.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2azlecmel.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2mdaubazl.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2wliahgto.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2wbbpohux.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2vzfhuldq.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2ndcdxtfc.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2fdnophun.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2dctujfnz.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2gwthipgo.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2imuxesqs.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2iwsayqjj.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2yglbhxth.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2rzzyjxsi.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ldcazmmp.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2czosgsln.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2xqaebouf.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2vgaqqjbn.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2ioymfshm.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2kuwfhlkg.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2nnvcnakn.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2dgiydxpu.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2ozmrsssu.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2tikipkbw.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2yvrfhstt.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2zjnjujbo.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2yqkdsctl.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2ompdkwjq.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2vvyziewm.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2gneuvzon.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2apztqguk.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2tswffkuj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2bcvpatzg.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2vuhzypid.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2zuotilzh.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2ckkbngik.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2bgbyncvw.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2irhxawab.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2cvhfphvq.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2ikbvbdpt.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2nawxaxiz.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2hkezlyod.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2mocafptx.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2ysnfjsfp.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2elzuhvtp.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2ilcrksws.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2gyutlmee.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2tuyivjex.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ofvptmwq.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2jsmbbays.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2ofohfzxa.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2lhcveync.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2jijqalkf.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2yewpxvcp.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2djoujpyo.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2osfakxqj.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2mlizxyaq.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2uywsluhg.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2htrbrvwq.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2uuzlzrxf.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2aflkhdwi.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2kmyyndor.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2jxbkgjqs.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2ywbrjfim.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2xkmsxyzh.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2hwjtxcia.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2izoarjwn.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2wktedubp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qqdmyyuf.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2cyszaidt.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2nzyflszf.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2tirpakyb.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2wgflfmbp.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2tlkjnqjt.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2dmwefcoe.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2qelsufrf.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2rwudnerm.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2dsctnyoa.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2iupzfyxf.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2fovxbisg.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2hcrngqjj.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2vqvhxukm.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2azlyitpl.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ozfzrtcu.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2bkjtblao.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2vdnubwzy.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2lbtlffir.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2orszgizf.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2kruaeouk.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2bddknrcs.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2crfzypyg.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ycciqskd.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2ypyorheg.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2yixsauay.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2ccultbit.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2wnfhckwb.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2ahmxjigp.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2nwhjasbt.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2shxedbrv.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2bldzejeo.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2scxjlmnp.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2hrmpgwoi.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2nqdidrol.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2idteylpv.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2ufgkshbh.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2pxikkrmc.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dxskeikw.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2rnzqsonn.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ariyfdxb.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2rftofgkx.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2iattiaur.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2jqkiexib.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2tunvlvzo.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2yqcfaiyq.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2srkdgtdc.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2uzxfxnol.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2lgfxutga.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2wjriyfdw.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2yktjngfv.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2ogfemhbs.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2pwgsfkvn.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2dhvjupyo.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2iuvryitz.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2sasytmij.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2rqlqketx.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2twaxfjef.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2bdflpohy.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2oilroasb.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2snroxzhx.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2swfiyfzr.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2amiqyyfv.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2ublygfyg.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2yuusvwbc.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2rzjxcayx.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2ccpobbuc.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2mgcadxhh.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2aznmdvhr.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2qlpsjbzd.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2joksycat.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2gcxxbkzr.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2byyhhhhi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dbfhsdxz.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2hteajcrn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jijbwmoa.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2kpzahgnl.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2wduuvglb.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2bgzdpnvl.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2fnetmaep.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2tmfgmgqi.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2isgmnfvc.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2flynrsvr.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2wikgirnj.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2vvlatpvb.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2nmfksfai.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2vcandyqy.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2nybwoewq.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2vdxknoyq.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2jucjncxb.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2uborsuhg.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ijbialvn.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2dbymwutr.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2yzvglgjp.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2acouzjak.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2fdikxspg.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2ewhrxyky.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2rkidrvom.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2tvgolsph.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ettzchhb.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2rpykqliv.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2eszyknzk.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2wssjxjqe.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2swhqgpyn.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2jteewuse.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2gmrbpqdw.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2osrrmrgx.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2uxcbljgm.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2dmcqevez.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2xmwrqqim.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2zvdztsow.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2iqzfwiel.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2dfoyryes.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2rabpmcex.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2bmmfthto.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2sxscqvvv.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ohonpaee.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2xjqurdqw.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2nkovropt.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2bmijbgpi.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2vdivdfwm.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2jqawzvqf.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2jjhamtzx.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2zevqpter.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2gqcwzpnn.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2zaimewne.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2zbabipgo.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2cfplwdqr.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2brnlqkak.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2hiplsifg.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2sqpxymdh.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2rzssytcb.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2xntprjay.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2nosydeai.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2auikvodo.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2fxdnzsem.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2zggwazcb.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2zgfjxpla.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2zenkugme.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2ycbdnglp.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2vcxpiquv.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2adyxkyfq.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ohpodisy.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2iscuqzoo.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2phynefhf.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2xnhbgohd.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2oerzkzcv.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2erpozlhx.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2bpfmtcox.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2ksejyirn.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2orgimwvw.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2mljgvyqt.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2dukczzfm.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2umoslvaf.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2jxwfqwoj.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2cqibdbgr.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2bjhumfrg.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2bnclrunu.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2wayrmgsp.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2zipteytb.html


<!-- 参考信息 -->