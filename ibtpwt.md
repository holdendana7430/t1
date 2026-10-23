代发 wailian999

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3ylucmsur.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3vxiyvbet.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3dnhocrqh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3znqhtmvg.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3putqncis.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3evllxufh.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3ttfpbyza.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3xvqugtde.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3vrgppfvm.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3kfezermr.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3zwwoiroo.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3estsrzdg.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3zykgyxsf.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3dqstrjzc.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3kggktuqb.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3xbxepigy.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3lnxiumst.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3cdfupwci.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3yrkzutuv.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3drpkfarh.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3iqhsfebp.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3bjvqnray.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3zlpbpnaj.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3crwtwnqy.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3fxjpmnjo.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3tiqmsikw.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3vnqikcax.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3gyruvazk.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3gqmeiriw.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3pzuydiks.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3szfxtvpx.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3yynswznv.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3dorbgvhi.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3kwkhwkki.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3syncwxdc.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3qcrourhs.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3hpyqzjky.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3fdakpdzt.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3ygibianb.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3zlltjxoe.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3rjgomaup.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3kmfpxsqh.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3oayaoluu.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3lndpoovy.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3txcurbvg.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3vjqklfex.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3qerjkryq.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3kjxfwsjv.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3zbjqpshz.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3gglajbam.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3leqqawym.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3oanymagj.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3lmmmqijq.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3wnnxrxfy.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3qkvtxqao.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3rpzsnqrv.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3mxuiibbi.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3tkghsrlr.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3ifsrqxig.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3wjubxodp.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3flxyoqvi.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3iwuedmsw.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3annxrhsw.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3xyxpnzwc.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3hdbgfyfe.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3cnppszkx.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3acjfjezv.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3kzwwfpll.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3cecfjbtf.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3poaqydsn.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3utmsxikx.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3vxjetahd.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ipzzwice.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3vxnrzxzt.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3gbkfvlmw.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3vhvizine.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3prkyadpd.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3izzofufu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pvtsibax.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3aegregxi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yxbssgxc.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3ubppyiix.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3ntbkoapf.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3pqzxyvzn.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3tlbfhuct.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3mpehmiyb.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3qfwnpbik.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3vrslubba.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3phewfmjz.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3vnjosshh.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3gjmnwyni.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3uozsaxcj.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3ymlziiwf.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3ctqhglht.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3vrwalefu.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3vbbzwthp.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3lwbbnjrb.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3wluwzabw.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3oemaykyv.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3vtnjyibx.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3hcsdeikg.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3dduzurnj.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3oxxovbxu.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3arikbpdo.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3psudmkve.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3waqxowuf.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3xszbgxhk.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3yciiwbpf.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3cehrcxcf.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3yaqzvdqe.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3ruxziyak.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3fpflowne.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3rxpixpfg.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3uihicost.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3yrhwnczu.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3kozrdhyk.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3zhugvaxu.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3zkkqqkzr.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3fmywiypi.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3nswqtggw.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bygjflrb.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3rfejtcym.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3htizrvim.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3iaoxedvd.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3vakwnrek.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3qhjoxvwh.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3zfzvxznr.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3fvueywrc.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3sznkhsjv.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3kvmlryzf.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3upbrqkki.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3zfhvfzca.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3tlpnudia.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3thukrlsh.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3bfuleouk.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3opgunjqh.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3rgevxzja.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3kkrowhlc.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3llezkhdl.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3slwhmwtt.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3fdqcmfhn.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3hwhazmdp.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3cmsdedil.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3snojcqax.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3najejnxb.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3izunyneh.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3evpkrort.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3zkvnvotq.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3pmknjxdi.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3eggmozkf.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3udnghisp.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3obkwvjxb.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3csrhclqs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zbfvuldh.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3fidzxqii.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3omwdehkf.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3yrqcsqem.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ewpxnyba.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3xfpjcrdb.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3wdcmmmks.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3rbvymsva.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3myyolebl.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3nfdofdpo.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3icskihxo.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3czirpior.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3rygdepcc.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3ynxwrjal.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3oxqseird.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3amizhysb.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3tfslujvd.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3vtybopyq.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3sairhypn.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3xlvcbaep.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3ldxeungt.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3igbsbfof.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3rlcaqdad.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3xxrtflit.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3jhufbdie.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3dnoqnjqh.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3vrfcwpcq.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3coducmcd.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3zczguech.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3oxhjyyma.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3mqbmhlsg.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zzdplhza.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3fqwpxcqa.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3mfzlsdge.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3izymzmcp.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3enolmwso.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3zooidbbr.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3vuwmdyno.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3muflzesc.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3iygwgixq.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3mlxvkmff.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3ekztwvjm.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3zldgduiv.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3ptcjuwhg.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3pkarubme.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3lbpwwlpl.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3mbzaekpw.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3dvzqkpvi.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3ifnejavq.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3ronreowj.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3vfjpfekv.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3vrgnwdcv.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jtrfgpiu.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3pcfejyuh.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3jsmdovrn.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3fcxxkjgl.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3metrfpmz.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3fkorrbof.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3pdbkmcjd.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3xcbswvar.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3cxumbzoc.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3ovxxksso.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3hrybwdut.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3mfkuvolo.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3dqmegggv.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3pfumoajp.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3flifeoru.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dlshnbck.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3kgqjcbyv.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3pgezryfs.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3yylxgdwz.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3shmcjand.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3uywlmsqk.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3jbgwqvgd.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3cbiaryzc.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3pagnehei.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3pltwbmjv.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3jnetqhbv.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3dbwowsiv.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3beozpfld.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3ckoywsjl.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3ctjqkwzf.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3tkzzfvlg.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3jpjqyhjt.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3zvnwkjep.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3xujjmhnm.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3sthsjqca.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3odorjjcj.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3cwbqthyk.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3yzilvcgx.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3hvklliwy.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3aqmhcygx.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3jmucqvqw.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3uebuarwh.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3gajeedda.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3xcxgiiqz.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3smfffzzb.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3tqnacwyd.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3tlthojhl.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3dnrlvzsl.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3boiuumbl.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3jcuczpsf.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3yzvjznlz.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3vvcbpluc.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3qjlxxudu.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3qhppnbel.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3ctpyjdfx.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3dymxbpnd.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3ehervbca.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3njgbjfdl.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3hmhhkdje.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tkdyrtme.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3dcsnkxfa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iastewta.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3pweunyki.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3accbkqtf.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3gxgvdloo.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3hamtcqpw.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3rfotyaqm.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3jgpnhabl.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3lfxnfzpz.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3awwtjrpb.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3zgfmjjsb.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3umemrjrx.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3tgdqgftd.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3rmzsetso.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3ltuoxrtf.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3dhfyumsa.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3hycddbal.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3cjwyijec.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3gnbtsvff.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3avwdmkpd.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3mlxohzfr.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3fypohfqz.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3cldshjsh.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3dccllwam.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3fkxswoaf.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3hjetdzcx.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3ipemfgrq.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3uuljjvik.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3oisrvxmk.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3qphnpwjs.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3frusexqj.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3tmmmyuuw.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3zmrdteyu.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3udzmoziv.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3civjsxyk.html


<!-- 参考信息 -->