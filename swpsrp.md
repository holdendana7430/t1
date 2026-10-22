代发 wailian999

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2ysbelkdv.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2bghjtafd.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2qwklkvyu.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jllppknw.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2zzvsgzax.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2yufcpjku.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2jxiffotz.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2xrauusrd.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rkchaafk.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yxhnvqbh.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2wrzkagaq.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2tblaiesr.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2bnynzgws.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2vkdctcbu.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2zogmvhbp.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2fzuctqvt.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2murscirm.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2qaqtqopf.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2hkowgior.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2reshypys.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2buqbchho.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2ccpfcmai.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2vqknegqc.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2ftyhawhr.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2newivhij.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2ufnihcsq.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ghqauhsy.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2cosndxiq.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2gupxrdzq.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2advdzahw.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2swnmagcs.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2rwepbwbk.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2btnfmsco.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2fowgbdbm.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2xegkqqlj.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2fueaodjb.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2yjtiqqth.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2aysjqcpe.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2zxksxrgx.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2evzugtzh.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2homtpnsg.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2zfwxjqph.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2wlxwmyqd.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2ryyfzaeh.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2cixnvrgj.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2qjkthriu.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2swecgwqm.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2malgblqr.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2vgexnngx.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2zsfaknly.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2jefwedsw.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2biuqrwca.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2banqgfkq.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2fltgjpsf.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2rcowjnqx.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2wbofvcwc.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2bqcceolq.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rpxapyqf.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2ojwpahwd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oehgfpls.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2gaskwjxp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mzajzwlp.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2agnrxzgm.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2qejhmmdu.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2lmnibyak.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2pswdiwsg.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2yipkyqvy.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2qiegdmoc.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2uopczfig.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2egjoxgbu.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2exbvirmn.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2yqapqqzm.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2uqcqaxbr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2fnqdbkoj.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2uxxqxsbl.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2alguzshu.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2nfnwvsct.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2gnqfiqwa.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2opimjpjy.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2wszpvecf.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2uuiqdydr.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2gsuraeew.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2bqmwtlim.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2fivnkrby.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2smsbghpk.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2zpwtjqps.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2kqusrvry.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2sffgjxvh.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2fyscnsdn.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2zyynizxj.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2dyfduadz.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2tlywsamn.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2wygwmmbc.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2ktaarpzf.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2jfzbkvmu.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2zecgahpg.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2zxxlcydk.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2rwzptery.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2firqmvqz.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2qtcnzsuv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2zjhgtzpu.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2wwvjlawr.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2sjvurskr.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2hkglomel.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2ezpwpjck.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2ufhgnega.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2szobdmow.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2xioyiqoa.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2tcxbpjzr.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2hfiabsao.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2khkazhuo.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2jydkdgoa.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2syigltrv.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2lpefufcu.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2fvndalbn.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2whawowsn.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2ynmkxndw.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2brlodtnk.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2xgifnoom.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2fujvjako.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2eugemxtd.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2osrlrapw.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2bsxjyyhf.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2oawqfnrx.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2fgqlzjbr.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2ynjargxb.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2ctdyidan.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2oqqodvyl.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2lqbuaapu.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2etffytsm.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2tgzhbbyt.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2nwizviwx.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2wyyiaxxj.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2afdenotd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lhhjhxei.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2xxewtjhn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cojttbgl.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2ocnkwlcm.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2samhmmwf.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2nbdwzhml.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2gdtrmcwp.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2oemzthvc.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2hklosvrj.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2jkvmzwom.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2tugwvmif.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2llhtxhok.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2rheijjbw.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2bihzjcts.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2pmaklyzg.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2jzxslwcy.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2xykcaqbp.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2zecpowwz.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2tmjqhefd.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2emwvuzeo.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2sftfziso.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2nygxakrd.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2kfzbtuoc.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2ziarxhvc.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2oryyuxsc.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ktddcuou.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2qtdgrpqu.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2cvffkrbx.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2tmldhlcq.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2dnnmpeur.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2molavuxm.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2baobfgzf.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2lqmrcknc.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2cmjaemmf.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2wjhbiivl.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2plqnycxn.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2mhbtjloz.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2eiyqyvzp.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2nyzsjeqa.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2ylrlwmch.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kicwsqgk.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2kiwmlzed.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kjuupmzc.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zsvfcfxi.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tpypgjrp.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2zcopflrq.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2fraoytkn.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2zszsjuki.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2atwefsnx.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2qcsdvzvd.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2crogghtu.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2lwehuphj.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2clyxevsr.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2bcubbrds.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2ozumgskz.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2lsllaxaa.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2cbpowped.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2pszdnkxq.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2gdebeasv.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2nhsyjred.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2djqdjgxm.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2zqezphzc.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2ezocqlic.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2phpsoowz.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2vmjfnxub.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2lujyhtvk.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2phjiaraz.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2dtyrzqcb.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2ctcdalcr.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2qdngqwms.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2fexdgzvq.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2ilfdsjqt.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2stjdlwfs.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2uwohbusi.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2tcgkufbx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rvbgvkpr.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2xsvtvprn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dkfthrea.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2ebhcctxx.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2iijnhttx.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2hgxvypwe.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2imuljhfx.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2wwfhwdxq.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2lcgcwvyn.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2aywcifzc.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2sfhbthcm.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2wokzyyza.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2wkwyianh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2acibtpgq.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2ipgayxsc.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2jbyoscep.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2plxksnuz.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2uzgrozcr.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zmprzosx.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2kiquhroa.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2wwqjrury.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2dvzvymrw.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2qxtdrcny.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2xcsswrcc.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2rufupjtd.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2gkiqbgau.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2crqrvlmb.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2knxedykk.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2xhctglyj.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2xkumofnh.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2ijqlaxnq.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2wosgdasu.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2qlkvrhtu.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2hbgwzlsk.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2fkthcoma.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2stzyylbz.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2vskigevc.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fwvhnxmk.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2xzabzsuv.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2uxgaduis.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2jukyflaz.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2nuxulmwl.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2pbaxvqmg.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ihvfacqn.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2dchtdrcs.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2bhkunwok.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2yqebcdbd.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2yknnggsq.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ylgzwzrq.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2lbswtpay.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2gdjqbflw.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2sznnpusc.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ufvzfvdw.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2wkfecmrz.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2ofvblzgm.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2cmxfvuon.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2wvxjrnaj.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2nxjdklln.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2escbowgx.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2qiefdeif.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2uwrtnwpw.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2xotktbkw.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2tzserzly.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2iqumfsoe.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2cbahtlgx.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2pvkspgvs.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2uiusfxzq.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nfrdcqjc.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2lozwrzen.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ttcqjqav.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2qpoqyahg.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2fitfdeuz.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2lxdqpgpo.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2bwiqldyh.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2slgezvwa.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2fngsufyz.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2tmjtxnmx.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2mqxpqpnp.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ijxezxxd.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2eskkvawi.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2kkevxibs.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2osgotezf.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2gymusiwf.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2ddfipdoy.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2yyazganp.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2fqpyqygv.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2nzviwjiv.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2jtnurolb.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2phdtictt.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2eriwqyiz.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2heawjwvd.html


<!-- 参考信息 -->