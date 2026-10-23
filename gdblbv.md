代发 wailian999

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3iccxvjnl.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3fvdlfzlr.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3ffeynzvw.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3dbwavbyz.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3fkicjwto.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3dmmtdcdv.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3zdonyjlx.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3tgahpwvs.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3xkbrnomu.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3ekatulvp.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3poukolkd.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3tzpwzmdu.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3sljqszfe.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3wwzybmxx.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3yvaaplmd.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3mzrrzhll.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3zulozeqt.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3mklvltsh.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3ugdlbohy.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3wnhrxxfx.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3wgcxncyf.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3ppovpinc.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3nsxkhvcy.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3rqpvrmzu.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3idirummt.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3hppefbau.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3kwlnfmyw.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3dkgxtmkl.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3xqsvanoy.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3lclipjgl.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3rgtpypir.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3wrwglqou.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3fiwnzysj.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3vtikvkfi.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3qgbposci.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3joprsodu.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3xzyskskl.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3vpmwgccn.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3tkylvlqb.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3gxvyznfj.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3dmbwthlb.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3rvocosnr.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3szuztqck.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3wydbutnm.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3voyqfkhx.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ulrfdsac.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3mtswrooh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ksbrigxv.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3cohtnuou.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ubfucjzn.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3lcwibeyp.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3hmovhrwq.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3tapndisc.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3oloucywz.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3phmafrjz.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3nrfmfksz.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3hzdsritk.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3ulviaxfy.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3bgxeeorh.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3ggxuakrx.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3luvxioxr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3qslhsnwq.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3tqazdrlr.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3utkjddpn.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3tgwubwsk.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3wystypsm.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3iydgiceq.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3dwyictka.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3bdfyknyl.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3jrjounek.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3povdnoyd.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3pnjebvrb.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3flsnelid.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3vsaajkgp.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3swqvvkxl.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3tactheaq.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3nivcblep.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3ucodlxbu.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3tcqgxqjj.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3vsqfcxbq.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3eudlrbfx.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3xtypbrjw.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3ahxzjrjx.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3uqzwjufz.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3wjdovxbc.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3obleemfb.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3zqtcwueh.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3okqrdyqe.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3uxqjewvb.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3zbikehgf.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3crlvrvfz.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3wtqxkeue.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3scejddzv.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3atijbezo.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3enoefofv.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3sfntwkzq.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3whnfurbs.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3ojmygjqd.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3mzyarksf.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3ouboncvd.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3qwxphykv.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3gpjfqvtb.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3oehqdzfv.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3zfabedsn.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3inptfrom.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3otvohnwk.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3vsanqhev.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3wvlbjhbu.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3prwzatjv.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3zoarkjuh.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3vqliutju.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3qnqbbfqa.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3ydwvorpz.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3skzplifd.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3uayjeskw.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3ganiobgs.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3klvwdjbb.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3ygptvkzt.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3vttythha.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3rlfgarph.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3yiugqttk.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3xucoqvpn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gtejuxxe.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3rrnbecdv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oovtdoox.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3gpgbvkqv.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3qnxoktnd.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3jpqlgrxm.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3gwufrdyo.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3eyjfvpdk.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3qynxjisu.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3okkppfpa.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3bvggloat.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3gsbobojk.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3wxvjrtze.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3oqgfuswv.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3cqdjzmlt.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3rvtjohiu.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3unmwgbst.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3awprueoh.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3bcwndhti.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3moymcass.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3dnkrkccm.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3ccxbqhvn.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ewojkprp.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3wuyjvegk.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3gerdpksb.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3ppurognr.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3kytevbwx.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3jithsiae.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3nhsdmwws.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3fvmyhlkx.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3pjgkegcc.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3cusscjfw.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3pjfifvvc.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3dpqvmyhq.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3fchauebx.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3mrxwedqi.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3tnqerqmx.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3vvvwmnqc.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3pcnevgjv.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3ximpuyqj.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jcluhklt.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3ugqzazzp.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gxhtwudz.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3sadcjpla.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3aksbrnhm.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3mglgfewg.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3popweunf.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3ibwrszub.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3rpqcibas.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3kmrpmhla.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3vanojjef.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3egprsgfp.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3hgpzwahu.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3oeqgmekq.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3weoevvtb.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3hwdprkys.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3iiqenckz.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3tdachdny.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3mzytdxlm.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3nyxesbvi.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3mmvcpogb.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3zuyrbsqz.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3pbwqrvle.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3vwkxvhms.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3rawfgetk.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3yqmjnlrr.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3vganctek.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3rxzleaty.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3ftchosvf.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3tyouforg.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3kfpzzjfn.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3xcteqhcg.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3ummbruzz.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3iiaylsss.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3kwtmxkzx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wmuoqrke.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3mtgwyjtd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ipnosetq.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3nkewusvo.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3gekcekmr.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3acgeegem.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ifojqsni.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3fxzdwfms.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3mokyqjxh.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3hpygumub.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3pbeaweeh.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3budkscfq.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3mbdydvod.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3kxvfevpy.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3gfltmznk.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3oqdcupkb.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3glcoxkna.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3rzdykwhk.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3wifdzvvy.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3xsbfuqub.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3ketkegtm.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3krsfpbtl.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3cpyjlpav.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3opkmanks.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3pqmsjrou.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3ikhckjqp.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3bresastw.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3toyeoywm.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3dbwgmlst.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3msuhfvph.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3elgmonnv.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3gymvcnlx.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3hdyvoctp.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3sfwavivt.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3gsgmemks.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3sodtohde.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3pcxaczvy.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3ehdrniik.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ihbznamy.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3obxhblvc.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3mqwaabdn.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3looyxobl.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3zzwnkrxs.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3fbholgee.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3qrhiivah.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3canddpyh.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3lxwqvkwe.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3oujhtdrs.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3aghilnlx.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3jkgyaauw.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3gpoqxpip.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hpqidvaw.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3xjirmttt.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3mqwzfkiu.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3bsjodojx.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3plubbzmb.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3yjiynvdo.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3oqznsqpo.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3iuedmigw.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3ktmvreug.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3aagjhgvj.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3ypbvnlah.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3hrwyfdru.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3xxlzwhkq.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3kkjxseoq.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3vkttkffa.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3ozuiqhbb.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3vefclktx.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3iriwctbn.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3durmzdmd.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3mervwomn.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3rjoblqne.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3kpsmyhqz.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3orcobayh.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3chpoyorj.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3vbbupnls.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3nxmjpbws.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3uyxgydga.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3tdpxmqaa.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3zjzmvjzt.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3fnlbguxu.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3mpeuaxgs.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3djxonroj.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3hspmdaeo.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3vebcaljy.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3hsltkcye.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3zwofurlt.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3ewrydepf.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3imvfbnlu.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3sicxgikp.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3kbwmcjho.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3dwqswyai.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3xeqvsscn.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3fqgrxyey.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3jumaguuw.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3jttvxdbq.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3sfnesuoc.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3hfvxtkpo.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3jnxshmvs.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ptyzwsla.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3cqfqxisy.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3axlnbvmi.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3rxqnpxsv.html


<!-- 参考信息 -->