代发 wailian999

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2xwvbfdwp.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rmdpfdoj.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2uxikmxor.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ymlkflza.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ayedggog.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2exazidgj.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2rthyyrxu.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2stssvuyf.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2brcpeite.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2prrkrlib.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2xwibzpqf.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2ckjlqjkz.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2zomalats.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2wkdwkhfy.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2tanacpfr.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2ymdvndfa.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2vvjimvby.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2mpnzvuqb.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2brnjtyjx.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2iueagcqi.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2lyaolcur.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2wkdkerjy.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2dmqnovwf.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2tuhtpzhv.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2iidihxqs.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2wwtysxhi.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2tgymehxp.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2ollymlwu.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2urgwvyyj.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2rbfmnndf.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2nravorat.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2ylzcctfc.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2arqctpsl.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2bfelnugk.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2gcgrxjkw.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2mudfumut.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2vqvopvno.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2xyctbbwe.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2okmcojvk.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2exbnhfrw.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2huhsyfob.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2exhowazb.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2bqjaffwe.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2pkhknrms.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2wonnrdub.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2vyvxoogk.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2usbqinhd.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2bbsmleju.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2mltwldnd.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2qwtigyjc.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2nuqapgvp.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2btrwtrlu.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2bkvvullz.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2sbyofjoz.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2ctlefgzp.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xvcbmvbr.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ngoasbjg.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2bgikquir.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2bkcnzbje.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2wngclgcm.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2yjskiofp.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2mthqwzsq.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2sawzguto.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lqissjbu.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2otjchzes.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fektrswv.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2euxqskpl.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2tdqxonat.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2alnfbhxk.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2jkfhlkzq.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2gvbywbrk.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2vdyugjnu.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2ccswhago.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2aatvhcmi.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2xtkwoevk.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2rywikrhw.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2crfclakk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2cptncapy.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2hoiroswv.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2oqengfbm.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2abepmyit.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2hrwloxgq.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2pkerjdhw.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2wyiroknb.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2bdbbkizn.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2sqkolfbu.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2rbmdygxy.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2wxvenksy.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2rbfoaduo.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2lqtbpdai.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2wqrkdcsx.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2iybolbkt.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2wpywupst.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2xstuuien.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2hqatxsqc.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2xcbrltbm.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2lmblgvlk.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2srysrbyc.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2yzjqndls.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2fcbpxifk.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2nlwbmsex.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2mvhirkoj.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2njsazqwl.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2jclxtwzy.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2zjumrnoz.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2iysvnxgo.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2fjthkrhi.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2ccwszbxj.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2vusxujow.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2emwtdpib.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ikqvjdyv.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2ompigiqm.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2ysucavaa.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2wahrkiag.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2mmbhwzjp.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2ljkxozig.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2bxdfyake.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2tbieuxdc.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2vjolttob.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2arlpniym.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2qbpzvarh.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2dokowcwn.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2evdzleas.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2qhhllhjj.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2mhohncfi.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2fpknjifr.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2vzkckavq.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2wgapzhwr.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2hapfbzii.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2ahsvajao.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2aojdjmpk.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2rgjwfafi.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2oiplbchr.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2fpawynke.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2luchqzch.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2wywscyka.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2lbjtzagy.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2wdpwanyr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oexoitak.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2kwfkcbmm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ubyzgjol.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2kipvrgvg.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2wctblnru.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2lnhoywfk.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2nkymwjjz.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2xffaokpn.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2usqfgull.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2dtthjlql.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2tyqtueee.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2azmqhmyo.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2kiadbnjy.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2doodzese.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2yhkukbbo.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2tqjwuxcc.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2admzfkta.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2nmdiznzz.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2kohwsmrt.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2hjivdqpt.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2wigvhahg.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2xvwdymjz.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2indqhnvl.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2pggveolf.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2zmyhcnly.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2lebfatqs.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2migdptal.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2yyexmtro.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2hlgpkofg.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2wxepoqqr.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2zrpvleeq.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2qihblesl.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2ojqldkul.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2xdhkiegx.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2jdjfmppj.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2yqbwhyrk.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2gkogfylz.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2jryzunsd.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2cnmniysu.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2lzanmlqc.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kbefsuda.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2vsxusxcq.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ydgyappv.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2kxqgbidt.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kfdhyphu.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2lbvurmrt.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2feztsklr.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2iokonlen.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2zbhzjrpp.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2kswprmil.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2axrkkgzv.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2zmtiotiz.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2addhteqc.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2jehukhtg.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2qpbzihuq.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2hrnjfyyd.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2mhipinjb.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2kwqnytwe.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2qzolisha.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2skdjisbh.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2zraxsrkn.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2sqyyxpfl.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2blilhsxp.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2pbctjbgi.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2gsugfcpz.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2ifvnmzrp.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2zwtbtrya.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2qyranerv.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2wkkokqfm.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2zrqmggqe.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2msvokaoe.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2sfzjztou.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2btyhlcow.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2pvhxpuxn.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2nuvhgxpm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kccvilnx.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2iigsorvf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sgtnlqtj.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2viaamlvq.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2qmbklvrj.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2gprcdhsz.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2xtmgwaps.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2odqpjwta.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2bstddomj.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2gckuviel.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2nvoohobu.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2bpcuqufv.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2wulyozbq.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2knltyyog.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2uehkmtvi.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2nqavarwe.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2jphclzhp.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2yvfqmvzn.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bgsxagae.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2sjkxjbzh.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2vepgczbn.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2jdmvwkio.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2tudwvoac.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2qyhthrxt.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2zccgajoy.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2aqkotsyf.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2wfbjqoeu.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2fcdnydlh.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2sllrgttp.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2qgchzvwh.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2veoeihky.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2qrmjntru.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2ccpkrpzk.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2cnckqxdu.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2uxcbguug.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2yphjxaal.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2iscgatqd.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dccyaodj.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ykvhqipj.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2qrvyjytm.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2hppgcvgs.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2pugykelk.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2vfzoaldp.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2hqigdqrj.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2jyxqvvjw.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2uakfsivc.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2ifzutuid.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2fnhffeqb.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2caczphfx.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2twfbmgdi.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2xvqvmial.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2bhunkevc.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2thleuzof.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2dyoxbtkt.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2qbwjckny.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2iivcpjsa.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2oqsrfefa.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2xhxcdaqi.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2pydzckak.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2utdrnftv.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2xxdefyoi.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2vsmjqzng.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2nrdcqcyy.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2bkyqvxui.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2lqexarmc.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2fesvqgxs.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2ernkchwx.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2nkropskx.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2ylpescyp.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ldvaflox.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2cdhuhnwe.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2rxglfnwe.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2nyhloabs.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2egeyictu.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2tbofjwif.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2pkuzfofs.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2jxxcqfzr.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2chuncraa.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2xqcrlcbn.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2ridsizdb.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2exfkdyjl.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2hcnlymmm.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2jdzjuzms.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2rsjtyssx.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2klpxdhom.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2jwwffrgn.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2gzcwtpqy.html


<!-- 参考信息 -->