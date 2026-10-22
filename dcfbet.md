代发 wailian999

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2ubhpzmpp.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2qyamqcyw.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2darnqqab.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2twwoyids.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2tmhshumq.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2yjpvlumd.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2kujqfrvi.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2hazmzpyz.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ephbzmkr.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2hvzlhflf.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2coodiaua.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rdyuesbx.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2hzpkddwk.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2bdnqpzpg.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2txhrdslt.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2daxdnktb.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2rminiwkz.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2utkgozxj.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2hhosvuhv.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2kpdgbqpx.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2akptgtyb.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2lmvphmra.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2aebhdygi.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2nnzxttgh.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2lblvercw.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2sutznoio.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2lhkrhews.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2sudwaxir.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2sinubeds.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2xtwnfsbu.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2fqgatluj.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2xfsvvlwv.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2rpippqpw.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ntryskul.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2gsmhiecz.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2mwmusutd.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2rxkmmqvx.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2tfejrjsr.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2deahnpmu.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2cfkmwhgm.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2nwchwbjq.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2hjmflvvd.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2ietypvgu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uljyhwsy.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2fnizxsoj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ytymucln.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2yyklkdum.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2hutcndof.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2qinptogf.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2yelipnde.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2pohmzqui.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2gqdfumef.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2wbqssqzk.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2woecwpvv.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2diqgihle.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2gcstrxoq.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2nbipnlpw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2invhgaop.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2vbutrrpc.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2epticodv.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2pswofysv.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2ivguqcrc.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2shwvdait.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2japumxlf.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2vzrzpbvf.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2upbubkdk.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2dnuewkig.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2ivdzeewu.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2pdzpulww.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2gmdkspve.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2ztjjkcfy.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2iebesdfe.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2khubjmdr.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2jyghkxaa.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2dflghgkr.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2ccxrtcwu.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2yhuuiutj.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2bxiceptz.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2wcjjkgmz.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2opyyyaoh.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2dyioemmb.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2frbbqexn.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2aqfjtojq.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2sadhhfmn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2jgrafiiw.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2useqpsyc.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2eizzwlct.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2irbuhfkw.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2jstudknt.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2kistkqfa.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rtfvqijy.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2kdrzweur.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2qrxmumav.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2nxpxtysi.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2semrytun.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2tbilsimg.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2mbeizwti.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2bdzyggto.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2wugumfoe.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2dsgzsyza.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2hnxhfeni.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2jwzcifzz.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2xoqddufh.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2vmzbzexg.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2zkjltiwn.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2lkbeoleg.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2xworoyer.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2nljjftmc.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2nqradbwm.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2uvyiqfnv.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2oksmfknz.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2erequsgd.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2jjtocpeo.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2zeucxffy.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2axqpjgii.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2ieqmxxxe.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2hagnmvon.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2shlbxhgz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gqkyeqsc.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2nnxwhvbp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iamwuxzp.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2vvnaxrvc.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2pskqprmc.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2dbypwrfa.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2wnhlddmx.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2xwzdsffx.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2kkbewegb.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2rlxvjkjk.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2sghxscks.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2wemdgvdu.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2nvrjlzch.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2inagioys.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2uelnwuov.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2lejykzoo.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2ocsiotpk.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2phqckbxb.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2reuidctf.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2zugujhvv.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2pkmgukxy.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2wzaihmvo.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2hqxtjcbm.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2dvuerbwu.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2aomhbuop.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2ruvruaqt.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2tqstkplm.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2fxnhnaxu.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2syutoirw.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2zsbguqfi.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2zpejmgpl.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2kurcpamf.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2sssmjhak.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2yghlnftd.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2txxxixmp.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2xwlmphwi.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2cfmslnrr.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2pwhcqpro.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2tgonarfb.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2urohwsfn.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dhpsneih.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2pmqmykxg.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2jcpetijw.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2qdkllwef.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vlimyfnt.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tzhqlguz.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2pmmuyicf.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2ysgxxbkn.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2qhyenizl.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2fecemhkk.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2couytcys.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2eonlhpbm.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2gxpjliwx.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2wpffvohn.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2wxgdsxod.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2nnzuvxby.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2yqkrhzxr.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2aqvjsvra.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2xpxvdqqg.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2ydxdenno.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2wzxcbwoq.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2oujdmzpa.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2gyghjzle.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2opzkhvlb.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2zijfgpso.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2rgkrqxmp.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2hdqmeron.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2wiginwyh.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2ulmddflb.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2fqxgsmyb.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2anqpgzzi.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2dzhakrbv.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2quxpxrse.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2zgbwizzu.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2ctmmvjzj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kalqyywi.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2ymzjlcsz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ghkczbzy.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2meraorcv.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2avxmcjli.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2mxrtujjj.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2cbawasvr.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2zmlzlkoj.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2xdjrnakz.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2nsmxrasj.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2mhhzgfjf.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2elvavdro.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2eundrkwl.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2cnirsgce.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2lzwmaeed.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2xthshesl.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2snjkrqtm.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2dbnprhnx.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dcqywqel.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2fcplogon.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2ffstnnwx.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2gzfloqfn.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2bqeuicdm.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2mlepjzrz.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2pvxadycy.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2ccuzpqyn.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2pnafgycr.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2etkdrbaz.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2utyfbqly.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2kkmzmeij.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2sppczjps.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mbdjgymg.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2laffckeg.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2lkuthivi.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2odgncapj.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2gbjencls.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2lldxhmmo.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2zacbfupq.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2qjizhoxh.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2knpkjbue.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ahqiofqp.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2jeqdznvy.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2nyfapqao.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2gvpbbazs.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2dorwvleq.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2wkkuwpom.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2iwgfngvl.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2bizrbigg.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2ksejhklg.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2piuwwgbf.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2eeupmsom.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2uynaijsf.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2cqqypmds.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2mijprpxz.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2usamikop.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2ithnzall.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2aoufxelr.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2waotbrdt.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2hczjvfzl.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2vnoyvqll.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2jyrvqmri.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2pvjnjmfu.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2naxzusbi.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2rvntcoly.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2omvdlzwc.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2hcbnypoc.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2bijlcure.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ypssrhky.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2isawmxwq.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2asuwmgca.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2xapnscoi.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2agapxnbn.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2idueycij.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2vadomrzs.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2lfqiodvh.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2srtruspu.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2gelyfgxt.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2mttbtnmw.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2kmwelzsv.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2wokzfljr.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2mkdfndbu.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2zapwqhla.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2yvepumos.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2veuxayrr.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2jaxiybqj.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2ftwyjdhf.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2ubrflaaj.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2yxbahqee.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2lbtlacwz.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2rzpsdluc.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2kqatyroi.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2mytxyhvn.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2zvcmczxx.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2xxoacbsj.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2mhfibbud.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2fklrjxfw.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2kjxuhitv.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2yaxpvznp.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2qaeacebe.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2fpjrffbd.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2wnflhbpd.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2lqedbvpe.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2gbnrupvf.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2iwsewjfr.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2krqowmvk.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2apbcdtng.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2behufbru.html


<!-- 参考信息 -->