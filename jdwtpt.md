代发 wailian999

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2linjblqq.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2qhhnrmyv.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2lctherij.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2lomgjsfr.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2kfbsriib.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2clohijwd.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2nwwaityf.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2uyzaqlkm.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2ncgvroai.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2odnmbakn.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2yokwtjgw.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2trkkrlwj.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2urhfgtcg.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2pteutmlp.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2hgatwqsx.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2dtjjseus.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2wfidlhjb.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2dkppxmdl.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2mynfiovh.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2bstridua.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2auwocqxp.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2rpzimlmb.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2pvzsjlqi.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2gvecyowm.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2pwuvanos.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2yntrtnnb.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2opbidrrv.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2edyxcsym.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2xgctfaas.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2mhxhflzf.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2zocigxno.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2wyxqlegv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2ldizwgpb.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2yxyjsgem.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2hxaqinrs.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2vhoakqow.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2xcwwbhrs.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2whvtaqcc.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2habsyuti.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2vcslkrdb.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2wbxfzxom.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2mtfhezxt.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2clzwuxcc.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2imurnupm.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2hhzkhhsw.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2saeyscyc.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2rrwpiltf.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2owtsgyce.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2inqieruw.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2btdwxzzu.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2kozoyjmb.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2vguuuzbd.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2dnxzhnug.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2ntrshuro.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2bfxggkhk.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2ozdhwrua.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2okzwzusp.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2hwnlrcch.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2cabricge.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2hvirowcl.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2vvebzuln.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2tjhhcrsi.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2yjegqojc.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2tirqqyan.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2ppzgggah.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2uxdjzlna.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2etcpxfcw.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2vjbwvnsb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2imlzpwwa.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2jktnmhql.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2yzrbsytb.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2qvltoebl.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2vxokksxy.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2vgzjdswt.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2ybrwsmgi.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2qctmacay.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2sserbdub.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2colkixap.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2ahxwfyyn.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2enudwlje.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2lsjwnfbp.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2sgfgcwst.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2drokvqlb.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2lleqbniz.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2btpqxzju.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2pjkgbjee.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2cdvdzxsy.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2bppenpkc.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2zmcelgmz.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2trjblelo.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2xpmhhuoj.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2qisqving.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2vraammxd.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2jahyqtus.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2iatzatwp.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2trfgbfxd.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2lbfkmtqk.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2tjxylrnk.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2gryjtrgv.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2mnhphvep.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2glnncfog.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2njkaxfgp.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2zemvpims.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2mefjmurz.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2fhbbwpfc.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2ydxzasjx.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2lnlxqbrl.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2tutkplyv.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mkcocfzv.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2kleaadsl.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2zmoyaztl.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hmpuvcmu.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2krlvrzrr.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2nfaxadqx.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2wlmaadmm.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2tudgsjbr.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2tvytawhf.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ndljnrfr.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2aezrhlkv.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2gbhgebbo.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2ljzyvmev.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2xofubeac.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2yikyyyfm.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2ucwngjah.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2yyqfjkmc.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2ubzdbzrn.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2brgqugyy.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2lwivtmil.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2aiqfidas.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2drdalqtr.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2oqeggczl.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2pyxlkavf.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2qgjjkffj.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2xfelyqxj.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2amgzqfhx.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2nmfsbmgl.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2qjfcwksi.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2xovwniae.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2paxzslrh.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2odouanpd.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2wszgvuez.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fnukiwos.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2wyulwhjp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qzligxbx.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2kcjppwct.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2nzofgfof.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2yisxyqmb.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2mokqpplh.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2jqplkvyy.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2intohuzw.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ryfqrcxd.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2pjyazfmr.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2zooqnrrj.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2qmvarjxj.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2plexerum.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2afkcanmm.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2lhurnzaw.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2xudiimwn.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2ktaokqgd.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fxwjfffi.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ssqlzpfu.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2tkxzhyeq.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2cnvurrtu.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2nilhkksr.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2erumbzzo.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2jxvbsgmr.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2asqikgnu.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2dvalpgsb.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2jchfawyj.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2nkiplfrw.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2aozmyhcs.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2adptsglu.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2lmsbrkgi.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2xjkfnyjh.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ipbqfsyj.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qpnmevjh.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2qzgzdxte.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2xepznsiz.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2twhvsdxd.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2svsubwef.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2dpjwsrpe.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2bvyvygqa.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2xktrvyop.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2coqbxcup.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2pdpcgghi.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2sabcjqsn.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2zubfgnps.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2bwdptnxb.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2orolyxll.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2jgltuzxy.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2ktifervj.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2iaxqiosj.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2caymgvtp.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xooryfuf.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2rxuiectc.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2yttftbup.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2lefhstic.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2iqdlvnxu.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2ujhjibbu.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2kphqeyme.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2qwxjsayu.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2tvllsafs.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2gwpponio.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2fjibyons.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2tnemumtv.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2xjrzcxun.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2ghkdcamf.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2xeiieixr.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2nvokowuo.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2agkhxash.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2seyzdrft.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2lcwmihzi.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2esietlby.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ygcbwtsw.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2qpyqaoii.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2jfjtioxb.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2qzbakbqw.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ynoraohk.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2knsqqmxn.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2rlpdophe.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2rgsxozvf.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2wryldbkg.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2vqurgvne.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ombesaap.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2vjmcmxek.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2ontcxpmn.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2muswakcx.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2dtbqetus.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2vlkxwsqy.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2njgrgxaj.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2jjrxdhjh.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2rjnajhhq.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2eapgavcb.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2brrloswz.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2wcxjhpdf.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2kcwvolwk.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2zldvduvw.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2xqjplfre.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2rzcrtgbp.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2lmtbbqiz.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2pwdsfywx.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2zghzzfym.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2tznskbxw.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2xwuhvpzv.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2prewovsb.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2pcyyujey.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2yqnolcqr.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2ceyikyuf.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2omhjxlds.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2akdfwuny.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2bqquxspi.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2qitinkyh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xumwrocr.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2lxeajydg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zrlbzpkm.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2qoszajhw.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2zxqrwgei.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2awrvbvtn.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2ovsbmply.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2jnyyjfka.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2ptfqydpp.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2anfzfphk.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2cjetctqk.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2flbqabcw.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2bcwarscp.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2zrctxshl.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2mjcrifdv.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2oxzkvboj.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2hwgzgatw.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2faeefyxe.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2bqksfeyx.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2frucilrq.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2xflgnnlm.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2hetmuljy.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2gpqnehsu.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2aoyzfzxl.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2ifveaspz.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2oyswyveb.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2qsdhkgyz.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2eybaawmz.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2whxpqzgg.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2gqdlgpqh.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2ncejqvuq.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2lekrvaxz.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2qvbjnysn.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rfnwrtwz.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rswvvilp.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2ivsmhvmw.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2lubasnnn.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2jrvjazuh.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nteoogou.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2wyduzgfo.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2kiyzvwaw.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2jwinrdun.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2dftatidq.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ebofnqnd.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2uesbwexp.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2hhgmihqj.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2rvpicljz.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2ofbgkfkc.html


<!-- 参考信息 -->