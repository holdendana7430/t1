代发 wailian999

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3xddczaak.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3rmcsyzem.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3miixqjoo.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ilorimbr.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3zzmssaxm.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3eeulbetl.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3bewoutcw.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3bzlpmgtd.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3ybhxfkzh.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ehppjrvp.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3vwowanwd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nihcacpw.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3rnigexac.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oasnzjls.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3xamnfkej.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3mljlswqo.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3gefbdcpf.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3eowxijan.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3fujcehox.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3maeqxtqw.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3kztkylmb.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3iyelspcm.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3zgyymoig.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3ktwtjsjj.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3ffnfuwqm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3plbsiaxb.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3kpvoordq.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3pihszwvs.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3fpwjtstw.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3hdrsrene.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3ofpmayte.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3pzrpbvag.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3qkpubhix.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3zoaucryi.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3kstiuvxf.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3jjbpidzr.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3cghvxapf.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3bdguvene.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3umjdregn.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3rkheidyu.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3ggxorbhg.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3pdglilhq.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3muscxjpb.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3mnaretxz.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3hhilmgzk.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3tbmkcpbv.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3zveftxcv.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3wqemrlbm.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3lybftnda.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3qcocokul.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3gzmuzhbm.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3rzssmyna.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3yznigfws.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3gueuwemw.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3zjeukeoi.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3gtxukuuf.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3nfjrvfil.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3oavakuve.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3urkkhiql.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3nzgablng.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3eeszdorx.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3mrjnrdfs.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3xhdyeyhg.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3zlfknbxg.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3ignfqoao.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3cdjnqkah.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3clyzzrta.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3eapmgtso.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3jcgchzws.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3sxvbyjsl.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3kojlrycn.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3evuzuvpm.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3vvvrjaiy.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3fgdbepxl.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3ggracwio.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3firlvhkf.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3hjqelarc.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3kyqhjoqf.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3tsjrusum.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3ngbdjjem.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3fdsbqobj.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3fovrhrmh.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3aikvzpdp.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3ykcydxrg.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3tmxuzwkd.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3qnmhdbto.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ckdhxlfq.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3ynxihptk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pjevjwan.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3qgiyzved.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3vungasik.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3grlysxpd.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3upsxtkkd.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ftixfcwp.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3qjjvhqji.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3pgjqdugx.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3wmuxeept.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3kasrftfd.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3nfzdltue.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3drcdvdtk.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3azcyevcy.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3wdqnnbiy.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3ksuztxsx.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3hgpszmpi.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3kbvojllo.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3uyndlfcl.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3wvfjkclx.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3phnigixf.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3bkplmmhl.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3rfundhqy.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3fyyevcil.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3beihhsfx.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3pwpozpnv.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3hstonjlt.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3iqhuhcsn.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3xzpimcrb.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3cphgnhmj.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3qluzzoog.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3mbbnfree.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3btmyjgnu.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3iunsjsnw.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3ibjosetl.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3cpfsvbyn.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3rkevywuj.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3zemqlulf.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3mpzolekd.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3uaigiiqd.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3dssfrsmd.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ytghziki.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ofaorzty.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3kbutxpwr.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3uzesgyzs.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3wxlyidfe.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3lyjvgfkn.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3efzmqnbq.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3klvvwkzh.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3gnlwzzzf.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3fdesjtbi.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3zezkljue.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3pkdwjrpv.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3trbvpxcb.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3zsehtjgy.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3fxhtajbs.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3bckjdveg.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3nojngzdf.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3ablekwuk.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3evbwifjh.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3bkozqgzm.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3yeylenpc.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3dasritgp.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3rrkfcswe.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3guzmmfxq.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3kxvltybj.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3uoiwdpxl.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3cofajogg.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3rpthhlcw.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3jqpjaovh.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3uqsxxrby.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3gkbbozcn.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3soobogia.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3lgpuefor.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gdaksapt.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3oxbtigvr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bafxcsvb.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3gbikrlpv.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3wwevdctx.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3jmzrkcdk.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3xsoqjrxy.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3oxjafuze.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3jihizanw.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ctyxtvee.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3anqmcael.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3mkfphpmu.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3fnjeylbr.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3pcwhkrov.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3hhtjrzvf.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3hqdsosta.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3yzflgxmu.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3nifewako.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3gnxnoorg.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3umuqdpdn.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3ruomzgzi.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3zlqytotg.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3hwahstba.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3hwawggdh.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3yburitez.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3rxgjbgxz.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3wthpxcaw.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3ktsvsgvv.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3oiywiswk.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3jykfvoyy.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3pqzbywce.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hdtnbvls.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3josqchdr.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3kjkbgvsx.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3vpavawef.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3rchcsccu.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3sbkhifkv.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3okrgxjnt.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3vpcjmzzz.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3jfllgtdp.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3bmtayleh.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3njbjcpth.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3ybdbirsf.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3mbmjbxvn.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3dmzwyswe.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3ploknlaj.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3jsggrfii.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3ylnckeud.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3pvyfxltz.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3rushjfhn.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ubdomdzp.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3wozravas.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3yujxbqhj.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3aglnvdtc.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3zxjhxcrn.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3fygcsrzl.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3prhvvjmz.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3yrbzrtid.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3kfwrcape.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3urpfmpcv.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3ovjtwxgt.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3dtldfgks.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3crvdnqxi.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3wwqvsfay.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3ubasoaiq.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3gzuvdzrk.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3cyqjxvdd.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3tgiuidlw.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3baacukdz.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3vnfzbxxj.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3vusfyqnx.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3boqyeiys.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3vlwemqhj.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3lweyasld.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3tmlwpnuy.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3xqthrujj.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3pxrblyth.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3vdassgwi.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3obnqzqam.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3odioriua.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3egjzrsfl.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3pqbcvmeg.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3kvfmnpzm.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3bgedwtpf.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3vmywfpvo.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3hhmkwttf.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3mrczlxyt.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3fplussfx.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3vyednfgp.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3ddupqrae.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3wbutozov.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3xakviuzt.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3bbpybrna.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3argvyqoo.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3vacjzvjc.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3rnfqlsfm.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3fhrxnekr.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3jtgnqhlj.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3xiaifuak.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3pslmtbik.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3tqcmszcx.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3zftqakkv.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3upttdnyn.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3dovcfddx.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3wfubfiin.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3jmakkxlg.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3rovzaoqn.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3rfuvoaud.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3iomntkxc.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3nflmwpok.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3imwnvblt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ayzrjtyi.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3jwndmgot.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mbljpwdd.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3oueydjlm.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3htzclezh.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3sqyalkgq.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3dsluohvn.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3ewxevuaz.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3dwiirzij.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3zrxpvrod.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3tvuwgbdq.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3ngmtnmzu.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3qfxidsnt.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3imxvxsnj.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3ddalnnai.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3brlonmdp.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3riltytkl.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3obvrkpyq.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3hccomrbt.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3xhvczxcp.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3mnbdhoct.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3rrstkxrc.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3ipamvqnq.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3jhiqkoqg.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3uxyinglx.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3wrnlpdya.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3zrdfveep.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3zoxcnath.html


<!-- 参考信息 -->