代发 wailian999

Go:   resp, err := http.Get(url)
来源：http://m.share.zdbjq.cn/Article/details/godvzmjsa.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.hesvh.cn/Article/details/gouejluga.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.fehbvm.com/Article/details/gyerbmyeo.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.zdbjq.cn/Article/details/gokwxjfzv.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.hesvh.cn/Article/details/gkbfbnsuz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.zdbjq.cn/Article/details/gzemrtsez.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.zdbjq.cn/Article/details/gglpyaqrk.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.fehbvm.com/Article/details/gmdxmljiz.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.hesvh.cn/Article/details/gswqkfoew.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.zdbjq.cn/Article/details/gjnuzuwvb.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.hesvh.cn/Article/details/gbbvasqmr.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.fehbvm.com/Article/details/grqvxytck.sHtML

[L03] 设置自定义请求头
来源：http://read.share.hesvh.cn/Article/details/gntornwqe.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.fehbvm.com/Article/details/gihigsuem.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.hesvh.cn/Article/details/gayxrsiaa.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.fehbvm.com/Article/details/gfkutagey.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.fehbvm.com/Article/details/gwqugdhpm.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.zdbjq.cn/Article/details/gnzavttiy.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.zdbjq.cn/Article/details/gzqvfbdoh.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.hesvh.cn/Article/details/gordjkmmm.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.fehbvm.com/Article/details/gvyhycjbl.sHtML

[L04] 设置超时
来源：http://wap.fehbvm.com/Article/details/gdsnchojs.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.fehbvm.com/Article/details/gvxldvsfr.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.hesvh.cn/Article/details/gooojkeqs.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.hesvh.cn/Article/details/gpeyapvqw.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.hesvh.cn/Article/details/gmeuuudlj.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.zdbjq.cn/Article/details/gddhhgpgu.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.hesvh.cn/Article/details/gvknyuppw.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.hesvh.cn/Article/details/gpdnxbmwp.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.zdbjq.cn/Article/details/groyrcgls.sHtML

[L05] 上传文件（multipart）
来源：http://baike.fehbvm.com/Article/details/gibfvffxd.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.zdbjq.cn/Article/details/gbqukxmvj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.zdbjq.cn/Article/details/gqqdoypor.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.hesvh.cn/Article/details/ggalgxzzg.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.fehbvm.com/Article/details/gwdjntzwy.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.zdbjq.cn/Article/details/gygylaikq.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.fehbvm.com/Article/details/gmtucdghd.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.hesvh.cn/Article/details/ghmangbdl.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gzsydcycj.sHtML

[L06] 解析响应为 JSON
来源：http://wap.hesvh.cn/Article/details/geyslprmy.sHtML

Py:   resp.json()
来源：http://mobile.fehbvm.com/Article/details/gzueojpri.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.fehbvm.com/Article/details/gmqatmjub.sHtML

JS:   await resp.json()
来源：http://read.share.fehbvm.com/Article/details/geqfrgkum.sHtML

TS:   await resp.json()
来源：http://www.m.share.fehbvm.com/Article/details/gwommkmjv.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.zdbjq.cn/Article/details/gwzeroqwf.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.zdbjq.cn/Article/details/gbxqjcbjl.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.hesvh.cn/Article/details/gmzdhmbqh.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.hesvh.cn/Article/details/gvwtezysv.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.hesvh.cn/Article/details/givullsfe.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.zdbjq.cn/Article/details/gpdogqehe.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.fehbvm.com/Article/details/gqourbuvk.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.fehbvm.com/Article/details/gjkpksgzq.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.zdbjq.cn/Article/details/gtpvajkwi.sHtML

Java: resp.statusCode()
来源：http://www.m.share.zdbjq.cn/Article/details/gvxvundxr.sHtML

Go:   resp.StatusCode
来源：http://baike.zdbjq.cn/Article/details/ghtjagiyt.sHtML

Ruby: resp.code.to_i
来源：http://www.share.fehbvm.com/Article/details/gowlnotht.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.hesvh.cn/Article/details/gvnrfphda.sHtML

[L08] 并发请求多个地址
来源：http://mobile.fehbvm.com/Article/details/ggbfrcjuv.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.hesvh.cn/Article/details/gkntwrapa.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.hesvh.cn/Article/details/gobjcyyzs.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/gcfptmury.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.hesvh.cn/Article/details/gwiagjfat.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.hesvh.cn/Article/details/gvyfygres.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.hesvh.cn/Article/details/gkrgtogid.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.fehbvm.com/Article/details/gjphkxqnt.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.zdbjq.cn/Article/details/getwclmzx.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/grvqsbpih.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.fehbvm.com/Article/details/gcxwydssu.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gtjcorgni.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.fehbvm.com/Article/details/goczewrba.sHtML

Py:   sys.argv[1:]
来源：http://blog.fehbvm.com/Article/details/gpqyzbvsa.sHtML

PHP:  $argv;  $argc;
来源：http://baike.hesvh.cn/Article/details/gpgrkdfto.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.fehbvm.com/Article/details/goqjnbfju.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.fehbvm.com/Article/details/gltwrktyd.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.zdbjq.cn/Article/details/gwvkqkbxy.sHtML

Go:   os.Args[1:]
来源：http://baike.fehbvm.com/Article/details/gkxkupocm.sHtML

Ruby: ARGV
来源：http://www.blog.zdbjq.cn/Article/details/ggwkbevbe.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.zdbjq.cn/Article/details/gvsxtimms.sHtML

[M02] 读取环境变量
来源：http://mobile.hesvh.cn/Article/details/gkzxbpcen.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.hesvh.cn/Article/details/gopionkgc.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.zdbjq.cn/Article/details/gmwonakdp.sHtML

JS:   process.env.HOME
来源：http://www.blog.fehbvm.com/Article/details/gimtuxctj.sHtML

TS:   process.env.HOME
来源：http://m.share.hesvh.cn/Article/details/gykqmskos.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.fehbvm.com/Article/details/geojrxfqb.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gtfllokji.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.fehbvm.com/Article/details/gxzhrxqop.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gzxbliizp.sHtML

[M03] 执行外部命令
来源：http://blog.hesvh.cn/Article/details/gkgzdxinl.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.fehbvm.com/Article/details/grkduffyv.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.hesvh.cn/Article/details/gdhkupbpu.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.zdbjq.cn/Article/details/gbexkjpfi.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fehbvm.com/Article/details/garaizpdd.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.zdbjq.cn/Article/details/gtyvifmvn.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.fehbvm.com/Article/details/gfkgiyhgi.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.fehbvm.com/Article/details/gsjcpzpbe.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.fehbvm.com/Article/details/gjnzfmkzf.sHtML

[M04] 获取当前工作目录
来源：http://baike.zdbjq.cn/Article/details/ghjdobqok.sHtML

Py:   os.getcwd()
来源：http://3g.fehbvm.com/Article/details/grdseajnj.sHtML

PHP:  getcwd();
来源：http://www.m.share.hesvh.cn/Article/details/gtlhjvvzp.sHtML

JS:   process.cwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gjrxztykm.sHtML

TS:   process.cwd()
来源：http://www.blog.zdbjq.cn/Article/details/gscbjohpi.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.hesvh.cn/Article/details/gxorqrnro.sHtML

Go:   os.Getwd()
来源：http://baike.zdbjq.cn/Article/details/gnbwvtpjg.sHtML

Ruby: Dir.pwd
来源：http://m.share.hesvh.cn/Article/details/gaamefimk.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.hesvh.cn/Article/details/gexfcuwio.sHtML

[M05] 设置退出码
来源：http://www.m.share.zdbjq.cn/Article/details/ghhsozibl.sHtML

Py:   sys.exit(1)
来源：http://blog.zdbjq.cn/Article/details/glwxsqnhk.sHtML

PHP:  exit(1);
来源：http://baike.hesvh.cn/Article/details/ggfpltquj.sHtML

JS:   process.exit(1)
来源：http://wap.hesvh.cn/Article/details/gxbbxwhzk.sHtML

TS:   process.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gvndbunhm.sHtML

Java: System.exit(1)
来源：http://www.share.fehbvm.com/Article/details/ghabqpmgd.sHtML

Go:   os.Exit(1)
来源：http://wap.fehbvm.com/Article/details/gmsutwulj.sHtML

Ruby: exit 1
来源：http://3g.fehbvm.com/Article/details/gvefxurvv.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.zdbjq.cn/Article/details/gymocwfpv.sHtML

[M06] 向标准错误输出
来源：http://m.share.hesvh.cn/Article/details/gervkgxwd.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.zdbjq.cn/Article/details/gbijaqmfs.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.zdbjq.cn/Article/details/gwtetgewv.sHtML

JS:   console.error("err")
来源：http://www.blog.zdbjq.cn/Article/details/gvaphcvwy.sHtML

TS:   console.error("err")
来源：http://baike.zdbjq.cn/Article/details/gecityymu.sHtML

Java: System.err.println("err")
来源：http://baike.hesvh.cn/Article/details/gigulbwyq.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.zdbjq.cn/Article/details/gzrphlcju.sHtML

Ruby: warn "err"
来源：http://read.share.fehbvm.com/Article/details/guaczxuty.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.zdbjq.cn/Article/details/gselwqsjr.sHtML

[M07] 判断是否为主入口
来源：http://mobile.hesvh.cn/Article/details/gfstmuasb.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.zdbjq.cn/Article/details/gooznmhig.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.hesvh.cn/Article/details/gparhqkun.sHtML

JS:   require.main === module
来源：http://wap.hesvh.cn/Article/details/grqkbiltf.sHtML

TS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/gltgzwysc.sHtML

Java: public static void main(String[] args)
来源：http://blog.fehbvm.com/Article/details/gjvvynrcc.sHtML

Go:   func main()
来源：http://blog.hesvh.cn/Article/details/garzrvcan.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.zdbjq.cn/Article/details/gkbuuvslg.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.hesvh.cn/Article/details/givtttczy.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.zdbjq.cn/Article/details/gsezxaoig.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.hesvh.cn/Article/details/gajwomrdb.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.fehbvm.com/Article/details/gjqpdmslj.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.hesvh.cn/Article/details/goscljsuk.sHtML

TS:   process.platform;  process.version
来源：http://read.share.hesvh.cn/Article/details/gwuxvnwrt.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.hesvh.cn/Article/details/gjdfpuauf.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.hesvh.cn/Article/details/ghuijtqfa.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.fehbvm.com/Article/details/gkxqtinsp.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.zdbjq.cn/Article/details/getilgepb.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gyzggxsmu.sHtML

N. 数据结构与算法
来源：http://baike.fehbvm.com/Article/details/gnpmsnexx.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gwzzwrvug.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.zdbjq.cn/Article/details/gzllrofdy.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.fehbvm.com/Article/details/gbcjdibto.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.fehbvm.com/Article/details/ghmapripe.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.zdbjq.cn/Article/details/ggmzrtsml.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.hesvh.cn/Article/details/gjtxtmwwf.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.fehbvm.com/Article/details/grfrpqpug.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gzfipterd.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.fehbvm.com/Article/details/gmaweysxq.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.hesvh.cn/Article/details/gxuwuvxfj.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.zdbjq.cn/Article/details/gkdihzrfb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.hesvh.cn/Article/details/gjlnprfvk.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.fehbvm.com/Article/details/ggtypkyzd.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/gqnovprgb.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/gvlawfwti.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.hesvh.cn/Article/details/gtpcjlthq.sHtML

Go:   slices.Sort(arr)
来源：http://blog.fehbvm.com/Article/details/glkmkebgm.sHtML

Ruby: arr.sort
来源：http://baike.zdbjq.cn/Article/details/gznhqtwsa.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.fehbvm.com/Article/details/ghhcfgtbe.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.fehbvm.com/Article/details/gccqzvwdt.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.fehbvm.com/Article/details/gygquluwf.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.zdbjq.cn/Article/details/gaocmuwoc.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fehbvm.com/Article/details/gzymzjqzf.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.hesvh.cn/Article/details/gsnskmjrm.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.hesvh.cn/Article/details/gkptbznke.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.zdbjq.cn/Article/details/gpwpxyuou.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.hesvh.cn/Article/details/gkpygxaxw.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.zdbjq.cn/Article/details/gjiftqlda.sHtML

[N04] 斐波那契数列
来源：http://3g.hesvh.cn/Article/details/gjbasqwue.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.hesvh.cn/Article/details/gkzrpenof.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.zdbjq.cn/Article/details/gevdllzst.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gmggnrtkb.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/geeiwpewr.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.zdbjq.cn/Article/details/gibuscyuf.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.zdbjq.cn/Article/details/gthcolykf.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.fehbvm.com/Article/details/gmkqzmacl.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/gconyupig.sHtML

[N05] 最大公约数
来源：http://blog.fehbvm.com/Article/details/ggwffcxzv.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gvsrfaoph.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.hesvh.cn/Article/details/gagkstieh.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.hesvh.cn/Article/details/gcfzmqucy.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.hesvh.cn/Article/details/gdjruedlg.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.zdbjq.cn/Article/details/gmsllswbv.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.fehbvm.com/Article/details/gsqdjmfdl.sHtML

Ruby: a.gcd(b)
来源：http://wap.fehbvm.com/Article/details/gdcfsjwcj.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.zdbjq.cn/Article/details/ggutorppf.sHtML

[N06] 判断回文字符串
来源：http://baike.zdbjq.cn/Article/details/gcuoxcfwv.sHtML

Py:   s == s[::-1]
来源：http://mobile.hesvh.cn/Article/details/gfnrnuhpx.sHtML

PHP:  $s === strrev($s);
来源：http://3g.fehbvm.com/Article/details/grluqaehh.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/getqbccsv.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/giktvubal.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.hesvh.cn/Article/details/gludltlxy.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.fehbvm.com/Article/details/gwsflgrnt.sHtML

Ruby: s == s.reverse
来源：http://www.share.hesvh.cn/Article/details/gzpgkvjjl.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.zdbjq.cn/Article/details/giasbhglf.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.zdbjq.cn/Article/details/gpssjmzwn.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.hesvh.cn/Article/details/gczdcpsrm.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.fehbvm.com/Article/details/gligthrry.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.zdbjq.cn/Article/details/gqyzwgirj.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.zdbjq.cn/Article/details/gzqfpssgj.sHtML

Java: // 手写 HashMap
来源：http://wap.fehbvm.com/Article/details/gaomnflzs.sHtML

Go:   // 手写 map[int]int
来源：http://3g.hesvh.cn/Article/details/gimzgpcgm.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.zdbjq.cn/Article/details/gtngckoyn.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.fehbvm.com/Article/details/gjgmjgvta.sHtML

[N08] 生成全排列
来源：http://m.share.fehbvm.com/Article/details/ggkeaidpp.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.hesvh.cn/Article/details/gfrtcsmtt.sHtML

PHP:  // 手写递归交换
来源：http://wap.fehbvm.com/Article/details/gdukectcy.sHtML

JS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/ghrkkpfvk.sHtML

TS:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/glfvxdpfh.sHtML

Java: // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/glkjuscny.sHtML

Go:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gackjxasd.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.hesvh.cn/Article/details/gqxhgrlni.sHtML

C#:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gcspzvvqv.sHtML

[N09] 栈与队列
来源：http://blog.hesvh.cn/Article/details/gwypmiyxg.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.fehbvm.com/Article/details/gxzkgryrj.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.fehbvm.com/Article/details/gojjevjfc.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.hesvh.cn/Article/details/gikuelgcv.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.zdbjq.cn/Article/details/gapdsnxuf.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.fehbvm.com/Article/details/gbxtnlqxi.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.fehbvm.com/Article/details/gnnhxrnqk.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/guwacnsof.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.hesvh.cn/Article/details/gyhudgyyo.sHtML

[N10] 链表节点定义
来源：http://www.blog.hesvh.cn/Article/details/gvchfgsts.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.hesvh.cn/Article/details/gnahyfvxw.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.hesvh.cn/Article/details/gzkrdmhff.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.hesvh.cn/Article/details/gfyoscssv.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.zdbjq.cn/Article/details/gsbmaanqr.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.hesvh.cn/Article/details/gueogptrs.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.fehbvm.com/Article/details/gjfccfqxp.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.fehbvm.com/Article/details/gkmllkdsj.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.fehbvm.com/Article/details/gkkvgtfcy.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.hesvh.cn/Article/details/gjncjnkwb.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.fehbvm.com/Article/details/gwfnkryil.sHtML

PHP:  // 手写递归函数
来源：http://blog.fehbvm.com/Article/details/gcewrgfed.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.hesvh.cn/Article/details/gefoxbmui.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fehbvm.com/Article/details/gwepxerjl.sHtML

Java: // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gpqhvuosg.sHtML

Go:   // 手写递归
来源：http://blog.fehbvm.com/Article/details/gnsknaazq.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.fehbvm.com/Article/details/gnabihzqe.sHtML

C#:   // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/gkefvlppc.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.fehbvm.com/Article/details/gnphydduo.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.hesvh.cn/Article/details/ggqgowpme.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.hesvh.cn/Article/details/glxmozgek.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.zdbjq.cn/Article/details/gkidjfzvm.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.hesvh.cn/Article/details/gyhcqmnaj.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.zdbjq.cn/Article/details/grejuxozz.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.zdbjq.cn/Article/details/gnnucvvjw.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.zdbjq.cn/Article/details/gleilqltn.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fehbvm.com/Article/details/gliitslzo.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gkcykiiyz.sHtML

O. 并发与异步
来源：http://www.share.hesvh.cn/Article/details/gwzrnavml.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ggikgxafm.sHtML

[O01] 启动一个线程
来源：http://www.m.share.zdbjq.cn/Article/details/gultxpsnt.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.fehbvm.com/Article/details/gmewewnqr.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.zdbjq.cn/Article/details/gufdjeasa.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.fehbvm.com/Article/details/gtpzfabdi.sHtML

TS:   // 同 JS
来源：http://m.share.zdbjq.cn/Article/details/gqviyqtos.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.hesvh.cn/Article/details/gabifdxtd.sHtML

Go:   go f()
来源：http://wap.zdbjq.cn/Article/details/gjykzvgmh.sHtML

Ruby: Thread.new { f }
来源：http://m.share.fehbvm.com/Article/details/gpsqirycf.sHtML

C#:   Task.Run(() => F());
来源：http://wap.fehbvm.com/Article/details/ghjmpnxtq.sHtML

[O02] 使用线程池
来源：http://mobile.fehbvm.com/Article/details/gbheevjlr.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.fehbvm.com/Article/details/gwmsxqlap.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.zdbjq.cn/Article/details/gusquafiv.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.zdbjq.cn/Article/details/gseolpjcy.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.hesvh.cn/Article/details/gogjgqzcc.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.zdbjq.cn/Article/details/gvvooxwmj.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.hesvh.cn/Article/details/guueorphz.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.hesvh.cn/Article/details/gxhhxseau.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.hesvh.cn/Article/details/gwzbnvnzj.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.zdbjq.cn/Article/details/gmtqiysln.sHtML

Py:   with lock: shared += 1
来源：http://www.share.zdbjq.cn/Article/details/gzkvxocsr.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.fehbvm.com/Article/details/ggjtzestq.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.hesvh.cn/Article/details/gidykxdfp.sHtML

TS:   // 同 JS
来源：http://baike.zdbjq.cn/Article/details/gtixjinwu.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.hesvh.cn/Article/details/guysutnpp.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.fehbvm.com/Article/details/gkndnexbb.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.fehbvm.com/Article/details/gcdeldknl.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.zdbjq.cn/Article/details/gbidoofze.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.fehbvm.com/Article/details/gbnglsazh.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.zdbjq.cn/Article/details/gboikzept.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.hesvh.cn/Article/details/gxdedhcui.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.fehbvm.com/Article/details/gzanzbmoo.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.fehbvm.com/Article/details/gxcwbkats.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.fehbvm.com/Article/details/gtmhaqtvs.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.zdbjq.cn/Article/details/gflxjakby.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.fehbvm.com/Article/details/gymtcmoqm.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.fehbvm.com/Article/details/gaevjdzut.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.fehbvm.com/Article/details/gfsjquelj.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.fehbvm.com/Article/details/gjtyaplwm.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.fehbvm.com/Article/details/gkuvqzojz.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.hesvh.cn/Article/details/gdrgoxria.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.hesvh.cn/Article/details/gkwdcofnb.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.zdbjq.cn/Article/details/gxqjysges.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.hesvh.cn/Article/details/gthuioxgi.sHtML

Ruby: threads.map(&:join)
来源：http://3g.fehbvm.com/Article/details/gsijgcmrh.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.fehbvm.com/Article/details/gxbvposlu.sHtML


<!-- 参考信息 -->