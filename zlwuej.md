代发 wailian999

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2svhpgjdw.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2htehhbuc.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2hfzzfaaw.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2llmwjszk.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2mnuqkcpl.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2zthusbjl.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2ypqxzbpg.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2nxmtlvmv.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2doyocxdr.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2qncpdkgb.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2yripljga.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2jhiwmulv.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2yxurmaii.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2fauqpnxd.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2jrgaiuaa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eymurjue.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2uerzqmry.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aflqcyxo.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2zgtpajcl.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2qwunumfw.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2cdutmxrc.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2clgwlrxi.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2uyeprlma.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2veyqhlct.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2bdazupsx.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2spgzrebe.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2grpebjvx.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2brjcueka.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2hfloaerz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2uwsqenus.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2mrbhdvkh.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2oaiiatbg.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2aebsqtvn.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2catxnhke.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2mpucxrxf.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2hombvvye.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2ynrtqcjn.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2bjrcttld.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2dvvirmdv.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2jdhuyqxn.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2ptcfiajp.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2bbzecrau.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2ixxxjfnl.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2sdaqqbjx.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2dpkboruz.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2xgyxxpex.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2pubglulb.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2rgltyonc.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2jxgrobgd.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2puobodwe.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2trnqpiiu.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2pvuwxxyw.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2fjfqofhd.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2bezbwmhv.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2tjnxwgaf.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2giogaigk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2ymfzmhrl.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2zklssiaz.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2vurqxspb.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2oqponkgj.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2foklrdbd.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2ixpyxsje.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2scnbplqy.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2poenfqqg.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2pzrcalwt.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2lzkkbbtm.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2sxgxurmw.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2oqptdccn.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2kirylhis.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2vlymgzzf.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2pyjbhkus.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2rhzybqdo.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2rxnbkuyz.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2pztburrk.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2ytvnehnb.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2xpmqsvrq.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2zvbfzosu.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2vzgmfsug.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2gukqvgms.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2huxuydby.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2usozeyco.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2vbvdnqdg.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2hjrrmdnr.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2rudcdhyp.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2yesukyjw.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2dzcavqvh.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2axrdsusi.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2fhwngdwa.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2lzhstpsz.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2axrjzapz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qqemzopz.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2mklelcgw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hbahyehc.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2jwbgybre.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2bvqxdtvn.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2ypnqpqbf.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ylivdzlj.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2ndxmwnzu.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2rmzrmucw.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2pgihfqsw.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2wuqrzhzn.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2hopxkxsq.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2opdbgmsh.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2kivpbbhg.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2ztrklfcm.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2wvqwuotz.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2zvwwwszn.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2moutggjq.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2rtjbwnua.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2tjzpadsv.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ejuxtynv.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2fgfdndwj.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2nvomynrd.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2cdqniqbw.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2sxwuoldg.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2sdnybwwi.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2szueiyty.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2xyxqvfep.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2gywzutis.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2pgkcooxl.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2nwddcmwd.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2fevifmpd.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2vklnhabq.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2hfjqurzb.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2dcoeinco.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2adsgyswm.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2dokuoucw.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2lawaafhi.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2geirhutf.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2ilbqkgdh.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2nyswzbmy.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2nwwqycch.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2daaeabcf.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pzhopmyx.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2mtgzfwlc.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ifdfxqqq.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2rswtgpva.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2pvaymfxv.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2jthrynop.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2vnbxjeue.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2lfnxqcpy.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2pzsxmebi.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2mopcosrr.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2vqqpxbog.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2itkyeflk.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2abadorca.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2yfosfssq.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2hmllwaon.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2ilconcot.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2mlyqifma.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2juatgdar.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2bltflxbg.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2lxsvpcid.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2uplytzlq.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2nrvdtsgt.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2mkieheus.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2hchrxbwl.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2pryssjbf.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2ncjvyptm.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2zbuawmqz.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2hcwfeyps.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2sagucunu.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2elseivdr.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2ushecdcr.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2heholvrx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ihqsyasu.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2jukinvon.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2itjfwfpm.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2tcedhcay.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2orxwzqlt.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2qejchvpn.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2zkekdacc.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2ldcyhsbt.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2vyovhlqd.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2osxwrlie.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2bjqkqdpr.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2gzlthvrr.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2bzlepjhd.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2yzuimnsr.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2vfvgakwo.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2mqeocucn.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2loygkglg.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2cahkvjjw.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2vbpynubi.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ztpgsfrm.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2erfjqgoi.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2pqwgtgnb.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2gqgjywzb.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2qmsriiuz.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2uuzfiqbi.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2ovuqbjjz.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2aqmnocqu.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2ejpyocve.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2jjcrkszk.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2zzdbjqlw.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2gmpnmmdx.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ltjprrop.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2ugckxaur.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2ofgjgkbo.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2kvuwueey.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2hswoitfe.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2rvxcezdo.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hshagcor.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2cikiffoy.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2vzjtfnvt.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2mmosoanm.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2cewbieef.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2lzgomncp.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2shngdvvw.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2asqyawbe.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2whmvvlzu.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2mhsfzaxu.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2xnrccwhp.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2syowtvmr.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2xjafsqvb.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2nnzxaexw.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2jshvwmcg.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2alvlaywz.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2zagfxuoz.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2zfptchlo.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2esvlydwv.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2vfyjntpy.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2xneqfquv.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2teljprib.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2lcltfhrd.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2yxhzggww.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2oaookfxt.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2wnhdfsmk.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2bgjapwmi.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2vsejqgah.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2mdphsjto.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2utwkckmd.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2osioganb.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2sglzukkg.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2xfsvkoip.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2mjwxwyyv.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2auvexfmt.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2qxwcncwf.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2jmmlnusz.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2qfkebefa.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2dposgmbd.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2xuvbcigw.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2unyzdvad.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2xrpwtibu.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2kbapopsj.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2acvbomcv.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2mixaxuzo.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2bynysdvq.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2joatlqzx.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2sdbmkaue.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2tkaxlcek.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2lphndoqn.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2fnjqhjbo.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2kpledfif.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2cueduytf.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2jlsjkejv.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2udedraqw.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2lqtggrzu.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2vfpwnyag.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2pnhmiayh.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2xdvpbmmw.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2mvxrarvo.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2nrptyies.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2fngrbhlo.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2qnlsvuoe.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2ruhsmlzn.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2nggeetua.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2ekzlfqnr.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2lxtigymr.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2xufxnymq.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2mgdaepcf.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2dwkphpmt.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2uhwhbcmu.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2igijvvin.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2zcoegjnj.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2fhkizhef.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yexuoijm.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2miznoesp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fkgtenkz.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2etopyirz.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2lwjnzwti.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2bvmrrtqe.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2umiemtez.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2uuntmnhm.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2gjfujrvq.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2xpjomuou.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2czbwvsim.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2iusrbedb.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2tfhqstaq.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2fdtgbkhm.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2eeedxpsf.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2irirpzie.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2cmomvbhd.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2tupponht.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2ixpwuzng.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2rpkuixsv.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2pkhafsav.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2vtxrdwiu.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2svydujwd.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2gkqihlad.html


<!-- 参考信息 -->