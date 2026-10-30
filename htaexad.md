代发 wailian999

Py:   requests.post(url, json={"a": 1})
来源：http://blog.zdbjq.cn/Article/details/giwcvsgth.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.hesvh.cn/Article/details/grqvdmqcf.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.fehbvm.com/Article/details/glnktubye.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.zdbjq.cn/Article/details/gllziogfv.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.zdbjq.cn/Article/details/giitqvcse.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.fehbvm.com/Article/details/gmwicyoun.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.zdbjq.cn/Article/details/gquvaogbb.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.fehbvm.com/Article/details/gkmpfdcwh.sHtML

[L03] 设置自定义请求头
来源：http://blog.fehbvm.com/Article/details/gecmjsjcm.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.zdbjq.cn/Article/details/gfixmokyy.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.zdbjq.cn/Article/details/gllnvbmcm.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.zdbjq.cn/Article/details/ghbpijlht.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.zdbjq.cn/Article/details/ggzloyhzu.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.zdbjq.cn/Article/details/ggulmhibc.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.zdbjq.cn/Article/details/gvwuhuykx.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.zdbjq.cn/Article/details/gxvygffeu.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.zdbjq.cn/Article/details/gqejpdfkp.sHtML

[L04] 设置超时
来源：http://www.share.zdbjq.cn/Article/details/gzhikuyps.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.fehbvm.com/Article/details/gmwvvvjmb.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.fehbvm.com/Article/details/gosnxyonx.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.hesvh.cn/Article/details/gtgaabnzy.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.zdbjq.cn/Article/details/gkvtcmrqs.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.zdbjq.cn/Article/details/gbgwesroy.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.zdbjq.cn/Article/details/gspnfsxlf.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.hesvh.cn/Article/details/gevbwlzux.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.zdbjq.cn/Article/details/guehwemaf.sHtML

[L05] 上传文件（multipart）
来源：http://wap.zdbjq.cn/Article/details/gzxqvihkg.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.hesvh.cn/Article/details/ghcflvnbg.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.fehbvm.com/Article/details/gzwbenqfn.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.zdbjq.cn/Article/details/gfppuynup.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.hesvh.cn/Article/details/gqmonwncz.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.fehbvm.com/Article/details/grhtovijh.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.fehbvm.com/Article/details/gctyfjpus.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.hesvh.cn/Article/details/gppbgvcwp.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.hesvh.cn/Article/details/goscdjbzw.sHtML

[L06] 解析响应为 JSON
来源：http://3g.fehbvm.com/Article/details/gqmkqyccs.sHtML

Py:   resp.json()
来源：http://m.share.hesvh.cn/Article/details/grttzfejz.sHtML

PHP:  json_decode($body, true);
来源：http://wap.fehbvm.com/Article/details/gzwllried.sHtML

JS:   await resp.json()
来源：http://read.share.zdbjq.cn/Article/details/gnlprywxq.sHtML

TS:   await resp.json()
来源：http://blog.fehbvm.com/Article/details/gelhbardd.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.fehbvm.com/Article/details/ghqhngjju.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.hesvh.cn/Article/details/gndvzewqy.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.fehbvm.com/Article/details/gjsqmkyad.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.hesvh.cn/Article/details/gupjtglqi.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.zdbjq.cn/Article/details/gpscuadwt.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.zdbjq.cn/Article/details/gyexomjde.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.zdbjq.cn/Article/details/gkyoglliq.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.hesvh.cn/Article/details/gdmsvsnsd.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.hesvh.cn/Article/details/gqxxotdln.sHtML

Java: resp.statusCode()
来源：http://3g.hesvh.cn/Article/details/guyyhjgmr.sHtML

Go:   resp.StatusCode
来源：http://3g.zdbjq.cn/Article/details/guawkszrj.sHtML

Ruby: resp.code.to_i
来源：http://m.share.zdbjq.cn/Article/details/gbkurghko.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.fehbvm.com/Article/details/gzdvmxnvr.sHtML

[L08] 并发请求多个地址
来源：http://read.share.zdbjq.cn/Article/details/gjjbuhicl.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.hesvh.cn/Article/details/gfatfvmqo.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.zdbjq.cn/Article/details/grtyhwsse.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.zdbjq.cn/Article/details/gvhlqtbel.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.zdbjq.cn/Article/details/gcqvuirmr.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.fehbvm.com/Article/details/gladdyjni.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.fehbvm.com/Article/details/gqkajnyas.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.zdbjq.cn/Article/details/gwjnthlsg.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gnpykvsii.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gwqdgacgc.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.fehbvm.com/Article/details/gpgmfljtq.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gwjukcwgp.sHtML

[M01] 读取命令行参数
来源：http://mobile.fehbvm.com/Article/details/gmxzbndcz.sHtML

Py:   sys.argv[1:]
来源：http://baike.fehbvm.com/Article/details/gfgvvwdhh.sHtML

PHP:  $argv;  $argc;
来源：http://wap.fehbvm.com/Article/details/geiyanalp.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.fehbvm.com/Article/details/ggiiosgwg.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.fehbvm.com/Article/details/gxbgctxlf.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.hesvh.cn/Article/details/giwbgakvl.sHtML

Go:   os.Args[1:]
来源：http://blog.hesvh.cn/Article/details/gzirkuyvu.sHtML

Ruby: ARGV
来源：http://www.blog.fehbvm.com/Article/details/gvrlgejeq.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.zdbjq.cn/Article/details/gglivajlg.sHtML

[M02] 读取环境变量
来源：http://m.share.zdbjq.cn/Article/details/gsobjclik.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/glfemsqjw.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.hesvh.cn/Article/details/gubonsbvk.sHtML

JS:   process.env.HOME
来源：http://read.share.hesvh.cn/Article/details/gpoofuwyo.sHtML

TS:   process.env.HOME
来源：http://read.share.zdbjq.cn/Article/details/gkemtmgjy.sHtML

Java: System.getenv("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gsjjnhyoy.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.fehbvm.com/Article/details/ghruzizlf.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.zdbjq.cn/Article/details/gobofmlri.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.fehbvm.com/Article/details/gkhebflrm.sHtML

[M03] 执行外部命令
来源：http://www.share.fehbvm.com/Article/details/gjfktjzqk.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.hesvh.cn/Article/details/ggeahqhtp.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.fehbvm.com/Article/details/gbluyyyhe.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.hesvh.cn/Article/details/gqgrupish.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.hesvh.cn/Article/details/gmczydzrj.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.fehbvm.com/Article/details/gqhyjpqfd.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.zdbjq.cn/Article/details/gpiewtiwc.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.zdbjq.cn/Article/details/gqegymoqy.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.zdbjq.cn/Article/details/gqkghbvex.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.fehbvm.com/Article/details/gwlihvnqz.sHtML

Py:   os.getcwd()
来源：http://3g.zdbjq.cn/Article/details/gwzrnckme.sHtML

PHP:  getcwd();
来源：http://www.m.share.fehbvm.com/Article/details/gaiqtfddu.sHtML

JS:   process.cwd()
来源：http://blog.zdbjq.cn/Article/details/gfzntssmm.sHtML

TS:   process.cwd()
来源：http://www.blog.zdbjq.cn/Article/details/gfhqfrvsn.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.fehbvm.com/Article/details/geuwbggdo.sHtML

Go:   os.Getwd()
来源：http://blog.hesvh.cn/Article/details/gnuatwrlh.sHtML

Ruby: Dir.pwd
来源：http://read.share.fehbvm.com/Article/details/guljjdjei.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.hesvh.cn/Article/details/gymwkhykv.sHtML

[M05] 设置退出码
来源：http://blog.fehbvm.com/Article/details/grnrguzwq.sHtML

Py:   sys.exit(1)
来源：http://baike.fehbvm.com/Article/details/guwhsowoy.sHtML

PHP:  exit(1);
来源：http://blog.fehbvm.com/Article/details/gsirbujfn.sHtML

JS:   process.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gvknsksfm.sHtML

TS:   process.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gdyupumno.sHtML

Java: System.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gmpdqommm.sHtML

Go:   os.Exit(1)
来源：http://www.share.hesvh.cn/Article/details/gibbghuxp.sHtML

Ruby: exit 1
来源：http://3g.zdbjq.cn/Article/details/gbuvgvkza.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.fehbvm.com/Article/details/gvltvrauq.sHtML

[M06] 向标准错误输出
来源：http://www.blog.hesvh.cn/Article/details/gadvzlckb.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.fehbvm.com/Article/details/gzlgzhnyx.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.zdbjq.cn/Article/details/gzujseicm.sHtML

JS:   console.error("err")
来源：http://read.share.fehbvm.com/Article/details/gmrnshlpd.sHtML

TS:   console.error("err")
来源：http://read.share.fehbvm.com/Article/details/gtwxdjgbg.sHtML

Java: System.err.println("err")
来源：http://m.share.zdbjq.cn/Article/details/ghpeyxhsl.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.fehbvm.com/Article/details/gictwbdqg.sHtML

Ruby: warn "err"
来源：http://www.m.share.hesvh.cn/Article/details/glfkeyxue.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gbfpgblot.sHtML

[M07] 判断是否为主入口
来源：http://blog.fehbvm.com/Article/details/gnvqqylvi.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.zdbjq.cn/Article/details/gepltkroi.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.hesvh.cn/Article/details/gilgugbwg.sHtML

JS:   require.main === module
来源：http://www.share.hesvh.cn/Article/details/gydhcurhw.sHtML

TS:   require.main === module
来源：http://www.share.fehbvm.com/Article/details/gercjuezm.sHtML

Java: public static void main(String[] args)
来源：http://baike.fehbvm.com/Article/details/gqalufuvz.sHtML

Go:   func main()
来源：http://wap.zdbjq.cn/Article/details/gtcwkkzch.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.hesvh.cn/Article/details/gymrtygzz.sHtML

C#:   static void Main(string[] args)
来源：http://3g.zdbjq.cn/Article/details/gxzqqzrmx.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.zdbjq.cn/Article/details/gokletxit.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.hesvh.cn/Article/details/grclaqvzg.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.hesvh.cn/Article/details/gwudrmerg.sHtML

JS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/gljmsungz.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.fehbvm.com/Article/details/gfnaowngk.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.zdbjq.cn/Article/details/gckjfpvrw.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.hesvh.cn/Article/details/ggsjfgstn.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.fehbvm.com/Article/details/gqrvvlkpu.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.fehbvm.com/Article/details/gyuulnzrl.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gbguszgmc.sHtML

N. 数据结构与算法
来源：http://3g.zdbjq.cn/Article/details/ggnxbcbge.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gbcrwckgh.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.zdbjq.cn/Article/details/gzbouassk.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gjvqkvmkg.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.hesvh.cn/Article/details/gaesxhlxg.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fehbvm.com/Article/details/gmxpasqoq.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fehbvm.com/Article/details/gstkflwaz.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.hesvh.cn/Article/details/goreyjtlz.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gpfgdhtog.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.zdbjq.cn/Article/details/gbgswdbot.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gdgejgilr.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.hesvh.cn/Article/details/gckcviweo.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.zdbjq.cn/Article/details/gxnyvlgup.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gmqpelzih.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gmookgpyr.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/gzpdfqouy.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.hesvh.cn/Article/details/goyafamww.sHtML

Go:   slices.Sort(arr)
来源：http://baike.fehbvm.com/Article/details/gnpfgszrt.sHtML

Ruby: arr.sort
来源：http://baike.hesvh.cn/Article/details/gcdkllsmn.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.zdbjq.cn/Article/details/gwkzbrffq.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.fehbvm.com/Article/details/gdfuwlrtk.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.fehbvm.com/Article/details/gkqgackyg.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.hesvh.cn/Article/details/geaipbbyt.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fehbvm.com/Article/details/gesnfbmdy.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.hesvh.cn/Article/details/ghnsetuqg.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.zdbjq.cn/Article/details/golbqjalq.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.fehbvm.com/Article/details/ghmckrwtv.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.hesvh.cn/Article/details/gvygoiybo.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.zdbjq.cn/Article/details/geichdwwf.sHtML

[N04] 斐波那契数列
来源：http://www.blog.hesvh.cn/Article/details/gnigeafqz.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/gvnbdbcxq.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.fehbvm.com/Article/details/gzdkpohgc.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/gqmwszecz.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/gzhfkjdii.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.fehbvm.com/Article/details/gzrxpemac.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.fehbvm.com/Article/details/gdtycyxgq.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/gwgzrddyy.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/gagwmiwqc.sHtML

[N05] 最大公约数
来源：http://www.m.share.zdbjq.cn/Article/details/guoirbkwk.sHtML

Py:   math.gcd(a, b)
来源：http://blog.zdbjq.cn/Article/details/gatebhwkv.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.hesvh.cn/Article/details/gpaiyzmsx.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.hesvh.cn/Article/details/geivsfqis.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.hesvh.cn/Article/details/gfptmgbur.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.fehbvm.com/Article/details/ghdkewtkp.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.zdbjq.cn/Article/details/gywvtltdh.sHtML

Ruby: a.gcd(b)
来源：http://m.share.fehbvm.com/Article/details/gffzzumiv.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.hesvh.cn/Article/details/gkpvbpxon.sHtML

[N06] 判断回文字符串
来源：http://baike.fehbvm.com/Article/details/gsjfojwao.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.zdbjq.cn/Article/details/gwjetzwsd.sHtML

PHP:  $s === strrev($s);
来源：http://wap.hesvh.cn/Article/details/gznetqfah.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gvdaudcau.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gdbzpwoxq.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.hesvh.cn/Article/details/gnvoexxel.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.zdbjq.cn/Article/details/gnvalkean.sHtML

Ruby: s == s.reverse
来源：http://blog.hesvh.cn/Article/details/gvwohdbah.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.zdbjq.cn/Article/details/gukocmswq.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.hesvh.cn/Article/details/gsczxfvng.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.fehbvm.com/Article/details/gehguxiub.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.fehbvm.com/Article/details/gyovxouqb.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.zdbjq.cn/Article/details/gjwdbppcz.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.hesvh.cn/Article/details/gioedvaek.sHtML

Java: // 手写 HashMap
来源：http://mobile.hesvh.cn/Article/details/gvxtdnbmf.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.hesvh.cn/Article/details/gqxchoeuf.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.hesvh.cn/Article/details/gddstkrre.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.hesvh.cn/Article/details/gnubarrdk.sHtML

[N08] 生成全排列
来源：http://blog.fehbvm.com/Article/details/glkmnchvv.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.hesvh.cn/Article/details/gcqvmcnht.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.zdbjq.cn/Article/details/gckgoxkuh.sHtML

JS:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gcewichfe.sHtML

TS:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gbemvrfdb.sHtML

Java: // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/grympwcgk.sHtML

Go:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gecucfzww.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.zdbjq.cn/Article/details/gzsslillv.sHtML

C#:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gmwcrjols.sHtML

[N09] 栈与队列
来源：http://mobile.hesvh.cn/Article/details/gvtnehmsg.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.fehbvm.com/Article/details/gyqqhdifs.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/goldakfiw.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.fehbvm.com/Article/details/ggbignqyp.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.zdbjq.cn/Article/details/ggfidyiec.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.fehbvm.com/Article/details/gkxtpyafb.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.hesvh.cn/Article/details/gxgizmcni.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gxgweseiz.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.hesvh.cn/Article/details/gpqqkjznl.sHtML

[N10] 链表节点定义
来源：http://www.m.share.hesvh.cn/Article/details/goxisflhw.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.hesvh.cn/Article/details/gwwkcepte.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.hesvh.cn/Article/details/gfuaygfao.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.hesvh.cn/Article/details/gxovteshx.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.fehbvm.com/Article/details/goyfcfkwb.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.fehbvm.com/Article/details/gfkdtlohn.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.fehbvm.com/Article/details/gqvjttric.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.zdbjq.cn/Article/details/ggwrtdsiu.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.hesvh.cn/Article/details/ghbndqafe.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.fehbvm.com/Article/details/gjkzjckkp.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.fehbvm.com/Article/details/gpqppdjdn.sHtML

PHP:  // 手写递归函数
来源：http://www.share.hesvh.cn/Article/details/gzgsmxftz.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/gvlhcyzdn.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.zdbjq.cn/Article/details/gopidnozk.sHtML

Java: // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gsizipnjd.sHtML

Go:   // 手写递归
来源：http://m.share.fehbvm.com/Article/details/gkgidmpvb.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.hesvh.cn/Article/details/gzmtumyjs.sHtML

C#:   // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gmrbluozc.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.hesvh.cn/Article/details/gxbjptuoa.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.zdbjq.cn/Article/details/gclbcvpqc.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.zdbjq.cn/Article/details/gaqlhoxmn.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.zdbjq.cn/Article/details/gidixfsbk.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/gqkbhnawx.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.fehbvm.com/Article/details/gnmkjlowf.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.fehbvm.com/Article/details/ggdmerhsv.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.hesvh.cn/Article/details/ganibwljw.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.zdbjq.cn/Article/details/gomebvbsx.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gpwuxtbcu.sHtML

O. 并发与异步
来源：http://blog.hesvh.cn/Article/details/gnoclrbbc.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gkrcwujyh.sHtML

[O01] 启动一个线程
来源：http://www.share.zdbjq.cn/Article/details/gxdbqgykt.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.fehbvm.com/Article/details/gejxzvdox.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.zdbjq.cn/Article/details/gjqhnglcy.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.fehbvm.com/Article/details/grafmsvny.sHtML

TS:   // 同 JS
来源：http://m.share.fehbvm.com/Article/details/gcofmwkic.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.zdbjq.cn/Article/details/gqgcubejw.sHtML

Go:   go f()
来源：http://www.blog.zdbjq.cn/Article/details/gawehoshx.sHtML

Ruby: Thread.new { f }
来源：http://baike.hesvh.cn/Article/details/gardjaqke.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.hesvh.cn/Article/details/gtfprwqmp.sHtML

[O02] 使用线程池
来源：http://blog.zdbjq.cn/Article/details/gurbxlawd.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.zdbjq.cn/Article/details/gxbqcufwp.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.zdbjq.cn/Article/details/guakgvkiy.sHtML

JS:   // worker_threads 线程池
来源：http://baike.zdbjq.cn/Article/details/gknhmqvhz.sHtML

TS:   // worker_threads 线程池
来源：http://baike.hesvh.cn/Article/details/gafewllvb.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.fehbvm.com/Article/details/gznfhicke.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.hesvh.cn/Article/details/gfrifckqn.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.hesvh.cn/Article/details/gikkaotdv.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.fehbvm.com/Article/details/gjhdmyfdf.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.zdbjq.cn/Article/details/ggoqcdsuy.sHtML

Py:   with lock: shared += 1
来源：http://wap.hesvh.cn/Article/details/gbpfemhfr.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.hesvh.cn/Article/details/gcrisoyhg.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.hesvh.cn/Article/details/gsmyaueaq.sHtML

TS:   // 同 JS
来源：http://wap.fehbvm.com/Article/details/ghavrnmkg.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.hesvh.cn/Article/details/gatqgvbfr.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.zdbjq.cn/Article/details/gthptltub.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.fehbvm.com/Article/details/gbroabqvi.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.hesvh.cn/Article/details/gnobpttab.sHtML

[O04] 定义异步函数并等待
来源：http://wap.zdbjq.cn/Article/details/gimycujzo.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.fehbvm.com/Article/details/gygfpxhxt.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.zdbjq.cn/Article/details/guoujgphq.sHtML

JS:   async function f() { await g(); }
来源：http://3g.zdbjq.cn/Article/details/geuhdjmkt.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.hesvh.cn/Article/details/gnmvffhbe.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.fehbvm.com/Article/details/gpxhxavpd.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.hesvh.cn/Article/details/gnsaovfsc.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.zdbjq.cn/Article/details/gpoctujpn.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.zdbjq.cn/Article/details/grlwyzxmm.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.fehbvm.com/Article/details/ghvpwymcq.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.hesvh.cn/Article/details/gqxhrmueh.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.zdbjq.cn/Article/details/gdcwafswj.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.fehbvm.com/Article/details/gezmctnri.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.fehbvm.com/Article/details/ghdlkubab.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.zdbjq.cn/Article/details/gxmhzohcz.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.fehbvm.com/Article/details/gnloxosgr.sHtML

Ruby: threads.map(&:join)
来源：http://wap.zdbjq.cn/Article/details/glegjdmdq.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.zdbjq.cn/Article/details/gndscoifz.sHtML

[O06] 使用进程池
来源：http://mobile.zdbjq.cn/Article/details/giskbvqfm.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.zdbjq.cn/Article/details/gwccugzdc.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.zdbjq.cn/Article/details/gmyzvthhg.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.hesvh.cn/Article/details/gomcgzqgq.sHtML


<!-- 参考信息 -->