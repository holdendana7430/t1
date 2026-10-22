代发 wailian999

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2maffnoki.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2untepjwx.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2ppnrtrot.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2mmfcpoxf.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2ybnwqgln.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2zknlfcml.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2fmcsetwj.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2cvriuodi.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2fuibtona.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2nrkowzyn.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2olovdczb.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2lcqzpqiz.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2zkepfdaz.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2vjtitikl.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2matgsjfj.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2yitkyxzx.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ruespsnx.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2fyyheiyv.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2pzciznpe.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2vhrwywsz.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2ftorxoqg.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2dkerbfde.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2vcijomzx.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2uuyvfkjh.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2mlizpbpa.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2bnumzzvw.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2izrbeotr.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2fjljijor.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2agjpevhq.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2slvlpkee.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2ccjofaxz.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2hzddmaku.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2rpojieok.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2boqmqwft.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2nyklgaez.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2llgnlbns.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2dlimvkod.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2mfynqbbx.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2zxzubxal.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xjsudfiv.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2qgexwdmp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2slaszomb.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2zwvtvhaq.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2hnjqcbyu.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2ireummtl.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2eltrrzaa.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2kczratrx.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2obhdadcs.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2cufuzpmb.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2utloezqp.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2jawbtmbt.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2qhiowblb.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2nmizyafs.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2lxbpyzlh.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2rpqhgmlc.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2apeictrq.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2vvrpjync.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2xqiqqquv.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2ykcdzirv.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2teioahun.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2pskoafmb.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2umjgcvim.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2fnhweapt.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2dngjeure.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2puphckku.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2rtkdputo.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2awsfmrda.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2jdvzexsu.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2yvnjpypu.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2mspzzjpa.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2xnrtsjai.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2ifxhuppm.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2ewpuckeh.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2wzmpuwjj.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2ogbotnvx.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2qtidaplz.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2ltzveybg.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2fdtjjqsn.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2vmgsvdoe.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2szskdlji.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2bxuckkvt.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2dsxhfrdu.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2zdnygrdh.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2nhilbnbs.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2egkkubfl.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2egqmmoow.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2cqsydmil.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ryebhyso.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2zskovbbp.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2fmdiyieu.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2pejaqdkb.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2diogxnch.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2cgutiofv.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2fpwgogoj.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2xtvxgnse.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2nfwiecif.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2pljhksiq.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2cgwlsdzp.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2nypbgngx.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2jjmrnlpf.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2myacycmq.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2axdjfjtn.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2hhlrbdat.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2vnxterpe.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2hahgqcni.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2cziambzc.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2crxvoqfb.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2uwltshzm.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2bhhbjqgk.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2sehcqucv.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2emononfq.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2fnhnlqwj.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2dvyfpxmd.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2tmplxwsb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bhcjccfh.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2eojetxxw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2orzhnmih.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2kubpdgbq.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2ajwpoxht.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2kzcuxtmb.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2lhvfxiuc.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2fmhduhfc.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2oainkufo.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2chrmspwp.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2pwcuvomb.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2hulyzops.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2grjndtrz.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2tffzzfrk.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2cbujslij.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2jedccpxa.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2rpjoiiue.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2nucxmjgl.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2rzsiybxt.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2vppdfgqr.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2zcfyaaie.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2pnsupafq.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2asaawvya.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2gmdedexk.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2kwspfnpj.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2zsfqnmxm.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2cgsjjgqu.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2jpdkychn.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2xredizeu.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2yknijwzt.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2ipaacfum.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2ohfhkvez.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2zxnwpjhn.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2xsheepjo.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2mvwjvjio.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2lbpxixlt.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ybmutcyd.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2wjnfigkp.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2zvjwevcp.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2jhaxzfrd.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2orlpnryr.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2cweqxbip.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2rnxmziag.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2qsgszmei.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2qduavsaf.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ajhvbtxr.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2cfwfxxtu.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2vfjcsxph.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2hiyfsyqw.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2fxnpshkh.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2kxvjenik.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2fhtxuyaq.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2upjigztg.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2kuseepkg.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2odimhbps.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2wqcrzghc.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2nmkaicpv.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2cnovcepa.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2tuxknnep.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2mrgbrkir.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2pyozqito.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2iowkwhoe.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2vxemqtew.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2inpxcdno.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2fvgghwek.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2mwlsaklu.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2suezjuzv.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2hbitqhis.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2yweuruei.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2nylgtnyy.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2pmsluvbz.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2ygrazjnh.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2ukstyzgd.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2ywnjxzgt.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2zmgibdbs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bcsxowfk.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2iypxbasz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cttfdsop.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2ykleezqr.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2lywnhens.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2hxadfdec.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2kpedwnqv.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2qwfajlww.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2jmvpvtkc.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2vuomsydv.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2vautbjiz.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2qnyyaihu.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2trojvopb.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2gjplrfuv.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2kowalxcd.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2qbwzhbdt.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2dxrikgsu.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2pwkmrbhl.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2grzvvekw.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2lyambgyg.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2aelcdyda.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2kfncajqp.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2tnmkjrxa.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2fxiitcdp.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2drmctzdt.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2ilxytxib.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2ugonixwn.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2nnlbiljc.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2nkfsobdz.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2lrcxnyte.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2fjygqkqn.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2ejoqyxqa.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2xefzghhl.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2dfezckvw.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2anzjgvnn.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2nudyxerq.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2bmitjcqx.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2chorfzjl.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2nwqshhrj.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2mvigzmlg.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2jpkbsgrc.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2cmnapryi.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2qqavmpjl.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2ebznyyxj.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2etnohdqa.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2puoeexfe.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2tsdefcqf.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2taclberi.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fnpybhyn.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2nkjdifrb.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2lasqqdep.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2wkiquaku.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2lcepuwxs.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2uulopbvl.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2jiwjybqv.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2vsnhmddf.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2cruzujub.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2urknnsnj.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2zlucgpkj.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2xbovhkbe.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2mvjdtmdv.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2cbzbazwo.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2wwuhsbrh.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2psirvyeb.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2lxoegszp.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2wdockros.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2ozmxwiwq.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2idnttfdd.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2prinnaid.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2pkkudhec.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2eocrqjsg.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2nadfekmi.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2dziwtqdu.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2ukitpbhg.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2rbzmwvlz.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2zorryyne.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2yrtwsqoh.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ukbzmawp.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2bsnnwpce.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2msafppdm.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2fhbuctzq.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2zvskqtdn.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2crpiqfbh.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2eblbcjzh.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2lyswonhi.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2sstltjeo.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2gitxwfpx.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2uwirslbv.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2kzqppmgq.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2hbimxscj.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2awvhiwqg.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2fwcxtoyf.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2ktgxgptm.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2rmcuxtcv.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2mlsuhelf.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2brwqjfka.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2rwrunnas.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2cvmjdcwf.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2snyknxxf.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2otozxbwq.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2hztlxmdl.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2cvwyaeel.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2smvoerah.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2chjcgnbv.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2neiktoyw.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2ccgvydfo.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2blmbfauz.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2xmlbsbgq.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2kegaifpu.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2quzynnxr.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2fywfyciv.html


<!-- 参考信息 -->