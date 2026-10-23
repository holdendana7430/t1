代发 wailian999

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3nlngbawt.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3cmpisuej.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3jtbcuqdv.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3apfqdnlu.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3dgoxaftq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3ypegssok.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3yotbwkvi.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3cbmpfbjq.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3ffqcimda.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3vhnxdjvh.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3dtgmdsqs.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3utvbumcs.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3deiuyoca.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3dszzesgh.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3maeimyvv.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3ovifggmc.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3mwdigtth.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3ojtalwwx.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3llvfglyz.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3psphlind.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3yfypgqoa.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3hecsqxkl.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3hyhxidzw.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3jxxsvres.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3svxbymne.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3equkehpx.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3nfscdzar.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3rrdmhmlj.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3tlxatuen.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3somcjrur.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3jkbhiekz.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3vzzvjyzp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3mbsivulj.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3kpjswbwa.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3nbnuwjph.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3jaywwucl.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3egzzagkp.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3hdfekgdd.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ixsgqcaw.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3mzeesqdi.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3awhzrpna.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3wfgpnkhn.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3wbzqvukp.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3zevpcbnc.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3ggseglxe.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3wiaxfges.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3wqxoclfb.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3qxailmee.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3xoyeumuu.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3tujslqdi.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3vpempzin.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3uroglglq.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3iedujqah.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3ajmronpd.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3hbphbjhx.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3kzqomvce.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3hkpcwhqt.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3accjzczx.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3negziiuf.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3dhsuvhvq.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3qqujxnrg.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3cbxxndqw.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3xycvsoob.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3cufjiivq.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3weqjegrj.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3bjdikuuf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eotsiozm.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3eofnwawm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zjcbhcjm.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3gurfbrzd.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3ykavicfa.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3hpwothhc.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3yqofmedo.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3kowytlhc.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3ynecuiff.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3jlzvfdgt.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3equfdqar.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3kuhbpsap.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3jxmgpzuc.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3slcyoeis.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3oagnuztn.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3iwhohfsp.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3zvoiegut.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3zwjaecqe.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3bqqwdjot.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3uvlknorg.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3bkjvkgdl.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3ggbsgxyg.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ioiudzyx.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3ehcewrhz.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3efzlrysg.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3flkttmfa.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3ahbkohch.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3uouumoua.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3utbhrzuj.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3vvqsxrzn.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3aoocvxaq.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3jsenpmti.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3hldjipgm.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3grrkjone.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3uhmeoeqs.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3tntbgfmm.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3fqbatmmf.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3cmletxvf.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3ogghdvrj.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3swoizuff.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dvgsiwyk.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3iaotwtsw.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vcrafkow.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3igfeepmb.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3flmljmsh.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3msnsainx.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3eqapvlmo.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3tfajuatm.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3ryrwtlik.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3rbkeybos.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3rspzfkbw.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3goonxvye.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ybouirvd.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3rjoyucqn.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3uenfjbpo.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3ndzdgfuw.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3dvessofz.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3cpyztuvd.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3vhmbmwin.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3mrvlivcz.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3vnguhkos.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3dsfwwuli.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3ncyowgxj.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3lvveoefi.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3ltorscsz.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3gawtygof.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3uaxdysqg.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3jihrsign.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3vkktfzcs.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3qqrnonfa.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3bxxhpyht.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3ffyybhpn.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3jqwajzmx.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3qsylgnli.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3zvujrhpj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jxlpqqse.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3ayslotag.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ftsjqvyu.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3glzywyax.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3pmeuncny.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3gvqbflyw.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3uuvrlchz.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3qkksxktl.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3wgdouwvr.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ifxwpvaq.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3iinknwmx.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ubihfpda.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3vaivdfju.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3vwoiwviu.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3njbzpwnv.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3vglliefq.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3axeefgcz.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3kbtgglis.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3cikhnxdm.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3azhxtgoq.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3ikysidzz.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3jqjldwkg.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3snoxasah.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3ocvkfywr.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3lzhnojyv.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3pyvajomt.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3vsjobmik.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3efsnxzce.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3ddtzgeez.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3kmtbuuaq.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3iwjaermh.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3njhpyupe.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3fknaufei.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ngcitjfo.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3lrtonfua.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3hebrbeaj.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3ezgmupch.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mzejpfqo.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3gavskzma.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3urtznmui.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3ripxkhpg.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3nwmyzltn.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3klhaqlkr.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3inluwsvo.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3dvaqinxh.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3cosuluxe.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3kgkgkzrw.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3yobiwsqo.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gijhcuxm.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3lwutunuz.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3ilnvfdtv.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3jirgotxs.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3nabrgwnn.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3jhmbqomh.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3enngrsps.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3ypxvxybu.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3rahmreta.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3foizyufu.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3fwyenqzl.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3lqsrryzd.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3nlengpfz.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3imaecfep.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3tpgltxbn.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3nukzzcge.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3pdibtsrb.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3qzibgxty.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3daqljpbc.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3kuflrlkt.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3wplgigfq.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ukvqwukw.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3twotkwio.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3jtjgagdw.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3qqjyyslx.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3nvqakcui.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3gyiouktm.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3jwzzozkj.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3tptdmplx.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3bmzeoiud.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ymndokxq.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3nxkcfuss.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3hnnygxae.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3etovyoiv.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3efsvcoba.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3yykugwsk.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3hybeghbk.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3uoxwuatn.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3bucxetqa.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3fgqpntoo.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3tbauwwta.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3nbysrazu.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3dpksafpz.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3rlpibfse.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3rdpbupux.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3mdcmreyb.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3qkpnchpe.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3bnvggfyi.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3ntfccrvl.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3watsgdbb.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3eluusqas.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ktzvwwdj.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3ejqyezut.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3nhometyh.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3kmlfpndc.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3blipnawn.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3ipvhuxqx.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3acbsdjix.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3bmqgzxdt.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3mnnxnzyc.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3wkkqnbkh.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3ruzxqxvf.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3qgygfusj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oilmixkc.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3flsknjjh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3obhdyyee.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3prwtfruh.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3hcqnwyfv.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3fbgadsvt.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3gjwqpgwu.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3zuwfvbib.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3ogeempgn.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3rpnmdiur.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3loancovi.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3eorhzmgc.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3vsezccfl.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3ahzrmjcg.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3jckfiqqc.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3fwtruuct.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3lhvzceik.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3mrxeqytu.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3rgzsoswb.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3sbemngso.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3qykowfgz.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3wibwgeij.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3ztcgqejw.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3xtssxtia.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3yqtzclvc.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3xfomfcdy.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ygjzcjeh.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3uwqutwvs.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3yyjpabvo.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3qcjadeik.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3wcjumskp.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3pfkmnuhh.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3fphhpvyb.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3immvngyv.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3ulkvsnrx.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3xxorepza.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3gccawwxs.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3fefbocwt.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qhtqognb.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3ykqrtgdj.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3bhedbmiu.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3wefryral.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3gggleseq.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3bzacbphq.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3axrxdmng.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3qjjzlhln.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3ahgsdaxw.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3ixdhpgcp.html


<!-- 参考信息 -->