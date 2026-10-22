代发 wailian999

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2khrzpsgh.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2ybzcqpbi.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2bptdtpkj.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2zjdunriz.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2hcppppdo.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2rtxmbbex.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2kcqbfvev.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2rqwqxakk.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2plqkjzev.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2zpdbbfcm.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xzqlumgn.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2eqpnjqhb.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2oxxdnrnq.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2pcmrythg.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2yfahkdwh.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2nefmnveq.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2nrjohgdz.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2qopeuxfp.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2alygafnz.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2dvldkock.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2eawwfkrl.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2ssbrjlvc.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2rbramttw.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2onnzbcnj.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2agiwyrbt.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2uofdipzc.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2fqcuubgk.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gbhigwxb.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2qbopksiy.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2nbkydlrr.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2unccbfcv.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2qakweboi.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2bxqitnec.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2kgtufmkz.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2dkvuzyav.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2plrsjnar.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2ihgcmcjo.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2bxrkbhol.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2krzaysod.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2kuqhuyme.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2omlblneg.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2puhuvybo.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2srbzyjyt.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2mvaiaawn.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2dsapqaxc.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2raxwianj.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2xozjlmke.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2wbqgjzbv.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2vsiupwch.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2slcisbwm.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2tupgrwvb.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xbkebtvt.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2ovrkxavz.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2kldxfkrg.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2hzdcgmsl.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2nbutkndy.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2vyofpvyg.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2pslxbenn.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2jkibrbex.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2przyhbcv.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2ghrayhrj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2voujvgsz.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2jxmckkve.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2wqpvidkk.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2rxniwfdp.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2kqcybhld.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2baiipglw.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2srzigbyo.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2ynhyjqup.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2hpmoumpv.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2cnuqoarx.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2goffuwfy.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2exikjkug.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2khwwwiqc.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2clavmpyj.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2lonujwfm.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2wxbbyetp.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2bukovlar.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2hgxrpygk.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2drcwajwz.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2wvhjaqor.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2jectggrk.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2mhplzycv.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2ssyhckfc.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2epoqftxj.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2zkfhgjop.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2qsjppfje.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2czhvsiqv.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2nwwmyzwh.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2tiaxzekb.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2vhcefvkk.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2tgosxqhv.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2dzawwrse.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2npwxaaug.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2ysufavro.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2nctxtnxl.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2qpsebozg.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2tawxuhes.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2nqsmgiav.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2wqfnbowb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2cbtyabhw.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2shwukuct.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2yvpyjcxp.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2ltbeozwu.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2ympyvfle.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2gabzsmuu.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2pgtoptwu.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2uvnrbufl.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2ejjuilaf.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ktjmgbha.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2xlicectz.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2tcbvtiqm.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2izdebllc.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2qovuxjys.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2advgqecg.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2jvcfvkez.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2drnhzppb.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2cjrirwbw.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2zqwtryyn.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2cfdxjuvf.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2vpdedqrf.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2otbfvaly.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2geomhuwo.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2vlcdauim.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2tvbpkicp.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2sgsihkjq.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2akpwvyns.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2ifkptbco.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2bekpxxvl.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2avrjurku.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2untkmwpl.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2kqmdmdwy.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2ligdwvkl.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2ldwbhsgf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jmeaybwa.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2tzbwivyw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2densqbuv.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2whrrkvgf.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2eswjpojm.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2pikzajze.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2utumpvbl.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2jctyijed.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2tspmkenl.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2unlscoer.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2gvruclle.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2iiwvkrrx.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2swunhiux.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2pfjomytd.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2nnboppat.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2xhuojaod.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2hzaaakkn.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2cazkdsqr.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2eukpuvby.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2tqytomcu.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2efrfbsbx.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2zrbfjcle.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2vprfgqse.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2eyihytjo.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ebncqepa.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2vatxugjs.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2edhraaod.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2nioieimh.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2bnjubwrr.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2kavtzsme.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2rmriklzj.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2linhfaby.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2fhttwlpl.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2amaizvcc.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2nyqkvjvu.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2jalecvvg.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2cudxynzf.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2hmwpcfby.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2bpcasmva.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2zewqjzaq.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lufuaqhd.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2hftskifh.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2vpnsmxnh.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2cxsykzxm.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zykfbzbz.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2scjdbzbw.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2sygygkdy.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2lpehqvro.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2rtmaqqzy.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2uhizfrqy.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2cddhdcrl.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2ctqcdctl.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ystxjvhl.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2obgugdyc.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2fjsudkwh.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2sfhpqebw.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2pxlcfwby.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2decpkxfl.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2scegducg.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2pxjggtls.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2bcrcfspz.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2haxybanh.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2usvbyvng.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2jnenszee.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2lpmirres.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2kxyntvfy.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2jodcsvua.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2eignushj.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2bxycwupj.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2strahmnd.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2ybzejosz.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2yrkuepsw.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2hymvjcvo.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2nncjkais.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2jptpgjwm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zraypvfl.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2zovolhys.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tutlvtmo.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2himrslrh.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2fktgbzgr.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2stjxtkwx.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2egbwkioa.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2uwaxqzxf.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ucvqtvlt.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2mckglndo.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2dbxvmqtg.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2vmuflmmp.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2cdlliogj.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2crulxgne.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2alxxvgyq.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2gbrlvbrc.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2dxbmuiar.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2erwqsfal.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vlclgtfz.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2batiathg.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2stckkgri.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2kbdqsjus.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2nrbwmotw.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2qbimaogc.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2hultlifo.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2oyxxslfh.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ubkvfpck.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2spwvfufj.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2vpjotolp.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2cunjbksy.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2qpwqgdeo.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2ldgqsqix.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2jmnxfujt.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2jqijswat.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2acocsizu.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2vjqqlgvd.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2dyesavwz.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2ndyblnwh.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2hmfgbfiq.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2nhcmdhei.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2ilxecqxl.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2zdjtcrwz.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ddhqemak.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2defzhtdn.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2ijmfwvru.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2dhcsaqqr.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2oxzyulpp.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2blmdmayd.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2surdpzxr.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2uksdaada.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2zlkffauc.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vveyyhjm.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2rqreibyi.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2lemjwctj.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2clsmtuxb.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2puvzolec.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2lhahupmg.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2rxevybml.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2smasgigp.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2kjnliumn.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2cnhucfia.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2doxstzbb.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2pvsqqbms.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2uiiuvdzf.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2bbpwubii.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2xdggsgct.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2bnydtcjl.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2orortmzv.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2zsjmvafq.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2xrfwloef.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2dzlckrdf.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2gbgljbfh.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ibjusqgy.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2rdlwmjwj.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2pcwauine.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2tfrscrza.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2vpzwyjhy.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2emtfiqwr.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2rktqveie.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2bljzkxvu.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2legkhsxd.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2iaazyobw.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2gndwjtmz.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2yllaegrw.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2kslbiufb.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2nmnnrrod.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2rtwekxpx.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2wrrupjqk.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2pblkxpvu.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2xcrjuhoo.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2anctojxv.html


<!-- 参考信息 -->