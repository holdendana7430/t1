代发 wailian999

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3azbhpcsa.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3fjbbdjxm.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3xorcbfmm.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3vydlgvyi.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3ofwbjlld.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3qhhqoahw.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3frvinjgq.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3cfkhxfgs.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3idepyffk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3jmywtfaw.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3obozevwl.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3gkfuxrlo.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3lziglcge.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3nralpmlz.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3xkbpnkte.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3ecvvvsac.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3bmrowylm.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3aypubxqv.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3alenguoj.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3oroepqtf.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3aqbmftea.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3fpqicnys.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3zizkpyog.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3jmgrzqck.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3mkbhgskd.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3abtkmpbp.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3becyihxr.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3ryyrwwcl.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3bljuqihg.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3qnxhwsrp.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3indihjem.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3xuskwgcn.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3miksysht.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3pvyhxiox.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3qxcfyvbq.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3kujekasc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3ahjjzgco.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3xjqkmvqo.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3knwaaivm.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3etwnanhb.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3qhsclnqy.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3dshuywup.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jueypudh.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3vaiztdmr.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3eczdmpya.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3qfxyrpkh.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3hdlxvpss.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3fzvtmvbt.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3bggokmbd.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3ivhpvldj.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3eqytbzmq.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3bnmttvmn.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3rvwhemnd.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3jivkkngf.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3zntotrpi.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3mfwnuibt.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3oohbmrab.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3utvtjart.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3naizikrq.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3nesxghvo.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3aafdocnl.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3afvwfcfb.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3brnslshy.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3wuymgmwg.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3krpmxsxa.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3agwhraol.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3lghxqgxf.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3ekdzyyvr.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3axtqpxio.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3whfjozhr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uubocigg.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3oalwcpza.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mbyjwfwn.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3eiybejut.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3dbunmfum.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3dnijqkoc.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3rikyoacy.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3xaqhyyir.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3uufhicny.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3zyikccpp.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3jdjezaay.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3uoixqhmj.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3hlylnotj.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3numkgtlq.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3higqhgwm.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3fgopmhji.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3ulwpbntq.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3rxuxexsw.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3pimzqpid.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3vvfrpudm.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3xickxvcw.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3fcupxklk.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3afxtarte.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3bibvxigk.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3qskezhds.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3qaxwbkft.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3kjifygnl.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3qlvgjmlj.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3rpqzkluc.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3hkwgtiwc.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3nxmredim.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3cxfcpped.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3jlmybovk.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3wmrasufm.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3xultwmeg.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3czsqiula.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3borsfruq.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3garpxeah.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3kqyfzaok.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3vaykcteo.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3kztvnkjl.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3xbduvkmw.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3lhbgiexz.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ypwgrsla.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3uekwlzqf.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3rmdwlnrq.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3pqzoacdg.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3xszkkivo.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3xjwwxgna.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3zogdcymh.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3wohupoef.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ielgxdql.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ljnkoojp.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3wgprxzku.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3fqbdxsbe.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3naayeirf.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3kmwmcenq.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3itqznwpq.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3xfvnrfaq.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3amavstnm.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3yknqcfga.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3aenvmiao.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3uttguhfh.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3jlzsuwcz.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3mmuhcaip.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3ivrtlggx.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3ikuhlpro.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3exdqoton.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3spgwjuaf.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3ppipznxv.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3iaaejajb.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3kqqyllsx.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3iuweedgz.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3nswsaulm.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3uwvypazb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fvckauqh.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3oubhjpzk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zyepfsjy.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3qigobdhg.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3shamgjgl.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3hanmxugb.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3vsvxeegf.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3dgcqyfah.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3nkwgwmkv.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3qesptdfo.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3rvgxbgdh.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3lcsyyvlj.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3krhztdzi.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3xuhoiztj.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3jbbafoji.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3nzczskws.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3cntvyphp.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3rstoecfd.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3urxshnjf.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3yjzjingf.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3cmchvczu.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3oszxljio.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3nujkptvj.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3jcksdiml.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3hlvkkndh.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3whpodyau.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3clgvgkhl.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3rqpjysop.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3cbrqpdcq.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3fxnhpihn.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3qpfxdajf.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3ebvoltpv.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3ystfhdtc.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3xyaegmjb.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3vqzirrvi.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3vlkvagyc.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3bbwfubrp.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3ugxjcdlt.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3rcnujlnx.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3smtvcyxz.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3nshhvxhn.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3ptogouzk.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3cwwnwsnp.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3tjxqjmpq.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3nloaakst.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3keeivyxw.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3dipmjevg.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3sonclekn.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hdjwopfu.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3uupiaujx.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3jdqvhnxf.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rbpbmydj.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3fvczwnrp.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3jlkklndb.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3xxsyfdqh.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3lnaaizzf.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3rjhptkzn.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3gunjpjea.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3fjgwxaie.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3dpjhoxmq.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3xzckeyys.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3bqyeooxc.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3labvykco.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3svkmijba.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3stxmgmkl.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3rqxnzdox.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3hzljhgar.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3ifrevsnn.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3chvpwjby.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3rbjwmolr.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3fsslzkxl.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3padmqzgl.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3rdxjatmi.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3yqaqnppz.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3rivqychw.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3tjcdasjq.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3usqjdgbq.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3rwdlqfbg.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3whqpdqab.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3upslsqbv.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3yqgscavh.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3gzptnmun.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3abbzabpe.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3szmjgxpi.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3jeecnpmb.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3qdgpgydg.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3spimffjq.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3cybxgbwo.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3grylefup.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3emrcihaj.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3farfahmp.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3aywcthty.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3uckbmedb.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3vmiczibn.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3wwmwcyjq.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3gbefukkd.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3gyrxsauw.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3euogpsam.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3lvkactsn.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ckemvrgj.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3aclxsbvo.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3mtolqkhb.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3kbvuaobf.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3rvceuqpl.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3rfsqzaxu.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3qiysinop.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3vwplaffe.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3zktriojv.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3dnuztxsg.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3nlcarbtr.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3haomjlbg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vmyoglof.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3usjelrax.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cutsvcju.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3nkflaqha.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3ecgunkxg.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3kqoezsmy.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3azetpdza.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3lyvgzfrm.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3mffhvfjt.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3rvajarzz.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3tvbxbshg.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3cyjbwfbh.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3gsojoveg.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3xwvzptmd.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3ernwrwfx.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3stcihzwf.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3eboogqmg.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3kyozuqsn.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3memodwvf.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3zulmutkz.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3ryydmhkc.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3qfogvvvn.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3ymnmlact.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3jtrxkhso.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3mqwneewp.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3cqvlmhbf.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3zktvdddk.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3radtbyds.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3updiebgf.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3sppzguzu.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3pxeegxtn.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3lybnsxnc.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3piplblpa.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3eygntyzm.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3dzwonvnn.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3ltvbvdpx.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3kzfqqoey.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3rqjmreqc.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3azyimbed.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3tgaabfiy.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3adqbxpmi.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3odmumsln.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3xfvzbgcu.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3kkrnhjmc.html


<!-- 参考信息 -->