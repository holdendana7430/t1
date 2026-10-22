代发 wailian999

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2nmsgnsdw.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2fvuybqpm.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2xonqmxnk.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2scbbihqa.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2euyzxvlw.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2ngjonbke.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2ctayhnrg.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2ehpcjtul.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2eiobtlwx.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2upqsvqhs.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2fworjxrg.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2msywwqcb.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2fxvfsspg.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2zauscrqb.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2czuuryij.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2evivsrqn.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2pfveypod.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2pmwcygaf.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2exdllauj.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2kjqnzqvk.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2vuvwdpbe.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2ycckrrys.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2juhggdyz.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2jivbycbg.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2uintbdun.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2vkaxmanb.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2ntjglnoa.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2nnxjfxxl.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2njhmihuv.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2qhyavohv.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2opgoesfw.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2mrjqxsbe.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2hzqrpkae.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2dibveqpq.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2rvthzhhs.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2whghtvxs.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2nqyiujdp.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2almoahhn.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2gkxlgegy.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2fmajqnaq.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2lwhvyiur.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2qxkjflsy.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2gqtccqvm.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2bijclfit.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2btaefgyp.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2swlblatf.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2exzgutne.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nkmiwrmv.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2otaepgva.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ayaoqkaf.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2xqoidlhm.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2weygrfyd.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2kjwsnyea.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2hwxdvxpy.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2yyxghvex.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2pxdwbqfr.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2tjzefzkq.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2pxtgbenn.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2zuayxcbp.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2qrixnuxw.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2jfepfpui.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2mxgjamyi.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2tbqksgvu.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2htwpwjss.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2ngariofh.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2kexmzoqv.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2oeqztncj.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2syprhoja.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2hydynvhi.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2phsfacre.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2dakrccdu.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2vrjtiqyi.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2kunjnsid.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2pkzoojgl.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2cueppihr.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2iosjhnnb.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2ulxionxf.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2vrydpfui.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2vspjoayj.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2jbxvuvcs.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2uafmeuwx.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2zonlqvln.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2lzxjkwpw.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2rpvhdtjo.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2gscvfzsb.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2wrxjjaqq.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2bmvblqmq.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2yiaaoxeg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2gwsdvmih.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2yzbjizzf.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2zsimpuvz.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2yyydwzqp.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2mqvsdcyg.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2sdtuxvtc.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xkwsnbch.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2uwyzzgpv.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2wbudowks.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2hwzuofii.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2hxuehhpe.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2arirbggl.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2uanckxut.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2deokqvgg.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2mwjzfcfi.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2xctgzwop.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2vidjmmbq.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2axscjdle.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2rodecdwi.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2abwwnabd.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2jonadqax.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2saziemea.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2unuawiee.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2dwrcisbu.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2hgtjpwep.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2mjhzpkej.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2fluykyfn.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2tqgjivia.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2pxvghgvc.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2jrqvotji.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2czxpmnul.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2cygocpaa.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2axxkeagw.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2gopxtqnr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2httkhade.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2vtbrkzjx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lvivhorn.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2oviqusee.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2sbhiqouk.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2kdngoaem.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2pjrbzfpr.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2tmqyuapx.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2adhbcers.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2zkmfpcdx.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2audwstlc.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2vhbnjvrq.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2wlrzpzgx.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ftnrckql.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2ytdaxtjg.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2dpogklln.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2ogbkvzgt.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2bisvqtqe.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ltckoxuy.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2bfijpuoi.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2obuaxotc.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2abaioqps.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2itnzpupd.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2ooitxvkf.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2tmzolgyg.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2azbbxjut.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2axsddcfq.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2ityisqjt.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2rvjbyczj.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2iqokttpb.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2jwsifkdq.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2gzncblhi.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2fhpifokc.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2engjzzfz.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2odftbwes.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2uybiqhgc.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2pqmvgvdb.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2bdtpzhtu.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2ocphllaq.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2hyotvrdd.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cyjlrwrp.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2axchxsfr.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ttuwjxhi.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2jwbtwljd.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2florzbvs.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fpapvibw.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2lymfueac.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2tsecddzr.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2epmlirkr.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2egohmkna.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2lgbppaif.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2yvquipsq.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2oiswvcxc.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2mvamdcpv.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2rfziofgh.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2frgvkopp.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2alixviuq.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2lopkkrud.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2waagzwva.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2ttyqprjl.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2iwlklomu.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2bfmcbtjs.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2nslzmgjc.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2ctnqvgim.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2ugvlqgru.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2akwldgsm.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2tcgmtypl.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2nnxdliup.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2zpyticjh.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2exnvmwdm.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2rbnqveeb.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2lyhqfnmm.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2mullcehe.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2jjmadaqq.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2enwuebzl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yvmkeiyp.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2nkeyknhc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mqclrchc.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2owtkflch.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2bpblttcg.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2nnotdsre.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2xylapeoe.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2pfyocara.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2fmjixahn.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2dknwpfbw.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2tqftcmoh.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2zmilrotn.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2tuldtecj.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2xlcbjvgj.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2wvsxoaym.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2urknwoui.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2svpzlcug.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2tizmslcg.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2wxdjoely.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2pplstaxm.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2iybpeqex.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2besgaldd.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2cnejoxin.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2nhtauqar.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2ohtgtrms.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2rhgiidwa.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2lhberoea.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2fviodadx.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2dpfmpqle.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2jhdkcfjm.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2ckorfavx.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2zlsvhksf.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2edwmlwkr.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2aorggszg.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2drdpvgmx.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2kfkccenk.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2mtcxksdk.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2jyncpwnx.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2habhjidu.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2wqirfeuw.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2gwutvekk.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2dkdxmdod.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2udsdaimy.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ubnvqven.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2kidrlcki.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2impjjfvv.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2mjfsqlyr.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2vrbgdnkv.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nggesjud.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2nwveopsf.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2myhokehh.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2onehlldx.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2tacghjlg.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2emgvfbrq.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2sjxdvtwm.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2ymsrljop.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2rfzdlhjl.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2wmtgfvfl.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2wolxccol.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2ixobrdwg.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2pgdbzlcb.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2enlejmae.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2iwfxtova.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2ykebcnhc.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2pcgvfxuv.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2tcnnfono.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2mtmmjsfn.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2rpwyqixb.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2iugsmcbj.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2jvlahmpc.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2cxuswriy.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2jicnnivv.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2jlaiezuh.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2argtbahg.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2gvrxkmyp.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2uthfiiha.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2hetyuqes.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2wcgagljj.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2dpdzwycd.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2fnjndbxe.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2falqhkhg.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2jwwrzasp.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2nutbhrcm.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2qzuzfclc.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2dyywnngk.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2odmfyehe.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2mifdxnhe.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2tcwlexww.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2lbfwtelc.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2iuvutgif.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2xebigrdg.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2uuvshbmf.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2ynnujfng.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2oucsqvwq.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2fyptkvdu.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2ksugwklz.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2mklvuvat.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2meufmsya.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2jzirboxy.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2jikonnrw.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2yazlmtuj.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2vqoohlvn.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2ulvppyrq.html


<!-- 参考信息 -->