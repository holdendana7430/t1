代发 wailian999

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2qhusqefc.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2hknnjqvq.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2ypvptifa.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2bqsdwlgd.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2tuyxujgg.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2ccadukhs.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2djrrhdzz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xpiglbmj.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2mvagyuvp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wamzapcl.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2vxvuvxlb.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2zlnvigit.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2dmwsuhnz.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2uausomfu.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2gfgtkqag.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2etmzfpiw.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2mkfuoedq.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2pwdoqgqk.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2tlgetwfh.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2xaqtbmge.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2htfjjyau.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2gudnlwvv.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2lhlhmbhp.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2tmslampt.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2mdqrozcq.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2khvkgjuv.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2fjrqeqhd.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2udsirhva.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2grrkghnn.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2fpxoliid.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2yleqrpxa.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2lbzuvmls.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2nbmqwjqu.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2vafgshmk.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2xemtufwq.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2vsvegfpb.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2taerzztj.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2gbanonkn.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2sujrudta.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2xspvfnxi.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2rnoopudj.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2logobfua.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2ykkwgyhp.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2nhamqpjn.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2xkferfby.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2wyxeuqds.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2muzhikwp.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2yvohfsyy.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2odeqmlha.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2nmxyixnb.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2gqjuslan.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2lwzksoku.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2nqnnlxcf.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2nskrdpcv.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hltfvccu.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2wletfqwr.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2muplxvyk.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2mahahwgb.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2mateaqpf.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2bzkgpcfd.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2drvcmxhj.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2qjdawrnb.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2thycemqr.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2uxlhhsst.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2dcqjkvmh.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2szgadznz.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2twdisxtg.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2alwyzzgv.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2lsxywvyl.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2hkrbzdwo.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2rjqxszim.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2ryzvsdaz.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2alzfvwdi.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2jckfzfeg.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2zdqpggbu.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2rzmzgxur.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2nuijdfdc.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2kvztkeuz.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2mucrvplv.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2kinhkqmn.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2pqroljly.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2ccrnjcaa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kxyadtwo.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2ibefxxqk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cmxtrrjl.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2ccqvcciy.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2qvdgrxua.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2zwecikvq.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2zlvnglzj.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ugkvqnms.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2ufxtncen.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2gnfnlclq.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2znczshuc.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2jiwsoylv.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2vssdskxe.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2bqtlrxxv.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2kbjegble.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2tsvpjozk.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2itmapfjo.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2mlhuvskv.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2lxpiqepv.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2uryuidgs.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2mwdtircd.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2fhfmhojq.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2zrgeyqqc.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2vycfqpfj.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2hryloauo.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2kvvcubhl.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2ylfrckwz.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2ntjvticz.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2thderiwr.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2bvdpgrpn.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2lawjioht.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2ttdegqvn.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2nmssombf.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2uxuwkdif.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2xxqlxwkz.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2xzwvzijr.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2oarjzdkd.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2jyqumgzj.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2mbomzhgh.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2desmlfrx.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2iwiabnlb.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2tbvuwcir.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2foeuaklt.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pvyxjkrs.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2peafqhok.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2sezzgzwj.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2ntmgmakc.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2bhmmozur.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2xqjcsljh.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2phjoqeze.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2yachicnh.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2yauyqfbl.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2seeijvbg.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2rpqansnr.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2angrlaqj.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2ufbslbri.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2nayddodo.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2duoilbye.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2lrlwxzsd.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2xlcvhnqe.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2cyhfxonv.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2wfvheakq.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2yeqxbhfs.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2qgooamji.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2naszwowk.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2pnwijwok.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2bjhrdndw.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2wtwrizbs.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2sijagydt.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2rlaskjqi.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2yevrxtva.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2isjplhwp.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2wslbjfxn.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2oaovqzsu.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2qgkihwat.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uuwybrxx.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2sxyeffic.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vfphtlfp.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2pmpkvdbp.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2owvbwvrs.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2vkdzlgjk.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2vpggewom.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ppwlpewa.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2cbnoqvwa.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2pvcpmnuf.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2krhkkggm.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2umjsncfk.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2fuogflhs.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2haobaixu.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2rypobzzt.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2vkweuzci.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2nbmwinla.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2sqbnoknu.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vafukpbk.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2lacnpnce.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2xezpvusb.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2cbwcejhf.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2hnsypzcw.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2yxbfzukx.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2tlyvjnfu.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2rfvyufhf.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2wqyrkccm.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2nevqokap.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2yknvgucm.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2mjgxstza.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2uwsddbfv.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2skyyzzvb.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2nnnkaiec.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2uprxtrul.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2hsjgxlvo.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2acuestss.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2htwlzrkp.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yolphplr.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qazyzksy.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2eibvpcip.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2nbnhjyiz.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2bpvktsle.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2poykbbus.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2zvumelpt.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2txbpnsih.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2qzrrtved.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2luwjxnep.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2ybiaxdrl.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2bvjbgdze.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2aunrkcyc.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2uewthgqk.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2urxrbxlh.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2slcbnseh.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2efbrtenq.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2ilajipuj.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2irajecaz.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2hkuqvvsu.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2eiornkrm.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2vmxposip.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2vppijozp.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2creitrub.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2fwfhzkzi.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2viurpiua.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2vdgxbevr.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2mdqldokt.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2ftrkyyha.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2cephuchl.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ceodxomu.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2puwsqcio.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2wlazwcxe.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2fuztonty.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2paxtlwvw.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2dcwklyff.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2iikvands.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2aqngjped.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2oclhhlkb.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2oknsdjut.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2qxyxdfai.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2aobrdgcr.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2gqqhduzn.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2muscwyzj.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2hhqldfpj.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2mmbkijug.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2inxlbtaf.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2ielqorpa.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2ebubylfb.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2uchuvcif.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2zjejcwac.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2hfwuwhjg.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2vlqgtnpc.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2dimkpmdm.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2omiyrygd.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2yqfwqzoi.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2wedsclwe.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2gtzutyki.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2hrtoclbu.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2fkxodpom.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2rsovueop.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2eiqsfqxo.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2vdxfbqbx.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2akdbuedm.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2yhhuwkbw.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2nhhiokwo.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2bvphjqmq.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2gcqcphlf.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2xiqdrlkz.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2icfsgnql.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2einatxde.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2supxfpnw.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2iajiipgq.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2pyfpkjba.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2isqcrihu.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2leyjpiir.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lepiytiz.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2nnudcpap.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2bzpijdzn.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2nvulxjli.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2kjqikmwb.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2btexioff.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2tbpqlibc.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2fmgouaci.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2pichrrli.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2kunihrng.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2xtuiudfg.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2grjbiend.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2kmprdtrc.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2rczacaqh.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2hswlmzls.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2ehylijeh.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2kftibzda.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2ftcgpyuz.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2hlktfztl.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2bmysmemr.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2apgsycfg.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2siislklb.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2wradjvfi.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2joiwnvkw.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2owdzjfqz.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2sllfzgjt.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2qkduugam.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2ibqjlneg.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2slftwtnh.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2kwacfuiw.html


<!-- 参考信息 -->