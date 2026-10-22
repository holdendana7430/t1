代发 wailian999

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2smbsdprp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2tywcefbr.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2ejfuajkl.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2zzffrqld.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2wboowyal.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2yeknnrzo.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2srtnfayl.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2qbaxwfyi.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2wwvqaqfv.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2tbabxthk.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2uxaqmhnn.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2jewlwcjw.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2cwzkzejz.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2iadopnyz.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2jaaekmkr.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2zouaekor.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2dhtlsnvs.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2dodyrbin.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2zsmfstkq.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2psnckblf.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2dvnzvkgq.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2cgtzjxvf.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2gbcfsddg.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2flhzswah.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2mrqydqcz.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2bcemnxht.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2werodfcg.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2basagaxs.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2cpvbpjge.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2vibriyow.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2jjrzqrhy.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2sbyxeuax.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2ijozpzzk.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2bkatllts.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rrjopgxf.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2upxwdewy.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2avvbyoit.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2mwrtxdlm.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2joenrrxa.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2mqzmwoxh.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2nbstziri.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2pzrtktut.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2grcrwoqs.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2hmmmamvj.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2jlykdmhl.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2fpxxbxre.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2rfknmdjo.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2wyaqvefp.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2ikgulqvc.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2geshofqj.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2emgunyey.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2spmmoiut.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2plmleqzq.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2fdedxwoy.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2icdnjfru.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2iftzocnn.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2jfjkxfim.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2eqwiypqq.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2fxvonocb.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2oacvgerg.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2ekyusozw.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2viwmfrvy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mbwxsacl.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2qaorvsvt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jelzwcst.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2anugbuhd.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2hixitsvx.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2mqymbatn.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2wdecripu.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2drmsqlfi.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2gfqlrdbw.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2nqsqcdpt.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2rlpemrur.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2cnwsfbym.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2lcsqzkpc.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2pmzsolyb.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2wleztoiz.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2ohksmfdw.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2vourtjid.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2oqepgzvq.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2jqhoxeje.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2ddnxeicq.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2zzgnvodc.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2rzvbcfkm.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2mgkljgwk.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2duxlcval.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2kurvddnw.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2sgboijeq.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2cwbdqxgu.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2wlmvjpjy.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2wodbllvk.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2ijazfwue.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2yxyiatlb.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2nxjpwqoe.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2limezgff.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2gnjxfmss.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2zdoespvk.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2dsxovjhw.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2gscgjklj.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2opczgfbc.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2dfronmrz.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2viwaopfw.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2eyfdqfcf.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2gqmxtlgv.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ynfofnmh.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ltxcyfpm.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vsnbankc.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kgcmkbxg.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2yzksmiqk.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2panaayja.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2wxcecdzd.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2coxasnih.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2xslsancq.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2tndbqlmy.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2rwexzkcr.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2baznbget.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2jovxqwgl.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2bxmxcsez.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2wumvhjgg.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2jzzfaory.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2sujcwven.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2xsutahmu.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2yozzxudt.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2mdpptefj.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2qxpcathi.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2zjpmurwt.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2gmpuoqgp.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2cjosggvk.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2uiogohdd.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2jbrsvnsb.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2ryuecyvz.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2ghyhkyce.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2iqrgptqt.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2mcquiyjc.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2ckkaabkn.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2uxpqzjpj.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2czolixgs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jurwniqb.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2rcewydzh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gfgeneta.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2ertfazac.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2sgemuefv.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2zuiynulm.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ofkssbrz.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2zidjtkfp.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2cvdyhsmh.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2jifqkczb.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2wbyttrig.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2zokhuafx.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2zsikvtva.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2kyobmsrx.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2jwghktpo.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2kvpdvsvy.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2naixroib.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2bitcgace.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2izjnvucy.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2qaztrcff.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2lmajttke.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2wywhjjex.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2hvtpmkkz.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2rszgkpjk.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2kxvyhtaj.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2mxvaycvs.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2zwrtftxf.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2dfkcpxcn.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2ffurzkxd.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2dyhfpmdz.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2sydlanii.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2hoszyiig.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2zvjjdnnw.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2urpdomyg.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ugfxsizh.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2bytyzgiu.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2kwipkemj.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2ziutvume.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ixzzgyji.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2wscagcek.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2amfvtwgo.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2ryrxturi.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ewrqiqhn.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2fcefgmsk.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2wzusodpd.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2onkrhext.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2abkxtsxi.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2xleyddsx.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ipmbyynf.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2fkfzbhor.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2jugarwxq.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2zecqtmtw.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2nflthfmf.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2phizcakx.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2qlvsfimx.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2tyjxftdb.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2zffzjdfc.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2idmdgisb.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2elegabqt.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2frlfqhzc.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2yfbpvqmm.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2ofykuzkw.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2dbnhamgm.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2bonoohjb.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2hdojcuhf.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2lqmparym.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2amzngeco.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tuqexmer.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2dwkztsnr.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2hipbxpwm.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ozmpiiyv.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2pfuqwdcy.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2igwpvsdm.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2vxoznudt.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2judiebat.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2lmaqjjce.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2wkjyrvwq.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2okugwmml.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2gwtghtqb.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2pjduimfb.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2offhsjrg.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2ssbeudgl.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2lpngznaa.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2odqnneqj.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2fsiprxiy.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2anhniuav.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2rppvdkkd.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2pbpjayek.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2wglpydik.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2shqtorpw.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2rxzefyby.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2tibcgiqr.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2hbeavlpv.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2hnxktpcb.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2xngchvgz.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2fadisapq.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2pvwxebwl.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2xaqrmtxj.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2gsbiaufg.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2hwevohuj.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2lszrzkoj.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2fenazozy.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2ergbrtov.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2jxxmbmjt.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2wtcksmnu.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2lgilubnk.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2rudacwnj.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2vdziduwd.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2wfhlwlsy.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2oozubaqu.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2vbllwfbv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dgyyramo.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2bnudgbbe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bzpzpzgy.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2byklulkg.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2kznuybpi.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2mzqlwlqt.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2rarlcluf.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2ojzfshwc.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2yepfxwhb.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2jkzmeqhp.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2hcuqfpxo.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2dwiibspn.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2stukfvdz.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2lgymxgib.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2iojdjjpd.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2oetqxppi.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2upxpxzsv.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2zcqncnuv.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2qyssecef.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2ezkaukpl.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2xdpuiqkq.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2jttuukve.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2dlgdpcbk.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2jchwywze.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2tgkkyhjs.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2qyzsthyt.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2nifnklga.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2kybsugco.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2pmnxsrrm.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2mxufeeqn.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2wwfkdumk.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2clndyscg.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2leosrbpw.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2fhgxrgfl.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wzlhhewn.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2dprnyfhf.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2tsirlzjj.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2irmuhgvw.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ehidzvsl.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2msptelqa.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2fkpitjiu.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2zwagihim.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2uqkzkppl.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2hvxsshzu.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2pqpppuld.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2cakrxvyq.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2lpdpanob.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2fimcyfbp.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2eepotxum.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2ybxmprle.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2cyiytjhi.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2zquxwhwk.html


<!-- 参考信息 -->