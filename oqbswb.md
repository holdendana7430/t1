代发 wailian999

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3ipgmkadc.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3fwdaepgv.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3qgeqcdjk.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3nuwlzezu.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3agyhuvqw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3yqpdmhtt.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3xyrnvefh.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3napkgxnn.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3aaqxuidu.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3mucmcjeu.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3moadvoqm.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3ohwrxidh.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3snmqllrz.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3jsdupxob.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3nprwxrif.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3qcixrfvr.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3mopeuglg.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3rgzfwzmp.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3jisqvnkq.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3nmyzenze.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3yehlrbms.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3gtgspnlq.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3cpmkeopa.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3liijtbyk.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3dpktxyhj.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3ncozosts.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3xocbueym.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3tfqhfvrw.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3tjonadxu.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3ibspzjtr.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3tkrarldu.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3msyzrcwq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3yhledcul.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3koemibsz.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3tamdsjmd.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3tiodbbyx.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3eemrguog.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3laxzblip.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3pkzfeaqz.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3jdscosrj.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3ujpafwgj.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ohlehpmj.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3ujzwvmun.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3ogbzmsag.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3znubblkp.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3anxnjbls.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3rbxhiqeu.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3dgvxygsw.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3iaqgpjif.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3kxxcdupu.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3lgfjtdqi.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3yrlkxace.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3hamnmsan.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3cfduiijz.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3nfjlmqao.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3meqqdwhq.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3pmanlmuh.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3labxgesk.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3fwimqral.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3ytbubyqz.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3thgqavfw.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3rsddjiee.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3flppnqkg.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3ofnuiusd.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3anflptlt.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3zwoqaxhz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ezotlhdw.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3fcllpgzn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qcrezcxe.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3hbknamnz.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3xnemzrhh.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3obmktadr.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3gxhybkxo.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3anlpyiyw.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3mtjahpyy.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3zmuilyrf.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3wwlddzpl.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3gavuuckg.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3suuyobgc.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3kxdrybxc.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3yrmhriuo.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3iwtkzvaw.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3pvsjqyjq.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3obkeaenz.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3afwkzjev.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3ciafuzem.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ggkmihhi.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3jmpebrfd.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3xzrfkgtk.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3kwpypztu.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3pwgcxvnc.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ubwtbpkp.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3lvlcmpkf.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3kuxfnakg.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3nepxcecu.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3pcqtgmxo.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3fdhmahsr.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3hsonskha.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3jpaickup.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3mvvgmjjm.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3pidwutib.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3hpopqyre.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ahdjgcdo.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3xbgqnuff.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3zixvtuil.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3jlqbpbhg.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3abtegnmj.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3hlpjlyyd.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3kgzmsscs.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3podpatuy.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fbgtycmq.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lurgwuqy.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3nkkthfkk.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3rihrkixm.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3bwjnhwyr.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3imsppokw.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3gafebmje.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3pamksbar.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3jjmxhmyl.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3airhsknv.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3gmcdmvji.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3udyjjqla.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3uxhxvspq.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3ooeorvbr.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3cltbhsap.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3sbtovrfp.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3ovuqcuod.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3vqfkrpvc.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3bzrjvffh.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3jwnlkglf.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3buwfhcfg.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3uqbyhmab.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3njpfplzq.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3fkbnerrq.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3grrbqilb.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3rjaoypjz.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3cjihlxot.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3wxswuozn.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3dwnoorxc.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3tblsuvgd.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3lkctomdu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ybuoklpe.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3bmqmwcng.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3elkulaqr.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3yohlwugb.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3fqndhhbj.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3pdycolss.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3dtqaaspp.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3ipnaomxc.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3oxvwkikl.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3iisabtde.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3wmrozalr.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3yozbozoa.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3tousjyel.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3dhgxjcgs.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3yjiidlzc.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3fkmvlwog.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3rrkwdnmz.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3rrxdjqni.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3mvrouaua.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3epbcmdah.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3wgnylwrt.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3zvpldiuk.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3kxwwtnoc.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3lgosmfgn.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3wcxaptfy.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3hnqqmarp.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3szensmua.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3qgxuytum.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3xhhpmihg.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3cwbayexk.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3qudofutm.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3nzhwgcoy.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3grbywbdy.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3zraezgor.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3kytxdfvp.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3xnglcbee.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3tsqkukpl.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bpzrgath.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3zymfldho.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3jeiplqgq.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3pdludbms.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3kbgsmkbk.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3retuyhlp.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3ezdnxgou.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3onunvcom.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3tumvuaiu.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3qimnzlyl.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3brjzersa.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mxrnoogi.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3hvnllyxl.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3wbqzqlwf.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3mhgmpaiv.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3momxsbox.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3budjuzxy.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3fltrupfu.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3gejdzmwo.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3eoflqjzx.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3nnhmajlb.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3wxevqjti.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3uqgocqxv.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3eurpolju.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3ychruowd.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3harmwcnd.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3chlsbkbv.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3sgemweke.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3quqttvje.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3knvubhoz.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nejvniuu.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3ylxivtrs.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3zwedejfx.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3rxespphn.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3dfifilhl.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3vccurzqm.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3qfnsvwfy.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3jtxihqhq.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3ujllohwz.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3zpwskrrw.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ctuapuwj.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3wbkympvs.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3oztabsjf.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3fspntyjk.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3gtsswayc.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3snwpqguf.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3ochvdhwi.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3pejsfdcn.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3mxcbqnjr.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3xqbymyio.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3ppxmicoi.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3dmjyimtc.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3lfaclxwn.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3zncklqsx.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3hnfqozoj.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3hihtuzeq.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3jqnqcmkw.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3unzdjhaq.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3lrmgsxsy.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3tsmukbpt.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3kziuctyf.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3mettggxc.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3yzcyonhd.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3ygfagyyg.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ajvmbpys.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3kkedtflo.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3ytadeuol.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3hovsglsf.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3jpsagced.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3rwydjzgp.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3yqjrmfbj.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3etsadulv.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3vzjymwdx.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3jcvrpyda.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ekhidrlq.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3pknbvdup.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gzpdpflz.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3njtvxteo.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3xmfazygb.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3xdlybttl.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3nsphmynr.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3xrtcnans.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3yedxnjay.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3vyncopjz.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3omkovedd.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3nmpibugh.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3rvteljfu.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3shwlcdvw.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3whxzyhyj.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3hjzqocnt.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3bnjemqmz.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3zenudnlr.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3lqhivjkh.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3hottrvbc.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3yyppflnh.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3eojnvybg.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3gpqjnsnp.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3pmotrxza.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3pwmyjlyx.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3oscfxszj.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3ibcongnf.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3lpogzkpk.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3lvdxptyt.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3unxjoxqw.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3uezbhbjb.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3rjmqingy.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3visvcvzh.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qimbafxf.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3uifydpgk.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3tzjwfilh.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3janmziay.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3gryzluqs.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3sohgiwgs.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3zidzondv.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3teyvawzc.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3wgbhunph.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3hmiaibzf.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3qgojpozt.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3yfrwaavl.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3xsshrnmq.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3gduuypam.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3hhlomcgz.html


<!-- 参考信息 -->