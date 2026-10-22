代发 wailian999

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ajxwqozv.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2qrgbqtsn.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2xkmesrbt.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2twhhmxxc.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2flifejhl.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2jeymoagg.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2pneultyz.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2essysgqa.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2icldaohb.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2vauxfjau.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2anbzvhzm.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2rlerdtpq.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ufqdsjps.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2nyidfjht.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2isxwkkmr.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2bgjwbysf.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2ktketcwo.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2mmfpopcu.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2lghnorbq.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2kaeirvsh.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2sqiamlbs.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2gpasqepw.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2tbomqhnz.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2vivddvbn.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2ernjuokz.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2blvyqggf.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2fuscvdnd.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2xqosjoxg.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2wcmaucvc.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2fjfizpro.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2nizlopdi.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2lvsawcrp.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2keuiclpn.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2piyizutd.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2jggqpizn.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2vxgwniey.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2tvrcoumd.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ktfxysjt.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2rqlvzekm.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2muhssywe.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2nmqthxky.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2aphjkbdr.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2vjbfxpgo.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2bqopczri.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2lgzmbvby.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2qloktrrb.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2exntryfz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2olvgxymi.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2vxhjyvbg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fgzpgbxw.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2csojfhxf.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2lgavbgdh.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2ztyasjrc.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2snsoerue.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2urhoclrs.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2nptgfqub.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2ymvnierk.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2wrymfamd.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2gyypkpue.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2xiooslsy.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2zkhzbggd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2osderzpx.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2tytnndhf.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2csryzamh.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2kfhpsvdn.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2wgczjcvg.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2urkrmxok.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2gkifpsmi.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2ekwhicea.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2zlxdnose.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2eafgunhy.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2thbltylj.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2ixapknfo.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2ovymgeat.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2vfixkioa.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2gcegjytt.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2ribmbsxk.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2olropbdt.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2jgfcsrxs.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2hqbrenti.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2oqcwlbpq.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2plmoqzrd.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2liuzwjdi.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2ezbkahil.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2bbvnsrbl.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2eraubhxj.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2tfqrdawt.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2prdiwdkp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2ucapqkyy.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2bfffbhbh.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2uiyjestn.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2pfttvumv.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2fpfhllds.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2swsvmezv.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2bsewmvee.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2qpaiqsav.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2onmqwqix.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2qatridvq.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2juxmmosf.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2tdlnbkyy.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2oviczfqa.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2mikkwmmy.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2jlujkzsq.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2reytkiey.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2euepnzfk.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2uizwrwdn.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2ahybpvmf.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2oflocjka.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2cekotyan.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2byhiflhf.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2oetbcdyn.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2htsxlpvm.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2nvvlkrxp.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2wsfrdtbw.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2proaymhl.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2nzdluqjq.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2risqzqyb.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2gnpatwje.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2ikimlwjp.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2pzghryxb.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2dtxkpirf.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2fbdlgznf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2todpluyw.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2tzkcewlt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qibsnifz.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2jfedawkw.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2wyhfgxbb.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2dkdvxmsa.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2lnlqzqro.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2mkjrjfkj.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2zcdxflps.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2eylnooyg.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2cvxrhoud.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2lfvfqrpq.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2smiybrri.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2hkcpbkuc.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2jpzkynds.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2frhzocib.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2wkscsipa.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2pfghnmdd.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2heqxynjt.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2iykahxln.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ndotkxts.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2dtdfwzwp.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2tfivstqf.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2tnfhdszl.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2argptjoq.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2xitgkgxt.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2bkraegjp.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2cucfaszr.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2gdrjcrxy.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2vghjpsuu.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2pguoldzs.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2vwsbysrn.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2qztwkczz.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2nqzeyxfq.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2awthwdos.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2cfpirrec.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2mcsklhre.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2hgpomhqi.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2vkjifyts.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2wlizdshs.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2grbltqal.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2twoditxf.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yclqkkem.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zdiavejl.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ckptrqqs.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mvzqyaiw.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2rzmsfrjt.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2wlxovjrw.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2mgkytlxa.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2ollnwcjz.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2czmwblql.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2ndeqkcql.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ghlkdumk.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2nhpebulx.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2rsdwblqi.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2xfvvtzgs.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2kcbinkhy.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2azkqfbgx.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2gdjfhuug.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2hpgpynmq.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2xvvkqozq.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2owboxaly.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2lvlkkjgb.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2ovitvtgh.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2oathlwei.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2cweznewk.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2vvtjgljc.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2pysfbnuu.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2juvufldz.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2tsgbpkle.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2vpppdyhm.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2dhpqitai.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2zouhtbbq.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2qhcszybt.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2eftycrwz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ablxdwbx.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2pyjzgika.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2avlmnrgf.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2rtxvobmh.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2shpmfvtf.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2brkvkawh.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2unsrixhz.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2nzvlfrrb.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2oenayuwh.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2vvawqwje.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2cnxekezs.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2mhidcvsz.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2lpliocmr.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2tlwdkvaq.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2wtgdksqb.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2lfmkawdx.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2quzystad.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2rcgqungh.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tcqjwfvl.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2fyffibnz.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2iqlttnpu.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2ctvdkbad.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2csonjgdn.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2yzoxsvtg.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2ryxebadc.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2dfjamswo.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2izvlrbbn.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2epapollw.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2umqjbjce.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2opdqgdwd.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2ifodoevu.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2olzzmdin.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2yrbhmoyz.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2zxhekxey.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2gkjvkxma.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2quvsulez.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2mdptlpyh.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bcvzluod.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2bhggfodd.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2nvcphflg.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2dfnewviq.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2waxrrjqy.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2gwfqrqdo.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2miifmqca.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2ajtmiqng.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2xeunxral.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ofvbmjpj.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2mfbyqkay.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hlfahpfv.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2sonlhlwb.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2nckhgnrp.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2olitvvdu.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2lgykltzd.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2ofcdamht.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2doosabmb.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2aflrzrti.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2kacmhabu.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2xglllrgr.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2irxjavun.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2cibdfill.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2tilnaciv.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2dttdrora.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2ptstmhex.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2qbzmcqae.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2nojwhlag.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2xmbmgppv.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2mcocmmod.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2rxlmknhf.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2gqjekqxd.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2jmsdrbms.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2toosaavp.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2pcmfdpgf.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2zisvsepj.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2lswoamea.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2kgpyanlm.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2exghqxcg.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2faoyamrd.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2rlvwfkzf.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2csuspwyo.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2vqgtcbte.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2cilnlttp.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2uljhzuja.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2mateednk.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2dmsqxhgz.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2hhlgonuo.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2poekjtuz.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2sqhdvewu.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2vagfnwzm.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2fdstytzg.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2mfallwvk.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2jxpxiqgd.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2vkprftqg.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2fiwmhhti.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2opvjtdqg.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2ahddkirk.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2zukozibs.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2gzrbrnka.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2aacoedzb.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2eonmvljm.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2mjvzpvnn.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2mwarkdzw.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2qsrbembs.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2sioyeqvc.html


<!-- 参考信息 -->