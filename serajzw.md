代发 wailian999

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.hesvh.cn/Article/details/goxrlkuxa.sHtML

JS:   await fetch(url)
来源：http://m.share.fehbvm.com/Article/details/gaisniypm.sHtML

TS:   await fetch(url)
来源：http://read.share.fehbvm.com/Article/details/ghumnqodl.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.hesvh.cn/Article/details/gpaqyelzq.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.hesvh.cn/Article/details/gubentslc.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.hesvh.cn/Article/details/gpvurmrbo.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.fehbvm.com/Article/details/gmhgywdwr.sHtML

[L02] 发送 POST JSON
来源：http://mobile.zdbjq.cn/Article/details/gaatkdcfu.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.zdbjq.cn/Article/details/gwdrqjthp.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.hesvh.cn/Article/details/gfpnigryy.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.fehbvm.com/Article/details/gtadxqxiw.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.zdbjq.cn/Article/details/gbhcggsva.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.hesvh.cn/Article/details/gjnbeoknv.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.zdbjq.cn/Article/details/gaylikckt.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.hesvh.cn/Article/details/gbikchplq.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.fehbvm.com/Article/details/gmgapgiye.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.zdbjq.cn/Article/details/gllmsfqoe.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.hesvh.cn/Article/details/gqgbhcgis.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.hesvh.cn/Article/details/gtgrtyqoh.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.zdbjq.cn/Article/details/gevylcjym.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.fehbvm.com/Article/details/gfwialzug.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.fehbvm.com/Article/details/gmptxjsvv.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.fehbvm.com/Article/details/guqoaulve.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.hesvh.cn/Article/details/gemrtewbd.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.hesvh.cn/Article/details/giimysodl.sHtML

[L04] 设置超时
来源：http://m.share.hesvh.cn/Article/details/ggzqmjgbd.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.hesvh.cn/Article/details/gndplplra.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.fehbvm.com/Article/details/gvuorjhkh.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.zdbjq.cn/Article/details/gchoqzbuq.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.fehbvm.com/Article/details/getrxdjtx.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.zdbjq.cn/Article/details/gloqxfage.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.hesvh.cn/Article/details/gtnuxnwjx.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.hesvh.cn/Article/details/gvausprbp.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.hesvh.cn/Article/details/gsszwzugm.sHtML

[L05] 上传文件（multipart）
来源：http://baike.fehbvm.com/Article/details/gewdgcack.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.zdbjq.cn/Article/details/gwitatlnz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.zdbjq.cn/Article/details/gueznyfie.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.hesvh.cn/Article/details/gdlugphcs.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.zdbjq.cn/Article/details/gkxhotvse.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.zdbjq.cn/Article/details/gtzwtyaog.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.zdbjq.cn/Article/details/gnodktzns.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.fehbvm.com/Article/details/ghaibhxep.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.hesvh.cn/Article/details/gskqrwxaj.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.zdbjq.cn/Article/details/guudqehoc.sHtML

Py:   resp.json()
来源：http://blog.fehbvm.com/Article/details/gavfdmqmy.sHtML

PHP:  json_decode($body, true);
来源：http://baike.fehbvm.com/Article/details/gwsgerejj.sHtML

JS:   await resp.json()
来源：http://wap.fehbvm.com/Article/details/gfwaabppj.sHtML

TS:   await resp.json()
来源：http://read.share.zdbjq.cn/Article/details/gexotokqq.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.fehbvm.com/Article/details/gbzsdxgfm.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.zdbjq.cn/Article/details/gompfvxrk.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.zdbjq.cn/Article/details/gmrhnnnmh.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.hesvh.cn/Article/details/grelpkycn.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.hesvh.cn/Article/details/gcaewdngs.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.hesvh.cn/Article/details/gkidcpoge.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.zdbjq.cn/Article/details/gcueozdpk.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.fehbvm.com/Article/details/gublxgpjf.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.zdbjq.cn/Article/details/gehxwxgku.sHtML

Java: resp.statusCode()
来源：http://read.share.fehbvm.com/Article/details/gvrvvqfhd.sHtML

Go:   resp.StatusCode
来源：http://www.blog.fehbvm.com/Article/details/gsznyxrkl.sHtML

Ruby: resp.code.to_i
来源：http://read.share.zdbjq.cn/Article/details/gmnwgplxr.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.zdbjq.cn/Article/details/guxxephgg.sHtML

[L08] 并发请求多个地址
来源：http://www.share.fehbvm.com/Article/details/gtkrrtybj.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.hesvh.cn/Article/details/gvkxrtpbk.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.zdbjq.cn/Article/details/gyrvdfzff.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/gwleapcrc.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.hesvh.cn/Article/details/gvrxfhtyw.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.fehbvm.com/Article/details/ggutvdcsx.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.hesvh.cn/Article/details/gphiwayye.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.hesvh.cn/Article/details/gdouckgpk.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.fehbvm.com/Article/details/gbuaoyocf.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gezemsbno.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.fehbvm.com/Article/details/gszmiiszt.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gzwiqrwjg.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.fehbvm.com/Article/details/gzmmmibaj.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.fehbvm.com/Article/details/gabjmlbwx.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.zdbjq.cn/Article/details/gammmcwbt.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.zdbjq.cn/Article/details/gibsndbzv.sHtML

TS:   process.argv.slice(2)
来源：http://baike.hesvh.cn/Article/details/gszwufcow.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.hesvh.cn/Article/details/gzhytqhie.sHtML

Go:   os.Args[1:]
来源：http://wap.fehbvm.com/Article/details/glbkxqotc.sHtML

Ruby: ARGV
来源：http://baike.zdbjq.cn/Article/details/gafrpfjdl.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.fehbvm.com/Article/details/gvfnqpzze.sHtML

[M02] 读取环境变量
来源：http://m.share.fehbvm.com/Article/details/glbschgys.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.hesvh.cn/Article/details/gxujmwdim.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.zdbjq.cn/Article/details/gfhzekxrz.sHtML

JS:   process.env.HOME
来源：http://wap.fehbvm.com/Article/details/gwcdieaeh.sHtML

TS:   process.env.HOME
来源：http://m.share.zdbjq.cn/Article/details/gvurjjkta.sHtML

Java: System.getenv("HOME")
来源：http://read.share.fehbvm.com/Article/details/ganxhpmon.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gesgjthxt.sHtML

Ruby: ENV["HOME"]
来源：http://wap.zdbjq.cn/Article/details/gyeujsuxq.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.hesvh.cn/Article/details/guzcqjdlm.sHtML

[M03] 执行外部命令
来源：http://mobile.zdbjq.cn/Article/details/gfqitkrkm.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.hesvh.cn/Article/details/ggkgngkjt.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.zdbjq.cn/Article/details/gzpjfjvgo.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.hesvh.cn/Article/details/genhroaii.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.fehbvm.com/Article/details/gzmcqouvt.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.fehbvm.com/Article/details/gtzdxiahq.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.zdbjq.cn/Article/details/gftdcmnfo.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.hesvh.cn/Article/details/gehkeubdr.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.fehbvm.com/Article/details/gzoxnsalb.sHtML

[M04] 获取当前工作目录
来源：http://wap.hesvh.cn/Article/details/gfzjoowfu.sHtML

Py:   os.getcwd()
来源：http://blog.fehbvm.com/Article/details/gerutmbwx.sHtML

PHP:  getcwd();
来源：http://read.share.zdbjq.cn/Article/details/gxadjokvk.sHtML

JS:   process.cwd()
来源：http://www.blog.fehbvm.com/Article/details/gqqfggvsh.sHtML

TS:   process.cwd()
来源：http://www.blog.fehbvm.com/Article/details/grshehpah.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.fehbvm.com/Article/details/gxkcnzwji.sHtML

Go:   os.Getwd()
来源：http://baike.hesvh.cn/Article/details/gwqdedyvo.sHtML

Ruby: Dir.pwd
来源：http://m.share.zdbjq.cn/Article/details/gdwqkatml.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.hesvh.cn/Article/details/glaapdzbp.sHtML

[M05] 设置退出码
来源：http://wap.fehbvm.com/Article/details/gvtbodgcy.sHtML

Py:   sys.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gvlyhqsma.sHtML

PHP:  exit(1);
来源：http://wap.zdbjq.cn/Article/details/gqrndkkft.sHtML

JS:   process.exit(1)
来源：http://baike.hesvh.cn/Article/details/ganjdctxz.sHtML

TS:   process.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gwyzadeey.sHtML

Java: System.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/glcwzjgce.sHtML

Go:   os.Exit(1)
来源：http://blog.fehbvm.com/Article/details/gaxxavedw.sHtML

Ruby: exit 1
来源：http://read.share.zdbjq.cn/Article/details/gvfisfvht.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.zdbjq.cn/Article/details/gjjwyyacg.sHtML

[M06] 向标准错误输出
来源：http://www.blog.fehbvm.com/Article/details/gubhcecks.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.hesvh.cn/Article/details/gkmvnghvz.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.zdbjq.cn/Article/details/gusxkrkbi.sHtML

JS:   console.error("err")
来源：http://blog.hesvh.cn/Article/details/gynlaryno.sHtML

TS:   console.error("err")
来源：http://baike.zdbjq.cn/Article/details/girpzeojg.sHtML

Java: System.err.println("err")
来源：http://read.share.fehbvm.com/Article/details/gxkuyirvy.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.zdbjq.cn/Article/details/gnanvcyma.sHtML

Ruby: warn "err"
来源：http://wap.zdbjq.cn/Article/details/ggwqrezzg.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.zdbjq.cn/Article/details/gazgnxthv.sHtML

[M07] 判断是否为主入口
来源：http://3g.hesvh.cn/Article/details/gdgjgmbtb.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.hesvh.cn/Article/details/gvezzehar.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.fehbvm.com/Article/details/gxgrwscjd.sHtML

JS:   require.main === module
来源：http://3g.hesvh.cn/Article/details/ggmaemtfh.sHtML

TS:   require.main === module
来源：http://www.blog.zdbjq.cn/Article/details/gevjzwloi.sHtML

Java: public static void main(String[] args)
来源：http://wap.hesvh.cn/Article/details/grtuqvqil.sHtML

Go:   func main()
来源：http://www.share.fehbvm.com/Article/details/gbxkoiwcw.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.hesvh.cn/Article/details/glejwszeo.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.hesvh.cn/Article/details/gmhawkder.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.fehbvm.com/Article/details/gvqmnylkb.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.zdbjq.cn/Article/details/gjwqswccb.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.hesvh.cn/Article/details/gbefndtoy.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.fehbvm.com/Article/details/gtwydhytu.sHtML

TS:   process.platform;  process.version
来源：http://www.share.zdbjq.cn/Article/details/ghbvbfgiq.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.hesvh.cn/Article/details/gqyiyijix.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.fehbvm.com/Article/details/glovqleaa.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.fehbvm.com/Article/details/ghbcbzyob.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.zdbjq.cn/Article/details/gptpfroeh.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gqwsmnebo.sHtML

N. 数据结构与算法
来源：http://www.blog.hesvh.cn/Article/details/gnlnhpjgd.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gxcdtnkoa.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.hesvh.cn/Article/details/gptqomqda.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gioyfifaf.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.fehbvm.com/Article/details/goijrfdof.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.hesvh.cn/Article/details/gogznsrtj.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.hesvh.cn/Article/details/gwyaeoddp.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gllkucdys.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.fehbvm.com/Article/details/gaqdrrtds.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.zdbjq.cn/Article/details/gfjuqoylf.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gkmyrkjok.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.fehbvm.com/Article/details/gsaoeyogy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fehbvm.com/Article/details/gamzpfmlk.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.fehbvm.com/Article/details/gsahmpebz.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/gpxfeqfua.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/gfethoveb.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.hesvh.cn/Article/details/glrdhjqow.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.fehbvm.com/Article/details/gqvwhfyyw.sHtML

Ruby: arr.sort
来源：http://blog.zdbjq.cn/Article/details/gnqjqxxcr.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.fehbvm.com/Article/details/gggbeopxu.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.zdbjq.cn/Article/details/gwoyzjvnq.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.fehbvm.com/Article/details/gljnrgjak.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.zdbjq.cn/Article/details/gtnnrhvih.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.zdbjq.cn/Article/details/gjzrjxghj.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.hesvh.cn/Article/details/gdtlhxaxd.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.zdbjq.cn/Article/details/gqejeyvqf.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.hesvh.cn/Article/details/gpxftmnrt.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.fehbvm.com/Article/details/gqxukxsbh.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.fehbvm.com/Article/details/gvriytexu.sHtML

[N04] 斐波那契数列
来源：http://m.share.hesvh.cn/Article/details/gvbqafmiu.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/gsoopxvye.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.zdbjq.cn/Article/details/gvvggkomu.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gnsiacldb.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/gnmrqsqow.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.zdbjq.cn/Article/details/griofexsf.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.hesvh.cn/Article/details/gczapxywd.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.hesvh.cn/Article/details/gqmugjitv.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/gyxxoqgoq.sHtML

[N05] 最大公约数
来源：http://www.blog.hesvh.cn/Article/details/gkwoindkn.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/gguzxvgzb.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.hesvh.cn/Article/details/gzxwsqsmv.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fehbvm.com/Article/details/gmmfwlpjw.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fehbvm.com/Article/details/gzjrnkghy.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.zdbjq.cn/Article/details/gkulttekq.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.fehbvm.com/Article/details/gjpypkqsu.sHtML

Ruby: a.gcd(b)
来源：http://mobile.zdbjq.cn/Article/details/ggfemyuti.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.hesvh.cn/Article/details/givxohgdk.sHtML

[N06] 判断回文字符串
来源：http://baike.fehbvm.com/Article/details/gaswxotoi.sHtML

Py:   s == s[::-1]
来源：http://www.blog.zdbjq.cn/Article/details/gsfxpetci.sHtML

PHP:  $s === strrev($s);
来源：http://baike.zdbjq.cn/Article/details/gkeqnamzo.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gwoyfnhug.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gjzyztlbw.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.zdbjq.cn/Article/details/gksbsiqnx.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.fehbvm.com/Article/details/gqxryocxe.sHtML

Ruby: s == s.reverse
来源：http://blog.hesvh.cn/Article/details/gnjmarqez.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.hesvh.cn/Article/details/gdxlzssbm.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.zdbjq.cn/Article/details/gcxjspspw.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.hesvh.cn/Article/details/ghhrwnedl.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.zdbjq.cn/Article/details/guucchemp.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.zdbjq.cn/Article/details/gvaoyiomw.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.hesvh.cn/Article/details/gihryamwi.sHtML

Java: // 手写 HashMap
来源：http://m.share.fehbvm.com/Article/details/gqcvsvcff.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.hesvh.cn/Article/details/gvptzirsq.sHtML

Ruby: // 手写 Hash
来源：http://read.share.zdbjq.cn/Article/details/gptrcnpwu.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.zdbjq.cn/Article/details/gohkwqliw.sHtML

[N08] 生成全排列
来源：http://3g.zdbjq.cn/Article/details/gokxesxrl.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.zdbjq.cn/Article/details/gplbhatsv.sHtML

PHP:  // 手写递归交换
来源：http://wap.fehbvm.com/Article/details/gbwdjtcxp.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gqsdbymwp.sHtML

TS:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gocipfzca.sHtML

Java: // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gushrflts.sHtML

Go:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gnynitzaf.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.fehbvm.com/Article/details/gbrcxnsbl.sHtML

C#:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gacsqismz.sHtML

[N09] 栈与队列
来源：http://baike.hesvh.cn/Article/details/gvoxvsmkc.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.zdbjq.cn/Article/details/gloswzfyj.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.fehbvm.com/Article/details/gduttickb.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gsheygwka.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.hesvh.cn/Article/details/gpmkdgxei.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.hesvh.cn/Article/details/gcnbezozl.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.zdbjq.cn/Article/details/gdsqtxzcm.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.hesvh.cn/Article/details/gkprpfgnt.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.fehbvm.com/Article/details/gnkiodicv.sHtML

[N10] 链表节点定义
来源：http://read.share.hesvh.cn/Article/details/gngvorpor.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.hesvh.cn/Article/details/gufwrfnke.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.fehbvm.com/Article/details/gpobasbky.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.fehbvm.com/Article/details/gusxklllw.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.hesvh.cn/Article/details/gmiemllpt.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.fehbvm.com/Article/details/gzjqtchzb.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.hesvh.cn/Article/details/gwfiorzix.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.zdbjq.cn/Article/details/gqcmbkwkj.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.fehbvm.com/Article/details/gfgwsuptc.sHtML

[N11] 二叉树中序遍历
来源：http://baike.fehbvm.com/Article/details/grrupunfh.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.hesvh.cn/Article/details/gnyxjhqto.sHtML

PHP:  // 手写递归函数
来源：http://m.share.fehbvm.com/Article/details/gierjgnit.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.zdbjq.cn/Article/details/gbsgtgogt.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.hesvh.cn/Article/details/gcynthydz.sHtML

Java: // 手写递归
来源：http://read.share.hesvh.cn/Article/details/gphdqlzjl.sHtML

Go:   // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gmlgcwycs.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.hesvh.cn/Article/details/gykzaqhfm.sHtML

C#:   // 手写递归
来源：http://read.share.hesvh.cn/Article/details/gypdqbaia.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.fehbvm.com/Article/details/girjsttxx.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.zdbjq.cn/Article/details/gycnvbknv.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.zdbjq.cn/Article/details/gjqpuwujm.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.zdbjq.cn/Article/details/gdqlzdzls.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fehbvm.com/Article/details/gldzjiohw.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.hesvh.cn/Article/details/gqrhcesfv.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.hesvh.cn/Article/details/gyfnjjkqq.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/gltvxhwjy.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.hesvh.cn/Article/details/ggovmllbi.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gyxrxhytn.sHtML

O. 并发与异步
来源：http://wap.hesvh.cn/Article/details/gtfgtobnz.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gwvireyll.sHtML

[O01] 启动一个线程
来源：http://3g.zdbjq.cn/Article/details/gnouxzimr.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.fehbvm.com/Article/details/gvlpfqmpx.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.hesvh.cn/Article/details/glhgznibe.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.hesvh.cn/Article/details/gelfmroun.sHtML

TS:   // 同 JS
来源：http://www.blog.fehbvm.com/Article/details/gztdirphr.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.fehbvm.com/Article/details/gihyvoolb.sHtML

Go:   go f()
来源：http://3g.zdbjq.cn/Article/details/gshuijbfw.sHtML

Ruby: Thread.new { f }
来源：http://wap.zdbjq.cn/Article/details/gnhwgrbhj.sHtML

C#:   Task.Run(() => F());
来源：http://baike.zdbjq.cn/Article/details/gyejfnwpm.sHtML

[O02] 使用线程池
来源：http://mobile.hesvh.cn/Article/details/guzsvbwzd.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.fehbvm.com/Article/details/gryhytpym.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.hesvh.cn/Article/details/gucpzbhsw.sHtML

JS:   // worker_threads 线程池
来源：http://wap.fehbvm.com/Article/details/gppmxvnqh.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.fehbvm.com/Article/details/grfuhnvml.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.zdbjq.cn/Article/details/gzutoiupi.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.fehbvm.com/Article/details/gozibzogo.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.zdbjq.cn/Article/details/gamuggkjc.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.hesvh.cn/Article/details/gkosmzhkt.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.zdbjq.cn/Article/details/guuxiujwy.sHtML

Py:   with lock: shared += 1
来源：http://wap.fehbvm.com/Article/details/ghjvywylq.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.zdbjq.cn/Article/details/geaytsftu.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.zdbjq.cn/Article/details/glzzmvjwr.sHtML

TS:   // 同 JS
来源：http://blog.fehbvm.com/Article/details/gwpfacbaw.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.fehbvm.com/Article/details/gyjjguyot.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.fehbvm.com/Article/details/gifngatam.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.fehbvm.com/Article/details/gknvggjre.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.fehbvm.com/Article/details/gysyvxqtw.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.hesvh.cn/Article/details/govpwiidh.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.hesvh.cn/Article/details/gioarazti.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.hesvh.cn/Article/details/gulqozrqw.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.fehbvm.com/Article/details/gagaxgzsy.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.hesvh.cn/Article/details/gsyaraiog.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.hesvh.cn/Article/details/gqheyxzcc.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.zdbjq.cn/Article/details/gebethqwm.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.zdbjq.cn/Article/details/gonkfniwg.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.hesvh.cn/Article/details/gkclqwzqc.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.zdbjq.cn/Article/details/glbxlejvc.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.fehbvm.com/Article/details/gffgtcemj.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.zdbjq.cn/Article/details/grulkxuuf.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.fehbvm.com/Article/details/glgygjlcr.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.fehbvm.com/Article/details/gkrlwjguw.sHtML


<!-- 参考信息 -->