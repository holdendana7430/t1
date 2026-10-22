代发 wailian999

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2iuybptmv.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2lopqnvcq.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2bodrccih.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2tyuwimrk.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2kombmzqu.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2smopzsvz.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2uyaetljv.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2xdtzzveb.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2qbwttqjy.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2qqakyltk.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2pcjdwepp.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2yfpppuco.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2odievdsk.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2szezsvbf.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2doykxdob.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2vjkszsxn.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2sdwvwnsm.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2yibxtlke.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ttxndrsk.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2vqaoxrlt.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2zfnyzcpe.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2hgywbgfh.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2lsqpiczc.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2afihvndg.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2wxrvxqwu.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2bifwfzuz.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2vcepumtv.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2oyocaylv.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2xbzomlci.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2wtafzlim.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2loyadldn.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2ghfdghge.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2dangprln.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2aatbwpye.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2lltoabfq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dnwxoqnm.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2lwcdsfww.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zubrnasz.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2erypvwss.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2lguumxcb.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2tlzkvybd.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2eofurmjp.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2fjmdbgqm.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2pvxmcvxo.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2phxtlwoy.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2xtcpoajc.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2mobrjgtd.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2mlihexik.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2glukajbi.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2sfitudyg.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2jkzlvtey.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2gcllgmdm.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2reohjdxn.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2jvlllpzb.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2zwcbupkv.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2avfokpcr.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2fmaxflsm.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2ondontmz.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2pqvnfmbz.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2ubhfxgho.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2xkdqtixe.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2wjpdtxwf.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2fdbtukko.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2fhstclhx.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2gpxlmqcc.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2pczgvasm.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2kkhifthj.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2wognjuwu.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2wcvktihx.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2hedtmued.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2ejcdqdof.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2lnhwosed.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2bwxqpzuc.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2tqgfjyqf.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2dvehullw.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2bueycrvn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2nstabpfh.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2kknhvjmo.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2ykhcqgpy.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2tmqnmfzb.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2nodqhwan.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2vhetmxhb.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2szplrzyg.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2zybchbti.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2gfwqdzln.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2hvqgyrbr.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2heqluahz.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2ikwozjod.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2blrljmen.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2riyhlkcw.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2gaohnunc.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2blpppjfc.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2cqseucdm.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2fnqwcvzu.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2zehsgndd.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2iagokail.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2urnwunwg.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2ugdwedqu.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2puatujli.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2dplmumey.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2ozqdyvpi.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2hvzvlbcx.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2spmeamua.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2puymlhsh.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2hrthifpt.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2pqksofvy.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2wlstiush.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2ryyxkpkr.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2lzycusge.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2qpjomtlz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oerhgjfg.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2hectcfdu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ahdexmns.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2jnygqujs.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2pulagmao.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2ucrhbajd.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ngsjctwy.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2ossufpix.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2gmmxaecv.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2ofkpmkuq.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2wojixmuj.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2paexqzhf.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2drfhgpeb.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2pxpyyzux.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2awrmrpvk.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2dfmukxef.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2qaebeqwt.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2dzimcrql.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2skkkfyie.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2cwchadlz.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2pxakajxz.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2yuikwoya.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2nyfmquof.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2vsyjvmdp.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2cplsvhiv.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2agvwkisp.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2vrcjjwlz.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2ckslyrdc.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2wxozwprx.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2dunekokk.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2zywnzxdd.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2bsyqllvp.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2olnlyrwq.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2coohzftu.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2kutmljvp.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2ponkoitj.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2jlsksyqk.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2tbqtvrca.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2racenuuz.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2bxjkntfq.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lrdxcixb.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2uhcqpuid.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nfcsjdlp.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2uozgotdu.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2tkqfvdam.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2kyjlumvt.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2qvshatps.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2iqqxuwaq.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2obslsnhw.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2nqujhstl.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2nkpkvskr.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2oadhdcey.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2rbsrbpvv.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2rmqbwqwx.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2xltfghli.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2nvxzmloi.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2qcfuoavb.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2ojkfdfqg.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2alarptpo.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2aymdmjdv.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2gwhltpzn.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2xygofpir.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2kqushayo.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2crhxcwot.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2qavjphlp.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2ksxbfezh.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2nphspfnd.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2zwylcpbh.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2plczueyc.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2ozphdxkm.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2jjveaiuw.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2ezravgyn.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2ifmzphrs.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2vcamuqrs.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2rjcorqrh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2luhlkxyc.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2lkdrkotm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bywursbf.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2xogdbzmt.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2cojwxdph.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2zugtdjtp.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2wvnvqtam.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2pcgbdpxq.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2zhopotvl.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2hxdzvpvb.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2pweefdfl.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2lmazcbmj.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2lfjfptmr.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2huwkyxbu.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2fsrzavji.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2byqfjdim.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2ssqrmrvo.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2bdwbkaui.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nebclccp.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2nfsmajfn.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2lodgnjuw.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2dlxkxxgw.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2gosgvlxn.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2fkreopzc.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2sxxkexgp.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2mehheeoc.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2rvyrabgo.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2kwfexekp.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2hslxgrxm.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2kdettfyf.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2oauialne.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2damhznyt.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2ogndgskb.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2tfidncpy.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2rzvoadyf.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2vinggkjp.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2umnqxayo.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xuxoztwt.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2rglcrggf.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2mxwbapwo.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2ayohshnn.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2ogjierzc.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2wqclkpbk.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2jhpnhwtz.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2uzutdeut.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2jyfgpflw.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2tamdxlqj.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2nnmhikaz.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rfrdwhkc.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2vqjvudnn.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2cvevrqrb.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2varjvlnv.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2bprhikrz.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2hocybcqc.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2snpmsklo.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2lyivgnjt.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2tjcrzlie.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2gwszzzcr.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2lalokpnw.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2ejnjwmxb.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2cjgwiyjc.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2frwkprws.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2zdevafdk.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2izldduub.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2lcqbouwa.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2ubtzpaqh.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2qlomhxeu.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2aegnijsf.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2jvtzrbsq.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ewioabcm.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ljnlkiil.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2grpbfscs.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2qkcebxnm.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2nxxupmlo.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2aydlirbb.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2hqkuydij.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2jlwtemlo.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2pzhzfdgh.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2vqymzatc.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2fwctaayw.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2rrgctklz.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2amjknczo.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2fwtrkceu.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2eehqcjqh.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2gpqtvtsc.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2evesutss.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2cbkxiwuh.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2opezcngm.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2rsfdetfo.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2czzabkan.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2lahdwyzx.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2wkwljljr.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2wlcbcwik.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2qcycsjlm.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2cpcbwzbz.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2kgxnqjnl.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2sfxrbtcv.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2pzpnowmk.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2qtgtvmsm.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2sjeowtyx.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2xcjgnnym.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2nzvdumyg.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2jhaucfkv.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2eecvatcx.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2gbvkawur.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2ncorlpsf.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2qlewmktd.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2pfkinhal.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2pzqvdmtf.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2doykmikv.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2chazizqs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zfkujxax.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2fnlgntfb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ngulcxyc.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2yvcytxie.html


<!-- 参考信息 -->