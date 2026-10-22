代发 wailian999

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2knngrvim.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2jsdqqsjz.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2vtooxyws.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2fzoanjtk.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2toavyamx.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2nwywixnm.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2xeardgzj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zbznkyqt.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2oorladns.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sgddpugb.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2fziotcot.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2cgusdhhd.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2szpqdbru.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2trjwoofj.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2trzpzhfh.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2beitrcxl.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2ocrniepj.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2udowlrww.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2inolryis.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2pzoiaxca.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2dyjuxstx.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2kgqbwxsg.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2myafjmfg.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2wvcgjpto.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2dblvaogl.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2tcvbqnxa.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2ioyudata.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2dohzhyyc.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2nmycykct.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2dfkuugtb.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2nffdoluu.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2guobwawv.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2bznysiqd.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2utbvjebr.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2jcqsdqjl.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2gjyxzyvp.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2sborbqds.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2kftejxtr.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2vpiddadw.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2vrcvzaqm.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2bsoknjzg.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2epyrichj.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2evrqcqip.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2yrmiwasp.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2gnluquin.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2hphiqddm.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2acijvymu.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2szfzosnj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2olfuucwe.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2kxielwtk.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2jdydfmzi.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2eqvujxqr.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2hrwuwtzr.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2xgcopjid.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2drxzpbgw.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2bhthrfgl.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2goxigcqd.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2wcyuukjl.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2yslfvtdi.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2ixzafoyj.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2gykqzaqy.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2ndazxgif.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2kdjcedzl.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2vinywals.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ggvyfuzj.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2wwwpyias.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2drxdgcig.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2xvtwjfgh.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2gmqxbgyj.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2mmwifcqv.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2hmsoarzv.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2derxmnlu.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2oboncrnl.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2blrzzkro.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2rbbpqtgt.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2cvqcnhrr.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2cewebhhy.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2fcowvvns.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2itddywmf.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2msxzeulp.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2ruwonkwv.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2ynfxyncg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bjomlbsi.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2ohkzedpo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ibimidaj.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2mfsrswbp.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2hvwshswf.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2asuoypgn.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2cpjokcij.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2mflxbmvg.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2tmaexbvr.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2vhcbgryx.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2hdqhiqlu.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2qmxnqrau.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2naeycljm.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2fcuhdcts.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2mvowxijh.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2vxodpwkl.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2gjhyuukx.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2eijzcjpd.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2bauytxcv.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2wmdjehaa.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2fhstcyhv.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2veofnnwm.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2cwejvpfo.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2fxeemkcr.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2wbcscjiu.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2rohhrglt.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2fvwfmhsl.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2yjrmnxpi.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2evkdluvx.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2gexqpuio.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2vfsbcoug.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2oyjufmlz.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2bvxgnrkz.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2bjmptrxx.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2ikagpyxh.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2jihspmjg.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ahqbodkn.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2qgamaopn.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2ruhzcebx.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2toegpiai.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rwwknyty.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2jxotooww.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2pkzldeqf.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2orstvyez.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2oldchipk.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2tzshvmfu.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2bqidjzct.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2nusojgfv.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2rsivfpoo.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2jartsqol.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2anfbkzeh.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2rodafmaf.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2kjlyztnq.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2lacsxlus.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2hditxcgg.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2najxmarg.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ojsjgfvo.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2ttaisvmn.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2pvskwzrj.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2lczxjidl.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2jarlkmhc.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2zyxadsvo.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2zsgdlruc.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2xabizani.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2dfloqdxn.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2uovygdkp.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2vnaempfk.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2xutjfvjy.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2jzstcdvd.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2qbcyvpid.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2hakayffd.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2lieeatkk.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2fxfdwphn.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2hcqzoeyo.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2zqbusrbq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gidttlgi.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2rgnyqafd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vkhzktat.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2rfggckqr.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2kuiwanob.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2tilnuwcj.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2dhsrbknn.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2myxmcqts.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2baefokrs.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ncalprok.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2phsejeco.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2mnysnfuq.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2mrtnltsd.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2tzyvywwu.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2ysbmonjb.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2nqntbtfo.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2zoogvmvz.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2fkyadkur.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jocrytao.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2tmglgxpv.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ppwtouvw.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2cdwsagdp.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2vgnlmszd.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2wwdofujj.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2tmzpphtc.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2rsmikbsi.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ixiwaibu.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2wyltixwx.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2yvgeayid.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2fqskhzti.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2eohvnpwl.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2knovqfiw.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2cpyswhap.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2stczcfmk.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2yaejokaw.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2odwqqlmj.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2gflfwpxe.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2ykaslcbr.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2eionbmip.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2glebjdiq.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ahuxyvnx.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2feszgbhp.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2qzlefknb.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2xokpjdte.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2vknxgeqf.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2zblckdgj.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2jozktofx.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2zicpnzho.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2sarawehv.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2ekpoaxws.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2mbqukmso.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ylxdsbzz.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2vphwtvnr.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2wkeifsht.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2cpyfqirp.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2wzmszxwz.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2qeerpzeb.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2tbmvftod.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2zeescpjl.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2fvsoohom.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2uxgrrluy.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2iwegxvix.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2zucmlkgx.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2xvhnlzxp.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2disvfdmn.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2kzwxnpan.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2eapniitv.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2uddwdyti.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2xvfjldmz.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2fmtmaigj.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2feqtzmlp.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2nsmhynwp.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2wtwecnnc.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2rthhiofl.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2xfpqeevj.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2mfdmcyfw.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2hqsusswg.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2bcaejluy.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2qyrcdweq.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2dputseuq.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2rxxbinqe.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2pzbceuhf.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2rfbfesqv.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2vbvowavi.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2ouaoccey.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2hybtxtqs.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2muygdyke.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2exzfrnle.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2zorwrirs.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2dkvykvak.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2zxkllnqp.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2jdpvjzsl.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2hexecpor.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2yxgbxsgb.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2auwzvyff.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2gjafqzsf.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2ipdptxaq.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2giblswse.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2gbbnozao.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2glwchfoe.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2xxxivfan.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2pkpmfhxs.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2yzsisrnk.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2gsxbmitj.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2rapnbbko.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2pvnjlhea.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2qyqsnzpm.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2shwdtrhr.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2gtauhebd.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2ejkkrrkk.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2trpkhocd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ddyiczdr.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2glhlyzrh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wheokysq.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2nyhemzdy.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2gvpxfyff.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2cvbjjmtt.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2wqzolpgh.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2nvmfsvsi.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2piwzupij.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2yenytmom.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2dkkzwjvo.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2gxwirtnt.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2jygnbrrr.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2qzroexnr.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2wsqtouxg.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2wriifpru.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2txizcbqe.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2ninrmvxz.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2filfdmfs.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2hzcmynbo.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2vhvduzbo.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2viocsuse.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2lvcmivvn.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2hjresihs.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2nszpxyrs.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2rlylhfwp.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2lgwuvopm.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2rfhfquhi.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2czxajxls.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2yrawtarq.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2amwmhnjx.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2sckvyoys.html


<!-- 参考信息 -->