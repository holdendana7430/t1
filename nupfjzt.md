代发 wailian999

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.fehbvm.com/Article/details/gsmyrgifc.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.hesvh.cn/Article/details/gphtzjvia.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.fehbvm.com/Article/details/gmyczpgkd.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.hesvh.cn/Article/details/gmamfeaxr.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.zdbjq.cn/Article/details/gpgvzdkll.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.fehbvm.com/Article/details/gddcrljyc.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.zdbjq.cn/Article/details/gpargfpns.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.fehbvm.com/Article/details/gscxmohes.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.fehbvm.com/Article/details/gxgqzqolu.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.zdbjq.cn/Article/details/gzuwojsmn.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.fehbvm.com/Article/details/gotikdkpv.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.fehbvm.com/Article/details/gkviyxros.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.zdbjq.cn/Article/details/gquwryqhv.sHtML

[L04] 设置超时
来源：http://baike.fehbvm.com/Article/details/gqbydwqjr.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.hesvh.cn/Article/details/gribqtgcs.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.fehbvm.com/Article/details/gtdwjoxll.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.fehbvm.com/Article/details/gdznzmpsx.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.zdbjq.cn/Article/details/gwkckpqpn.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.fehbvm.com/Article/details/gyqwowomm.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.zdbjq.cn/Article/details/gxkomeibo.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.fehbvm.com/Article/details/gbwkcmrjx.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.fehbvm.com/Article/details/gtuitxwgv.sHtML

[L05] 上传文件（multipart）
来源：http://baike.hesvh.cn/Article/details/gtebcebdg.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.zdbjq.cn/Article/details/glhqjfrps.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.fehbvm.com/Article/details/grauzhrms.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.fehbvm.com/Article/details/gqpqnvbzv.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.hesvh.cn/Article/details/gtecqljnp.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.zdbjq.cn/Article/details/gxxpgrils.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.zdbjq.cn/Article/details/gyekcmapb.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.hesvh.cn/Article/details/gvimwivzp.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.zdbjq.cn/Article/details/guqzgwyih.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.fehbvm.com/Article/details/gxexbabui.sHtML

Py:   resp.json()
来源：http://baike.zdbjq.cn/Article/details/gqxtnyiwz.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.zdbjq.cn/Article/details/gersmcxck.sHtML

JS:   await resp.json()
来源：http://read.share.fehbvm.com/Article/details/gekfwjkio.sHtML

TS:   await resp.json()
来源：http://baike.hesvh.cn/Article/details/gszipbwpe.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.fehbvm.com/Article/details/gxajqjbqi.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.hesvh.cn/Article/details/geiahclpb.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.zdbjq.cn/Article/details/gbunfpgyl.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.zdbjq.cn/Article/details/golwnfbos.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.fehbvm.com/Article/details/gcvojvmdz.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.hesvh.cn/Article/details/gtiwgyehd.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.hesvh.cn/Article/details/glixfizzs.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.fehbvm.com/Article/details/gfczymene.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.fehbvm.com/Article/details/gdavnvkib.sHtML

Java: resp.statusCode()
来源：http://wap.hesvh.cn/Article/details/gtcntifch.sHtML

Go:   resp.StatusCode
来源：http://3g.fehbvm.com/Article/details/glwdquygz.sHtML

Ruby: resp.code.to_i
来源：http://3g.zdbjq.cn/Article/details/grfrdziob.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.hesvh.cn/Article/details/gjtsklxeo.sHtML

[L08] 并发请求多个地址
来源：http://read.share.zdbjq.cn/Article/details/gtsuxgpga.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.hesvh.cn/Article/details/gclpglckt.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.hesvh.cn/Article/details/gdylreyrz.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gbjbhbeze.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/gqvprjnxk.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.hesvh.cn/Article/details/gjgtraaqq.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.hesvh.cn/Article/details/gcmahmvnx.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.fehbvm.com/Article/details/ghhmxbwet.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.zdbjq.cn/Article/details/gtyhbrgwb.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gvkquhbpf.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.hesvh.cn/Article/details/gmwqdicht.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ghbvnqzao.sHtML

[M01] 读取命令行参数
来源：http://read.share.zdbjq.cn/Article/details/grpdeyvqv.sHtML

Py:   sys.argv[1:]
来源：http://wap.hesvh.cn/Article/details/gqbvzjifg.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.zdbjq.cn/Article/details/gipercrfs.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.fehbvm.com/Article/details/gfagbnfao.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.hesvh.cn/Article/details/gxmymqipm.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.hesvh.cn/Article/details/gfnvmnbtz.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.fehbvm.com/Article/details/gelykwpyk.sHtML

Ruby: ARGV
来源：http://read.share.hesvh.cn/Article/details/gzrnbfotn.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.fehbvm.com/Article/details/gqhsyqtpu.sHtML

[M02] 读取环境变量
来源：http://mobile.fehbvm.com/Article/details/gaanqmbvz.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.zdbjq.cn/Article/details/gewcgqbfk.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.hesvh.cn/Article/details/gappaucqz.sHtML

JS:   process.env.HOME
来源：http://www.share.fehbvm.com/Article/details/gsptaiwup.sHtML

TS:   process.env.HOME
来源：http://baike.fehbvm.com/Article/details/gjxdhbroh.sHtML

Java: System.getenv("HOME")
来源：http://www.share.hesvh.cn/Article/details/gsbrhrbar.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gsqydrhnt.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.fehbvm.com/Article/details/gifqbmseb.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gjbhkspxn.sHtML

[M03] 执行外部命令
来源：http://3g.hesvh.cn/Article/details/gltguegdi.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.fehbvm.com/Article/details/guchbszpd.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.hesvh.cn/Article/details/gwnewypoe.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.zdbjq.cn/Article/details/grnrpkhpp.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.hesvh.cn/Article/details/gcxocziiw.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.hesvh.cn/Article/details/gkdsbwzij.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.zdbjq.cn/Article/details/gajbfmvoi.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.zdbjq.cn/Article/details/gtakyfqxf.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.zdbjq.cn/Article/details/gaigskkeg.sHtML

[M04] 获取当前工作目录
来源：http://blog.zdbjq.cn/Article/details/gvhxmvqfl.sHtML

Py:   os.getcwd()
来源：http://www.share.zdbjq.cn/Article/details/ghoupxpba.sHtML

PHP:  getcwd();
来源：http://www.m.share.hesvh.cn/Article/details/ggkhghtfa.sHtML

JS:   process.cwd()
来源：http://3g.fehbvm.com/Article/details/gghsnoxzv.sHtML

TS:   process.cwd()
来源：http://read.share.zdbjq.cn/Article/details/ghxewoqhg.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.zdbjq.cn/Article/details/gkjuhnbje.sHtML

Go:   os.Getwd()
来源：http://m.share.hesvh.cn/Article/details/ghziydeau.sHtML

Ruby: Dir.pwd
来源：http://blog.hesvh.cn/Article/details/ggguhywvy.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.zdbjq.cn/Article/details/gwruiqduq.sHtML

[M05] 设置退出码
来源：http://blog.zdbjq.cn/Article/details/gvqqkvthm.sHtML

Py:   sys.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gebvjbijm.sHtML

PHP:  exit(1);
来源：http://m.share.hesvh.cn/Article/details/gaswmtppy.sHtML

JS:   process.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gimqexzsl.sHtML

TS:   process.exit(1)
来源：http://3g.fehbvm.com/Article/details/gqmeewxfu.sHtML

Java: System.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gkqvtgcag.sHtML

Go:   os.Exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gigjslpcl.sHtML

Ruby: exit 1
来源：http://www.share.hesvh.cn/Article/details/ghibzyfuy.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.fehbvm.com/Article/details/gvxaltywg.sHtML

[M06] 向标准错误输出
来源：http://mobile.hesvh.cn/Article/details/gpqvftfdx.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.fehbvm.com/Article/details/gswbipkhi.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.fehbvm.com/Article/details/grqqhiprb.sHtML

JS:   console.error("err")
来源：http://wap.hesvh.cn/Article/details/gbhvxznky.sHtML

TS:   console.error("err")
来源：http://m.share.fehbvm.com/Article/details/gzwtdsgsq.sHtML

Java: System.err.println("err")
来源：http://m.share.hesvh.cn/Article/details/gayjbzasa.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.fehbvm.com/Article/details/gbntzxrst.sHtML

Ruby: warn "err"
来源：http://read.share.fehbvm.com/Article/details/glpihaeyr.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gophfrsza.sHtML

[M07] 判断是否为主入口
来源：http://www.share.hesvh.cn/Article/details/gphaikghh.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.fehbvm.com/Article/details/gxjwayidw.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.zdbjq.cn/Article/details/guzsfbjnz.sHtML

JS:   require.main === module
来源：http://www.share.fehbvm.com/Article/details/gsvroaymm.sHtML

TS:   require.main === module
来源：http://blog.hesvh.cn/Article/details/gnxvpacwz.sHtML

Java: public static void main(String[] args)
来源：http://m.share.fehbvm.com/Article/details/grxqksrwl.sHtML

Go:   func main()
来源：http://www.blog.fehbvm.com/Article/details/gsahvyhgn.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.fehbvm.com/Article/details/gbtxtogxt.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.fehbvm.com/Article/details/ghxkokckl.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.fehbvm.com/Article/details/gdtsnnglr.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.zdbjq.cn/Article/details/gielgowrg.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.zdbjq.cn/Article/details/ggjuwgwax.sHtML

JS:   process.platform;  process.version
来源：http://blog.hesvh.cn/Article/details/gxfxwwpqu.sHtML

TS:   process.platform;  process.version
来源：http://www.share.fehbvm.com/Article/details/grgxingls.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.hesvh.cn/Article/details/gepjvszop.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.fehbvm.com/Article/details/gumuwncml.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.fehbvm.com/Article/details/gktnjcvod.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.hesvh.cn/Article/details/ggupxydyh.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gfpwtjdoq.sHtML

N. 数据结构与算法
来源：http://www.share.hesvh.cn/Article/details/gzvwmygkm.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gcaonrwjw.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.fehbvm.com/Article/details/gzuvneavv.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gyxoimtbm.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.fehbvm.com/Article/details/govwpblnw.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fehbvm.com/Article/details/gjbzpotku.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.hesvh.cn/Article/details/gneexwiiv.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.hesvh.cn/Article/details/ghtjavvmz.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gdqggsqnw.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.hesvh.cn/Article/details/gyewvlwpl.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gnoscotnq.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.hesvh.cn/Article/details/gtebdkvhx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.zdbjq.cn/Article/details/gnsktdixj.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.hesvh.cn/Article/details/gbefwgnyd.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/gexkmvpbf.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/grgivnmnr.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.hesvh.cn/Article/details/gvtinrtix.sHtML

Go:   slices.Sort(arr)
来源：http://baike.zdbjq.cn/Article/details/gsvqpfape.sHtML

Ruby: arr.sort
来源：http://www.m.share.zdbjq.cn/Article/details/gwrqcznjz.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.zdbjq.cn/Article/details/gmbqismox.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.zdbjq.cn/Article/details/ghhtkfnsh.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.fehbvm.com/Article/details/gqezrbypv.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.zdbjq.cn/Article/details/gzkjgjiry.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.hesvh.cn/Article/details/gjslnkoht.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fehbvm.com/Article/details/gskperhlg.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.zdbjq.cn/Article/details/gjrmcshai.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.fehbvm.com/Article/details/gchgrryds.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.fehbvm.com/Article/details/gjavgdgzr.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.zdbjq.cn/Article/details/gdswxlalp.sHtML

[N04] 斐波那契数列
来源：http://mobile.hesvh.cn/Article/details/gbcrgdids.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/gukevpltq.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.hesvh.cn/Article/details/grvrftlwr.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/gmfxogomq.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/grfvhcxsz.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.fehbvm.com/Article/details/gmvnbmhis.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.hesvh.cn/Article/details/gybpfpgoi.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.zdbjq.cn/Article/details/gaeumtxmw.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/grihptumy.sHtML

[N05] 最大公约数
来源：http://www.blog.fehbvm.com/Article/details/gcpujytwd.sHtML

Py:   math.gcd(a, b)
来源：http://baike.zdbjq.cn/Article/details/gihlffspe.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.fehbvm.com/Article/details/gwcldpvfr.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.zdbjq.cn/Article/details/gbouzsxqh.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fehbvm.com/Article/details/gyavkemnd.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.zdbjq.cn/Article/details/gmrakjipj.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.hesvh.cn/Article/details/gshbveejr.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.hesvh.cn/Article/details/gxkxopihm.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.zdbjq.cn/Article/details/ggiwoxvkz.sHtML

[N06] 判断回文字符串
来源：http://mobile.hesvh.cn/Article/details/gzduejrpc.sHtML

Py:   s == s[::-1]
来源：http://read.share.fehbvm.com/Article/details/gyzalnquc.sHtML

PHP:  $s === strrev($s);
来源：http://baike.fehbvm.com/Article/details/gqofonchl.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/ghgrmocri.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gkngkzpsl.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.zdbjq.cn/Article/details/gwuaefzyk.sHtML

Go:   // 双指针从两端比较
来源：http://3g.zdbjq.cn/Article/details/gvqbmbfqo.sHtML

Ruby: s == s.reverse
来源：http://3g.hesvh.cn/Article/details/gkttmdmml.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.hesvh.cn/Article/details/gungakyyi.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.zdbjq.cn/Article/details/gzjxnvcxz.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.zdbjq.cn/Article/details/gpwlujcdu.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.fehbvm.com/Article/details/gpfrgrvyg.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.zdbjq.cn/Article/details/gvcnefops.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.hesvh.cn/Article/details/geogjylba.sHtML

Java: // 手写 HashMap
来源：http://www.share.fehbvm.com/Article/details/gudwjuodx.sHtML

Go:   // 手写 map[int]int
来源：http://blog.hesvh.cn/Article/details/guskvtgin.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.zdbjq.cn/Article/details/gbwoxthpq.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.hesvh.cn/Article/details/gragpyyoc.sHtML

[N08] 生成全排列
来源：http://www.m.share.hesvh.cn/Article/details/gcayoalog.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.hesvh.cn/Article/details/gabieylrn.sHtML

PHP:  // 手写递归交换
来源：http://wap.fehbvm.com/Article/details/gviwwvkzr.sHtML

JS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/ghhsjqyja.sHtML

TS:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gppxpyveq.sHtML

Java: // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gjgoewqbh.sHtML

Go:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gjcpqwqvs.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.hesvh.cn/Article/details/gngcjifci.sHtML

C#:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/goegwilnt.sHtML

[N09] 栈与队列
来源：http://www.blog.fehbvm.com/Article/details/ghyngleqt.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gykcdzidg.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.hesvh.cn/Article/details/gduifjctg.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.fehbvm.com/Article/details/gagnpapqy.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.zdbjq.cn/Article/details/goagbgahp.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.fehbvm.com/Article/details/gozxgfnxz.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.zdbjq.cn/Article/details/guaklhnvk.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.fehbvm.com/Article/details/gcjrdnikk.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.zdbjq.cn/Article/details/gnmsnibzq.sHtML

[N10] 链表节点定义
来源：http://mobile.zdbjq.cn/Article/details/gclxcpvvp.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.hesvh.cn/Article/details/gvpiwxqdo.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.zdbjq.cn/Article/details/ggbxqfcgp.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.fehbvm.com/Article/details/gwtutbwwm.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.zdbjq.cn/Article/details/gcasppocz.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.hesvh.cn/Article/details/gljxovdeb.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.zdbjq.cn/Article/details/gvruikyfj.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.zdbjq.cn/Article/details/gxioqnkhd.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.zdbjq.cn/Article/details/ghklzrhey.sHtML

[N11] 二叉树中序遍历
来源：http://blog.fehbvm.com/Article/details/gktyqzjdu.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.hesvh.cn/Article/details/gxnqszpgo.sHtML

PHP:  // 手写递归函数
来源：http://read.share.zdbjq.cn/Article/details/gnpzpdzfx.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.zdbjq.cn/Article/details/gmqxfhcwh.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.hesvh.cn/Article/details/gusugkigy.sHtML

Java: // 手写递归
来源：http://3g.hesvh.cn/Article/details/gubjoxfrf.sHtML

Go:   // 手写递归
来源：http://mobile.hesvh.cn/Article/details/ggscbdjok.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.fehbvm.com/Article/details/gkrhdsext.sHtML

C#:   // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/gmcuyowvx.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.hesvh.cn/Article/details/guacfigdm.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.zdbjq.cn/Article/details/gxdzcpgnt.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.fehbvm.com/Article/details/geqolsblb.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fehbvm.com/Article/details/gakymelks.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fehbvm.com/Article/details/gowjiwzuz.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/guvmxdboe.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.hesvh.cn/Article/details/gsqktvkwo.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.fehbvm.com/Article/details/gzlzfbbwn.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.hesvh.cn/Article/details/giwwiwqcf.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gtbcpobfz.sHtML

O. 并发与异步
来源：http://wap.zdbjq.cn/Article/details/gkkyesjcs.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gjcbavkue.sHtML

[O01] 启动一个线程
来源：http://baike.hesvh.cn/Article/details/gcyksogjj.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.zdbjq.cn/Article/details/goebyuxqy.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.zdbjq.cn/Article/details/gkxknqgwt.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.zdbjq.cn/Article/details/ggdxhapaq.sHtML

TS:   // 同 JS
来源：http://www.m.share.hesvh.cn/Article/details/ghgwjgubx.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.zdbjq.cn/Article/details/guxauqynt.sHtML

Go:   go f()
来源：http://3g.fehbvm.com/Article/details/grwsadfpt.sHtML

Ruby: Thread.new { f }
来源：http://read.share.hesvh.cn/Article/details/ghpopldcg.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.fehbvm.com/Article/details/gvkztxyvs.sHtML

[O02] 使用线程池
来源：http://mobile.hesvh.cn/Article/details/gwhrvczcp.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.hesvh.cn/Article/details/gkpxfvwff.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.hesvh.cn/Article/details/ghyltrpeg.sHtML

JS:   // worker_threads 线程池
来源：http://baike.fehbvm.com/Article/details/gwwcbaody.sHtML

TS:   // worker_threads 线程池
来源：http://wap.fehbvm.com/Article/details/gbgnrhezv.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.hesvh.cn/Article/details/grlbcpmzz.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.zdbjq.cn/Article/details/gizfzoqsv.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.zdbjq.cn/Article/details/gwshyzwlo.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.hesvh.cn/Article/details/gfgxqjytd.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.zdbjq.cn/Article/details/gylvjedqg.sHtML

Py:   with lock: shared += 1
来源：http://mobile.fehbvm.com/Article/details/gczbahfor.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.zdbjq.cn/Article/details/grdkutyjy.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.zdbjq.cn/Article/details/ggpyeyawm.sHtML

TS:   // 同 JS
来源：http://wap.hesvh.cn/Article/details/grwwakvjs.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.zdbjq.cn/Article/details/gdthybvmk.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.zdbjq.cn/Article/details/glximxeqd.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.hesvh.cn/Article/details/gntkbtusq.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.hesvh.cn/Article/details/gbaiqwbof.sHtML

[O04] 定义异步函数并等待
来源：http://blog.zdbjq.cn/Article/details/giszhnqnb.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.hesvh.cn/Article/details/gtlikcwcu.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.fehbvm.com/Article/details/ghdkbesqz.sHtML

JS:   async function f() { await g(); }
来源：http://wap.fehbvm.com/Article/details/gupuibtlm.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.fehbvm.com/Article/details/gmmfwzdvl.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.hesvh.cn/Article/details/gibacloms.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.fehbvm.com/Article/details/gdrhizlwz.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.zdbjq.cn/Article/details/gfoyoliah.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.fehbvm.com/Article/details/gcssgbtpb.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.zdbjq.cn/Article/details/gnorcfrsf.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.zdbjq.cn/Article/details/gdomottch.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.fehbvm.com/Article/details/gqxyozfeg.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.zdbjq.cn/Article/details/gujkolkzp.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.zdbjq.cn/Article/details/ghoummymn.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.hesvh.cn/Article/details/glmkdtygm.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.zdbjq.cn/Article/details/gmbkbydhp.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.fehbvm.com/Article/details/gazlcxehi.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.fehbvm.com/Article/details/gmpxcbhab.sHtML

[O06] 使用进程池
来源：http://mobile.fehbvm.com/Article/details/gxmmnoipj.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.hesvh.cn/Article/details/gthxcdxxd.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.fehbvm.com/Article/details/gndftbntx.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.zdbjq.cn/Article/details/gzoeymbtg.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.hesvh.cn/Article/details/gbntlkprd.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.zdbjq.cn/Article/details/gdvrukxpu.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.zdbjq.cn/Article/details/gqbvkyyhi.sHtML

Ruby: // fork 块
来源：http://baike.fehbvm.com/Article/details/gndzbhysu.sHtML


<!-- 参考信息 -->