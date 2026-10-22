代发 wailian999

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2mfgbcqmq.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mgajehtz.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qpygvlkg.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2vndctfjf.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2kvhwtnva.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2oiplsxxt.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2kmunkaef.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2avjcqdga.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2zdpsyvih.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2jcovmxju.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2ajyisixm.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2ycogtjex.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2kcaadqfv.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2ruczrjtd.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2glgvqfgw.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2scduuvrz.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2irqitxqi.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2lpryoqyp.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2yplewhvx.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zxuiptrc.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2hqizjiuh.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2mfclvhya.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2ongeriov.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2atiooqxm.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2edvmeqio.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2fzosbite.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2pveniywx.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2pmwdaznv.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2nzmpubjq.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2fcmmiwde.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2woavbkvt.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2vcoqsviu.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2raggesya.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2ftgwzzfl.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2glahfvlw.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2ibdnyuum.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2fivdfxfv.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ikyhvlay.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2tzlxdvef.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2ebhvpyyk.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2omhwacub.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2pbeqnomn.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2zwicywti.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2dxhgnxmh.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2cimorntr.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2hgutjyvg.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2cfwndkon.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2qvxilgou.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2ssryvfbl.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2enngkwto.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2afoomvvr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xouokmgz.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2bncvewiv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wnenuyus.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2siqoswdt.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2mqxoujqn.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2tnmhgmgf.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2pqcaipxi.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2xevbgceo.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2xvlhfdpn.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2rkpfuhoe.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2ljqokeum.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2guhjkbvd.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2zyworyjx.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2jwbyvykx.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2hhsfyolu.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2fjrhlakt.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2xrmznzka.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2ssbnbxdw.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2dacaduqp.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2gagjwlpf.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2wixosdgb.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2qlslyuco.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2zmkxttxu.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2pcsrokgz.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2zpcravip.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2dkafcviy.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2qbrafnqv.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2tsheymim.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2lcqnqzgt.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2lmxoavag.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2iehshkri.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2yyojwosk.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2dnxoyfkc.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2tthwgdmp.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2uavvpttn.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2ssaeeuek.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2gfachgbd.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2joqqoxpp.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2bvwsuxut.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2kltelvau.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2zvgrndmh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2iutcgxrr.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2azzmrgoj.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2pkwiaaza.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2gtrsexhp.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2xhjekwzm.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2uzmabmxy.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ibiebxma.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2mitkpbms.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2nmtzuuup.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2fnpjctom.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2guoggqmf.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2difmtoul.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2ecrnwrxh.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2cmeccljk.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2mbsvdaff.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2zfideepf.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ephkubsx.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2cparixoy.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2pojolnzk.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2qrqzjuek.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2dnhvwnfg.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2ikykkecx.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2xgmtdhnm.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2wyleoawi.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2qgqazial.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2nuvagsxt.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2ekwohgco.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2ygpwhmvs.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2kbvklnon.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2pseoygte.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2vgswdcsu.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2dhgzznij.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2elgfjlka.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ienoyymy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yuzubxde.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2naqehvte.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vfdttwsj.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2dkveidlq.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2nkarpmcw.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2jzqkbzwb.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2kfsgrtck.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2tyvheioa.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2cbcqbsxm.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2lbcokjet.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2sgdwetet.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2idxtgflx.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ckwvxhbr.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2wxgqsmqh.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2zwszaktu.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2zwfuvhdl.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2oiqgbnov.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2xgtfvhii.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2wmhvikjd.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2lxtsdhqh.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2tkqwikdy.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2wkbgosak.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2mpcshzpx.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2rtyktftn.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2upldmlbs.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2qsbzdorb.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2rpcrhokf.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2hsdmsuvj.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2efjwoayk.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2zgjdqoqq.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2wcpdvtqg.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2rcrfmlvz.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2wnoshocc.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2jxyxsxwx.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2pxadxjnp.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2iafrdwhq.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2hrpzstyo.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2lgeccmsg.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2egsgsgxa.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2libejdks.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2hligtmym.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2yxltyfmm.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2qllbpxob.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2sfgnyvmk.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2buwtbmij.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2dpxehegd.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2mzqxmibf.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2qoqtlpbv.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2uqopzael.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2ehjyxrwm.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2duhtwspe.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2qnaectqp.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2teqbrjpc.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2txqvxkmu.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2hpddwwls.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2ddialojl.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2tlqdtrmb.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2ygalviss.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2bqxfbrji.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2ygcxwtba.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2nlrpudgc.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2aeeswdtl.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2hpikuvla.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2xuesjmpw.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2khoexiqg.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2xxhruhpw.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2uzxqwfgu.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2hkvbiqou.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2onxffayl.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2epavtvnq.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2cuiszspb.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2laeksknm.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2gzdvrrbk.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2xvokqpkj.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2vkgcftcz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2unpdqfia.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2znjeeswm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dehtoxaq.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2xelgerce.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2coegxejx.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2pdifulpe.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2ffiwuvst.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2sghuytxd.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2lcrkuhet.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2anvkerfh.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2tewdkvzb.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2whsvwgms.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2vgizzhyd.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2xryaxsjo.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2pihizajo.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2efcrdyja.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2ejklkogp.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2outzdsxr.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2omgrwamj.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2umwqmgfu.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2pjtzsoxc.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2mzstnosk.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2uhkdygmh.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2fkhdrmqw.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2glxfqdhj.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2dvrfqdsp.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2gxybgpwn.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2jstsqudy.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2atjnkhtt.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2myrtadgs.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2vdpnnbqm.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2ysxpiqcd.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2rdzcenij.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2abotkzyj.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2beykpwng.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2whvainui.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2nzoxckho.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2jadvygka.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2kwqrbqlt.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2chhxwful.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2sxnjfwsi.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2btincqxo.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2kdscwnqd.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2tklmgrvg.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2gkabshvn.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2fdzxdgmw.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2zvqbpejl.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2wcepiycj.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2jjreaigj.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2dxgkocme.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2ucnehztc.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2xzovtmsg.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ztdudgna.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2djcoducg.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2tyadmsiu.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2pkwgyfda.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2ekceacdm.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2sigttuwa.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2qohxaxzb.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2lqujghmm.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2vxtwbqmz.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2kdnzfrqr.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2dsvkckep.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2riiqkitv.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2glvqqxus.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2qeebikkj.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2cvqzkyjs.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mmheqqth.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2dkbepwzx.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2nthqjxpj.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2gnylgsgm.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2bgklgext.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2edhzrsdh.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2usccfkez.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2nobxumsa.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2vmtxwzds.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2bujuvfuj.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2mzjgzkxd.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ooaqifkt.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2dhtqausa.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2haisdywx.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2oywhlwdc.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ennhfxrr.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2atkrdohy.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2zdzbllhi.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2nctfqwbz.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2ehmjqnwz.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2moqohzrs.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2jxdbwxgc.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2afjdvqpl.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2getbpyrj.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2opwrdzyu.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2jjjxdvdd.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2cptptjfp.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2vfpvzzhi.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2koqqyhzw.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2qmjjypoq.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2vowqdfmn.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2cqfttiyv.html


<!-- 参考信息 -->