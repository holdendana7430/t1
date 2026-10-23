代发 wailian999

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3zwptqjsb.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3cfdkqara.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3phdbqury.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3unumqteo.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3nlnkqmgh.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3znonpgxf.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3iwnhfchb.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3johkmuaa.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3qrboqulp.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3pnxpsjcs.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qkgvgpkv.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3kmbsqzqp.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3yalsfsei.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3btkquxsv.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3ntkxlebd.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3zonzqtqi.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3fzvwnrdf.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3zylpzxeg.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3wpftopix.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3yabjaevr.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3sijonhne.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3prjgkjvm.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3gcjdzkzh.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3bfvhkqug.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3flihqyyu.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3bymahsaf.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3oifrqtyv.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3znkfumrk.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ntfietne.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3nvtivknq.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3zoilhzem.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3xnrjhspo.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3bqntanlc.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ekndjxka.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3voruulgd.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3uaipkzbk.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3gtssifsb.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3hkbzlgbx.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3xycfesoa.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3aepbpucn.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3ubjkhsin.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ixpurcjs.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3vgxtfdlq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zenlsswy.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3mfqbtomr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ztacpplo.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3fxunwkme.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3ouzbsowb.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3eudjyfzk.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3mzhvxyoy.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3sgirqylq.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3pedemdhd.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3ulfllcqb.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3labhdupr.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3bzgrhili.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3xjononiv.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3bacwkkum.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3onpbgnou.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3juvdqkgr.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3rldrysgs.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3wpcoizof.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3tflohaxn.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3wrnjydwn.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3iljnehsf.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3tlitcaqr.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3yyzglmvp.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3puxdoejq.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3braxxjuq.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3rcjvgwau.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3sifuswjq.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3nsyirvch.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3tzhnoivw.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3fundhqgs.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3ntltacgt.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3koeolzkb.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3yevkictz.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3efzgnnjn.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3ndvtjsqr.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3rmixnbxm.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3cwekorcd.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3mggnhwws.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3epdkfrei.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3wfpfsdrx.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3thiusfzy.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3tfqxncsq.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3vhmdbcwf.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3jbtfkbuo.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3eredylxy.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3gmrncffr.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3cfboclza.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3woijwnrx.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3egjaxnbf.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3qmipyaeq.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3vrefrvmb.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3rvhjymag.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3mrwurhix.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3xiiuthgb.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3msalqrvu.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3yxaqtuhu.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3rildrkzz.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3yvjjihkj.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3aenurwwc.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3dpvsgunr.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3vuoreyoa.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3gvjoflvz.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3aarksqka.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3equikzjz.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3uoenxtsl.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3hyrauglt.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3cpcurfns.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3yftjvlxk.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3iljmffhf.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3kcgghpuq.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3ozdwalgs.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3hrfryypy.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3uajhrqxk.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3icbbhbnn.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3mujezpgx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uentclxt.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3apjcxkhc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xfyetred.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3liazxxld.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3fklnvvni.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3ehnvnqnm.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3nagzdpuo.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3phmikwke.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3enavxiuj.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3kvmoiwnp.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3dovihnhb.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3fmzlztje.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3imaqhmnb.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ksaqpqto.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3vvjkxrnq.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3bpdhjbtb.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3nzygbeme.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3sbiygtfw.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3wvdqihdc.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3szrmyecz.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3hpfmzehd.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3nfkzidqi.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3xgqsbghn.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3cjmoahys.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3aglubwts.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3gvtpkaxp.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3jxjrkpzr.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3zruwuhhu.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3mlyfqzhe.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3vgyqchst.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3nmommaud.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3ssqjwshr.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3eeyxkrud.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3twcocddv.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3yldfmicx.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3wvmizboz.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3kbpwpwap.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3kturniaw.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3npbpgglt.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3tfeczfgg.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mhfcwesm.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3fajqbolo.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3iiqevmtg.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3htaiirib.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3izewpgkl.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jqxujlxo.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3mdjomixw.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3lsvtnuaa.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3avxgjvcd.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3dhlwacnh.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3hhyvtsqd.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3skgtinzo.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3yybhwdea.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3wyjzthjk.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3fpgikuqv.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3oeatdlyb.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3iaxtumnb.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3qkictpyr.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3enuzjdtr.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3rytnnugl.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3ljgfplna.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3llvzosle.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3tlfubvye.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3ehhpgzhu.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3xtbufcnf.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3mtpnbbig.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3vbizyego.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3ggwaruqb.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3eiboufxl.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3dbznykdi.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3ojenwmxo.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3ktklzbja.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3qpryngga.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3wkjnbaqc.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3mdvoqach.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ybluvyst.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3pkayjcpl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3icpirjfd.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3cxuyhbyd.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3htxcrrys.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3imajjfro.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3dgapjuat.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3rjefvjpk.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ibjqamwj.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3xyrvftrn.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3pdkfebbh.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3cmznplpf.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3tpylwopu.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3fwihpciw.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3swacusqr.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3jijtblhj.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3mkmryqyg.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3irhafcld.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3jnpsllis.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3pcotladr.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3bsxsbzqo.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3ifbexlyu.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3kzzqcrxe.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3sxtxnjss.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3xlhtuajb.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3rxmmpobn.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3hfmqkqll.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3idwelzap.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3rdwbmrtn.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3fowtcgst.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3pazttdeq.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zflszsox.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3oxvsmcxd.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3hbyueebn.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3wuaebmuj.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3qgfpktgv.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3txjhyags.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cdqnspnc.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3uehwjysh.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3xhqzyzfh.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3vqfdpujl.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3tozrrzmh.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3eieafyer.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3vmjtriyj.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3byawwiiv.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3ngevagca.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3ighptgul.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3tgzndhvt.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3waaqotnt.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3wtdimnzr.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3rukdkjcm.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3efwkrvwu.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hsllfrpk.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3rtzgjjoo.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3ircjxxuj.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3cscblgcw.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3knazpxsb.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3ooifhurt.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3qmosomrk.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3rcipjuxj.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3erkqwgwc.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3vzswgsmt.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3pgqcbqhk.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3mocwbcbd.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3incshmfh.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3poflkpiq.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3tvlikkja.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bjopenmw.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3dfhowtfg.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3vcdrpuva.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3tmmvuzgd.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3elfhigbx.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3zwygmhvm.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3efdcbeqw.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3rzidxgzg.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3jaeasgej.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3vbhhcyvt.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3kmmovlvp.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3drxuidju.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3dmzzopqi.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3iszyxrro.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3tobexkae.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3evzlbmbx.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3tvatjndn.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3xsfvtrto.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3vmhrekmv.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3swubbuwt.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3vpjyiezk.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3wmeyhape.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3jxzsjvtd.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3ubacirfz.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3uhigqzrb.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3zbqaxroz.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3zlmiplpk.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3cexkbodv.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3teuvhrzg.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3hfpfqjaf.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3eavaxvhj.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3lltkukgs.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3zvxusghy.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3wsnwqwwf.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3kcsmnlrz.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3pkrvguca.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3xesstngx.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3tlzdsapl.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3nkjgdjxf.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3mytwvjqu.html


<!-- 参考信息 -->