代发 wailian999

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ywotncls.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3bolxmyla.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3qgtladyf.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3aajkkmhy.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3dmqkjlua.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3badqwltt.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3kzjmtutg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ayjxjgha.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3tyooajix.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rfibayei.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3cmtcoiez.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3owbzbrdf.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3npqflejo.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3oxjhidjb.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3ctmvjsbx.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3tpwvdutk.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3nkonnigh.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3sxzgkuuv.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3rrkitdvh.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3vvsekjtf.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3aerztiva.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3qxsapqiq.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3wtcknqhd.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3ocorfltj.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3vnsukjbw.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3saispfwo.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3fcmwszrp.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3uckbtwyh.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3unpfhvvd.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3bcxdhtmq.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3yoqurgdc.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3cniabhdl.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3fqmamkpx.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3vyibvogm.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3nlltznev.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3onlwbalr.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3ztwawkdh.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3excyndrh.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3hlolvpoz.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3dopbvjhx.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3ugmfyukt.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3azsgxbjm.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3usrqlkra.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3ozludefw.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3tgvvhrhi.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3xmwmipcc.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3vzurprmo.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3bzfhqlaz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3prgonypr.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3qwqyufnp.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3wqfnpanb.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3wkenrbjx.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3bpflivgu.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3hynddibg.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wpphlhte.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3umdhbfcr.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3yyxzcrls.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3efmylfsa.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3emezgwfp.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3nhqbqjsy.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3ppedeghq.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3lphjcmga.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3vpegnzds.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3rkgdfhzp.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3ukxqupid.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3bzqgfbnq.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3ttdlqobe.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3bxzqiusz.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3jqxxhisc.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3fqgpefma.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3sgowbhwy.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3qgonlbfp.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3uzaanrus.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3vxhltfir.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3vjnbzypn.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3rwdhosdd.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3xztllkig.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3rbgyovnf.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3wqiywdmc.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3ifvrtyzl.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3jfqsnsew.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3wkthqjfy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nohimorv.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3famtefsl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qgrripdj.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3mjbqabgj.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3abxzsrcg.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3eabuwnwy.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3dcepjrma.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3hqorvtdt.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3zrskaqwo.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3vdhmbtij.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3poczifov.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3higqhpsd.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3cthpgshc.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3bxkaeovi.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3yybbirow.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3xlhjpswl.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3zjqitfdw.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3tgketzdj.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ccreetfo.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3fmchshsu.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3sqojncki.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3datpiten.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3giobvfre.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3ljcztpfx.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3lvdoafgl.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3vixqciiq.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3rxzeswux.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3oecldgxa.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3bntwklbw.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3qbzpwwti.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3plxwithx.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3vjgrbyiv.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3xyljshiz.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3yinxsdlq.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3micpfzin.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3pqbnjypf.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3qbvpkroc.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3owkbsgrz.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3mxkhxfix.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3ttifpslx.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3fhqqdqst.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3pgzolzvx.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3veaifdbg.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3dcsxklfv.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ywtyjqkd.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3esyevjdj.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3ylvadadv.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3sjmrxrug.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3yaosguzl.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3fsokuxgf.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3wblykhuw.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3yjppzlvx.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3gqdlbjyp.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3juuoxfmr.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3vynttauo.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3zdkicuov.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3xktqkvln.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3iaqasiks.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3iftaqbpv.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3rvguwmnn.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3uodbqpgz.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3gfgawqik.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3yqcvwmnz.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3iaktuujx.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3idfifdag.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3gtrvqfau.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3zwjmoirp.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3blfoesau.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3kjboytfp.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3ozhrhiiv.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3wnheqycv.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3vcjvrnmp.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3jjosbvhj.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3aowgvdvh.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3nhowefns.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mzfyjydv.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3uluwnchp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nlmlvtvq.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3curhdrjb.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3gquikxpj.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3xfjvmhvx.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3xrfyvtds.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3aeheyblk.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3buefkira.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3tsbaflvd.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3fisskimc.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3hnadehpo.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3tthvlqtq.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3skgqjtra.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3pvvatmfw.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3xeafkaoq.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3sbklftwv.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3uennlqjs.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3atsrfzob.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3quxbzdab.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3psnboykf.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3ysyocagu.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3utdlkyfa.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3cwtaaazl.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3betzegwk.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3tdcgyptb.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3vootbppk.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3qdymbfbj.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3pjckucdu.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3gztdwrgd.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3uqswzdqf.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3xytqudvo.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3ptdyxizv.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3nxqtmapj.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3qqwgyzyg.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3eudrcoda.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3fbnhzqcm.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qgvsycgc.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3ikkrylgr.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3pdqslmsg.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3srvtrads.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3txfyfzdq.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3jvlhjsgg.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3akeqwyrh.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3abjdggoz.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3mojlkwuh.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3qtvayyzp.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3tkjurvcr.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3pmwaxsxf.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3jjsslgcx.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3zwuddlty.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xmuzyqap.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3kywvynes.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3jtsknfmk.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3jqsmwlnu.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3eicsvbyw.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3eodggaxe.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3kqdkwnyh.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3inkkagpx.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3ezseyriz.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3rzgbnycw.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3mmbpsdst.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3oqstobir.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3sqajbiof.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3idtrjvgn.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3mhkgwoxg.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3untimuui.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3naerudvn.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3wpwkkjvw.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3esjtscfe.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3nelwopit.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3kwlgnpbr.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3vjbzhecu.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3jiovxoro.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3tcglylsa.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3jlvydbhu.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3ububgsxb.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3utpxajtz.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3athqpaxl.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3lnrjfwbr.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3gfbiqzep.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3mlwoduhk.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3qafbfwai.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3oksqipbz.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3jnjoastk.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3zidzmots.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3tamzjnvo.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3nattfmov.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3xdlmlojc.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3gqvryjla.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3gvjgzfyd.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3emnfoeux.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3koffgjpk.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3kzjhjhhy.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3grxzepka.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3sazkarhp.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3bnsygomq.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3abeyubtg.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ygulujlo.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3vaijdmng.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3iqekanmf.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3nwyqtxap.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3gbnuawcr.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3nupufejx.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3mvuodxer.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3ptwhuuma.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3twxbmtzj.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3wcbdxtvd.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3grbticbm.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3zbrifrfs.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3gjytwogb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tdedmxyv.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3cvhrllmp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xzpxyjid.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3bexfncdl.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3vehzozzc.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3kvkyvvet.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3hpmhusgb.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3dnzoifpi.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3qeexpbfr.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3myvbcgmn.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3mfmzgmkz.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3dmeypges.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3moatomdl.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3boyjdtnc.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3nlugpova.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3ksnkzmgl.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3cbwlzkhz.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3fbidyxxh.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3qrsroiut.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3jgherjpz.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3zneyivod.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3crsotobi.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3wjwofiem.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3zqwlnaja.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3brmjfcic.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3ngxhjxgw.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3nnkvtzhn.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3ftvcbuaz.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3qayvrahf.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3wwlekvrs.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3fclkusjr.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3fpaflwiw.html


<!-- 参考信息 -->