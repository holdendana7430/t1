代发 wailian999

Py:   requests.post(url, json={"a": 1})
来源：http://blog.fehbvm.com/Article/details/gvlqwoitt.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.zdbjq.cn/Article/details/gsghutors.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.zdbjq.cn/Article/details/gtnqblmxk.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.fehbvm.com/Article/details/gajgvadwj.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.fehbvm.com/Article/details/gkbxtejys.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.hesvh.cn/Article/details/gyjpmbnah.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.fehbvm.com/Article/details/gmmcoutww.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.fehbvm.com/Article/details/gfthgdtca.sHtML

[L03] 设置自定义请求头
来源：http://mobile.fehbvm.com/Article/details/gdvvcihdb.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.fehbvm.com/Article/details/gehypbzot.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.zdbjq.cn/Article/details/gbtsizvqj.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.fehbvm.com/Article/details/glqzavwsi.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.fehbvm.com/Article/details/gfxczrqbz.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.hesvh.cn/Article/details/gqfzjtlpp.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.zdbjq.cn/Article/details/gwljtifbf.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.fehbvm.com/Article/details/gkdrcmjxl.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.zdbjq.cn/Article/details/gchvqkcbb.sHtML

[L04] 设置超时
来源：http://www.blog.hesvh.cn/Article/details/gmbhwknvh.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.hesvh.cn/Article/details/gnnaprcny.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.fehbvm.com/Article/details/gwkdjebjc.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.zdbjq.cn/Article/details/ggzqnyygc.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.hesvh.cn/Article/details/gievmgmcw.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.hesvh.cn/Article/details/gfjxalfas.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.fehbvm.com/Article/details/gyikjaumx.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.fehbvm.com/Article/details/ghrhkrfyj.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.hesvh.cn/Article/details/gwozxurlw.sHtML

[L05] 上传文件（multipart）
来源：http://baike.zdbjq.cn/Article/details/giejbrrbq.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.hesvh.cn/Article/details/gnbikjoog.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.zdbjq.cn/Article/details/gwdtnbsxl.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.hesvh.cn/Article/details/gxbaiczzn.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.zdbjq.cn/Article/details/gbgmxokgc.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.hesvh.cn/Article/details/gkufxtywu.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.fehbvm.com/Article/details/gnfmaztkv.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.fehbvm.com/Article/details/geoqjyvap.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gseqcizry.sHtML

[L06] 解析响应为 JSON
来源：http://3g.zdbjq.cn/Article/details/gnyvseorz.sHtML

Py:   resp.json()
来源：http://blog.zdbjq.cn/Article/details/gjjjqoops.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.fehbvm.com/Article/details/gmmydwnpw.sHtML

JS:   await resp.json()
来源：http://read.share.zdbjq.cn/Article/details/gajjjonjd.sHtML

TS:   await resp.json()
来源：http://wap.zdbjq.cn/Article/details/gotpaytpk.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.zdbjq.cn/Article/details/gshzlttvc.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.hesvh.cn/Article/details/galgpazko.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.zdbjq.cn/Article/details/gecqckysd.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.hesvh.cn/Article/details/grswqepft.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.hesvh.cn/Article/details/gulusuqxj.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.zdbjq.cn/Article/details/gpbpkzhmn.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.hesvh.cn/Article/details/gsejnsssm.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.hesvh.cn/Article/details/gmtgleneb.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.fehbvm.com/Article/details/guisxqjeo.sHtML

Java: resp.statusCode()
来源：http://mobile.fehbvm.com/Article/details/ggfnyeddu.sHtML

Go:   resp.StatusCode
来源：http://baike.zdbjq.cn/Article/details/gxgvawcfs.sHtML

Ruby: resp.code.to_i
来源：http://wap.zdbjq.cn/Article/details/gkkcuuybp.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.zdbjq.cn/Article/details/gvmydrktn.sHtML

[L08] 并发请求多个地址
来源：http://blog.zdbjq.cn/Article/details/gxclbbgbk.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.fehbvm.com/Article/details/gxsfyglin.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.hesvh.cn/Article/details/gnuelmggs.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.hesvh.cn/Article/details/gloehwtxn.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.hesvh.cn/Article/details/geayzowfz.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.zdbjq.cn/Article/details/gmfzgedwt.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.fehbvm.com/Article/details/gkwdkzrei.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.fehbvm.com/Article/details/ghnonvcpq.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.hesvh.cn/Article/details/ghfcxnztl.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gccczojby.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.zdbjq.cn/Article/details/gypyfrwpb.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ganoiqkpn.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.zdbjq.cn/Article/details/gxowsvprh.sHtML

Py:   sys.argv[1:]
来源：http://read.share.hesvh.cn/Article/details/gduupgvrd.sHtML

PHP:  $argv;  $argc;
来源：http://wap.hesvh.cn/Article/details/gcjmvhbic.sHtML

JS:   process.argv.slice(2)
来源：http://blog.zdbjq.cn/Article/details/ghnwqbxmz.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.zdbjq.cn/Article/details/gwqdnpcvu.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.hesvh.cn/Article/details/gearzfasl.sHtML

Go:   os.Args[1:]
来源：http://blog.hesvh.cn/Article/details/gblbzsuga.sHtML

Ruby: ARGV
来源：http://www.share.zdbjq.cn/Article/details/ghoweeviv.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.zdbjq.cn/Article/details/girifvaat.sHtML

[M02] 读取环境变量
来源：http://wap.hesvh.cn/Article/details/glbrrmrnv.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.hesvh.cn/Article/details/gxzyqwcqw.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.hesvh.cn/Article/details/gnyumyzcw.sHtML

JS:   process.env.HOME
来源：http://www.m.share.hesvh.cn/Article/details/gyutkxwxs.sHtML

TS:   process.env.HOME
来源：http://blog.zdbjq.cn/Article/details/gcirvsfje.sHtML

Java: System.getenv("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gzhybqphk.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.fehbvm.com/Article/details/giriafngh.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.hesvh.cn/Article/details/gqzvvgqky.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.zdbjq.cn/Article/details/gxbnlqskc.sHtML

[M03] 执行外部命令
来源：http://wap.zdbjq.cn/Article/details/gmtlzunsw.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.hesvh.cn/Article/details/gkmiouonu.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.hesvh.cn/Article/details/gxdmlteim.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.hesvh.cn/Article/details/gtskvfont.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.fehbvm.com/Article/details/gffsdjwty.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.fehbvm.com/Article/details/gqtubcboo.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.fehbvm.com/Article/details/gvgaqnoau.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.fehbvm.com/Article/details/ggnghnupd.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.hesvh.cn/Article/details/gufcknofh.sHtML

[M04] 获取当前工作目录
来源：http://m.share.fehbvm.com/Article/details/gbgiqjxya.sHtML

Py:   os.getcwd()
来源：http://www.blog.fehbvm.com/Article/details/grehjpppp.sHtML

PHP:  getcwd();
来源：http://m.share.zdbjq.cn/Article/details/gykoexptg.sHtML

JS:   process.cwd()
来源：http://www.blog.zdbjq.cn/Article/details/gtxeczdlh.sHtML

TS:   process.cwd()
来源：http://wap.fehbvm.com/Article/details/gvoymvrxl.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.hesvh.cn/Article/details/gxegwymbl.sHtML

Go:   os.Getwd()
来源：http://www.blog.fehbvm.com/Article/details/gowjlecrc.sHtML

Ruby: Dir.pwd
来源：http://blog.zdbjq.cn/Article/details/gtbyxbuic.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.hesvh.cn/Article/details/ggremeeyo.sHtML

[M05] 设置退出码
来源：http://www.m.share.zdbjq.cn/Article/details/gkfvocioe.sHtML

Py:   sys.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gvkpnkdkd.sHtML

PHP:  exit(1);
来源：http://www.share.hesvh.cn/Article/details/galolfovo.sHtML

JS:   process.exit(1)
来源：http://baike.fehbvm.com/Article/details/gjmjvpxni.sHtML

TS:   process.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gmzhqhssu.sHtML

Java: System.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gseyfbqgg.sHtML

Go:   os.Exit(1)
来源：http://wap.zdbjq.cn/Article/details/gtpkkjccm.sHtML

Ruby: exit 1
来源：http://www.blog.zdbjq.cn/Article/details/gkmbzkxpk.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.hesvh.cn/Article/details/gmvsvhuiv.sHtML

[M06] 向标准错误输出
来源：http://3g.fehbvm.com/Article/details/ggfubmieo.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.zdbjq.cn/Article/details/gekivkglv.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.fehbvm.com/Article/details/glljgigbu.sHtML

JS:   console.error("err")
来源：http://blog.hesvh.cn/Article/details/gnygtwfug.sHtML

TS:   console.error("err")
来源：http://read.share.zdbjq.cn/Article/details/gvkztypbw.sHtML

Java: System.err.println("err")
来源：http://baike.hesvh.cn/Article/details/gehrfmfwv.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.fehbvm.com/Article/details/ghyhtpxcp.sHtML

Ruby: warn "err"
来源：http://www.blog.zdbjq.cn/Article/details/gslttihbn.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gftlgiiek.sHtML

[M07] 判断是否为主入口
来源：http://baike.zdbjq.cn/Article/details/gwbgjbiud.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.hesvh.cn/Article/details/guonjkcsy.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.zdbjq.cn/Article/details/gzgwlmguc.sHtML

JS:   require.main === module
来源：http://blog.fehbvm.com/Article/details/gcozwfrib.sHtML

TS:   require.main === module
来源：http://m.share.fehbvm.com/Article/details/gprnnnzln.sHtML

Java: public static void main(String[] args)
来源：http://baike.zdbjq.cn/Article/details/gdfippfhg.sHtML

Go:   func main()
来源：http://wap.zdbjq.cn/Article/details/gllbsktfw.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.hesvh.cn/Article/details/gfwfnrciw.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.hesvh.cn/Article/details/gvrgyfuar.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.hesvh.cn/Article/details/gpdikzfes.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.zdbjq.cn/Article/details/gslgciqno.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.zdbjq.cn/Article/details/gpvceeqrc.sHtML

JS:   process.platform;  process.version
来源：http://read.share.zdbjq.cn/Article/details/guvkwhsul.sHtML

TS:   process.platform;  process.version
来源：http://www.share.zdbjq.cn/Article/details/gmrfopfik.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.hesvh.cn/Article/details/gqiuhislo.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.hesvh.cn/Article/details/gduezzehu.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.hesvh.cn/Article/details/gkgkczena.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.hesvh.cn/Article/details/gdbdfbkbs.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ggejfbmfa.sHtML

N. 数据结构与算法
来源：http://baike.zdbjq.cn/Article/details/gdefhnxhv.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/guxettnho.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.fehbvm.com/Article/details/gvdzgveaa.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gllhvflai.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.zdbjq.cn/Article/details/gclggxihz.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.zdbjq.cn/Article/details/gdqrycngy.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.hesvh.cn/Article/details/ghrxyrtlz.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.hesvh.cn/Article/details/gjqaufnar.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gbmrmgcol.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.hesvh.cn/Article/details/gbzyrmxgt.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gfagowqai.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.fehbvm.com/Article/details/giykqvedk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.zdbjq.cn/Article/details/gmfqoeobh.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.hesvh.cn/Article/details/gmoyiwysd.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/glnkmockx.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/ghtouvpkq.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.hesvh.cn/Article/details/gwlcsaqve.sHtML

Go:   slices.Sort(arr)
来源：http://blog.hesvh.cn/Article/details/glicgkknj.sHtML

Ruby: arr.sort
来源：http://www.m.share.zdbjq.cn/Article/details/guosmskaw.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.fehbvm.com/Article/details/gyjcsgrlk.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.fehbvm.com/Article/details/gmxebdjgj.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.hesvh.cn/Article/details/gyzxortfx.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.zdbjq.cn/Article/details/gpxcqloue.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.hesvh.cn/Article/details/gtsvuwemv.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.hesvh.cn/Article/details/giloyemkn.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.zdbjq.cn/Article/details/gwhmhbkdl.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.fehbvm.com/Article/details/gnhwvikrk.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.hesvh.cn/Article/details/ggfrbiare.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.zdbjq.cn/Article/details/gdpmzvmft.sHtML

[N04] 斐波那契数列
来源：http://www.share.fehbvm.com/Article/details/ggnzmsecd.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.zdbjq.cn/Article/details/gbsadbjir.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.zdbjq.cn/Article/details/gfvsqpdmr.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/gqhtjjfvr.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/gyoydecxb.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.zdbjq.cn/Article/details/gtyhyxvhp.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.hesvh.cn/Article/details/guxcqckhj.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.zdbjq.cn/Article/details/gxoyahwkm.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/gjqkcnsuh.sHtML

[N05] 最大公约数
来源：http://3g.zdbjq.cn/Article/details/goupgcscf.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gfwfcltvd.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.fehbvm.com/Article/details/gzkracbax.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.zdbjq.cn/Article/details/gnwxlaexh.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.zdbjq.cn/Article/details/gmjdvwced.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.zdbjq.cn/Article/details/gbpngyyop.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.fehbvm.com/Article/details/gdmxbgmqf.sHtML

Ruby: a.gcd(b)
来源：http://read.share.zdbjq.cn/Article/details/gkwkyvnyf.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.zdbjq.cn/Article/details/gevxopgzo.sHtML

[N06] 判断回文字符串
来源：http://wap.hesvh.cn/Article/details/gfignavvc.sHtML

Py:   s == s[::-1]
来源：http://read.share.fehbvm.com/Article/details/gmpvxfsgw.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.fehbvm.com/Article/details/gpcietmep.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gquropwcf.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/grhaptzpq.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.zdbjq.cn/Article/details/gabhhzxli.sHtML

Go:   // 双指针从两端比较
来源：http://wap.hesvh.cn/Article/details/gqotyurye.sHtML

Ruby: s == s.reverse
来源：http://baike.hesvh.cn/Article/details/gjxoyhnlc.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.zdbjq.cn/Article/details/ggpilkpav.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.hesvh.cn/Article/details/gzdwileym.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.hesvh.cn/Article/details/gbezmijlw.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.hesvh.cn/Article/details/gvoqhddyj.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.zdbjq.cn/Article/details/ghlbillhr.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.hesvh.cn/Article/details/gudqtytjw.sHtML

Java: // 手写 HashMap
来源：http://3g.zdbjq.cn/Article/details/gpqpiznfn.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.hesvh.cn/Article/details/gzuysklfj.sHtML

Ruby: // 手写 Hash
来源：http://blog.zdbjq.cn/Article/details/gmmtfoclc.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.hesvh.cn/Article/details/gixdbmbbq.sHtML

[N08] 生成全排列
来源：http://www.blog.zdbjq.cn/Article/details/gvovoxzbr.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.hesvh.cn/Article/details/getbaskgx.sHtML

PHP:  // 手写递归交换
来源：http://mobile.fehbvm.com/Article/details/gjqyspdub.sHtML

JS:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gjpqudsvx.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gpsfnvhxu.sHtML

Java: // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gdzezuvpk.sHtML

Go:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gegjynjjd.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.hesvh.cn/Article/details/gnvywlugc.sHtML

C#:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/grtvwiyat.sHtML

[N09] 栈与队列
来源：http://3g.zdbjq.cn/Article/details/gxggbqrxc.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.fehbvm.com/Article/details/glmiixgea.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gywsrplgp.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.hesvh.cn/Article/details/gevvhcqlv.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.fehbvm.com/Article/details/gpbjpzfrd.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.fehbvm.com/Article/details/gbeqgrfhw.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.zdbjq.cn/Article/details/gikuwusyc.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gedtijlqg.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.zdbjq.cn/Article/details/glbuotvfa.sHtML

[N10] 链表节点定义
来源：http://www.blog.zdbjq.cn/Article/details/gwgyhilji.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.hesvh.cn/Article/details/gtdwyidro.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.hesvh.cn/Article/details/gscfvwbps.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.hesvh.cn/Article/details/gnmkqsnxv.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.fehbvm.com/Article/details/ggsworpjv.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.fehbvm.com/Article/details/gcvqdsyna.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.fehbvm.com/Article/details/gqqpxmalv.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.hesvh.cn/Article/details/ghkzbqvrp.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.hesvh.cn/Article/details/gcozogzui.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.hesvh.cn/Article/details/galrfdlke.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.zdbjq.cn/Article/details/ggawygroo.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.hesvh.cn/Article/details/gapznshfe.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fehbvm.com/Article/details/gykmcnzrd.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.zdbjq.cn/Article/details/gunrfcbtg.sHtML

Java: // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gvygaalgj.sHtML

Go:   // 手写递归
来源：http://read.share.fehbvm.com/Article/details/ghclhhyee.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.hesvh.cn/Article/details/gfizxxewd.sHtML

C#:   // 手写递归
来源：http://www.share.fehbvm.com/Article/details/gjofssaqr.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.fehbvm.com/Article/details/gmmyqqcfz.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.hesvh.cn/Article/details/gugrgtagl.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.zdbjq.cn/Article/details/gzpfqibgd.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.hesvh.cn/Article/details/gnvcidama.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fehbvm.com/Article/details/gvshpbkzt.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.zdbjq.cn/Article/details/ggjdttyva.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.fehbvm.com/Article/details/gyqaqbsge.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.fehbvm.com/Article/details/glswpzcwi.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fehbvm.com/Article/details/gdnvvmflk.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gqftzumiz.sHtML

O. 并发与异步
来源：http://read.share.hesvh.cn/Article/details/gnssjrhid.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ghwqylpgq.sHtML

[O01] 启动一个线程
来源：http://3g.fehbvm.com/Article/details/gmboplhww.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.fehbvm.com/Article/details/gnrpfprlp.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.hesvh.cn/Article/details/gqlhpfqeg.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.hesvh.cn/Article/details/gimsewucc.sHtML

TS:   // 同 JS
来源：http://mobile.fehbvm.com/Article/details/gngcqphdl.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.fehbvm.com/Article/details/guesqirnw.sHtML

Go:   go f()
来源：http://baike.zdbjq.cn/Article/details/gyhnjrgjn.sHtML

Ruby: Thread.new { f }
来源：http://wap.zdbjq.cn/Article/details/gpemxexxr.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.zdbjq.cn/Article/details/gmhosfonv.sHtML

[O02] 使用线程池
来源：http://baike.hesvh.cn/Article/details/ggggggnav.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.hesvh.cn/Article/details/gvixuwevo.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.hesvh.cn/Article/details/gntcjvjah.sHtML

JS:   // worker_threads 线程池
来源：http://wap.zdbjq.cn/Article/details/gxzrgrswg.sHtML

TS:   // worker_threads 线程池
来源：http://blog.fehbvm.com/Article/details/gjduabyor.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.fehbvm.com/Article/details/gcjrbfmmg.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.hesvh.cn/Article/details/gtmkhwgze.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.hesvh.cn/Article/details/ghipwnnaw.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.zdbjq.cn/Article/details/gndlgsxoe.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.zdbjq.cn/Article/details/gkbwujhvi.sHtML

Py:   with lock: shared += 1
来源：http://blog.zdbjq.cn/Article/details/gxzrbmgdo.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.zdbjq.cn/Article/details/gejzgnkfl.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.hesvh.cn/Article/details/guiktihkf.sHtML

TS:   // 同 JS
来源：http://3g.hesvh.cn/Article/details/gktszfbha.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.zdbjq.cn/Article/details/gnprnxndl.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.fehbvm.com/Article/details/guibgboxx.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.fehbvm.com/Article/details/gjakbhubl.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.hesvh.cn/Article/details/gsjyjecco.sHtML

[O04] 定义异步函数并等待
来源：http://blog.zdbjq.cn/Article/details/gxtzavnjm.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.zdbjq.cn/Article/details/gnljxlwrt.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.hesvh.cn/Article/details/ghzjezdcn.sHtML

JS:   async function f() { await g(); }
来源：http://wap.fehbvm.com/Article/details/geycpdyhu.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.hesvh.cn/Article/details/ggvcodsjo.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.fehbvm.com/Article/details/gsnnpclza.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.zdbjq.cn/Article/details/gstpanguo.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.hesvh.cn/Article/details/gtbczgpvq.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.hesvh.cn/Article/details/ghfbkfugl.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.zdbjq.cn/Article/details/gzqczxciv.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.hesvh.cn/Article/details/goilnfptm.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.hesvh.cn/Article/details/gpgdtginn.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.fehbvm.com/Article/details/gkjcuvdsu.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.zdbjq.cn/Article/details/gxlbrvfpt.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.fehbvm.com/Article/details/gzwkakjwo.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.zdbjq.cn/Article/details/ghkdzytbd.sHtML

Ruby: threads.map(&:join)
来源：http://wap.fehbvm.com/Article/details/gfndsqdgz.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.hesvh.cn/Article/details/gskkexyin.sHtML

[O06] 使用进程池
来源：http://m.share.zdbjq.cn/Article/details/gkirbvkwx.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.zdbjq.cn/Article/details/gwhxrpeho.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.fehbvm.com/Article/details/gxhtfrogc.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.fehbvm.com/Article/details/gsrfqkbce.sHtML


<!-- 参考信息 -->