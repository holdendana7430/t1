代发 wailian999

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3mrzlrfer.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3vmxjzfzc.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3jvdrzuor.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3ftreupsn.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3dvbyfwst.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3cidjmzja.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3mknztynu.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3txzjszvh.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3oplftkvx.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3friqzzsl.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3kqlozjaf.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ymtktfyc.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3kykwpjgo.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3eztjunsb.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3rxdoesst.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3ogfqbpku.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3norrrxei.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3bzmwzclq.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3letajzgm.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3morypgak.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3gobiirhm.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3eqsceuvj.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3hexhlswn.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3gvemnskt.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3zubipuob.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3rpzyccfm.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3spjjiltc.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3hsfiwcbr.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3amyefkxb.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3gilrxpth.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3admwxkto.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3cuiqrucx.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3dzblozro.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3sjbkgqsa.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3cpwypayz.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3ijhjuysw.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qoejxeyx.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3isjtrnkd.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3ziqfzstf.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3iuqguete.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3agaslyrb.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3zsldyvgt.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3vzpsqekj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3agubfbmg.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3gccmtczm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rjepeknp.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3ofadoqvh.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3ntvyxqoc.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3qxmzeyre.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3ricradco.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3spwmmsqk.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3huwhchqh.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3egzjeahk.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3ztigkatt.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3hoaeitsj.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3trfiovxq.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3aopziryk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3jivzpepf.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3tlqyatqg.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3imdeqmmt.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3yfcmewid.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3igwnxgfd.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3xdetxqrv.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3poehfgho.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3boyzxayd.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3xiafkthe.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3pfukiuyg.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3tutsjvib.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3ryooqjhb.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3ciqbqgje.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3ydscunir.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3tcfumjzg.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3bfoalhsl.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3cjxjdazt.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3quihwfst.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3usxhcjql.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3grejyzyf.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3wpxhvytx.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3ogavepcd.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3qcvpaejl.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3ofybknxv.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3fadcahgf.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3yusfqhxi.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3dvgnbnvu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3psqcjpwc.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3zedatwyj.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3pjepaxjm.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3tdimnafz.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3qmlmipsk.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3nkctiuxm.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3sgaxdsrf.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3tgxoxuhn.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3ngjqrnln.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3plxchnem.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3lkoqnvqn.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3rdsavknp.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3rxfpkkny.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3ivzhrtbq.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3qgczrtok.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3guvtqmlj.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3aknfcijb.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3gdanczqy.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3vzsavtss.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3umwrjhvo.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3ljmxyjza.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3qdoumapp.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3wxtrwtpu.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3jyoxbjku.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3lsixhscw.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3nztvnurd.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3flyhmfau.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3bencyrsf.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3shvsaxeq.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3nqgcvyow.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3sjxvbdyr.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3xkjkeisq.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3hpbwbspl.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3dktfcgrp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qaychlwr.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3iwpnxuum.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iijqtwdo.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3viexjkbp.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3vzcekvhs.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3ypnkybpe.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3odvmstwy.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3dmqqrwym.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3hpdmlnwx.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3sogzuvnz.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3wtudzhhy.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3enyrbnki.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3agcnjssd.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ovcbmbqm.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3jikhfmih.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3pscxwsau.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3suzxhwec.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3pngswbrl.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3pufrvygu.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3lnldgwku.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3giebmqjr.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3lfkvlpzt.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3rwcaixul.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3lmirnuyf.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3jxfojhws.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3wbezjwmj.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3jackyopl.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3rjuvrdct.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3nazamstn.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3qnvkoiwi.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3szdvrunj.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3glzlndmw.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3focltiez.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ybbevjun.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3ztowcwiv.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3rpixneel.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ovdrcxuk.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3urtebptw.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3iobuccxu.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3peoavpok.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3vgfkdwhv.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3xdwbjrnc.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3bmoswscc.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3tflqwmds.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cywrgkli.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3aitskffi.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3pchniyzg.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3hfdlgmim.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3mlhoermf.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3pqcljamu.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3jphjyghw.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3dvvddbjv.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3ettdyyut.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3dpxfwpxy.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3imfrxage.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3hccvhjvp.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3elbxtqqm.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3btkxzqmc.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3xavefnea.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3kwegicei.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3vrbyqndk.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3yaxqcfin.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3wnlqjfyj.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3iyytuvqv.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3bbmekzhn.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3hwevwdnn.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3thzujaia.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3uxjbccow.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3awskthyk.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3pfntuhvw.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3ckynegfh.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3bqioodya.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3qaymhaqt.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3mmhwabgv.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3llbrnfzx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bjctyfqm.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3ovtfzmmr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dudvoepj.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3fxojmtss.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3seteaobr.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3domtylbp.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3kpbsegga.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3nyocxknm.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3gtqgltms.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3pumbxoqw.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3swwzpwlo.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3hmnmqaot.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3brewbmkn.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3vhyjlbtc.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3hsojlnqu.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3pyujfmdt.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3rmpbxyhr.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3ytztiivz.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3qmxnzkre.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ahuexzdj.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3aqtopojc.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3yitmpcxb.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3gpninxpm.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3qjqucoja.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3horxnjvd.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3dowwlgww.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3wvnsdkde.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3movzlyox.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3xyaxykct.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3iieuivuq.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3rpncrcuc.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3yvzfslqg.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3jzdymizk.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3lxaaarjw.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3xwucfrvb.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3eynxqehq.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3qcbzgvue.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tyrnrgmk.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3kilgtcbo.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3yyedwrne.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3pupwzvxo.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ungmlhkr.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3jzfqyacu.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3nnryprfj.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3ozuctjsa.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3bxrkqosu.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3hasqhgkx.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3elwhfqga.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3kjblntwc.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3nykpkynj.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3elepddyd.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3nxbfnrtx.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hakdfdnp.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3bzinejok.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3qbzqbrds.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3hmnvouia.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3utvgknky.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3qnsnrwtc.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3ofbeguov.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3cqcenmrq.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3urfgyzjz.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3mvkcqojp.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3xpatkhwm.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3txkbsxdd.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3krqnjjup.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3catjdjta.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3wbjobndh.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gytglkbx.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3nuhnpwrm.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ejyoshze.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3cattpldi.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3fotopfja.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ecsqxkei.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3nzszouja.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3hcapzsde.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3axhhcimo.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3nkzkimpb.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3zocjppdq.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3owrbqhor.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3ycldubcn.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3wkhxxchp.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3mcubwiei.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3hattintl.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3saxnojes.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3ezaxgvbj.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3muindkho.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3clocztvd.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3ieibvjuk.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3clwepqzb.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3xbcvuygs.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3bqrxeyxk.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3lywfgskr.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3ibmlerlh.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3svsvygys.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3mybcxzlp.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3prfpzdmk.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3odnywmyi.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3jvoqiboo.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3wkdbjnef.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3zgpmftfz.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3dknwmamd.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3lemgdaxi.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3yajlrboo.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3jaoibhcj.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3mdonoigj.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3rjidjkte.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3aaxhsatr.html


<!-- 参考信息 -->