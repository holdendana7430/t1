代发 wailian999

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2iboeiwcl.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2iteulfpj.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2blrmobxq.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2icxmhuot.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2botrhgya.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2loljmigr.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2ngfcxkjs.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2iwktvnow.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nocxzflh.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2ckimxfcr.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2mxaqlwkv.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ddjwerpx.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ntqfyosr.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2qoedmzvt.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2obqisdlk.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2fijokdzz.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lvgeptog.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qbtifjoi.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2mbovblqp.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2qlnzippy.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2hnodkowa.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2qgkyvvcr.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2glajewln.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2msrqlmwv.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2pbygszji.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2ttjlxfxk.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2rygclfbq.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2uvgucmyd.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2djcuhlyq.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2udtykolf.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2egcmdxyv.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2ohehtpkr.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2hnsbgjdb.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2uebutazt.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rlytaaaj.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2duglqbvi.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2bbnztnft.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2ifmymhvn.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2gazczazq.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2mokjneyz.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2jldjibbn.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2umavserg.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2ulfleotg.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2sugfbyap.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2maufkzdv.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2bngoynlh.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2smfcgxkw.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2omanuwqy.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2ywjnbqpj.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2fsqtdeiu.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2fhhpocvu.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2alrtylps.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2fcqappol.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2rpbhsomf.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2dhumocyy.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2dmxjlpub.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2qgxlqqrm.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2mhbngatv.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2gcmuofvj.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2yoqcezpc.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2mhbgoxkn.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2mpfgyrdv.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2nkxxjicm.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2jvbpboaf.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2zyaqztij.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dmjulden.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2ucklxcij.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lujaasio.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2hjkvifwc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jcbleifv.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2ukgicqay.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2fpknxvna.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2hxrvylqq.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2yxdjnlcm.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2lfftkezb.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2bgnxvmmn.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2nljcwmaz.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2auzkzoxf.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2nadhtloq.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2kfxgopuu.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2hfmjnrlw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2touekivt.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2gpcprsiw.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2ixlldjan.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2fbdehhaq.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2sucnhcqm.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2htfewjqd.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2mhhotiyt.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2ubvnqexh.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2txifhelc.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2osrovfco.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2jqobvrqm.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2pzfglygf.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2vevwrpfq.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2lruwirwo.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2oykinfli.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2jovlseqh.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2kbpsfdog.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2vzppfhis.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2augufpde.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2rdwevyzr.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2hviuzbpr.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2aejkfkvf.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2bwbjrhog.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2jympubro.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2cwbiqear.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2zhdcpgkl.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2tvzamoyu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2gwhphxnf.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2ufdwsjop.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2qvcxwhrw.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2elmwxdos.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2xzokasub.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2sjwvkqeg.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2afrhjgct.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2naihskkx.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2vyaoiytn.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ywqcwvbf.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2qgasswto.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2bvyipaga.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2hfmysktu.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2ltowgjso.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2xesobpvx.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2xqixpgmb.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2unkxcrwt.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2jujseujx.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2tcylbbci.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2gttkinss.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2jlpxtlom.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2vdalqdif.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2ndbqtegc.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2pxnqgxym.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2wtpvhlsu.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2dhthxylz.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2etxijniv.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2efosxtmv.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2milosnon.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ggdmqqvn.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2ojtvpxuw.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2vnvytrdy.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2qosvvsnu.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2vpseufon.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cdyocvyd.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2sjgkevlc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2okqufvum.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2poyflsbb.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2qvmymjou.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2vcpglyhh.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2qbramkwo.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2fklcywlt.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2zbszllna.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2fovrtetf.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2dokihykw.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2zejnunjn.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2hmlptmiz.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2jkhayydw.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2zlgykhey.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2lpyqylsz.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2cryprypw.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2snbcietr.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2gxacziho.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2eistoqwa.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2oklnbxrq.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2yjqekkkh.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2ydlczzdd.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2omaqsgcg.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2azjgdhvh.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2zdhjwrdk.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2ieiynmav.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2vrbvaypl.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2qdseeegg.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2gsntxlmu.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2zejzqidi.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2wrcpvlfr.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2hprbrhkd.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2hsvkpjpa.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2efpvghkn.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2ahtgzped.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2aoszjlvy.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2brajkhqk.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2bbtoilsa.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2jroezfdu.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pttoacnc.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2cugrrngv.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2aauhkhqf.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2nterffpm.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lgtihivk.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2tofyyjjf.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2junvwknq.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2fonczxas.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2ipfxciwt.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2tblsgfud.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2xaoalbzg.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2nlrmgvgp.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2wsmsxjon.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2jhsrijsl.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2edyvscul.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2yqhuxqdo.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2wdulpdrt.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2nllmptyc.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2aptsjfqs.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2ceydmbcr.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2fhvcdtlo.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2aihluvhi.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2ninrjjfi.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2pdlxlzij.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2ujhbdegw.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2wwklndrg.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2maypstie.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2ejkuuvhc.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2mrtqndnx.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2jwxiqsea.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2uhinufnf.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2pcwfqliy.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2wpxchdly.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2ufrnzlcj.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2lkaooxes.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yckaoqww.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2nnixhbuz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2azaujpbs.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2sucnpiia.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2nesljkbt.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2xmuutqlc.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2glkzhbbi.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2mcmrhggi.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2avdoelwc.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2foxskbtb.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2tiygfpwx.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2gmnhlskt.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2jdbknfeo.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2gukowxrr.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2rstxyfmn.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2ouirqdar.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2ljtwyiks.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2jpwbzsoo.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2miqwrkec.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2hnhgrdyu.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2wbymcbzi.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2akscnunn.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2pmkxpeof.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2bnpeonjx.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2pvxxyuwt.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2tgilvwst.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2gjropnac.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2vimlgqvd.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2yshbshav.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2mrvdgdly.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2mzcmqeei.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ahzvpwtr.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2zdxhcsmk.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2thuaknqu.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2ixidzmfg.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2qatbnwup.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2dlffbmpq.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2wmetrvfo.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2tilceuyn.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2rnpmyexe.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2cnhjjtum.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2soqezmgm.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2bwiftnan.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2hkzfsuof.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2nkxqqmiv.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2xpihaxfc.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2clvhqmyj.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2uhlhdwrx.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2cbefpphy.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2onepnhmc.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2aaabttnt.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ijbwizie.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vpommuun.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2xtszpban.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2kkpojbub.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2fxsgsyxo.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2whnwuuzv.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2sidddmxl.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2updbkodf.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2xyljvwru.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2tezfygyf.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2rkgyvgeb.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2hstampya.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2fmhwznfc.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2qintrtix.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2tkfodadk.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2tklukjuq.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2cmnjncty.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2cglrxcws.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2bhddjhkf.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2pfzhecod.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ucjhcswf.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2qrjuowyq.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2dhglrssn.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2lkkvbcja.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2vkloxwua.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2bgknmabq.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2jhvmmynm.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ffxjurbe.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2uqqacnez.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2ywjofvyf.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2pqfwisei.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ehpoiems.html


<!-- 参考信息 -->