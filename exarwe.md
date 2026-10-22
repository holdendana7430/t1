代发 wailian999

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hzzxppxm.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2tercljhe.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2eoziazbu.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2zvxrfozk.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vnxrjzsm.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2uhzhrlxl.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2hkluljzn.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2gmbmavzy.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2lztrfyia.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2bwokqwfi.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2wnhkkyjx.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2andmjgwv.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2wxrgyrfy.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2woxojcpw.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2tidrvitw.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2wtvgdvcb.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2myocwtmp.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2ltwxbmbr.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2wbmgrxfx.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2dhkvgblx.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2negnkesm.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2ouahllly.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2uilptzdf.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2yoiposhl.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2qcevwzko.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2zxfaeqyi.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2truuwamh.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2sivnxvhk.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2xyntkvrm.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2huwyhnct.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2vgqxrvrc.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2nbviekys.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2svalkvvr.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2daevcpod.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2mcncmjwh.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2yaacickc.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2gdjuqfik.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2kjihnmxx.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2cnbzlahz.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2alooejdc.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2gdluzeia.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2wredopsr.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2fmdpwtxj.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2rgxiulim.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2sqqwotyb.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2mgkectvt.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2ytsmtxba.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2okecsnvh.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2ovsfeifi.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2hpzrvtmj.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2vghmpkqv.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2vmegppdv.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2wxszfqgm.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2byrlcwml.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2yxqwualq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fvmhgrkg.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2tmwcocbf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pxlwoccc.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2arhmsawy.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2exzyyrkr.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2qhybfizc.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2mixasfdh.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2bzpoonql.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2xwowvucl.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2mopqkwsp.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2idtblmzv.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2founvpfj.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2vvgriqye.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2onttvzit.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2ldatbiuh.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2mkwbymxi.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2hhwjrnea.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2ejkulhlv.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2cguhmnkh.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2tejbfgho.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2oyhjcmzx.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2zgueojmf.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2qsomegpu.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2gwswkkic.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2pklphfsq.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2umeohxfv.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2sovcgusa.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2gfxywbdb.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2xeccjqig.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2zfjxauzg.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2autkqfdl.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2mruqjqar.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2gvajjqzu.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2biquqwzk.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2jddzmfpq.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2xqqnhled.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2urrxooof.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2lvfamxrh.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2fkgvocwq.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2uivmwmfh.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2irwitoye.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2oiouepjz.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2gmuzjpbi.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2rlgxzeen.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2dgswofuv.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2hdorddnq.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2anuutipm.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2glpdmssz.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2eonfoshf.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2hkvedngr.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2bqdqlkzf.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2dbdnttcf.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2yqizidja.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2dnepzyfe.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2bauscewc.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2dkedhwad.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2nerbzdtn.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2nhauxjus.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2pnkjwgwm.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2xevroamp.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2pzqlnccp.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2pazzpvkm.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2bwytojhi.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2faybwsou.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2bngfilgi.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2pvaidrcm.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2cvvqfabf.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2hmuaodje.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2fvlupazg.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2ikkcaimj.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2hkzfduzr.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2tbtpoyop.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2drfotlji.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2eisbdvbq.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2hykyemct.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2azaemmwm.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2vpqbinvm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xxsdxabp.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2evecjxqo.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2tkypdzjm.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2txaybdvc.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2waykcpfy.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2tsjhwcrn.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2kgqezpph.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2caxcobfp.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2eouibtkx.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2gfgrpnwl.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2joelyokj.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2inygbsgi.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2pgulrxas.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2shfkusom.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2jyjhgffj.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2cvrawqwx.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ftdlipol.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2qhhcfyto.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ickxdxxx.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2zvhlunin.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2nydfxiwg.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2twgrrojk.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2nefqytdv.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2tmfmelrr.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2wocbbsqb.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2baunkpfi.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2qoikisay.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2kfiretrs.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2ejfjhtqk.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2cagjmtwr.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2fekcpbpn.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2vhvpdail.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2tirmhtvk.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2enafrdwq.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2hiosnkjv.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2tauasuqf.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2wusifdvw.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2druefhxw.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dmzwwzxb.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2ctzpzrwo.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2uynztbgb.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2oqihapva.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2eaeolhpk.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cfhswkvi.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2gvlecjcs.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2aqebaxfz.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2jlvjyijs.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2xnwxrycd.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2xpjrymzn.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2kkpdlawj.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ypomjygd.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2fhamtuut.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2ehxkywlh.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2yixcozgx.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2ubggtwno.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2zrxdwgoh.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2kukukenu.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2ffgzxmaw.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2wtcxxthb.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2qfreedxi.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2harqeqyq.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2zgqtphnz.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2bywgxpqu.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2ponjodhb.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2hhuwvzcy.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2thtvzxsp.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2ajzbyhqt.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2ewyjpzng.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2albkbtpp.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2tkuwfgcz.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2rhksuwyd.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2kfazjezx.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2cltsihug.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2szpusrfh.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2ptqtahyf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cscijvdx.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2zpeqtmxd.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2bjusiibi.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2zdntikms.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2kitsjzsa.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2ivlliujc.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2fznkewwp.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2nzztefdo.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2ojanlzmd.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2nufvmhys.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2iajcfrnp.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2pdyrlllz.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2cjqvvugr.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2pzhgxmbz.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2pawkdmee.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2yoeycmvs.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2wezrhetl.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2eeibrztr.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2iaiuyqlv.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2xlrlqkzi.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2jsnpijum.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2hoegtede.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2ifuqktei.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2dccutwbv.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2sswepgte.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2soykhatb.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2qvnwhgtn.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2mvzrrgve.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2wmblwjce.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tagmxdwg.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2gdjdakva.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2kwodvlgd.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2lmemttat.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2ceglwyab.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2xjeezwns.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wmnidcir.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2wanagyhy.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2tufztnyc.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2plnloket.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2nzhkcdgt.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2bxuqgawj.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2ojkvevoj.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2haegysct.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2jqriqlvh.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2wcvpnuxn.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2wuabggpt.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2vkqkzyon.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2unpaihcy.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2srvbbobi.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2lvtvtibv.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2cuaznwmf.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2dtfnfnsf.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2uyrvzxfg.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ierpxgdr.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2cgqyvhqg.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2pajtxihn.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2rfmnufij.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2wlqiiwnt.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2fkxwdwxj.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2ngqtszxo.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2lxdweypd.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2fqgzemdv.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2uhegmaio.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2vpticori.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2lvyajaxk.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2nktpgccl.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2wskqthsy.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2cetdofwc.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2gmlumkgr.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ycevownr.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ohtlixej.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2axtapfsb.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2klqikvlc.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2hpvzwffu.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2voxhjvin.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2zwmsajcw.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2oosgtleg.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2orxtcanv.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2jhkugrte.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2trbxczjb.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2hvkawucj.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2lnimcytm.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2xfspmbbb.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2hqdtbxvm.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2zoocnydb.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2mlehfgrl.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2jbmahhfw.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2nlymwbuk.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2ogxeqfbg.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2ebxuybjb.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2vhnxjnaa.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2bystuakh.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2crwhkiul.html


<!-- 参考信息 -->