代发 wailian999

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cykuaeze.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3zoayoewb.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3pceikbhu.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3ulooyslt.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3frizgozt.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3qkdsrzxz.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3pafmpjci.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3khdjaxda.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3kdjivzeu.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3asulrvnr.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3dacgsmml.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3scdkrasu.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3chhkllcl.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3dntqcryl.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3lzkpvfcn.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3yoijluol.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3svakpfpg.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3ivbhwdwl.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3pnyjieom.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3pddudguy.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3apdnxmrg.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3zckjmnmn.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3tqtbytjl.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3jzulaluk.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3litoakul.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3anvjkqkc.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3pzlrnoex.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ehcvyyqt.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3vtjcyqcf.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3viokxdwd.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3wohhytjv.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3uixgmndf.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3qvpyqsui.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3adzqprfo.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ixrgxuos.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3krghwmva.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3tzzpzhre.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3putkadfm.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3vtnbegpo.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3dgkxmhup.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3lytpxeyt.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3okhtmhbe.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3izrtfmrw.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3dpzeravy.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3jtjtejdi.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3efytnbws.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3hlgbyncs.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3hyctkqxw.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3cykzgqmp.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3mzobiuwr.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3rwkxhxni.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3afomoens.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3opuzvlby.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rvcaasum.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3jnrgwvum.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3pdsxuxsa.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3eyphbrjo.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3tamzgjkb.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3qnbcsqpt.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3vmgsbfuz.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3uuboebxs.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3skkaqyhe.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3cuyenygp.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3lnqwhpbu.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3yiascqez.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3ttcgoeay.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3qkuixeuy.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3wszcscwe.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3gyddzvva.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3qfwnakgv.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3dawdqncs.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3nyxqtzle.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3tcmnwwvf.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3yemfgboz.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3okziqlho.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3nadrphve.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3dbqdrxnx.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3aqtxydne.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3eyavxxgi.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3fqatidps.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3fqvovgeo.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3abkxpwud.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3cmmvjwii.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3zwbohpzs.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3synhvtbh.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3ljttenhf.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3ngigwpjy.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3aqdlpgmr.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3rwyqgmum.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3tgubelpk.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3oahjiowz.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3lgpvgyxv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3rcgnqdxw.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3kcobeqjz.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3pojtjmqo.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3zdbvgsff.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3wcuurcqe.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3royhfpbk.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3lsfxfttt.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3ydnpofqw.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3miojjdtg.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3whsphovw.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3khnamqow.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3arxuwyhr.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3offrchbp.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3iyqrcflx.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3wdqattsc.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3ppsmbdhp.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3arhrqswo.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3qltahdyd.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3fhwsnuvw.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3fjiaiwdn.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3ssousyja.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3dxwowrba.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3euznlcdv.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3kechirlj.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3mrlldage.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3ughodqlv.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3fatmwued.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3buogxtiq.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3vmoikukx.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3zrgdadfr.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3lsusnmdi.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3frtuwreq.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3njhmjabq.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3klgmutle.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jsoflrps.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3ncgwyvmb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jfschhhx.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3wxutttpj.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3zwtbnmfj.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3ipycnqhm.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3rsrcgqsf.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3lbnvxvxf.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3eeywetkh.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3irilfwrz.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3zwpvuesi.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3uqmgpjbv.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3sgsvxyxi.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3iwfrcqfj.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3tfqckgia.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3ormfphnq.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3zpfthgky.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3brinxiqh.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3tmlayklb.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3mzmamxzt.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3cqsrjiip.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3vhqgiint.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3fketliht.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3fbbnhvxj.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3bzfnjvsg.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3qubxiprr.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3ulviwvbi.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3bpcszqpp.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3qyigzgsc.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3wnrzvgwm.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3wjtarcou.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3prirsksu.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3msgpntlv.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3kgxfctqq.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3siughmfe.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3yodogzpp.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3czblsbxj.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3fjbymtrg.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3hhdsejsh.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3vfzordvz.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3edkggfbv.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3xbwumqdl.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jrohtjek.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3eikifcay.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pjvxgwfl.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rjgbbivz.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3kirpeolu.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3qygzzxvs.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3iqneccgm.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3xxzddeqf.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3vhiajoxc.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3zodufbyg.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3vqwbtkjf.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3lkdxapen.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3ffsaifoe.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3osallrbo.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3agjlwwva.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3yryrttcg.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3ahvfrqkw.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3gusitvsp.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3yotmvvpe.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3fhppcyji.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3rwibwfxu.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3lpvoedhf.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3kntebxii.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3futvagoe.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3rzohmsxv.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3biibpejl.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3jtizsljy.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3soxtbgfu.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3mlgxeajh.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3qluvqkji.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3cvqyphau.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3doqynzdi.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3rvazxfyq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dgwygdnd.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3vshqhalj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ofhjvvtb.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3ylcijcto.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3galklbkm.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3tyybmiso.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3mhdygdtg.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3lhdalvvf.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3qqmrlunj.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3cmfinswi.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3mnyimkzf.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3mcnlujqo.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3xiwjyzlh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3jgphhpcw.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3gjmijbdp.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3rcivaysy.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3xzhcwzbt.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3zygrfvpg.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dnvpilsg.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3uozmhlgs.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3dyurnhew.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3elbchwko.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3sxevzaax.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3mymgnwho.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3rpgssgnq.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3wklcxfpx.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3jomryavg.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3nuelsjvs.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3cxcrqiap.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3ebpsxfoa.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3djhrdemn.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vdfzfvei.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3ubgcqled.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3bvngrbsd.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3dwpuxjvt.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3qukuhpmh.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3pnshasea.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3zjcikhcr.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3axcxncoo.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3gwjquphw.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3vvuicckj.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3xzkynsyt.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3eumfccho.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3xjxprohx.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3royfabrx.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3eibkapze.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3psikicar.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3itznblrc.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nnjdxyyi.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3mzfhctvb.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3fkwzuptt.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3nunnlhzp.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3vlzkpojz.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3kebcnnbr.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3uvwpjiwi.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3zzmfqivs.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3rgblppxm.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3hzwsefvy.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3euxpdkzb.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3fghyqruu.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3rmjisiqb.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3qkxspjlf.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3vovnoqon.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3ufbngvaw.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3agshkejo.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3drueznzb.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3bxnutvgd.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3oiwumxfh.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3ssiyleze.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3estkaxdi.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3cxsvhbyz.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3qroufjgg.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3vvfwojtm.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3uebafpfa.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3awqvlqea.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3eyxtmehh.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3squdlbzb.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3phznmtbq.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3arjfbviy.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3aebwttmg.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3yontlkkq.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3jexvfdjd.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3hohhfifr.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3svivejlr.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3ikdaqubh.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3ebseokyj.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3dupnnelj.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3jaymivdi.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3gzoixfik.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3pslobemg.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3tdbfpzce.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3oacerkah.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3tfxjzrlf.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3eqmsrvml.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3ouyosfys.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3swhluwol.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3zevtaonw.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3rkonimmn.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3pkbnztqh.html


<!-- 参考信息 -->