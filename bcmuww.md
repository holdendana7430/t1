代发 wailian999

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2suhdojcb.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2cdibbqjn.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2smwqwmmt.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2kackcluu.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2gbykyfwo.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2kbtxnzwa.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2deijykpj.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2ljfgsleh.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2pluhmrrn.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2motgxllj.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2uoxsskaq.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2eerxstcs.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2jgzqaaum.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2suzwbnfa.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2civfbxaz.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2xezlahau.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2nbwljhec.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2biqvezhm.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2xnsxiyys.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2sqkzhosl.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2beulnvci.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2sgcrgrzs.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2rrkyjxea.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2onvcdgau.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2mtyyeppn.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2bhzrpawl.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2pmwwrktk.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2dyefsbtc.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2vsivuhdm.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2mthrrkmf.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2zcwasrar.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2bvhfeero.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2whqjytxp.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2xcbbgivh.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2mjwsqeuo.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2bfswcqpc.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2vomhbrtz.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2hurcfnxn.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2lcmhywag.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2anvvoybg.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2sctyrubr.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xhuojoif.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2cryafrek.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2temsbmuq.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2nhjdlggo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wsvvcuzt.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2nskgbykb.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2qqramjrb.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2tkaikauc.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2ixtxohcr.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2khjxsgxv.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2xqfrknvc.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2afhumswt.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2rxkshurn.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2fgnpqhcm.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2zdfqxvvj.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2rbwtelhi.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2ofqbquyf.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2cnmpccaa.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2vwuorvis.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2czqiwclb.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2bxmhyimc.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2hxvhjovd.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2gzazkgij.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2pxvfsmct.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2udcnsnou.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2xgwpssnp.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2zjyrdkir.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2xgrdpyjm.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2rgvfiyxk.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2rwamljln.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2vimnbrsc.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2qzpeccgj.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2ogrcnytr.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2fwxuqsuw.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2foezgpte.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2evelbwsm.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2mphgyvvd.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2fvcqbypj.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2zmxymiif.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2jyufezre.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2fbskvgmp.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2vspcapjv.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2npgwfpjb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2wnoepplv.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2uyabqvwz.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2fuzfzaxf.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2trpvzcvl.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2ejmaztzi.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2bnsnbnwi.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ogblqloh.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2zaanqbpl.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2dqminnhe.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2esxxgpbl.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2mlbhlmfq.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2kjuadosq.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2yhcxibmb.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2ykvydbxw.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2ailttjzg.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2aezcgxvu.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2xyhhcuxx.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2smhygebn.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2clsnxcit.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2zyrnsvnw.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2wgvtgojy.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2zwreqfqu.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2meluapxf.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2xcfqnipu.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2wdigueyq.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2wymhlgju.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2wvpbcbqa.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2lhikrrkg.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2mnzxgmfh.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2mdbpevdy.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2vdhxoota.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2ksywmloj.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2siyauenj.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2hwnyptvj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tbsoiwbf.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2xtkubmjk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zzgeuvxv.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2tqugdqef.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2gdysvnzw.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2bxwvopxy.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2eptkgwks.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ugblavcw.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2zskxyenm.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2ddasiwew.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2xapmjbmw.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2jiscvsnk.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2jstdgcvx.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2bmhtbtxo.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2ergbtref.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2orioekbk.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2abggzwst.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2kpbljnwj.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2fxcrivmy.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2oknvsrnd.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2efcougzz.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2ocsecdne.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2livoxeth.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2pyicxult.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2nzqxgeei.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2xhfnuhma.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2otwwucap.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2tbmbgxpo.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2kvxahdvm.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2nvadywff.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2ucrhgjtr.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2mjnejlwm.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2ovqlyjxf.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2kobzmnbr.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ugrbfbvw.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2padormih.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2pnphrfjg.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2gsvpmufi.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2jqjocusb.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2nnapezoo.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2frqlmnjg.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2uqztuhoy.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2grntcroo.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2moxdivzg.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jjfregbk.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pnrwrfyk.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2elwbiarq.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2uunqqdtc.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2rrmiimxr.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2kjpxxnqc.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2vaskagas.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2olqkpcvd.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ghgxdplt.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2dmqnplkv.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2mmcxwobb.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2qpybjmqd.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2avawxqww.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2qsejzrpb.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2wydbtstc.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2gmhivpcm.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2yymrrocr.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2aeummmdi.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2yayxrzbc.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2phgnohrt.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2goeuhbee.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2rqaxbqmh.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2nwkcvahn.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2cwvqxlpm.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2anhbgpbs.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2lknbchrj.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2hqefmeqc.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2qvhkzttc.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2esybqlvo.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2pgznpyil.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2elvzartj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rseoopgb.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2wimpmgpr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2daztiyog.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2zchgklze.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2zznklxkn.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2aqsqrjxg.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2lczkyfuh.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2wckmxaew.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2jkrrocth.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2omnxtyed.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2eyuomcmm.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2aykeoqdf.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2bchsjrjc.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2cfbmelgy.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2kcuzsowi.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2hcdlrjtv.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2vateckys.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2bkvjxvmx.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ixpdaabd.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2huoltuvz.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2ikagplcf.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2qhtfrzew.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2zahzahwp.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2uddycont.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2qallwtdb.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2agtaqmws.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2ycvtneyb.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2spoescba.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2hziphqhs.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2bqmnfplh.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2zvkcrtgh.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2isqkssva.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2dzkvclpd.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2oetsbtvq.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2ujhiraws.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2hewrpiqx.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2klpdwwxp.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fgxatvti.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2aceruxnr.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2vouwebyb.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2hprqniqz.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ybynairx.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2bzrxdihs.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2auldognh.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2opncohfn.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2yzmlsxji.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2lljibwlo.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2chxbacdr.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2fvpaxsuq.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2nfsimehy.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2hlgmtrbc.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2jqyrlwyw.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2wxhyrbrw.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2paxwsdct.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2bfkpepzg.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2qkofvkhe.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2ftbobdyf.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2ukkyegwg.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2txbezeoy.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2buswbyen.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2wljomlmo.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2ohmltofe.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2muiytsoj.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2qgaplbre.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2ghikzlft.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2jsggxsez.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2omksakqv.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wodmknft.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2egcboxvu.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ojvoqxod.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2kbawhimq.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2chvtnpam.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2iedhcvan.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2jtzaoueu.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2nlcdvgvv.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2sfojdwcz.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2sfszrxns.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2lgaeygpb.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ztmjidff.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2yensqtsq.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2wjnwtazo.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2vlrabcjy.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2kipfvwri.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2xuklrjga.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2oiolshjg.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2tvvcvzed.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2ymwsffyi.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ygnvksmt.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2hnbnuaid.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2updddynr.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2maarhlhb.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2pdjsirgi.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2ooeoqizg.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ifnoqrra.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2baiiodgs.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2byuccjog.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2lwfdnyay.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2dxilibhv.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2socgigjv.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2ionfjpvp.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2pzkeijtl.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2tcxujxed.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2lanxdydx.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2dtvqxsek.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2fingmbxu.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2zxqraare.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2nkxpffkc.html


<!-- 参考信息 -->