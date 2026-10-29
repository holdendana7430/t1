代发 wailian999

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.zdbjq.cn/Article/details/gaoxotyll.sHtML

JS:   await fetch(url)
来源：http://blog.zdbjq.cn/Article/details/gaxhycjqj.sHtML

TS:   await fetch(url)
来源：http://read.share.zdbjq.cn/Article/details/gcsqedzed.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.hesvh.cn/Article/details/ggoioxbfm.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.fehbvm.com/Article/details/giyihkjha.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.fehbvm.com/Article/details/gbajnssrb.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.hesvh.cn/Article/details/gxxtgvxwq.sHtML

[L02] 发送 POST JSON
来源：http://read.share.zdbjq.cn/Article/details/gxqncolry.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.fehbvm.com/Article/details/gfzyobwsu.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.zdbjq.cn/Article/details/gdcykyjyr.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fehbvm.com/Article/details/gzowxtptj.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.hesvh.cn/Article/details/gkzsnfbhz.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.hesvh.cn/Article/details/ggmmhenki.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.hesvh.cn/Article/details/gcxkvmrjh.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.hesvh.cn/Article/details/gawvmeprs.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.hesvh.cn/Article/details/goabmlkmr.sHtML

[L03] 设置自定义请求头
来源：http://m.share.fehbvm.com/Article/details/gxqbbrusi.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.fehbvm.com/Article/details/gontzclot.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.zdbjq.cn/Article/details/gljczuczu.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.zdbjq.cn/Article/details/gczqqgiwt.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.zdbjq.cn/Article/details/gxuxmjsfa.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.zdbjq.cn/Article/details/gtacrvdgf.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.fehbvm.com/Article/details/gxiiimult.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.hesvh.cn/Article/details/gkzudkcfj.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.hesvh.cn/Article/details/gwhdevtpi.sHtML

[L04] 设置超时
来源：http://www.m.share.fehbvm.com/Article/details/gnyscxlke.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.hesvh.cn/Article/details/gomuufvye.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.hesvh.cn/Article/details/gumaacetm.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.hesvh.cn/Article/details/gnzxjmxwd.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.zdbjq.cn/Article/details/grcijvqfq.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.fehbvm.com/Article/details/gznkwigey.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.fehbvm.com/Article/details/gzdxbbkjr.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.fehbvm.com/Article/details/ggtbelihf.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.fehbvm.com/Article/details/gwuqaeqza.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.zdbjq.cn/Article/details/gaaxtzlsu.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.hesvh.cn/Article/details/gdrytzwdo.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.fehbvm.com/Article/details/gojlptfts.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.zdbjq.cn/Article/details/ggcufmjav.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.hesvh.cn/Article/details/gffsfwekp.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.hesvh.cn/Article/details/gsmhongfw.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.zdbjq.cn/Article/details/gupisjghv.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.zdbjq.cn/Article/details/gekwpcsjl.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.fehbvm.com/Article/details/gjkuahqyb.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.hesvh.cn/Article/details/gurqkgjei.sHtML

Py:   resp.json()
来源：http://mobile.fehbvm.com/Article/details/gyofptubz.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.hesvh.cn/Article/details/gqsbfpknp.sHtML

JS:   await resp.json()
来源：http://mobile.hesvh.cn/Article/details/gqhyywuwv.sHtML

TS:   await resp.json()
来源：http://www.blog.zdbjq.cn/Article/details/geqhowjdm.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.zdbjq.cn/Article/details/guildilcv.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.zdbjq.cn/Article/details/gcovjuncl.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.zdbjq.cn/Article/details/gkoummkis.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.zdbjq.cn/Article/details/gpnkomitc.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.zdbjq.cn/Article/details/gynexcakf.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.hesvh.cn/Article/details/grfqghpjp.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.hesvh.cn/Article/details/gvbwuobke.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.fehbvm.com/Article/details/gdlflktnk.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.hesvh.cn/Article/details/ghlbqbrot.sHtML

Java: resp.statusCode()
来源：http://read.share.fehbvm.com/Article/details/givscuxrb.sHtML

Go:   resp.StatusCode
来源：http://mobile.fehbvm.com/Article/details/gsitjpqdm.sHtML

Ruby: resp.code.to_i
来源：http://mobile.fehbvm.com/Article/details/gmjedwvaq.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.zdbjq.cn/Article/details/gtinbfbjm.sHtML

[L08] 并发请求多个地址
来源：http://m.share.fehbvm.com/Article/details/guwgxyllt.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.zdbjq.cn/Article/details/gjwskmtnq.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.hesvh.cn/Article/details/gplzeommx.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.hesvh.cn/Article/details/gsuzeqeoa.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/grshvdryi.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.hesvh.cn/Article/details/gjbduwljr.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.zdbjq.cn/Article/details/grjqwjfet.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.hesvh.cn/Article/details/grdciinit.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.fehbvm.com/Article/details/gesyprkrp.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gmxacggmo.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.hesvh.cn/Article/details/gjxbzgvjc.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gaalzeuvd.sHtML

[M01] 读取命令行参数
来源：http://read.share.fehbvm.com/Article/details/gcyldxapg.sHtML

Py:   sys.argv[1:]
来源：http://mobile.zdbjq.cn/Article/details/guzyosajg.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.hesvh.cn/Article/details/gbkqvlxis.sHtML

JS:   process.argv.slice(2)
来源：http://3g.fehbvm.com/Article/details/gtvxkbpbf.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.zdbjq.cn/Article/details/gsqwmattw.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.fehbvm.com/Article/details/gdolgbgun.sHtML

Go:   os.Args[1:]
来源：http://blog.fehbvm.com/Article/details/gyestqine.sHtML

Ruby: ARGV
来源：http://www.share.zdbjq.cn/Article/details/gvwccadds.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.hesvh.cn/Article/details/gumvpjoce.sHtML

[M02] 读取环境变量
来源：http://read.share.fehbvm.com/Article/details/gxjmsbrhm.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.fehbvm.com/Article/details/gkyzxhvgq.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.hesvh.cn/Article/details/gepwjzolw.sHtML

JS:   process.env.HOME
来源：http://www.share.hesvh.cn/Article/details/gibebgujq.sHtML

TS:   process.env.HOME
来源：http://baike.zdbjq.cn/Article/details/ghibhfdzg.sHtML

Java: System.getenv("HOME")
来源：http://m.share.hesvh.cn/Article/details/gfmrkigjw.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.hesvh.cn/Article/details/ghrnfhouy.sHtML

Ruby: ENV["HOME"]
来源：http://wap.hesvh.cn/Article/details/gdqnhjzuu.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.hesvh.cn/Article/details/gzfmqtsqq.sHtML

[M03] 执行外部命令
来源：http://mobile.hesvh.cn/Article/details/gidzemcjx.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.zdbjq.cn/Article/details/gstmsvwfp.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.hesvh.cn/Article/details/grchnrgnb.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.zdbjq.cn/Article/details/gmxavrjjk.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fehbvm.com/Article/details/gpkupinqa.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.zdbjq.cn/Article/details/gmycgtboc.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.hesvh.cn/Article/details/gkxkbvzey.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.hesvh.cn/Article/details/gyqrohgmo.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.hesvh.cn/Article/details/gtadybavu.sHtML

[M04] 获取当前工作目录
来源：http://blog.zdbjq.cn/Article/details/garcuwoqh.sHtML

Py:   os.getcwd()
来源：http://www.share.hesvh.cn/Article/details/geiecnavw.sHtML

PHP:  getcwd();
来源：http://www.share.hesvh.cn/Article/details/gvmuqripy.sHtML

JS:   process.cwd()
来源：http://wap.hesvh.cn/Article/details/ghdovkoch.sHtML

TS:   process.cwd()
来源：http://www.blog.fehbvm.com/Article/details/gttghurls.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.hesvh.cn/Article/details/gesawtore.sHtML

Go:   os.Getwd()
来源：http://www.m.share.fehbvm.com/Article/details/gwjyneatd.sHtML

Ruby: Dir.pwd
来源：http://3g.zdbjq.cn/Article/details/glsyyyoqq.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.zdbjq.cn/Article/details/gnrblsndp.sHtML

[M05] 设置退出码
来源：http://blog.zdbjq.cn/Article/details/gzqkktlwa.sHtML

Py:   sys.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/ghnolipsg.sHtML

PHP:  exit(1);
来源：http://www.blog.fehbvm.com/Article/details/gmdadczej.sHtML

JS:   process.exit(1)
来源：http://baike.fehbvm.com/Article/details/geaxrhvbx.sHtML

TS:   process.exit(1)
来源：http://blog.hesvh.cn/Article/details/gegbmgnov.sHtML

Java: System.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gazzmuelz.sHtML

Go:   os.Exit(1)
来源：http://m.share.hesvh.cn/Article/details/gfsfbznkh.sHtML

Ruby: exit 1
来源：http://m.share.hesvh.cn/Article/details/gbxutybzx.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.fehbvm.com/Article/details/gdublxdox.sHtML

[M06] 向标准错误输出
来源：http://blog.zdbjq.cn/Article/details/gooapjzgu.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.fehbvm.com/Article/details/gdmzntrwq.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.fehbvm.com/Article/details/gncdtsoaz.sHtML

JS:   console.error("err")
来源：http://3g.zdbjq.cn/Article/details/gxkkovryf.sHtML

TS:   console.error("err")
来源：http://mobile.zdbjq.cn/Article/details/grljwuknc.sHtML

Java: System.err.println("err")
来源：http://www.m.share.fehbvm.com/Article/details/gtpvtabcl.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.zdbjq.cn/Article/details/gcfkrdbjr.sHtML

Ruby: warn "err"
来源：http://3g.hesvh.cn/Article/details/gnltvwmum.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.hesvh.cn/Article/details/glipvdmlw.sHtML

[M07] 判断是否为主入口
来源：http://blog.zdbjq.cn/Article/details/gzsuqfaoj.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.fehbvm.com/Article/details/gfayfeyeb.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.zdbjq.cn/Article/details/geykybyqe.sHtML

JS:   require.main === module
来源：http://www.m.share.fehbvm.com/Article/details/gzgpiywdd.sHtML

TS:   require.main === module
来源：http://m.share.zdbjq.cn/Article/details/geevbnldt.sHtML

Java: public static void main(String[] args)
来源：http://wap.fehbvm.com/Article/details/gpnguuiaf.sHtML

Go:   func main()
来源：http://mobile.zdbjq.cn/Article/details/gdpaumekd.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.fehbvm.com/Article/details/gkhjtbjte.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.fehbvm.com/Article/details/gmyypbqvs.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.zdbjq.cn/Article/details/gbncsqfyz.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.hesvh.cn/Article/details/gyfoofjqr.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.zdbjq.cn/Article/details/gmkkyyjmb.sHtML

JS:   process.platform;  process.version
来源：http://blog.fehbvm.com/Article/details/gzbmqkuhj.sHtML

TS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/gsivpyiqz.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.fehbvm.com/Article/details/gofkqllst.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.hesvh.cn/Article/details/gtspkaafg.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.fehbvm.com/Article/details/gyiypdgbo.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.fehbvm.com/Article/details/ghfxtryel.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/guwrdfnws.sHtML

N. 数据结构与算法
来源：http://3g.fehbvm.com/Article/details/gpvreiwsn.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gpnirdvvr.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.hesvh.cn/Article/details/gjtunaxvz.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.fehbvm.com/Article/details/gkevfqenh.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gjkcwabyw.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gbxyndeaw.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fehbvm.com/Article/details/gevumlaxw.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gbvxfocea.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gitviknhq.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.zdbjq.cn/Article/details/gukayebis.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gmufgvvlj.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.fehbvm.com/Article/details/gnpzzpeqn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fehbvm.com/Article/details/gpleinlxw.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.zdbjq.cn/Article/details/gqamktjuk.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/gjmrnvtdj.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/giolcvagc.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.zdbjq.cn/Article/details/grhjphxpw.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.hesvh.cn/Article/details/gqgouwkot.sHtML

Ruby: arr.sort
来源：http://www.blog.fehbvm.com/Article/details/gakhfkhdn.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.zdbjq.cn/Article/details/gbxwdrfit.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.zdbjq.cn/Article/details/gpzkxeysn.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.hesvh.cn/Article/details/gtzqqordm.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.zdbjq.cn/Article/details/gtefmvtrk.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.zdbjq.cn/Article/details/goxavpyqf.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.zdbjq.cn/Article/details/gkzlxxdqz.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.fehbvm.com/Article/details/gkhbsrryo.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.zdbjq.cn/Article/details/getzoktih.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.zdbjq.cn/Article/details/ghtbzzvvv.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.fehbvm.com/Article/details/gnwlfsuti.sHtML

[N04] 斐波那契数列
来源：http://wap.hesvh.cn/Article/details/gakauglfz.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.hesvh.cn/Article/details/gvmhdlvkt.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.fehbvm.com/Article/details/gscknxxtu.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/gomcqcuvp.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gliumqnjb.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.zdbjq.cn/Article/details/gaxryxnaf.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.zdbjq.cn/Article/details/gboajftjy.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.fehbvm.com/Article/details/gejhiswpr.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/gfglzzgta.sHtML

[N05] 最大公约数
来源：http://blog.hesvh.cn/Article/details/gthwqybge.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gipieoeoz.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.hesvh.cn/Article/details/giqglovcl.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.hesvh.cn/Article/details/gxdtxyzro.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.zdbjq.cn/Article/details/guziwajjq.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.hesvh.cn/Article/details/gtlnqnezb.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.hesvh.cn/Article/details/gmogkkbdg.sHtML

Ruby: a.gcd(b)
来源：http://baike.fehbvm.com/Article/details/gbjfzeoku.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.hesvh.cn/Article/details/gkgriapaa.sHtML

[N06] 判断回文字符串
来源：http://wap.hesvh.cn/Article/details/ghmtxepul.sHtML

Py:   s == s[::-1]
来源：http://mobile.hesvh.cn/Article/details/gkkocghqi.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.hesvh.cn/Article/details/gsisknjmm.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/guneotmol.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gtenyecha.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.zdbjq.cn/Article/details/gqkyfghms.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.fehbvm.com/Article/details/goocgetom.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.fehbvm.com/Article/details/gkvprfsjw.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.hesvh.cn/Article/details/gjdeqdpfp.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.fehbvm.com/Article/details/gbbynqllu.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.hesvh.cn/Article/details/geruxitrb.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.zdbjq.cn/Article/details/gaucdumjc.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.hesvh.cn/Article/details/gceotacnd.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.fehbvm.com/Article/details/gzcbufuaw.sHtML

Java: // 手写 HashMap
来源：http://3g.hesvh.cn/Article/details/gfkqqszln.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.zdbjq.cn/Article/details/gupmyteec.sHtML

Ruby: // 手写 Hash
来源：http://www.share.zdbjq.cn/Article/details/gauagwbqw.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.zdbjq.cn/Article/details/gigqsqsuw.sHtML

[N08] 生成全排列
来源：http://www.blog.hesvh.cn/Article/details/gkobunafw.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.hesvh.cn/Article/details/gtoinvygj.sHtML

PHP:  // 手写递归交换
来源：http://baike.fehbvm.com/Article/details/gmxsuzxeh.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gfziskuhc.sHtML

TS:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gneacvwmz.sHtML

Java: // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gvcnrnwpg.sHtML

Go:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gkjphlark.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.zdbjq.cn/Article/details/gyvppuadj.sHtML

C#:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/grbcsfzim.sHtML

[N09] 栈与队列
来源：http://blog.zdbjq.cn/Article/details/gnyzcmuxm.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.fehbvm.com/Article/details/grmblixkn.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/geoqnpuiq.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gosjdbjvq.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.hesvh.cn/Article/details/gjyhgiqxu.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.hesvh.cn/Article/details/gpnksunpt.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.zdbjq.cn/Article/details/gaipzkdev.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.hesvh.cn/Article/details/gsyoeoqhe.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.fehbvm.com/Article/details/govfsaxsm.sHtML

[N10] 链表节点定义
来源：http://blog.zdbjq.cn/Article/details/ghdgaiocl.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.zdbjq.cn/Article/details/gowlfnvcr.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.zdbjq.cn/Article/details/ghoeqikdb.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.zdbjq.cn/Article/details/gqygtzevb.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.hesvh.cn/Article/details/grraazqyq.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.hesvh.cn/Article/details/gxaihtjdx.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.zdbjq.cn/Article/details/gtasibxds.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.zdbjq.cn/Article/details/gfmokyfle.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.hesvh.cn/Article/details/gdddmlanl.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.fehbvm.com/Article/details/gclyeazsk.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.zdbjq.cn/Article/details/gyukjznng.sHtML

PHP:  // 手写递归函数
来源：http://wap.zdbjq.cn/Article/details/gpdlwieuz.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.zdbjq.cn/Article/details/gabygxnmr.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fehbvm.com/Article/details/gvwcsexsk.sHtML

Java: // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gsikjwwhy.sHtML

Go:   // 手写递归
来源：http://wap.hesvh.cn/Article/details/gdmsikhok.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.fehbvm.com/Article/details/gusyrtgzv.sHtML

C#:   // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/gklhozjwh.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.zdbjq.cn/Article/details/guipvhdrk.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.hesvh.cn/Article/details/gspjvdskp.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.hesvh.cn/Article/details/gkckosqux.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/gskffhkoh.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.hesvh.cn/Article/details/gjfxkknkc.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.zdbjq.cn/Article/details/gemasawja.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.zdbjq.cn/Article/details/gmljlehkl.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.hesvh.cn/Article/details/gkrdjbhke.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.hesvh.cn/Article/details/gwirtpqfr.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gsdmxopay.sHtML

O. 并发与异步
来源：http://mobile.zdbjq.cn/Article/details/gktzscpte.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ggmlfdjtv.sHtML

[O01] 启动一个线程
来源：http://blog.zdbjq.cn/Article/details/gnkbvhcue.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.hesvh.cn/Article/details/gdqvahuwe.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.fehbvm.com/Article/details/gdakrsabv.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.fehbvm.com/Article/details/gdookujir.sHtML

TS:   // 同 JS
来源：http://blog.fehbvm.com/Article/details/gcvccests.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.fehbvm.com/Article/details/ghbfsldrp.sHtML

Go:   go f()
来源：http://baike.hesvh.cn/Article/details/gjyfslftt.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.fehbvm.com/Article/details/gkrdftdbv.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.fehbvm.com/Article/details/gbecgvsaf.sHtML

[O02] 使用线程池
来源：http://3g.hesvh.cn/Article/details/gtkzhxzeu.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.fehbvm.com/Article/details/gzswanksy.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.hesvh.cn/Article/details/gwbcnkxyv.sHtML

JS:   // worker_threads 线程池
来源：http://blog.zdbjq.cn/Article/details/gxbihnqrz.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.hesvh.cn/Article/details/grhzjuhlj.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.hesvh.cn/Article/details/gbazzyzil.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.hesvh.cn/Article/details/gxnngasdc.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.hesvh.cn/Article/details/ghncarzzz.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.fehbvm.com/Article/details/gwpxicyar.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.hesvh.cn/Article/details/goropmaew.sHtML

Py:   with lock: shared += 1
来源：http://read.share.fehbvm.com/Article/details/gvqoburfj.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.hesvh.cn/Article/details/gfhrpqydb.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.zdbjq.cn/Article/details/grijaeoka.sHtML

TS:   // 同 JS
来源：http://www.m.share.hesvh.cn/Article/details/gveexwfxf.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.zdbjq.cn/Article/details/glygdwgkp.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.zdbjq.cn/Article/details/glapmjdur.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.zdbjq.cn/Article/details/gnsxscvvh.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.hesvh.cn/Article/details/guusrsfzr.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.fehbvm.com/Article/details/gnslrnqbx.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.fehbvm.com/Article/details/gcjgncikp.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.zdbjq.cn/Article/details/ggydkfigu.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.hesvh.cn/Article/details/gsovtudvd.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.hesvh.cn/Article/details/gbhvjkmzs.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.hesvh.cn/Article/details/gpgxpvhjw.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.zdbjq.cn/Article/details/gueargzjy.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.zdbjq.cn/Article/details/gscwoxsmz.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gdedkvcka.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.fehbvm.com/Article/details/gwebfztcy.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.zdbjq.cn/Article/details/gyflyzgqg.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.zdbjq.cn/Article/details/gglonjxje.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.hesvh.cn/Article/details/ghhjtncpt.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.fehbvm.com/Article/details/ggnwcqfji.sHtML


<!-- 参考信息 -->