代发 wailian999

Py:   requests.post(url, json={"a": 1})
来源：http://baike.fehbvm.com/Article/details/gtdzfoqva.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.zdbjq.cn/Article/details/grtirtudi.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.hesvh.cn/Article/details/gvtuxqvju.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.hesvh.cn/Article/details/gmpoailqj.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.zdbjq.cn/Article/details/gdgcschkx.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.fehbvm.com/Article/details/gbdcltwsj.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.zdbjq.cn/Article/details/gsdelewvo.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.zdbjq.cn/Article/details/gwicsyxun.sHtML

[L03] 设置自定义请求头
来源：http://mobile.hesvh.cn/Article/details/goqgzgqsh.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.hesvh.cn/Article/details/gjmxqflag.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.zdbjq.cn/Article/details/grvptnbtc.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.fehbvm.com/Article/details/ghblceicq.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.hesvh.cn/Article/details/gzzecgkrd.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.hesvh.cn/Article/details/gdwirngrk.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.hesvh.cn/Article/details/gxujhjbhj.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.zdbjq.cn/Article/details/gjgimuznl.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.fehbvm.com/Article/details/gqjdoymnm.sHtML

[L04] 设置超时
来源：http://read.share.fehbvm.com/Article/details/gjpexuqlz.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.hesvh.cn/Article/details/gmotbtptl.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.fehbvm.com/Article/details/gfbvnhest.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.zdbjq.cn/Article/details/gtgwwzfmc.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.hesvh.cn/Article/details/gejiobdcq.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.zdbjq.cn/Article/details/gppiaimeb.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.zdbjq.cn/Article/details/gbnahvhug.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.zdbjq.cn/Article/details/gzfqrgxik.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.fehbvm.com/Article/details/gxwihwxch.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.hesvh.cn/Article/details/gklraapdv.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.fehbvm.com/Article/details/gzxouhsuq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.hesvh.cn/Article/details/gcmuwrkuc.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.hesvh.cn/Article/details/gbwsncdzy.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.zdbjq.cn/Article/details/gmjefmaah.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.zdbjq.cn/Article/details/gskcwefxy.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.hesvh.cn/Article/details/gzuhkylkl.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.hesvh.cn/Article/details/gfeoqfwpl.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.zdbjq.cn/Article/details/gwqutgptl.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.fehbvm.com/Article/details/gioswpspo.sHtML

Py:   resp.json()
来源：http://wap.fehbvm.com/Article/details/ghmrszhss.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.fehbvm.com/Article/details/gmoolrhmr.sHtML

JS:   await resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/gotwdwzhc.sHtML

TS:   await resp.json()
来源：http://baike.zdbjq.cn/Article/details/gdzutdgkf.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.fehbvm.com/Article/details/gvoecgxes.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.zdbjq.cn/Article/details/glzismdam.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.hesvh.cn/Article/details/gllcpugha.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.fehbvm.com/Article/details/gqzxkfzyd.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.fehbvm.com/Article/details/gxffbbesi.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.zdbjq.cn/Article/details/gswvghzvf.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.fehbvm.com/Article/details/gaubisgkg.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.fehbvm.com/Article/details/gdsmmmbhl.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.hesvh.cn/Article/details/gmqetocsl.sHtML

Java: resp.statusCode()
来源：http://baike.fehbvm.com/Article/details/geolxzxnd.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.fehbvm.com/Article/details/gevzlvxqu.sHtML

Ruby: resp.code.to_i
来源：http://blog.fehbvm.com/Article/details/gzqbefefz.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.zdbjq.cn/Article/details/gxdvhwipp.sHtML

[L08] 并发请求多个地址
来源：http://blog.fehbvm.com/Article/details/gtclrmric.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.hesvh.cn/Article/details/gnylwfmdb.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.zdbjq.cn/Article/details/gcnyqxrro.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/gyrloerev.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.zdbjq.cn/Article/details/glcztyzbq.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.fehbvm.com/Article/details/gekhyruay.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.fehbvm.com/Article/details/gaogtyfyy.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.fehbvm.com/Article/details/gtvriuztz.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.hesvh.cn/Article/details/gjzvsncek.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gqyyaxkpl.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.hesvh.cn/Article/details/gyoykolnp.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/grqicdplp.sHtML

[M01] 读取命令行参数
来源：http://wap.fehbvm.com/Article/details/gsugoiion.sHtML

Py:   sys.argv[1:]
来源：http://www.share.hesvh.cn/Article/details/girftjwjd.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.zdbjq.cn/Article/details/gywjsvmnd.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.hesvh.cn/Article/details/gmgefeowd.sHtML

TS:   process.argv.slice(2)
来源：http://wap.zdbjq.cn/Article/details/gveqhivlq.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.zdbjq.cn/Article/details/gzmgoccqh.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.fehbvm.com/Article/details/gyuejjkdo.sHtML

Ruby: ARGV
来源：http://www.share.zdbjq.cn/Article/details/gzyjoccua.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.zdbjq.cn/Article/details/gaevdytic.sHtML

[M02] 读取环境变量
来源：http://baike.zdbjq.cn/Article/details/gaxzoopqe.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.zdbjq.cn/Article/details/goeahphfi.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.fehbvm.com/Article/details/gmunscdwn.sHtML

JS:   process.env.HOME
来源：http://m.share.hesvh.cn/Article/details/gqctxeyfn.sHtML

TS:   process.env.HOME
来源：http://3g.zdbjq.cn/Article/details/grbjzilnp.sHtML

Java: System.getenv("HOME")
来源：http://www.share.hesvh.cn/Article/details/gkncqhotq.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gwzkrhhkm.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.hesvh.cn/Article/details/gpsilkpxq.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.hesvh.cn/Article/details/gruvbqrco.sHtML

[M03] 执行外部命令
来源：http://mobile.fehbvm.com/Article/details/gafwooiqt.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gmtqfgidc.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.fehbvm.com/Article/details/ghyzypzba.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fehbvm.com/Article/details/gcqbctanl.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fehbvm.com/Article/details/gdzcsbxod.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.zdbjq.cn/Article/details/gwftmbuaq.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.fehbvm.com/Article/details/gkgdspffr.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.zdbjq.cn/Article/details/glteuapng.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.fehbvm.com/Article/details/gnvfyiatu.sHtML

[M04] 获取当前工作目录
来源：http://3g.zdbjq.cn/Article/details/gbsejbhme.sHtML

Py:   os.getcwd()
来源：http://www.m.share.hesvh.cn/Article/details/gkbajgxpc.sHtML

PHP:  getcwd();
来源：http://read.share.fehbvm.com/Article/details/gsbafulqn.sHtML

JS:   process.cwd()
来源：http://baike.zdbjq.cn/Article/details/giwqrrndr.sHtML

TS:   process.cwd()
来源：http://baike.hesvh.cn/Article/details/gvbqrclam.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.zdbjq.cn/Article/details/gnyzwepac.sHtML

Go:   os.Getwd()
来源：http://3g.hesvh.cn/Article/details/gqtyyatyu.sHtML

Ruby: Dir.pwd
来源：http://blog.hesvh.cn/Article/details/gyfkbyrqh.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.hesvh.cn/Article/details/gkgnbjkrs.sHtML

[M05] 设置退出码
来源：http://baike.hesvh.cn/Article/details/gxghmymzy.sHtML

Py:   sys.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gltscjwix.sHtML

PHP:  exit(1);
来源：http://www.m.share.zdbjq.cn/Article/details/gczfuzyds.sHtML

JS:   process.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gqzwdtjme.sHtML

TS:   process.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gkqtdgsmr.sHtML

Java: System.exit(1)
来源：http://blog.fehbvm.com/Article/details/gafruwkzb.sHtML

Go:   os.Exit(1)
来源：http://www.blog.hesvh.cn/Article/details/glvktdpqs.sHtML

Ruby: exit 1
来源：http://m.share.hesvh.cn/Article/details/gtpammttw.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.hesvh.cn/Article/details/gmqdirsqf.sHtML

[M06] 向标准错误输出
来源：http://baike.fehbvm.com/Article/details/gihpchybw.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.hesvh.cn/Article/details/gcsukhibf.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.hesvh.cn/Article/details/gsxpqzglr.sHtML

JS:   console.error("err")
来源：http://www.blog.zdbjq.cn/Article/details/gxcdahxtk.sHtML

TS:   console.error("err")
来源：http://wap.fehbvm.com/Article/details/gfaoryzru.sHtML

Java: System.err.println("err")
来源：http://wap.zdbjq.cn/Article/details/gdcsfwxrm.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.zdbjq.cn/Article/details/gllnowgji.sHtML

Ruby: warn "err"
来源：http://blog.fehbvm.com/Article/details/gbgcbjczh.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.fehbvm.com/Article/details/gweempnym.sHtML

[M07] 判断是否为主入口
来源：http://read.share.zdbjq.cn/Article/details/ghsragbin.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.fehbvm.com/Article/details/gqzghbcos.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.zdbjq.cn/Article/details/gwteunbae.sHtML

JS:   require.main === module
来源：http://wap.fehbvm.com/Article/details/gzqsacqea.sHtML

TS:   require.main === module
来源：http://blog.zdbjq.cn/Article/details/gqgpuwasg.sHtML

Java: public static void main(String[] args)
来源：http://blog.zdbjq.cn/Article/details/gmnkionce.sHtML

Go:   func main()
来源：http://mobile.fehbvm.com/Article/details/gveozdhqe.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.zdbjq.cn/Article/details/gcsrklnkd.sHtML

C#:   static void Main(string[] args)
来源：http://blog.hesvh.cn/Article/details/gvmsrudzf.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.hesvh.cn/Article/details/grcpfooic.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.hesvh.cn/Article/details/gubyribgo.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.fehbvm.com/Article/details/gellgffcy.sHtML

JS:   process.platform;  process.version
来源：http://m.share.fehbvm.com/Article/details/geqcfwneo.sHtML

TS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/gqyymeslq.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.zdbjq.cn/Article/details/guwsrnrtt.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.hesvh.cn/Article/details/gexbzthfh.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.fehbvm.com/Article/details/gsfntxbum.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.zdbjq.cn/Article/details/gcbbqjshm.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gdhlcfecb.sHtML

N. 数据结构与算法
来源：http://read.share.fehbvm.com/Article/details/gyexpkpej.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/giwrvujbz.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.zdbjq.cn/Article/details/gsatzciqq.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gzvhuxwfm.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.zdbjq.cn/Article/details/gffndftpk.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gwdyncere.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fehbvm.com/Article/details/ghqvnsfeg.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gbytywije.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gsbbnsvup.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.hesvh.cn/Article/details/gauxdxllp.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gqxcrpbzx.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.hesvh.cn/Article/details/gxvbfilix.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.hesvh.cn/Article/details/gtrznxrbb.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.zdbjq.cn/Article/details/gkjdihcwz.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/gdcfndifw.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/gmsgpnldo.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.hesvh.cn/Article/details/gcixqqjjd.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.fehbvm.com/Article/details/gbojedfyb.sHtML

Ruby: arr.sort
来源：http://mobile.hesvh.cn/Article/details/gowlgrbrm.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.fehbvm.com/Article/details/gymwvqffi.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.zdbjq.cn/Article/details/guvonpyno.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.zdbjq.cn/Article/details/gwololruf.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.fehbvm.com/Article/details/gmwwnrmxo.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fehbvm.com/Article/details/gmmomiyof.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.hesvh.cn/Article/details/gmiwfuojd.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.fehbvm.com/Article/details/gtqittehx.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.hesvh.cn/Article/details/gokbewwnl.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.hesvh.cn/Article/details/gqeweckba.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.zdbjq.cn/Article/details/gnbcfnarn.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.hesvh.cn/Article/details/gattyurff.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.fehbvm.com/Article/details/gtfmhyrkt.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.hesvh.cn/Article/details/gkityhgmo.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gdnxvzhzr.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/gkfpspcyl.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.hesvh.cn/Article/details/gqzlfbqzh.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.zdbjq.cn/Article/details/gqlzfjdau.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/gzbxjhnpf.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/gdlgbxjpe.sHtML

[N05] 最大公约数
来源：http://3g.zdbjq.cn/Article/details/gpdjjqdia.sHtML

Py:   math.gcd(a, b)
来源：http://blog.zdbjq.cn/Article/details/gwgqqlflc.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.zdbjq.cn/Article/details/gvhequobt.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fehbvm.com/Article/details/grgkunygo.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fehbvm.com/Article/details/gyaxevaor.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.fehbvm.com/Article/details/gvqsjommf.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.zdbjq.cn/Article/details/glcrdfigr.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.fehbvm.com/Article/details/gpyxfcusa.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.zdbjq.cn/Article/details/ghmwehgxo.sHtML

[N06] 判断回文字符串
来源：http://blog.fehbvm.com/Article/details/gqxmvjroq.sHtML

Py:   s == s[::-1]
来源：http://read.share.hesvh.cn/Article/details/ghyfensuw.sHtML

PHP:  $s === strrev($s);
来源：http://blog.zdbjq.cn/Article/details/gnilyxbzw.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gnmgvmrfl.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/ggjlqnfqg.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.zdbjq.cn/Article/details/gytjibsak.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.zdbjq.cn/Article/details/gbdtlptik.sHtML

Ruby: s == s.reverse
来源：http://mobile.fehbvm.com/Article/details/ghihbwhed.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.zdbjq.cn/Article/details/gikwojepx.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.fehbvm.com/Article/details/gzxzjkawe.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.zdbjq.cn/Article/details/gcmcxgyrr.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.hesvh.cn/Article/details/gioorjhvx.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.zdbjq.cn/Article/details/gfzcezozg.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.fehbvm.com/Article/details/gcviwkinv.sHtML

Java: // 手写 HashMap
来源：http://3g.hesvh.cn/Article/details/gkfphogxw.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.hesvh.cn/Article/details/gfriaxqnk.sHtML

Ruby: // 手写 Hash
来源：http://3g.fehbvm.com/Article/details/ggvjkndqe.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.hesvh.cn/Article/details/gaarmclyp.sHtML

[N08] 生成全排列
来源：http://www.m.share.hesvh.cn/Article/details/gutjytfsk.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.zdbjq.cn/Article/details/gvolmhqnp.sHtML

PHP:  // 手写递归交换
来源：http://read.share.zdbjq.cn/Article/details/glgwrowah.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gbvviyzyd.sHtML

TS:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gqzfqiabr.sHtML

Java: // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gwevnbedn.sHtML

Go:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gumtoagbw.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.zdbjq.cn/Article/details/ggmjashlv.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gsnfgjhwn.sHtML

[N09] 栈与队列
来源：http://m.share.hesvh.cn/Article/details/gjaufukdh.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.fehbvm.com/Article/details/gjexznker.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.fehbvm.com/Article/details/grlszeema.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/gbyhlwmpn.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.zdbjq.cn/Article/details/gquosqmsr.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.hesvh.cn/Article/details/guxguwlnf.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.zdbjq.cn/Article/details/gjqddddpa.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gojbpribk.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.fehbvm.com/Article/details/gbethzbni.sHtML

[N10] 链表节点定义
来源：http://blog.fehbvm.com/Article/details/guvqsqdfq.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.hesvh.cn/Article/details/gzwzoxcte.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.fehbvm.com/Article/details/gepdmmqol.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.zdbjq.cn/Article/details/gssowxdhr.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.zdbjq.cn/Article/details/gslhoqehh.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.fehbvm.com/Article/details/gmcowyxsy.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.zdbjq.cn/Article/details/ghfdbtmxp.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.fehbvm.com/Article/details/gnfvsczyt.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.fehbvm.com/Article/details/grgzojlas.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.hesvh.cn/Article/details/gwakflrtx.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.zdbjq.cn/Article/details/grveulmnm.sHtML

PHP:  // 手写递归函数
来源：http://baike.zdbjq.cn/Article/details/gjgiuabeb.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.hesvh.cn/Article/details/gyvcnjwdr.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.zdbjq.cn/Article/details/gnwibnqby.sHtML

Java: // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gylllevvm.sHtML

Go:   // 手写递归
来源：http://baike.fehbvm.com/Article/details/gickruogi.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.zdbjq.cn/Article/details/gioqgtryz.sHtML

C#:   // 手写递归
来源：http://blog.hesvh.cn/Article/details/gumoanuyh.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.hesvh.cn/Article/details/gsfemjenw.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.hesvh.cn/Article/details/gpgdtnsvq.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.hesvh.cn/Article/details/gzsceumts.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.hesvh.cn/Article/details/gymedcpgx.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.hesvh.cn/Article/details/gmcmzwpoh.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.hesvh.cn/Article/details/gxlpurbuc.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.fehbvm.com/Article/details/gugpuiaqs.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.fehbvm.com/Article/details/gnrljgikb.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.zdbjq.cn/Article/details/gptmzudxw.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gopcbglct.sHtML

O. 并发与异步
来源：http://wap.fehbvm.com/Article/details/gbebtszqj.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gyrqzvfon.sHtML

[O01] 启动一个线程
来源：http://read.share.fehbvm.com/Article/details/gwnqnyzbm.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.fehbvm.com/Article/details/ggfnbvxqc.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.fehbvm.com/Article/details/geajeqrhc.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.zdbjq.cn/Article/details/gyarqdbsi.sHtML

TS:   // 同 JS
来源：http://baike.hesvh.cn/Article/details/gevpcfyvy.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.hesvh.cn/Article/details/gthquehqt.sHtML

Go:   go f()
来源：http://www.m.share.fehbvm.com/Article/details/grygbmthe.sHtML

Ruby: Thread.new { f }
来源：http://blog.fehbvm.com/Article/details/geqygtrnf.sHtML

C#:   Task.Run(() => F());
来源：http://wap.zdbjq.cn/Article/details/gkqskqtrw.sHtML

[O02] 使用线程池
来源：http://www.share.hesvh.cn/Article/details/ghrknmmwl.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.hesvh.cn/Article/details/gwgoebsem.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.zdbjq.cn/Article/details/geljmwozu.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.hesvh.cn/Article/details/gijtuwfqp.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.zdbjq.cn/Article/details/gtewqfdvn.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.fehbvm.com/Article/details/gihfdvbpn.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.zdbjq.cn/Article/details/gfuisdwpx.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.zdbjq.cn/Article/details/gbbzuqyxq.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.zdbjq.cn/Article/details/gglfliwrc.sHtML

[O03] 加锁保护共享数据
来源：http://blog.hesvh.cn/Article/details/gbwtpxcqg.sHtML

Py:   with lock: shared += 1
来源：http://baike.hesvh.cn/Article/details/gxvubswjo.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.hesvh.cn/Article/details/gkmguxlkv.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.fehbvm.com/Article/details/gmdjddpdv.sHtML

TS:   // 同 JS
来源：http://wap.fehbvm.com/Article/details/gqxvhcdjf.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.zdbjq.cn/Article/details/gwqwhwjug.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.hesvh.cn/Article/details/ghclkvbef.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.zdbjq.cn/Article/details/glmomtvet.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.fehbvm.com/Article/details/gwiayxtvs.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.zdbjq.cn/Article/details/gycjinzkn.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.hesvh.cn/Article/details/gadlptrup.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.zdbjq.cn/Article/details/gyxxczvoo.sHtML

JS:   async function f() { await g(); }
来源：http://3g.fehbvm.com/Article/details/gnymoveyl.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.fehbvm.com/Article/details/gxzayciqj.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.hesvh.cn/Article/details/gtjjogbsh.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.zdbjq.cn/Article/details/gmrookxxh.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.zdbjq.cn/Article/details/ggnoshavm.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.hesvh.cn/Article/details/gnmszjvvn.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.zdbjq.cn/Article/details/gbhhmmzaz.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.fehbvm.com/Article/details/gxrjnycmb.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.fehbvm.com/Article/details/ggmsdiwvn.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.fehbvm.com/Article/details/ggjqwvzkk.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.fehbvm.com/Article/details/gdjygpddx.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.fehbvm.com/Article/details/gncaewveb.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.fehbvm.com/Article/details/gomjjutiy.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.hesvh.cn/Article/details/gikjhicjg.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.zdbjq.cn/Article/details/gwnixoett.sHtML

[O06] 使用进程池
来源：http://mobile.fehbvm.com/Article/details/gbxwkpjcl.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.hesvh.cn/Article/details/gusvembnb.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.fehbvm.com/Article/details/gpnjeupai.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.zdbjq.cn/Article/details/glrcwayrj.sHtML


<!-- 参考信息 -->