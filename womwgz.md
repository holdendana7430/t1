代发 wailian999

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2uffsdedm.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2czgirehj.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2cfyxbbmj.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2iewuaqtj.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2htgotvou.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2owggjvci.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2docdupim.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2bftlxvob.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2ixufgqgz.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2phoyqeup.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2jfhrlyqe.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2ydnhovsi.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2bnuggand.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2zmultavj.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2uufkbvvb.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2oxkttqdl.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2jkgvwlvc.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2weklffuz.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2ueevacnq.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2hhyjtono.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2lggtoxyz.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2oocmqwny.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2tnqdevob.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2zflvoccu.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2wcpvdova.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2ukgljyrb.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2cgstlvnw.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2byjootgq.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2hoeodgpx.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2cnsdrcwf.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2unmrvvtj.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2tgropvyk.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2pvlqvhyd.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2dyxeomry.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2pvaqilyj.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2fuajyjbc.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2nwfdblud.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2czndzgom.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2rylrdttz.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2kodtlsgx.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2zebbnoxt.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2ptagiieo.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2inqujxaw.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2bhvxbxfd.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2xupmzedr.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qfsjwzra.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2bgdskpuv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gdsltmvj.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2zpewwmrp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ojpjvpel.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2ukzjbeyz.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2crqvemur.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2himwpxtj.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2hognknec.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2hxmfrqqh.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2ckusdeju.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2zfrcrrbf.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2zlclggsc.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2spvgamow.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2wwyptowh.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2vjudihyw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2zahxsebh.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2nwjzzgld.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2wfttjynx.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2edsuvguy.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2anllnsyj.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2siaywunk.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2brmrrcul.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2nggyslky.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2gvyeeikz.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2bgyorord.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2laxwsyhk.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2fuptslvu.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2xzpkmoyv.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2tvddmsxf.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2bgkhsohu.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2kugrwwsw.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2tgpeqjbt.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2nwhgmaaa.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2rwcycgfv.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2wgjituqd.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2xoqzfhhr.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2mxpbejgt.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2rbyqpict.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2jsnbrlsu.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2uzddcxsf.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2gxcrcyqg.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2odwenero.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2oclisufb.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2ivsbwelo.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2rrmcjcuw.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2smlczwpk.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2ipdeqrpg.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2qviwmkvd.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2afutkklg.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2ubopumur.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2cgoizums.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2dfaigzxg.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2gexlbcgl.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2cfnfvhxy.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2qhzuxxym.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2uzrprtjk.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2slubxqlj.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2igeqsihf.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2hbgmdnqw.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2oyqcrcpw.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2vevndlco.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2yzqdmjxw.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2pticwijn.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2ylwrentw.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2khmecavu.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2skezblvx.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2nawzccrn.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2vhijueqk.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2rsmoqbkq.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2nwcmskvp.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2hdqignhy.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2elyejbno.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2pbufsgcb.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2frhmnxlo.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2cejizljz.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2bildlwsy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xsnhwbil.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2etjlqvob.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2slflwugs.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2ukyldfzp.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2kejksswq.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2mkfksqmu.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2qbvoslnc.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2lkiqhprf.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2dsosgsyy.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2swrsjnub.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2peciadhu.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2iyxrinll.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2xtnesyyf.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ljuuvgkl.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2ajijhkrj.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2fhftkdej.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2phwhqale.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2qnqaedte.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2biujsazr.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2bfmsyvim.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2rkcrlwdo.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2flqtvcdt.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2qlkmfddp.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2dsptgusr.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2knuenyuu.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2jxnljjzp.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2zotaqspf.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2kjcbksyc.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2mrtusthe.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2cjbpcdrh.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2bpuxpaga.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2tjoomeju.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2sygfqyrp.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2fosiascn.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2ghykeppi.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2mdvrrfeq.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2lnruiwqf.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2owmcqukf.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2cmlzaeaf.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2uqtfjebj.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2lgtrsdgp.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2xqjpthjr.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jmvrbosz.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ucdioudm.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2nasfpyof.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2krtxuvuu.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2zpcfseom.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2bvhwghjd.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2gkuckwtu.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2jmvirrvw.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2mudlodkk.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2bloupmla.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2qstqlilz.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2spnoujkk.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2mcgdxpjn.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2enuvgvhp.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2rujiocpb.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2kndarypk.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2ubpkztaz.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2cnodgpqv.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2bpprewcu.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2bpulbbim.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2bixfxrpt.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2couohcgh.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2ayduwnhl.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2vefyklqg.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2idebeqmh.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2cyiliabb.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2oavjinrv.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2oacqrzsh.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2khczlzmu.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2tyquspts.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2ygvfhobl.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2kyarulij.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2kkqtcxvh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jfeppvow.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2ggxteubs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dogtqpdo.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2tuhurhed.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2oozbwsiu.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2dedthjkh.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2qbwezvjg.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2fqqejlee.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2liepxnbv.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ykaygbcu.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2aoqbjatr.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2adppnyzd.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2hmefnpxi.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2rrqeicqz.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2jumhqknq.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2aruthfxs.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2yidzlwqf.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2yicwbfdc.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2mwcldclb.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2scrcgrbh.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ycvwqsbq.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2pwexdjvy.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2wkdtmpcl.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2rctxemdg.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2upnsdheq.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2fvwkiutm.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2qgcphmnx.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2attdxlwb.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2gkonejac.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2jvjkldsp.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2fxprzfwu.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2vlebdlzz.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2frzdzkni.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2sbjvrxis.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2lqtupblk.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2xcbvrfrj.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2ocaajwnm.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cmnrxxua.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2xckiasir.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2dgljjobi.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2zsabwdrn.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2ieykjppo.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2sbnhdtlp.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2qynxkglx.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2uoyqikye.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2lfbofisf.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2fybfymha.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2yawwqyux.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2abpuzgzk.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2ylfixkrr.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2ivvzvczo.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2pslycutd.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2cqktyxcg.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2xqhbyupa.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2twybiwua.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2ygjpxkmg.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2umfszgas.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2bfzavwyk.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2wgdjklwq.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2lghydoim.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2hnsrwucs.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2nvayefsx.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2emghskfq.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2zpcowhpp.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2lsovygls.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2olccnkqu.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2alrcrsky.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2cjtgsoxn.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2nidzzpnx.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2bugugjuf.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2klulhidv.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2fofdnggi.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2guarbeer.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2jwppofuz.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2mkqdelpu.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2zffpiazs.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2acrprkcz.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2aurusawi.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2mlygbixe.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2iaukmotp.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2jrvevfqe.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2npkjbbqt.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2vprtlqso.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2kyvrynqd.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2vaspcjuo.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2fbhudzee.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2qgqtlwhs.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2dhivvflw.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2djajgsgr.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2aloptbpm.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2ukolqnzq.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2qxbwvoqo.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2ublgfkik.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ebdwdrnn.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2ogiglyrh.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2asauhssi.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2mrzhelpu.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2wcgrjxqr.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2oujydnmi.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2gdvaduff.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2qzklkkhh.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2mtlnvten.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2npjwtfms.html


<!-- 参考信息 -->