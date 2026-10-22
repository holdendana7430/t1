代发 wailian999

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2aqwwhjbb.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2vnsapeqe.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2hferdscr.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2xcuhjnyo.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2ehbyyhdr.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2nqhorpzf.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2qrlcqmxo.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2ebtcabrb.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2iedfyqih.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2nkbntctb.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2oscozbxv.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2yvfanbly.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2thwokrzy.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2kcacdzvp.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2ydswtuxe.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2sgzxrdrp.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2vcblhwxg.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2bybxlmjr.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2czdqnnsf.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2conmgduc.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2swwbwtba.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2ouolvzlc.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2etaclphl.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2pvpcszag.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2orxwbckz.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2fougytbi.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2qavgvbon.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2mkcpwetz.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2yjpwifaj.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2caqjbjxd.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2iezbmivf.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2dzzthpzc.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2zorhrmrg.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2tgtlmyzt.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2pdaswroe.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2attxnkmt.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2ezwjwdmn.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2eozdfyhr.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2iypbbqph.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2trklxnxb.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2kbkzghjh.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2ppwywoog.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2xylvynqx.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2vzlsrxkx.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2ulgleonp.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2eubjbkpr.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2eylotqpt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qocepulr.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2pzsdauaq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zzjmekft.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2oabopciy.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2mzuokkxj.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2tjtlvtit.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2etrcgnri.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2kpcqlywm.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2vqyhukyp.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2zpvgbpuf.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2jhoeejsh.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2uegfykgf.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2lcmevlzr.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2ouxzpxva.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2qrtzqnal.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2dfbmleyf.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2qosudtxo.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2ydangkxt.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2pucsairw.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2ojqvlltc.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2cowsapfr.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2anmzzicj.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2yptwlgkm.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2nswpegal.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2tsacrcmx.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2ookrnvoy.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2fffujgge.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2bfasfbvt.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2dojpabbg.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2wcxzktjs.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2jqetjzzm.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2cyduepee.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2nonsrqyp.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2hlawajzt.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2wrgqctnx.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2xwzaedlt.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2wfcowoyy.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2ozyjwrkn.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2gdadtvap.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2yphknmlg.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2xmonduye.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2ntfgrynx.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2hvcooyfk.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2xepfwbbu.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2yhemzyvr.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2kwivxvkg.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2seuepgsh.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bwuuacfm.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2scelkluc.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2bipqnuwv.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2gkvsntee.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2veiufjzl.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2lzcgolyd.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2hnwdbpjd.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2nfbqgmhx.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2lxaswjbj.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2cbtsmjzf.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2xsnzjtsq.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2fiiixqra.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2jalvplls.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2nadimkzq.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2akqscpll.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2ydhtydya.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2ssrmnfqj.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2iqzvoyie.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2budgmmju.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2dggtosqw.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2rvfixqrh.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2wrzhfxsj.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2otlqmgqf.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2prcdnslq.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2qyggdtww.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2ktnqulsf.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2mgipmfdg.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2binvxzpm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qmhqfntq.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2lvosubow.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mxjncxoa.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2ldanszaz.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2bvkksgrp.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2hbpbfgqs.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2fgnfdjev.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2metlxbnf.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2obohzmhg.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2reibxifh.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2cssbagzv.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2bkbjvnjr.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2edrcxhno.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ylluapfr.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2axvcjyxk.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2uenankup.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2rjrfndsb.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2yvfmcvcs.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2uwtubkzv.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2yxneltbh.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2xpevmxzt.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2ghxlrlbx.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2lqbpmwxu.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2kbweftyl.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2egwncaif.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2ekehtelh.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2oncprunz.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2fxkhtfau.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2qtjccimg.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2ocybwwjm.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2pcsfnpaj.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2ippxwsww.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2dvpwwupx.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ciuzsekq.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2hqjrutux.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2atmydbcw.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2pbixnqkg.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2wbwpdyrs.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2qexdeuez.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2qihnvica.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2qrakblzo.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2reckhrna.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bfdiafzs.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gxiiczks.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2lvxyfwho.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2khyuuzcy.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2vwyonhra.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2wjuucfqp.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2ougdtbmf.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2lkjleqrm.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2kwrngqsn.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ztdyslav.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2dnghkcwp.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2eedazxsv.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2mforbwsu.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2qyhywuab.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2dmgfmrws.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2fluycbne.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2srualoju.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2ypmqasuz.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2rpihiqzt.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2fowfblvo.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2czmrllnr.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2wrxcsdeo.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2ofjcjsfk.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2ibdzekkf.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2uermwoqd.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2llwthhpu.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2igxvcmzt.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2dsnoxoue.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2zrzxfbow.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2fcuslfgi.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2echsofop.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2cpftgsmf.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2aanwnqyj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2shhiquiv.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2vhlngxly.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lqtxfxoj.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2tsqrzfke.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2btgjhgvx.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2mbqfmhjz.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2lwdgivzm.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2prmzwpii.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2rfkfbeka.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2saynebvr.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2enuodowe.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2pgsbggyv.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2ylttsidy.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2dgarknxl.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2kemqoadu.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2wjeswnvl.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2basxgczz.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2qrhkfowm.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2mxrwafbs.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2phsgolym.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2ebevwnpu.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2bhfjrpkr.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2qtfcdyfw.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2piwcswnv.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2nsfybrft.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2glmqwobg.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2tqexqadc.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2zfieayhz.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2yebezcjx.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2tbzgpmom.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2yhvigine.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2akzamoyq.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2aocmtbft.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2qlugglfn.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2xzasrsvm.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2esdaegwi.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2aioiikai.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2lgxwbupv.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2rqyloust.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2jevpzfyn.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2jxuysxny.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2wohwncac.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2vszoiype.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2zsglqcwq.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2otrdhzvs.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2baezjugt.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2okebuquz.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2acuodaja.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2osrpjlsr.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2hregdpka.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2hbysrukt.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2wrlfykqf.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2dowqzxuv.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2tetxwkok.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2tydedfyw.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2lowyxjkb.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2odipmgge.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2efemfsno.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2zgeylbzi.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2mbdofqrt.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2nkzrmtzk.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2uvyqaxdq.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2jghmkoss.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2jxpfwlyq.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2xszjnvyw.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2xtrmzueq.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2vnfixjxl.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2uogsrvci.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2xcwytcxo.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2mbhfnynq.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ozsdqqjc.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2abmsxxig.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2xauqeest.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2hhgolxre.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2gtzxnyxx.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2cgcbromp.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2xkhcbykn.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2lzjxhqwb.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2lsidrkec.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2cijnqkav.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2dcaeycoz.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2qzvpiylf.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2fkjvtynn.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2tvdtyuoy.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2dkfrqiwi.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2nyypaubb.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2ozwqggbl.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2scanldlt.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2wehiuqnk.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2nvfjoumh.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2ivippscd.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2evbfjnmv.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2plgqflhz.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2vkdkptfo.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2bdrfomep.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2vvailufz.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2wkuurwlg.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2vjfdwcch.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2brycdmmx.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2gfqujhpz.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2hqlynyrr.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2luypvsap.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2xxkhleoy.html


<!-- 参考信息 -->