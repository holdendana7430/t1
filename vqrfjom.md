代发 wailian999

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.hesvh.cn/Article/details/gskfzkyxr.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.hesvh.cn/Article/details/gcxtqqgqb.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.fehbvm.com/Article/details/gooapjdoc.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.fehbvm.com/Article/details/gubhsarvh.sHtML

[L03] 设置自定义请求头
来源：http://wap.hesvh.cn/Article/details/guylxdonj.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.hesvh.cn/Article/details/geuvfgpez.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.zdbjq.cn/Article/details/goaiyjgcr.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.zdbjq.cn/Article/details/galksrqhz.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.fehbvm.com/Article/details/gzulqtnwl.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.hesvh.cn/Article/details/gqksszbxj.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.fehbvm.com/Article/details/gxbrrtdph.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.zdbjq.cn/Article/details/gunegicvb.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.zdbjq.cn/Article/details/gbrxijcwa.sHtML

[L04] 设置超时
来源：http://3g.hesvh.cn/Article/details/gpukijlku.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.fehbvm.com/Article/details/gocyegdhy.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.fehbvm.com/Article/details/gtbnyspex.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.fehbvm.com/Article/details/gggrzawml.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.zdbjq.cn/Article/details/gvqfrojph.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.hesvh.cn/Article/details/gaobcyhrh.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.hesvh.cn/Article/details/gbcxxlrwx.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.hesvh.cn/Article/details/gkdxqetnd.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.zdbjq.cn/Article/details/gxcmpzwob.sHtML

[L05] 上传文件（multipart）
来源：http://baike.zdbjq.cn/Article/details/gvnihshjk.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.fehbvm.com/Article/details/ggcvmsvnr.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.hesvh.cn/Article/details/gauweznvo.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.hesvh.cn/Article/details/gawtkmgdo.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.hesvh.cn/Article/details/gcmhvqqpo.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.hesvh.cn/Article/details/gqjviodnd.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.zdbjq.cn/Article/details/greymmfrm.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.fehbvm.com/Article/details/gjvolhqmo.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gfmpepbht.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.hesvh.cn/Article/details/gbrvgefct.sHtML

Py:   resp.json()
来源：http://wap.fehbvm.com/Article/details/gbupoyjpk.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.fehbvm.com/Article/details/gbpfdlmof.sHtML

JS:   await resp.json()
来源：http://baike.hesvh.cn/Article/details/gbmktpckf.sHtML

TS:   await resp.json()
来源：http://www.share.zdbjq.cn/Article/details/goqrqcmyd.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.fehbvm.com/Article/details/gihodufny.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.zdbjq.cn/Article/details/gonjyizpq.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.zdbjq.cn/Article/details/gclqizciz.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.zdbjq.cn/Article/details/gxujkvlri.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.zdbjq.cn/Article/details/gcszksbds.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.fehbvm.com/Article/details/gpoytdrwx.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.fehbvm.com/Article/details/gkusatknv.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.hesvh.cn/Article/details/gzamoknie.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.zdbjq.cn/Article/details/gzkorwgfj.sHtML

Java: resp.statusCode()
来源：http://wap.zdbjq.cn/Article/details/gtvshqwjg.sHtML

Go:   resp.StatusCode
来源：http://wap.fehbvm.com/Article/details/gzywkiktu.sHtML

Ruby: resp.code.to_i
来源：http://www.share.zdbjq.cn/Article/details/glbweuzqr.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.zdbjq.cn/Article/details/gyrzixqat.sHtML

[L08] 并发请求多个地址
来源：http://mobile.zdbjq.cn/Article/details/gsyppkope.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.hesvh.cn/Article/details/gakygywal.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.zdbjq.cn/Article/details/gxtdesjis.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gzrxnnjfj.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.zdbjq.cn/Article/details/guqatncnq.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.zdbjq.cn/Article/details/gdaosszbl.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.zdbjq.cn/Article/details/gsbzlljrl.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.fehbvm.com/Article/details/grmwwpbxs.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.hesvh.cn/Article/details/gtrvwxsnx.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gjxvhngbr.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.fehbvm.com/Article/details/gfiyfofuk.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gkgehiroh.sHtML

[M01] 读取命令行参数
来源：http://mobile.hesvh.cn/Article/details/gwcpxddmg.sHtML

Py:   sys.argv[1:]
来源：http://wap.fehbvm.com/Article/details/glduanxqv.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.fehbvm.com/Article/details/grdqefkpv.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.zdbjq.cn/Article/details/ggdluenva.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.hesvh.cn/Article/details/grjfivokj.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.hesvh.cn/Article/details/gpwetgxlc.sHtML

Go:   os.Args[1:]
来源：http://www.blog.fehbvm.com/Article/details/gfsnbtked.sHtML

Ruby: ARGV
来源：http://blog.hesvh.cn/Article/details/gddyunwuq.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.zdbjq.cn/Article/details/gijojcnwt.sHtML

[M02] 读取环境变量
来源：http://3g.fehbvm.com/Article/details/gqlervbww.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.zdbjq.cn/Article/details/ggjoiegvs.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.hesvh.cn/Article/details/gdcvlzsrp.sHtML

JS:   process.env.HOME
来源：http://m.share.zdbjq.cn/Article/details/gdulfgicx.sHtML

TS:   process.env.HOME
来源：http://mobile.fehbvm.com/Article/details/gfajpjham.sHtML

Java: System.getenv("HOME")
来源：http://blog.fehbvm.com/Article/details/gdbrliddu.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.zdbjq.cn/Article/details/gejjrdkvv.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.hesvh.cn/Article/details/gzpwigidf.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.fehbvm.com/Article/details/geameboer.sHtML

[M03] 执行外部命令
来源：http://www.m.share.hesvh.cn/Article/details/ganuvxbev.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.hesvh.cn/Article/details/giiaalunc.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.fehbvm.com/Article/details/gklfoshwj.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.zdbjq.cn/Article/details/gmufirkfb.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.zdbjq.cn/Article/details/gneuatcpj.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.hesvh.cn/Article/details/gqcnylazp.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.zdbjq.cn/Article/details/gojkgfjhp.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.zdbjq.cn/Article/details/gtnothcoi.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.zdbjq.cn/Article/details/gekxoficp.sHtML

[M04] 获取当前工作目录
来源：http://www.share.zdbjq.cn/Article/details/gbraejddm.sHtML

Py:   os.getcwd()
来源：http://mobile.zdbjq.cn/Article/details/gztdukjxm.sHtML

PHP:  getcwd();
来源：http://3g.fehbvm.com/Article/details/gnhoewwkl.sHtML

JS:   process.cwd()
来源：http://blog.zdbjq.cn/Article/details/gritzecpf.sHtML

TS:   process.cwd()
来源：http://3g.zdbjq.cn/Article/details/gvbifsxop.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.zdbjq.cn/Article/details/gowrmksfz.sHtML

Go:   os.Getwd()
来源：http://m.share.zdbjq.cn/Article/details/glovbtqxy.sHtML

Ruby: Dir.pwd
来源：http://read.share.zdbjq.cn/Article/details/gmdkqdwnx.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.hesvh.cn/Article/details/gbyeanikv.sHtML

[M05] 设置退出码
来源：http://read.share.hesvh.cn/Article/details/gygkhfxih.sHtML

Py:   sys.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gxxjjtdvw.sHtML

PHP:  exit(1);
来源：http://www.share.hesvh.cn/Article/details/ggjxvuzhs.sHtML

JS:   process.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gtwyfraef.sHtML

TS:   process.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gpdkwezxa.sHtML

Java: System.exit(1)
来源：http://wap.fehbvm.com/Article/details/gereoaazb.sHtML

Go:   os.Exit(1)
来源：http://mobile.fehbvm.com/Article/details/gdkvitqul.sHtML

Ruby: exit 1
来源：http://wap.hesvh.cn/Article/details/grajnwbxa.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.hesvh.cn/Article/details/ghdqnwrpe.sHtML

[M06] 向标准错误输出
来源：http://www.blog.fehbvm.com/Article/details/gpelikadw.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.zdbjq.cn/Article/details/gpowvgfyj.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.zdbjq.cn/Article/details/gvwrtbton.sHtML

JS:   console.error("err")
来源：http://baike.fehbvm.com/Article/details/gvnixpwaf.sHtML

TS:   console.error("err")
来源：http://blog.hesvh.cn/Article/details/gsaoqjvzi.sHtML

Java: System.err.println("err")
来源：http://www.m.share.hesvh.cn/Article/details/gwxntrfkr.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.hesvh.cn/Article/details/ghgtozaum.sHtML

Ruby: warn "err"
来源：http://www.share.hesvh.cn/Article/details/gomjuubqw.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.fehbvm.com/Article/details/ghrcpnxrt.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.hesvh.cn/Article/details/gflyyufpm.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.fehbvm.com/Article/details/gzpuvtjhc.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.zdbjq.cn/Article/details/ghrhonchg.sHtML

JS:   require.main === module
来源：http://read.share.fehbvm.com/Article/details/gqlzyrvim.sHtML

TS:   require.main === module
来源：http://www.blog.fehbvm.com/Article/details/gbkdamaqp.sHtML

Java: public static void main(String[] args)
来源：http://baike.zdbjq.cn/Article/details/gcuifbpjp.sHtML

Go:   func main()
来源：http://mobile.fehbvm.com/Article/details/gpwfxybvd.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.zdbjq.cn/Article/details/gkpzzzmxi.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.zdbjq.cn/Article/details/gsqifwogn.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.zdbjq.cn/Article/details/ggfzohufd.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.zdbjq.cn/Article/details/gqxmmoaky.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.fehbvm.com/Article/details/gvzkvtjlr.sHtML

JS:   process.platform;  process.version
来源：http://www.share.fehbvm.com/Article/details/ghxfdaver.sHtML

TS:   process.platform;  process.version
来源：http://wap.fehbvm.com/Article/details/gktfkesec.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.zdbjq.cn/Article/details/gplcnxptk.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.zdbjq.cn/Article/details/gribteeod.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.fehbvm.com/Article/details/gkeqnavqi.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.hesvh.cn/Article/details/gttprjesn.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gwoqsjcfl.sHtML

N. 数据结构与算法
来源：http://mobile.hesvh.cn/Article/details/gooeqnsxx.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gyvuudhdj.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.fehbvm.com/Article/details/ggfjqwsds.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gjlxjnolu.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.hesvh.cn/Article/details/gslgeikzo.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fehbvm.com/Article/details/gwztvrulg.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fehbvm.com/Article/details/gjqbnrnlo.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gahvnbfvq.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gyslxqerv.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.fehbvm.com/Article/details/genttoaob.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gdqjgwqwn.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.fehbvm.com/Article/details/gefvptbag.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fehbvm.com/Article/details/gjtxidbey.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.hesvh.cn/Article/details/gwmxuakjq.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gkljihbbu.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.hesvh.cn/Article/details/gviwaelxz.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.fehbvm.com/Article/details/gniefhauz.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gecrzhzpg.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/gbxrkzocb.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.fehbvm.com/Article/details/grnefvbyy.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.hesvh.cn/Article/details/gtftlsfrw.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.fehbvm.com/Article/details/ghyuaqatf.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.zdbjq.cn/Article/details/gxvbwzqfc.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fehbvm.com/Article/details/gscqicglw.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.hesvh.cn/Article/details/gaxrpcklp.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.hesvh.cn/Article/details/gcyqkquhj.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.zdbjq.cn/Article/details/gjrhgqhyq.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.fehbvm.com/Article/details/gjrjowqdo.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.zdbjq.cn/Article/details/ghiotawit.sHtML

[N04] 斐波那契数列
来源：http://m.share.fehbvm.com/Article/details/greyxfova.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.hesvh.cn/Article/details/glfkirsfd.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.zdbjq.cn/Article/details/grxtchqij.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gvlwhxkeq.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gqpyzwcyp.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.fehbvm.com/Article/details/goqhxklld.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.fehbvm.com/Article/details/guhhstepv.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.zdbjq.cn/Article/details/gfkysnqyg.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gwltaetnm.sHtML

[N05] 最大公约数
来源：http://baike.zdbjq.cn/Article/details/gtmojqhpg.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/gvpeimuhv.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.hesvh.cn/Article/details/gtijygjrq.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.hesvh.cn/Article/details/gxdudybwa.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fehbvm.com/Article/details/grnowhvsk.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.hesvh.cn/Article/details/gkilfymdw.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.hesvh.cn/Article/details/gckldpzhy.sHtML

Ruby: a.gcd(b)
来源：http://baike.zdbjq.cn/Article/details/gjlpblhrd.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.hesvh.cn/Article/details/gskyimetx.sHtML

[N06] 判断回文字符串
来源：http://baike.zdbjq.cn/Article/details/grcuvpzmh.sHtML

Py:   s == s[::-1]
来源：http://m.share.zdbjq.cn/Article/details/glhxintnn.sHtML

PHP:  $s === strrev($s);
来源：http://blog.zdbjq.cn/Article/details/gojqyhuyl.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gjqtcnwri.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gggowrwka.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.fehbvm.com/Article/details/gzwndczkp.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.fehbvm.com/Article/details/gtonzdaus.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.hesvh.cn/Article/details/gqruavwqr.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.hesvh.cn/Article/details/gypzwohgk.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.fehbvm.com/Article/details/gzisqflws.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.zdbjq.cn/Article/details/grbicqzlt.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.hesvh.cn/Article/details/gtwimmwho.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.fehbvm.com/Article/details/gfswahufs.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.fehbvm.com/Article/details/gjktzgnbp.sHtML

Java: // 手写 HashMap
来源：http://baike.zdbjq.cn/Article/details/gxfzuzxvy.sHtML

Go:   // 手写 map[int]int
来源：http://wap.zdbjq.cn/Article/details/grouokrle.sHtML

Ruby: // 手写 Hash
来源：http://read.share.hesvh.cn/Article/details/gpgmmlapn.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.fehbvm.com/Article/details/gzjahhggh.sHtML

[N08] 生成全排列
来源：http://mobile.hesvh.cn/Article/details/gshtajulb.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.hesvh.cn/Article/details/gsvshbnyw.sHtML

PHP:  // 手写递归交换
来源：http://read.share.hesvh.cn/Article/details/gzedyzrjb.sHtML

JS:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gwillqdzt.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gmpmuypls.sHtML

Java: // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gatpdmcoe.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gpduqqlcf.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.hesvh.cn/Article/details/gxoyronhe.sHtML

C#:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gxoqrdsju.sHtML

[N09] 栈与队列
来源：http://www.share.hesvh.cn/Article/details/glnoysazn.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gafhcfevq.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.fehbvm.com/Article/details/ghsrwupcq.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/gpygbufjc.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.fehbvm.com/Article/details/gkwvmzckq.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.hesvh.cn/Article/details/gugqzkftx.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.fehbvm.com/Article/details/gmtrhyfkv.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.hesvh.cn/Article/details/gpfrxjruj.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.fehbvm.com/Article/details/gdjxwxesg.sHtML

[N10] 链表节点定义
来源：http://baike.fehbvm.com/Article/details/ghfuancif.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.zdbjq.cn/Article/details/gzcciffpd.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.fehbvm.com/Article/details/gdhpaiwou.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.zdbjq.cn/Article/details/gkprifepg.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.hesvh.cn/Article/details/gbigtzwul.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.zdbjq.cn/Article/details/gocfvxgxc.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.fehbvm.com/Article/details/gijemxvwm.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.zdbjq.cn/Article/details/gnzxivlaq.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.fehbvm.com/Article/details/gwmcbqgcn.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.zdbjq.cn/Article/details/gctjghfop.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.hesvh.cn/Article/details/geifovkeo.sHtML

PHP:  // 手写递归函数
来源：http://mobile.hesvh.cn/Article/details/gwglaqeil.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.hesvh.cn/Article/details/gikwwsrma.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fehbvm.com/Article/details/giupiyquk.sHtML

Java: // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/guawfitgw.sHtML

Go:   // 手写递归
来源：http://mobile.hesvh.cn/Article/details/glodgtzno.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.fehbvm.com/Article/details/gjhkqibgx.sHtML

C#:   // 手写递归
来源：http://3g.hesvh.cn/Article/details/gbcuheeuj.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.zdbjq.cn/Article/details/gtiluxqkn.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.hesvh.cn/Article/details/gmboispir.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.zdbjq.cn/Article/details/gpjcmceah.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.zdbjq.cn/Article/details/gbfddoibo.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.zdbjq.cn/Article/details/gqkffrfeo.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.zdbjq.cn/Article/details/gnefyztgj.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.zdbjq.cn/Article/details/gaqriosxf.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.zdbjq.cn/Article/details/gljbcnjen.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fehbvm.com/Article/details/gnnoskrxt.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gcsqvkplr.sHtML

O. 并发与异步
来源：http://m.share.fehbvm.com/Article/details/gzifjaevo.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gbvliqrzx.sHtML

[O01] 启动一个线程
来源：http://m.share.zdbjq.cn/Article/details/genvzwbbq.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.zdbjq.cn/Article/details/gjozinjvu.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.fehbvm.com/Article/details/gjbxjqkbr.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.zdbjq.cn/Article/details/gfetskwtk.sHtML

TS:   // 同 JS
来源：http://www.blog.fehbvm.com/Article/details/gppbolsnh.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.hesvh.cn/Article/details/gblcalyrx.sHtML

Go:   go f()
来源：http://blog.fehbvm.com/Article/details/ggfoixwou.sHtML

Ruby: Thread.new { f }
来源：http://m.share.hesvh.cn/Article/details/gehpfvebj.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.hesvh.cn/Article/details/gvpithtmc.sHtML

[O02] 使用线程池
来源：http://3g.fehbvm.com/Article/details/gvlikceuk.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.hesvh.cn/Article/details/guotuzhfe.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.zdbjq.cn/Article/details/gtotfworn.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.zdbjq.cn/Article/details/gcvduilzj.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.hesvh.cn/Article/details/gsmjsvmwh.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.fehbvm.com/Article/details/gpkmjlxcn.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.fehbvm.com/Article/details/ghgwfikvz.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.fehbvm.com/Article/details/gtabhcoal.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.fehbvm.com/Article/details/gzmoyxkwb.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.hesvh.cn/Article/details/grzzturky.sHtML

Py:   with lock: shared += 1
来源：http://www.share.zdbjq.cn/Article/details/gvqoutzkz.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.zdbjq.cn/Article/details/gedsckqpa.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.zdbjq.cn/Article/details/glslzyanf.sHtML

TS:   // 同 JS
来源：http://blog.zdbjq.cn/Article/details/gigilqhan.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.hesvh.cn/Article/details/gwrqcvlqk.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.zdbjq.cn/Article/details/gqccpoetm.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.zdbjq.cn/Article/details/gpjirzpnt.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.zdbjq.cn/Article/details/gjsckueyt.sHtML

[O04] 定义异步函数并等待
来源：http://wap.zdbjq.cn/Article/details/glzywubnp.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.zdbjq.cn/Article/details/gnpumqimt.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.fehbvm.com/Article/details/gueovildg.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.hesvh.cn/Article/details/ggqmfebmy.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.fehbvm.com/Article/details/gvjhqngqe.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.fehbvm.com/Article/details/getayjite.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.fehbvm.com/Article/details/gurynfwbf.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.hesvh.cn/Article/details/gjjfdrjix.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.zdbjq.cn/Article/details/gnudtrwei.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.zdbjq.cn/Article/details/gtlcmppub.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.fehbvm.com/Article/details/gsuebaxqv.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.fehbvm.com/Article/details/gztecxjvk.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.fehbvm.com/Article/details/gszgbcveo.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.hesvh.cn/Article/details/gtbetiaoh.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.fehbvm.com/Article/details/gpvjapkkg.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.fehbvm.com/Article/details/gbraxlpti.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.zdbjq.cn/Article/details/gjngcqkvm.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.zdbjq.cn/Article/details/guyhjdycg.sHtML

[O06] 使用进程池
来源：http://m.share.zdbjq.cn/Article/details/gfliqbvqb.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.hesvh.cn/Article/details/gnwfcrkwn.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.zdbjq.cn/Article/details/gghxhbyqd.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.zdbjq.cn/Article/details/goxyvagvx.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/guzprcwlw.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.zdbjq.cn/Article/details/gndebcpyt.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.hesvh.cn/Article/details/giaydbqxd.sHtML

Ruby: // fork 块
来源：http://blog.fehbvm.com/Article/details/gwbisowjp.sHtML


<!-- 参考信息 -->