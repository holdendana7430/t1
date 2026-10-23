代发 wailian999

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3odkuortj.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3bbdhwnme.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3mhgzkthx.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3hesrkcof.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3ffobjvuo.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3dqnwajfu.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3wolmihed.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3esltkqob.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3nlruahth.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3gmugoxsx.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3rcttzlal.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3somkhpvw.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jrndetuz.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3nehddomh.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3bbvnvfqb.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3cfooknic.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3xfrslrtl.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3xemltdxc.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3hrvqwqub.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3yexnsgng.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3zcxnwhct.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3ufvnohar.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3wwjcvazk.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3kngpqoxd.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3dzljskis.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3hmbsknhp.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3ghqvdqaq.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3krtvqzay.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3yomjuxbp.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3cqxormvr.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3rfbjowjf.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3vatpmbbm.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3tztniyny.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3iighfeqq.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3yuxmiuwz.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3vdfkdonz.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3yktuecho.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3taczxeas.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3wolycxmt.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3pegqskoh.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3gtyqjmma.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3evvutybk.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3qjgtwhdx.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3gobpsjvc.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3iktybqet.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3dgctwirc.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3sqaffycr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3izddubhq.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3osanlxob.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ircjdudk.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3pulrsbqd.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3hkywiohl.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3uvkcgxwh.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3zyaqztmj.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3ggrygnjk.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3uwolderr.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3xbmxiafx.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3igvzcfme.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3mmralxbo.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3uwsjqfiv.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3prtxmwjm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3xjkspywr.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3wttjycqs.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3slfepjoc.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3yvwtvryg.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3gvrkuvfd.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3pnfzaenw.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3jmpkasrk.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3sujekggn.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3ecexszgk.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3iyvbnjfa.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3chdmqpfj.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3iqfxtrfc.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3udcprxir.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3zyhwfhjv.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3iyjeocmd.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3pnmbvhwf.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3nfptqyoq.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3tsbsdbbu.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3tvjegort.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3fmneqldw.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3bnshprom.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3ozmfoquy.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3dylnzakx.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3dbrutvcm.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3guadcscv.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3qgcwoasu.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3yyydtxqc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3ldzdjnti.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3brhpkwng.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3adzynvyr.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3hbnzykwq.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3engokzpr.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3ehcxdiwh.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ghhwwrmz.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3rytumusl.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3izmhwvdl.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3razyujrz.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3bnqqlzzv.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3ycdmikte.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3mlytksgo.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3uubrvudw.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3wdrhwnrb.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3nxpgptyn.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3hweuohxk.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3ujhflbvz.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3fhxbjocs.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3jdqdikws.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3tgrrwpot.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3zkvtenlo.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3fetqsdqd.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3ytwzfnpc.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3wcqmabxu.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3demrgaxr.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3yurkrpaq.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3kledqwak.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3bodxmjxx.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3qzdvwqyi.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3zynfawlj.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3gfidwnny.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3sdyauxec.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3aiqpkisa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qqjafzcv.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3tumuweup.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dkgytdya.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3mfmtswen.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3nbduqviw.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3jtdjfcee.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3zckzqbde.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3acklljjt.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3jgdkyrnz.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3jeseiyzm.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3vwnnxxgo.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3oeccrrch.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3hjltyasm.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3zywlhuol.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3tdjdsfnu.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3egzwxzwv.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3lonaltot.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3azbdyitf.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3qotvzlst.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3jysnudzm.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3irzcclba.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3duuzxcnt.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3vvwjkhyb.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3npwdwtuu.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3tjrpbttp.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3ocfmqgsy.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3qfdahjmc.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3vkgfaacs.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3jozvywbp.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3byyxzpvl.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3hkojdnlo.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3fbaceaxg.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3uohnugbw.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3bhmecymf.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3poyybkuo.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3mkkqebwc.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3jhdzpejf.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3ddktfaij.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3bnzypccr.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3hibumigk.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pqoqodfk.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3hwqjyhaz.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3sgmuamjs.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3scamssnk.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3wrsilrdm.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3dodfvzqd.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3cnkcdnwi.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3oiutuzhq.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3clccakfd.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3wvphxtip.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3dofrqiwv.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3gtfheluj.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3txdghahu.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3stggbyzt.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3jyxgjjug.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3awekzjvy.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3wgboacjr.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3wgqvlsnu.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3ahfteopb.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3tdlmgcya.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3inhqiwpt.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3zoilocyf.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3axrmbetx.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3mtbpxtsu.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3iofaxyzl.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3xhmvsnxl.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3jkzozhic.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3stfwuzfl.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3pqkhlkny.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3holmyaln.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3bzuotfxw.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3tiutmalf.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3djnxpzgp.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3mqwlsrpg.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3elwfswut.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vhiewoih.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3bmqyxspq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3phadiaav.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3blfkqxut.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3qabxxgkk.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3aeocpdgg.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3qrqkioan.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3xlydlyur.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3noclwuay.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3udohziyf.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3wzxvthoc.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ofzgzpzq.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3zxqdxnmk.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3vintqhwi.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3kfdwwdjn.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3fxelgtms.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3vtfulxnr.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3zixwknlh.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ksrduxth.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3jijazvxq.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3lhvnbkih.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3xckvrvkc.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3dvdwpcsd.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3vzvhnsht.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3krcjkecy.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3izeiwgtv.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3ingwwvwd.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3hvsunmev.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3ygorapbx.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3rbvrlwkp.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3pktapyxo.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3ahkttslx.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3ktebtvxt.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3phkigabt.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3jbopjxwc.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3uqfytacw.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3kowselgb.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vnnovzrz.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3szahyabr.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3ohfjvfag.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3fktepvru.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3jjscectd.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3micluzbw.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3uadsblcg.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3gbfkupsw.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3jpftcqil.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ysxyfxsj.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3mzxaglii.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3xasmahxj.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3pjmhgdpc.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3exxymngn.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3vrhtcoqh.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3dvloilat.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3xufvotbo.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3ipfbfosk.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3qpvikfjr.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3qzzjpapu.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3okkwqzro.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3fhyacbbl.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3pazksopk.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3iorcsmdk.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3ihmodaas.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3helzjflq.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3jlpdnrpe.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3vykpmjzq.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3lijcurkl.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3hbubtosa.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3hhhtbwdr.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3irvebhev.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3qaqjnkkt.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3atjcttnz.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3vfsgrhys.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3tgdibkpm.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3pyiphyfk.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3fikpvhsn.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3rcerbzqd.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3snuanwul.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3bfdvslqz.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3qsxcjbtm.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3ossrdciy.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3xytxpvna.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3vjhbvsfp.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3odnzcwyb.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3mtknnliu.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3bfwyytyv.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3ofzjaahd.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3nvxldjqp.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3fqyulxog.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3ctuxgmmz.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3hechnevr.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3voixvwmg.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3njkdhgcb.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3jnjkxvyz.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3bwpgtmrq.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3qdopoyrs.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3xextuwws.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3cruopgka.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3mdwdposh.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3qmswhozz.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3woekjswf.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3wvejeypk.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3gonweyte.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3tyiuzqlf.html


<!-- 参考信息 -->