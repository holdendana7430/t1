代发 wailian999

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.hesvh.cn/Article/details/gujxzvnbw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.zdbjq.cn/Article/details/gzkdqjccc.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.zdbjq.cn/Article/details/gydcgjgzt.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.hesvh.cn/Article/details/gqfwllumr.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.zdbjq.cn/Article/details/gipjzifjs.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.fehbvm.com/Article/details/gzlxvbzms.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.hesvh.cn/Article/details/gjehlaref.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.fehbvm.com/Article/details/gtlizharf.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.zdbjq.cn/Article/details/gxllmgnbj.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.fehbvm.com/Article/details/gpvdxkvrp.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.hesvh.cn/Article/details/gliczruwf.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.fehbvm.com/Article/details/gldxbnxhm.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.zdbjq.cn/Article/details/gxsxuycop.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.hesvh.cn/Article/details/glskwwudr.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.fehbvm.com/Article/details/gvtfppvdn.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.hesvh.cn/Article/details/gwkaxhccq.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.fehbvm.com/Article/details/gidylnllo.sHtML

[L04] 设置超时
来源：http://wap.fehbvm.com/Article/details/ghruugipp.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.hesvh.cn/Article/details/geowvnzln.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.fehbvm.com/Article/details/gkikfuhvz.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.fehbvm.com/Article/details/gulwyfgur.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.fehbvm.com/Article/details/gwehizkgy.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.zdbjq.cn/Article/details/gltvbrrow.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.zdbjq.cn/Article/details/giloollwj.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.zdbjq.cn/Article/details/gyresuxbk.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.hesvh.cn/Article/details/ghbkqsvsm.sHtML

[L05] 上传文件（multipart）
来源：http://wap.hesvh.cn/Article/details/gqyifgyhc.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.fehbvm.com/Article/details/gnhyxcxqu.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.fehbvm.com/Article/details/gkayvhlxc.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.hesvh.cn/Article/details/gmljimqdq.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.fehbvm.com/Article/details/ghbbzljwh.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.fehbvm.com/Article/details/gqisbyqdv.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.zdbjq.cn/Article/details/gsrgscxyz.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.fehbvm.com/Article/details/gklbyedlx.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.zdbjq.cn/Article/details/ggtrqyjwk.sHtML

[L06] 解析响应为 JSON
来源：http://wap.hesvh.cn/Article/details/gjsumtpjx.sHtML

Py:   resp.json()
来源：http://read.share.fehbvm.com/Article/details/gfnukqnqz.sHtML

PHP:  json_decode($body, true);
来源：http://baike.hesvh.cn/Article/details/gjsipbwyl.sHtML

JS:   await resp.json()
来源：http://3g.zdbjq.cn/Article/details/gwjbhgjhy.sHtML

TS:   await resp.json()
来源：http://www.blog.fehbvm.com/Article/details/guryksbed.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.zdbjq.cn/Article/details/giixaxgnx.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.hesvh.cn/Article/details/gqzxdtwvw.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.fehbvm.com/Article/details/gigeiwlau.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.fehbvm.com/Article/details/gbsunbdzj.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.fehbvm.com/Article/details/gxyicnwll.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.hesvh.cn/Article/details/glvymmgew.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.hesvh.cn/Article/details/gsvflllcn.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.fehbvm.com/Article/details/gpdydbtcq.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.hesvh.cn/Article/details/gbjyusttl.sHtML

Java: resp.statusCode()
来源：http://mobile.hesvh.cn/Article/details/gzkarbmpa.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.fehbvm.com/Article/details/gdysrrixq.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.hesvh.cn/Article/details/griamxevh.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.hesvh.cn/Article/details/gkzmibyvw.sHtML

[L08] 并发请求多个地址
来源：http://blog.hesvh.cn/Article/details/gkrfsrptb.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.zdbjq.cn/Article/details/gzepvmbhr.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.fehbvm.com/Article/details/gkyjhexrz.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.zdbjq.cn/Article/details/giwuanmxa.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/gwlnhnilk.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.zdbjq.cn/Article/details/gkmntbpcw.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.zdbjq.cn/Article/details/gdrvrhgyc.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.zdbjq.cn/Article/details/gjlizzovn.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.hesvh.cn/Article/details/gnahuzpjw.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gslfdezmq.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.fehbvm.com/Article/details/glbnwdsna.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gxmmqvfza.sHtML

[M01] 读取命令行参数
来源：http://3g.zdbjq.cn/Article/details/gtdkbjome.sHtML

Py:   sys.argv[1:]
来源：http://baike.fehbvm.com/Article/details/ghhrvblka.sHtML

PHP:  $argv;  $argc;
来源：http://3g.hesvh.cn/Article/details/gfoqvywhj.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.hesvh.cn/Article/details/guplhklal.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.zdbjq.cn/Article/details/gaqnfaszf.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.fehbvm.com/Article/details/gsloderkp.sHtML

Go:   os.Args[1:]
来源：http://m.share.hesvh.cn/Article/details/gxodovkbp.sHtML

Ruby: ARGV
来源：http://baike.fehbvm.com/Article/details/gcbmnnmlt.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.zdbjq.cn/Article/details/gmvbevjml.sHtML

[M02] 读取环境变量
来源：http://m.share.zdbjq.cn/Article/details/gmtvbgmzl.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.fehbvm.com/Article/details/gjhuonvst.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.fehbvm.com/Article/details/gdadafgbd.sHtML

JS:   process.env.HOME
来源：http://www.blog.zdbjq.cn/Article/details/guskklbmw.sHtML

TS:   process.env.HOME
来源：http://www.blog.hesvh.cn/Article/details/gafglpfgt.sHtML

Java: System.getenv("HOME")
来源：http://www.share.hesvh.cn/Article/details/gyktzvmtw.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gvcrooisx.sHtML

Ruby: ENV["HOME"]
来源：http://blog.fehbvm.com/Article/details/gxdscutej.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.fehbvm.com/Article/details/gfuawjuto.sHtML

[M03] 执行外部命令
来源：http://baike.hesvh.cn/Article/details/gfghxghvd.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.fehbvm.com/Article/details/goqzkdptj.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.zdbjq.cn/Article/details/gfkajeecm.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.zdbjq.cn/Article/details/gbhxdfktf.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.hesvh.cn/Article/details/gjnpqcixc.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.hesvh.cn/Article/details/grijftsvn.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.zdbjq.cn/Article/details/gwvvivaxf.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.fehbvm.com/Article/details/gnzazplhg.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.hesvh.cn/Article/details/ggwhjpxif.sHtML

[M04] 获取当前工作目录
来源：http://read.share.fehbvm.com/Article/details/gufbjntsz.sHtML

Py:   os.getcwd()
来源：http://baike.fehbvm.com/Article/details/giydiysbr.sHtML

PHP:  getcwd();
来源：http://www.m.share.hesvh.cn/Article/details/gipgrveeb.sHtML

JS:   process.cwd()
来源：http://m.share.zdbjq.cn/Article/details/ggyknleqr.sHtML

TS:   process.cwd()
来源：http://www.m.share.hesvh.cn/Article/details/ghicoxbqs.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.hesvh.cn/Article/details/gkjuaqhmq.sHtML

Go:   os.Getwd()
来源：http://baike.zdbjq.cn/Article/details/gzssvistp.sHtML

Ruby: Dir.pwd
来源：http://www.share.hesvh.cn/Article/details/ggczmcyhi.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.fehbvm.com/Article/details/gzglvgmcp.sHtML

[M05] 设置退出码
来源：http://mobile.hesvh.cn/Article/details/grehegmxo.sHtML

Py:   sys.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gahedazhl.sHtML

PHP:  exit(1);
来源：http://www.m.share.zdbjq.cn/Article/details/gighwlsje.sHtML

JS:   process.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gngfwfxfl.sHtML

TS:   process.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gxdjhyqnd.sHtML

Java: System.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gkvggdagb.sHtML

Go:   os.Exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gnlbntzak.sHtML

Ruby: exit 1
来源：http://3g.zdbjq.cn/Article/details/gldlgmgds.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.fehbvm.com/Article/details/gzeaspqme.sHtML

[M06] 向标准错误输出
来源：http://www.share.fehbvm.com/Article/details/glyrbyflv.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.zdbjq.cn/Article/details/ghftqruer.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.fehbvm.com/Article/details/gkxqtbxtn.sHtML

JS:   console.error("err")
来源：http://baike.zdbjq.cn/Article/details/gbfsrwaaz.sHtML

TS:   console.error("err")
来源：http://m.share.zdbjq.cn/Article/details/gbsckywkf.sHtML

Java: System.err.println("err")
来源：http://3g.hesvh.cn/Article/details/gpeaxhxfv.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.hesvh.cn/Article/details/gepnfbeag.sHtML

Ruby: warn "err"
来源：http://www.share.fehbvm.com/Article/details/gmumkataw.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.fehbvm.com/Article/details/gdjtiqrrg.sHtML

[M07] 判断是否为主入口
来源：http://www.share.hesvh.cn/Article/details/gmxaxegpt.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.zdbjq.cn/Article/details/gwvgttpzd.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.zdbjq.cn/Article/details/giaaplunc.sHtML

JS:   require.main === module
来源：http://mobile.fehbvm.com/Article/details/gvsydqtph.sHtML

TS:   require.main === module
来源：http://www.m.share.zdbjq.cn/Article/details/gtafvfyqe.sHtML

Java: public static void main(String[] args)
来源：http://3g.zdbjq.cn/Article/details/gjplghimo.sHtML

Go:   func main()
来源：http://read.share.fehbvm.com/Article/details/gyrnqwzxu.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.hesvh.cn/Article/details/gyemxtslm.sHtML

C#:   static void Main(string[] args)
来源：http://3g.zdbjq.cn/Article/details/grjtoddku.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.hesvh.cn/Article/details/grqyhvgjb.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.hesvh.cn/Article/details/gzzutjfoj.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.fehbvm.com/Article/details/gdlacwivk.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.hesvh.cn/Article/details/gaelbsbkc.sHtML

TS:   process.platform;  process.version
来源：http://m.share.fehbvm.com/Article/details/guyxdwmoj.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.hesvh.cn/Article/details/gwpnylath.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.fehbvm.com/Article/details/gahepmerw.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.fehbvm.com/Article/details/gczxfknfx.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.fehbvm.com/Article/details/gqzchsjlv.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gqselcfyv.sHtML

N. 数据结构与算法
来源：http://read.share.fehbvm.com/Article/details/gbpezczbs.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gxpdsfblt.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.hesvh.cn/Article/details/gqklvqjpo.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gwqhkybji.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gwaaticdj.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fehbvm.com/Article/details/gtchjsgxy.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gsrdjatab.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.hesvh.cn/Article/details/gpnlcwsxt.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gspwwprkj.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.hesvh.cn/Article/details/gxhyzhjou.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.fehbvm.com/Article/details/gtfmpgyuz.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.hesvh.cn/Article/details/goeymnhvr.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.zdbjq.cn/Article/details/gejryfgon.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.fehbvm.com/Article/details/glpbpqhpb.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/gjgacnwrf.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gmoywjacl.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.fehbvm.com/Article/details/ghwlrpdbb.sHtML

Go:   slices.Sort(arr)
来源：http://blog.fehbvm.com/Article/details/glnnsnmgu.sHtML

Ruby: arr.sort
来源：http://www.blog.zdbjq.cn/Article/details/gsgtfiztn.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.hesvh.cn/Article/details/gcnvrajyc.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.fehbvm.com/Article/details/gxuxoijhd.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.fehbvm.com/Article/details/gqffjlffj.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.fehbvm.com/Article/details/gpkziossu.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fehbvm.com/Article/details/gmpobgpuz.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fehbvm.com/Article/details/gtfbvitdt.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.hesvh.cn/Article/details/gsreunfpr.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.zdbjq.cn/Article/details/gzimlzgyi.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.fehbvm.com/Article/details/gmwrdenwn.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.hesvh.cn/Article/details/ggxhwaxxr.sHtML

[N04] 斐波那契数列
来源：http://blog.hesvh.cn/Article/details/ghhbrijos.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.fehbvm.com/Article/details/gbiryxhbk.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.hesvh.cn/Article/details/gcvnbafed.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/grjygqrlq.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/ggxyhlnhb.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.fehbvm.com/Article/details/gftzipuqt.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.zdbjq.cn/Article/details/gsrfdmkdp.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/gxxvpdabw.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/grboltxyd.sHtML

[N05] 最大公约数
来源：http://read.share.zdbjq.cn/Article/details/gppnuetrn.sHtML

Py:   math.gcd(a, b)
来源：http://baike.hesvh.cn/Article/details/ghkrucxuv.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.zdbjq.cn/Article/details/gsynddxbq.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.hesvh.cn/Article/details/gvnztpnol.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.hesvh.cn/Article/details/gnfjanxxp.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.fehbvm.com/Article/details/gsawjwaez.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.fehbvm.com/Article/details/gvjjqbbwt.sHtML

Ruby: a.gcd(b)
来源：http://blog.fehbvm.com/Article/details/ghknacugf.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.hesvh.cn/Article/details/gyfexkdko.sHtML

[N06] 判断回文字符串
来源：http://m.share.zdbjq.cn/Article/details/gutdfnahn.sHtML

Py:   s == s[::-1]
来源：http://3g.fehbvm.com/Article/details/gzhpxyxak.sHtML

PHP:  $s === strrev($s);
来源：http://blog.zdbjq.cn/Article/details/gpscfzzya.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gxrzqtjvj.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/guctdihnq.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.zdbjq.cn/Article/details/gydohgfyp.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.hesvh.cn/Article/details/ghwfzvuvv.sHtML

Ruby: s == s.reverse
来源：http://3g.fehbvm.com/Article/details/ghuwiaryy.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.fehbvm.com/Article/details/gxiwhzctr.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.fehbvm.com/Article/details/gqwpkhzpc.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.hesvh.cn/Article/details/gpdaechub.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.fehbvm.com/Article/details/gehhlumfb.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.hesvh.cn/Article/details/ggsggwwpy.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.fehbvm.com/Article/details/guaywygia.sHtML

Java: // 手写 HashMap
来源：http://baike.hesvh.cn/Article/details/gmqolkdli.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.zdbjq.cn/Article/details/gbvxnqwkj.sHtML

Ruby: // 手写 Hash
来源：http://wap.hesvh.cn/Article/details/gcfrciazu.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.zdbjq.cn/Article/details/gabhkhrcw.sHtML

[N08] 生成全排列
来源：http://wap.hesvh.cn/Article/details/gfstusuqc.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.zdbjq.cn/Article/details/gfwniwvdt.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.hesvh.cn/Article/details/gkcoliqau.sHtML

JS:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gxjryjmbn.sHtML

TS:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gzyxmtjcv.sHtML

Java: // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/ghsdrwlyc.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gfvhidtuc.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.fehbvm.com/Article/details/gmyolgtwi.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gkbvjxbux.sHtML

[N09] 栈与队列
来源：http://www.share.fehbvm.com/Article/details/gugtrvnvn.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.fehbvm.com/Article/details/ggztasacw.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.fehbvm.com/Article/details/gqedfbmzo.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.hesvh.cn/Article/details/gvmeawnvp.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.hesvh.cn/Article/details/gpjiiicmb.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.zdbjq.cn/Article/details/gxbylqogv.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.hesvh.cn/Article/details/gjthkxffo.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.fehbvm.com/Article/details/gqgrtecwf.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.fehbvm.com/Article/details/gqfbwoskq.sHtML

[N10] 链表节点定义
来源：http://3g.hesvh.cn/Article/details/gmfntqgcz.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.fehbvm.com/Article/details/gbxfnevup.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.hesvh.cn/Article/details/gpisolfrr.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.zdbjq.cn/Article/details/gpccgtkis.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.zdbjq.cn/Article/details/glkdlnfpr.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.zdbjq.cn/Article/details/gqlovpkod.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.hesvh.cn/Article/details/gvqgxlsiw.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.fehbvm.com/Article/details/geymecntk.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.fehbvm.com/Article/details/giusyptng.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.zdbjq.cn/Article/details/gbpbnxdbp.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.fehbvm.com/Article/details/gyoexfapu.sHtML

PHP:  // 手写递归函数
来源：http://3g.zdbjq.cn/Article/details/ggcpmovlj.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.hesvh.cn/Article/details/gkgzscwvz.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.zdbjq.cn/Article/details/glpzpvmeu.sHtML

Java: // 手写递归
来源：http://read.share.hesvh.cn/Article/details/gprtispkl.sHtML

Go:   // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/godkchcnh.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.zdbjq.cn/Article/details/gscvbvkjf.sHtML

C#:   // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gqwoldemf.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.fehbvm.com/Article/details/greyjeibf.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.hesvh.cn/Article/details/gbqetdtqv.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.zdbjq.cn/Article/details/gzwxntpic.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.zdbjq.cn/Article/details/gbexymalu.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.hesvh.cn/Article/details/gmrncuexl.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fehbvm.com/Article/details/gzolcxerp.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.hesvh.cn/Article/details/gktnbmxmi.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.hesvh.cn/Article/details/geskdjxeb.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fehbvm.com/Article/details/ghhbbdjjn.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gbxcgsani.sHtML

O. 并发与异步
来源：http://3g.fehbvm.com/Article/details/gscybhabj.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/goptiefkf.sHtML

[O01] 启动一个线程
来源：http://wap.fehbvm.com/Article/details/ggtboapgx.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.fehbvm.com/Article/details/gevarvtbe.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.hesvh.cn/Article/details/gltrnikom.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.hesvh.cn/Article/details/ghpvrgqgv.sHtML

TS:   // 同 JS
来源：http://www.blog.fehbvm.com/Article/details/ghiplorki.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.fehbvm.com/Article/details/gqoqflmcn.sHtML

Go:   go f()
来源：http://www.share.zdbjq.cn/Article/details/gcbacbmvm.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.fehbvm.com/Article/details/gntnylswc.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.fehbvm.com/Article/details/gzsqjdhew.sHtML

[O02] 使用线程池
来源：http://read.share.hesvh.cn/Article/details/gttcqntir.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.zdbjq.cn/Article/details/gdjtzcekt.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.hesvh.cn/Article/details/gecvgxmoj.sHtML

JS:   // worker_threads 线程池
来源：http://wap.hesvh.cn/Article/details/grxpnnhjc.sHtML

TS:   // worker_threads 线程池
来源：http://3g.zdbjq.cn/Article/details/gzrwkwamc.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.zdbjq.cn/Article/details/gqvpdozqe.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.fehbvm.com/Article/details/gamodnobp.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.fehbvm.com/Article/details/gpihiyvrf.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.hesvh.cn/Article/details/gyxamdfdp.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.hesvh.cn/Article/details/gjzkbyepw.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.fehbvm.com/Article/details/gipcrywvr.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.zdbjq.cn/Article/details/gbawnedrh.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.fehbvm.com/Article/details/gnapijvkj.sHtML

TS:   // 同 JS
来源：http://read.share.zdbjq.cn/Article/details/gtcpimitb.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.fehbvm.com/Article/details/gqbymzugm.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.zdbjq.cn/Article/details/gmhdibpes.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.fehbvm.com/Article/details/ggpumodaa.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.fehbvm.com/Article/details/gxrdydesm.sHtML

[O04] 定义异步函数并等待
来源：http://blog.fehbvm.com/Article/details/geurkpevw.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.hesvh.cn/Article/details/gercxlvpc.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.fehbvm.com/Article/details/gtsyxkzlf.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.hesvh.cn/Article/details/gencgzypt.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.zdbjq.cn/Article/details/gpnbjuuhf.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.hesvh.cn/Article/details/ghqbunkpj.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.zdbjq.cn/Article/details/gqdofqjpj.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.zdbjq.cn/Article/details/gqksmtyww.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.zdbjq.cn/Article/details/gogdmcgwi.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.zdbjq.cn/Article/details/gqokyfjtt.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.hesvh.cn/Article/details/gvuubarba.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.zdbjq.cn/Article/details/gfjfylmqh.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.hesvh.cn/Article/details/grplyadqq.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.zdbjq.cn/Article/details/gvrqyimfw.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.fehbvm.com/Article/details/gapaeicgt.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.zdbjq.cn/Article/details/glmbocetm.sHtML

Ruby: threads.map(&:join)
来源：http://3g.zdbjq.cn/Article/details/glpobmapz.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.fehbvm.com/Article/details/gwgvukbef.sHtML

[O06] 使用进程池
来源：http://3g.fehbvm.com/Article/details/gdyhmobcl.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.fehbvm.com/Article/details/gvkuhfycj.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.fehbvm.com/Article/details/gkjnazxvc.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.hesvh.cn/Article/details/gztcuvxbp.sHtML


<!-- 参考信息 -->