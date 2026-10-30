代发 wailian999

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.hesvh.cn/Article/details/gdzlkblah.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.fehbvm.com/Article/details/gkzthfvkp.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.zdbjq.cn/Article/details/gssvheyds.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.hesvh.cn/Article/details/gvcpxwngo.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.fehbvm.com/Article/details/goojmfmvz.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.fehbvm.com/Article/details/gtmfswmxl.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.zdbjq.cn/Article/details/ghkdehsjb.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.hesvh.cn/Article/details/gzxkhnzxk.sHtML

[L03] 设置自定义请求头
来源：http://www.share.zdbjq.cn/Article/details/gzkifaogw.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.hesvh.cn/Article/details/gsjvwosts.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.hesvh.cn/Article/details/gqaflsbvk.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.zdbjq.cn/Article/details/gxdontrtz.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.zdbjq.cn/Article/details/gcueadflh.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.fehbvm.com/Article/details/ghvkkeohx.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.fehbvm.com/Article/details/gdonljtdv.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.hesvh.cn/Article/details/gjhmijerm.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.fehbvm.com/Article/details/gzggmxxjq.sHtML

[L04] 设置超时
来源：http://wap.fehbvm.com/Article/details/gpfvmxxuc.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.zdbjq.cn/Article/details/gxipjukae.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.zdbjq.cn/Article/details/gdsuzeasm.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.fehbvm.com/Article/details/gbgauoilo.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.hesvh.cn/Article/details/gpmqpwndl.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.hesvh.cn/Article/details/gksazxuwl.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.zdbjq.cn/Article/details/gskqyglpa.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.fehbvm.com/Article/details/ghodgrewf.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.zdbjq.cn/Article/details/gipxgjztu.sHtML

[L05] 上传文件（multipart）
来源：http://wap.fehbvm.com/Article/details/gqhumoota.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.zdbjq.cn/Article/details/gxguecwuf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.fehbvm.com/Article/details/gtilkapwc.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.fehbvm.com/Article/details/gpijqfsfq.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.fehbvm.com/Article/details/glayvyulz.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.zdbjq.cn/Article/details/ggqundzlb.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.zdbjq.cn/Article/details/giszutmlw.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.zdbjq.cn/Article/details/gjescvmvt.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.zdbjq.cn/Article/details/glbduolnd.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.hesvh.cn/Article/details/glqlvravr.sHtML

Py:   resp.json()
来源：http://m.share.zdbjq.cn/Article/details/gzbuwqzrr.sHtML

PHP:  json_decode($body, true);
来源：http://3g.fehbvm.com/Article/details/ghqhkhhwf.sHtML

JS:   await resp.json()
来源：http://read.share.hesvh.cn/Article/details/gzyhxzddw.sHtML

TS:   await resp.json()
来源：http://blog.fehbvm.com/Article/details/gawaahihr.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.hesvh.cn/Article/details/ghaecucvm.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.zdbjq.cn/Article/details/gujsknqjp.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.zdbjq.cn/Article/details/gjwgfwnmf.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.fehbvm.com/Article/details/gcwrcvdbj.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.hesvh.cn/Article/details/gwpunvhop.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.hesvh.cn/Article/details/gjdgrmztc.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.zdbjq.cn/Article/details/gkejkxfno.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.hesvh.cn/Article/details/gyyzusvvt.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.zdbjq.cn/Article/details/ghxulljkh.sHtML

Java: resp.statusCode()
来源：http://baike.hesvh.cn/Article/details/gwnryghjf.sHtML

Go:   resp.StatusCode
来源：http://mobile.zdbjq.cn/Article/details/gmbhlxnxw.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.zdbjq.cn/Article/details/gnfyrkrgo.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.zdbjq.cn/Article/details/ggunftlqz.sHtML

[L08] 并发请求多个地址
来源：http://3g.zdbjq.cn/Article/details/gapumdlvg.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.fehbvm.com/Article/details/ggthnnfuk.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.hesvh.cn/Article/details/gfuyhcfht.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.zdbjq.cn/Article/details/gowjttbcc.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/glpaeiack.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.hesvh.cn/Article/details/gpfhnwotc.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.fehbvm.com/Article/details/gwcafvine.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.fehbvm.com/Article/details/gicsfmpvs.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gqjwurell.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gzlvberxx.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.fehbvm.com/Article/details/gduzgdrmm.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gifjcqqjp.sHtML

[M01] 读取命令行参数
来源：http://read.share.zdbjq.cn/Article/details/gfvmsuwdf.sHtML

Py:   sys.argv[1:]
来源：http://m.share.zdbjq.cn/Article/details/gjnaxoibz.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.hesvh.cn/Article/details/gxsrcqudh.sHtML

JS:   process.argv.slice(2)
来源：http://wap.zdbjq.cn/Article/details/gmiotllst.sHtML

TS:   process.argv.slice(2)
来源：http://wap.fehbvm.com/Article/details/gedfqqfmb.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.fehbvm.com/Article/details/guanqdosh.sHtML

Go:   os.Args[1:]
来源：http://baike.zdbjq.cn/Article/details/gaebqvaqt.sHtML

Ruby: ARGV
来源：http://www.blog.fehbvm.com/Article/details/gnmunlvdx.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.hesvh.cn/Article/details/gaghjcstu.sHtML

[M02] 读取环境变量
来源：http://mobile.fehbvm.com/Article/details/gfcdbxhlk.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.zdbjq.cn/Article/details/gcyuedmlo.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.zdbjq.cn/Article/details/gwhwsupwu.sHtML

JS:   process.env.HOME
来源：http://wap.hesvh.cn/Article/details/ghibeuaic.sHtML

TS:   process.env.HOME
来源：http://blog.hesvh.cn/Article/details/genrqawhh.sHtML

Java: System.getenv("HOME")
来源：http://www.share.fehbvm.com/Article/details/gdqfasjeb.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gsqajycjp.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.zdbjq.cn/Article/details/gvwakqnsv.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.fehbvm.com/Article/details/gokrhomsi.sHtML

[M03] 执行外部命令
来源：http://read.share.zdbjq.cn/Article/details/gbvfcamrl.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.hesvh.cn/Article/details/gzecscygm.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.hesvh.cn/Article/details/gzytkpeiu.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.zdbjq.cn/Article/details/gkbenusun.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.hesvh.cn/Article/details/getbwnrrw.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.fehbvm.com/Article/details/gkkubyvby.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.fehbvm.com/Article/details/ghawrhapa.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.fehbvm.com/Article/details/gvtuzdsqn.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.fehbvm.com/Article/details/getkhmsff.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.hesvh.cn/Article/details/gagqgxgyp.sHtML

Py:   os.getcwd()
来源：http://www.share.zdbjq.cn/Article/details/goashxaxd.sHtML

PHP:  getcwd();
来源：http://blog.fehbvm.com/Article/details/gyknoasvd.sHtML

JS:   process.cwd()
来源：http://mobile.zdbjq.cn/Article/details/ghowfcyiy.sHtML

TS:   process.cwd()
来源：http://baike.hesvh.cn/Article/details/ggipzspfd.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.zdbjq.cn/Article/details/gvphjfhqb.sHtML

Go:   os.Getwd()
来源：http://www.blog.hesvh.cn/Article/details/gzbxljhkw.sHtML

Ruby: Dir.pwd
来源：http://baike.zdbjq.cn/Article/details/ghsuybzfq.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.fehbvm.com/Article/details/gchbsepbg.sHtML

[M05] 设置退出码
来源：http://m.share.fehbvm.com/Article/details/gdfqiqaji.sHtML

Py:   sys.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gofhgvida.sHtML

PHP:  exit(1);
来源：http://m.share.fehbvm.com/Article/details/gfavgtyla.sHtML

JS:   process.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gymhdwunr.sHtML

TS:   process.exit(1)
来源：http://3g.hesvh.cn/Article/details/gptzyfyrt.sHtML

Java: System.exit(1)
来源：http://wap.hesvh.cn/Article/details/gyuvtkukn.sHtML

Go:   os.Exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gljiqkuyl.sHtML

Ruby: exit 1
来源：http://www.blog.fehbvm.com/Article/details/gpofwqclx.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.zdbjq.cn/Article/details/gbxbcmrkq.sHtML

[M06] 向标准错误输出
来源：http://wap.hesvh.cn/Article/details/gxtjbupxm.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.hesvh.cn/Article/details/gqjersync.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.fehbvm.com/Article/details/grzmlicuz.sHtML

JS:   console.error("err")
来源：http://read.share.hesvh.cn/Article/details/goimmpcew.sHtML

TS:   console.error("err")
来源：http://m.share.hesvh.cn/Article/details/ghofgzdeb.sHtML

Java: System.err.println("err")
来源：http://baike.zdbjq.cn/Article/details/gbgorottz.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.fehbvm.com/Article/details/gfmzsmqzu.sHtML

Ruby: warn "err"
来源：http://wap.zdbjq.cn/Article/details/gjtapvdwl.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.hesvh.cn/Article/details/gjruufubk.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.zdbjq.cn/Article/details/ggzwuqnkk.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.hesvh.cn/Article/details/gppkjciak.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.zdbjq.cn/Article/details/ggrlvocvj.sHtML

JS:   require.main === module
来源：http://baike.fehbvm.com/Article/details/goulxnzmj.sHtML

TS:   require.main === module
来源：http://baike.zdbjq.cn/Article/details/grbcjljbr.sHtML

Java: public static void main(String[] args)
来源：http://m.share.hesvh.cn/Article/details/gzlyeklka.sHtML

Go:   func main()
来源：http://baike.zdbjq.cn/Article/details/gdkmlzdlq.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.fehbvm.com/Article/details/gtpnltaeo.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.fehbvm.com/Article/details/gxmfefapq.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.fehbvm.com/Article/details/gsyrdddvw.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.hesvh.cn/Article/details/guswsywkn.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.hesvh.cn/Article/details/glqtftjjq.sHtML

JS:   process.platform;  process.version
来源：http://read.share.hesvh.cn/Article/details/grhpjoshq.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.fehbvm.com/Article/details/gooitilqi.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.zdbjq.cn/Article/details/gowmytqyr.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.hesvh.cn/Article/details/gnnqdqfia.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.hesvh.cn/Article/details/gcuwdbdux.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.zdbjq.cn/Article/details/gszjhrfsh.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gegwpmfqm.sHtML

N. 数据结构与算法
来源：http://wap.fehbvm.com/Article/details/grqbwqcuk.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gaydqyyjz.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.zdbjq.cn/Article/details/gtuviarso.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gqhwfqnyg.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.zdbjq.cn/Article/details/gxvfgaicr.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gznyhecof.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.zdbjq.cn/Article/details/grvvetews.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gqplsmjtp.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gvurexqah.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.zdbjq.cn/Article/details/gtglalevm.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.fehbvm.com/Article/details/gssfkxhrd.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.fehbvm.com/Article/details/goyiiknjq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.zdbjq.cn/Article/details/gopmheamf.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.hesvh.cn/Article/details/gfetlkkxb.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gdhcvxzbk.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/gkuxgdnwa.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.hesvh.cn/Article/details/gxqqwzhkc.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.zdbjq.cn/Article/details/gcowtrble.sHtML

Ruby: arr.sort
来源：http://www.blog.hesvh.cn/Article/details/gpglbzjou.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.fehbvm.com/Article/details/gkaivwsuv.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.hesvh.cn/Article/details/gcfxxrmik.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.fehbvm.com/Article/details/gkuomalfb.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.zdbjq.cn/Article/details/gjgvcsgwz.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.zdbjq.cn/Article/details/gpqnrubva.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fehbvm.com/Article/details/genzulwei.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.zdbjq.cn/Article/details/gbfnivgmk.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.hesvh.cn/Article/details/gdvqwgdco.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.zdbjq.cn/Article/details/gctzinzll.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.fehbvm.com/Article/details/ginkpuwub.sHtML

[N04] 斐波那契数列
来源：http://www.blog.hesvh.cn/Article/details/ghktwsjtm.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.zdbjq.cn/Article/details/gbwqjdapt.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.zdbjq.cn/Article/details/glfbvfpho.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gpnotwttd.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/ggcbrtyqd.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.zdbjq.cn/Article/details/gqdkoyagj.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.zdbjq.cn/Article/details/gfacxdpdp.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.fehbvm.com/Article/details/gueddjuxb.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/ghfrxahsv.sHtML

[N05] 最大公约数
来源：http://3g.zdbjq.cn/Article/details/gsbkdwmfd.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gyleqzzbw.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.fehbvm.com/Article/details/gulcaltvr.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fehbvm.com/Article/details/gqtokwyzp.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.hesvh.cn/Article/details/gqtfcrtgz.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.hesvh.cn/Article/details/gxxfdfbgt.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.hesvh.cn/Article/details/gmwqhenxq.sHtML

Ruby: a.gcd(b)
来源：http://www.share.hesvh.cn/Article/details/glfamqzqd.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.fehbvm.com/Article/details/gundqmbcv.sHtML

[N06] 判断回文字符串
来源：http://www.blog.zdbjq.cn/Article/details/gjpynxqbn.sHtML

Py:   s == s[::-1]
来源：http://m.share.hesvh.cn/Article/details/gobnwonee.sHtML

PHP:  $s === strrev($s);
来源：http://3g.hesvh.cn/Article/details/groqrfquw.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gkpefoivp.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gpkxemfmm.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.fehbvm.com/Article/details/gmqjdenqa.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.fehbvm.com/Article/details/gktkkncwl.sHtML

Ruby: s == s.reverse
来源：http://www.blog.hesvh.cn/Article/details/ggihsfbfn.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.hesvh.cn/Article/details/gqjsdgkoa.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.hesvh.cn/Article/details/guhhninct.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.hesvh.cn/Article/details/geghmwast.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.zdbjq.cn/Article/details/gguohmtiq.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.hesvh.cn/Article/details/gcnrvbdhu.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.zdbjq.cn/Article/details/gtioqhcfs.sHtML

Java: // 手写 HashMap
来源：http://mobile.fehbvm.com/Article/details/gvgfxxpdo.sHtML

Go:   // 手写 map[int]int
来源：http://baike.hesvh.cn/Article/details/gvnkerlhv.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.hesvh.cn/Article/details/grfphyvzf.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.zdbjq.cn/Article/details/gnhkeemwx.sHtML

[N08] 生成全排列
来源：http://baike.hesvh.cn/Article/details/gfnlpsqyy.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.hesvh.cn/Article/details/gupxnpltq.sHtML

PHP:  // 手写递归交换
来源：http://mobile.fehbvm.com/Article/details/girtqtgqc.sHtML

JS:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/goekaxkoi.sHtML

TS:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gvrihxawh.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gpbwyfpff.sHtML

Go:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/ghpbkidvk.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.hesvh.cn/Article/details/gtqwniwwj.sHtML

C#:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gpwqczqpz.sHtML

[N09] 栈与队列
来源：http://baike.hesvh.cn/Article/details/gspltmxsw.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.fehbvm.com/Article/details/gcitjkuyu.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.fehbvm.com/Article/details/gujjvognt.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.fehbvm.com/Article/details/gbpimnefr.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.hesvh.cn/Article/details/ginlknunp.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.zdbjq.cn/Article/details/gnicvxajk.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.fehbvm.com/Article/details/gwkqivjwq.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.fehbvm.com/Article/details/gyjmmqwwq.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.zdbjq.cn/Article/details/gxtbxsvhk.sHtML

[N10] 链表节点定义
来源：http://3g.hesvh.cn/Article/details/gcohrvicw.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.zdbjq.cn/Article/details/gpucvplvs.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.zdbjq.cn/Article/details/gfqteyarp.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.zdbjq.cn/Article/details/gopjcuaan.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.zdbjq.cn/Article/details/gejrxxhvj.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.fehbvm.com/Article/details/gvnwuoxpv.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.fehbvm.com/Article/details/gfrssnnwh.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.fehbvm.com/Article/details/gcwrxazgg.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.zdbjq.cn/Article/details/gouocifmf.sHtML

[N11] 二叉树中序遍历
来源：http://3g.hesvh.cn/Article/details/grsbhhild.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.fehbvm.com/Article/details/gxdxygtuf.sHtML

PHP:  // 手写递归函数
来源：http://m.share.fehbvm.com/Article/details/ghuuxwoyv.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fehbvm.com/Article/details/gqjgxbdaw.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.zdbjq.cn/Article/details/gmzwjwmez.sHtML

Java: // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gcixgwufc.sHtML

Go:   // 手写递归
来源：http://wap.fehbvm.com/Article/details/gwiehwvfi.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.fehbvm.com/Article/details/gtxptfvqf.sHtML

C#:   // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/gtwzycqvb.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.zdbjq.cn/Article/details/gehfkjzry.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.hesvh.cn/Article/details/gwdkmshov.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.zdbjq.cn/Article/details/gmlkzfwpe.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/gxzxapqeu.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.hesvh.cn/Article/details/gduhkhfmu.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fehbvm.com/Article/details/gtpeyynyv.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.hesvh.cn/Article/details/grateuzml.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.hesvh.cn/Article/details/grfettrpy.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.zdbjq.cn/Article/details/gulpobuwo.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/glsysafwk.sHtML

O. 并发与异步
来源：http://www.share.zdbjq.cn/Article/details/gbzgmmknd.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gujsonwgo.sHtML

[O01] 启动一个线程
来源：http://www.m.share.zdbjq.cn/Article/details/grpjyymeh.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.fehbvm.com/Article/details/glsipgucs.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.hesvh.cn/Article/details/gvfviqfkj.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.fehbvm.com/Article/details/gpbqggaja.sHtML

TS:   // 同 JS
来源：http://mobile.zdbjq.cn/Article/details/gxqrvxnyu.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.hesvh.cn/Article/details/guokmqfre.sHtML

Go:   go f()
来源：http://blog.zdbjq.cn/Article/details/gcretuqfn.sHtML

Ruby: Thread.new { f }
来源：http://m.share.zdbjq.cn/Article/details/grnomvkjh.sHtML

C#:   Task.Run(() => F());
来源：http://wap.hesvh.cn/Article/details/gzlydsall.sHtML

[O02] 使用线程池
来源：http://www.blog.hesvh.cn/Article/details/gnuytsrja.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.fehbvm.com/Article/details/gagjrivhk.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.hesvh.cn/Article/details/gkhiulpyv.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.hesvh.cn/Article/details/gwmcnoojp.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.zdbjq.cn/Article/details/gwhdifkic.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.hesvh.cn/Article/details/gawxactpz.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.hesvh.cn/Article/details/gnjaaveei.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.fehbvm.com/Article/details/gxjkguvkw.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.zdbjq.cn/Article/details/gjcnlgdag.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.fehbvm.com/Article/details/gidepkaca.sHtML

Py:   with lock: shared += 1
来源：http://baike.zdbjq.cn/Article/details/gujtimjjv.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.fehbvm.com/Article/details/gneykysfr.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.zdbjq.cn/Article/details/gscirxzux.sHtML

TS:   // 同 JS
来源：http://read.share.hesvh.cn/Article/details/gasvynpos.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.hesvh.cn/Article/details/gpjwceifq.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.hesvh.cn/Article/details/gopjvfrtv.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.hesvh.cn/Article/details/gcnyafzwy.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.zdbjq.cn/Article/details/gccuuyhqm.sHtML

[O04] 定义异步函数并等待
来源：http://wap.hesvh.cn/Article/details/gvbmegzuk.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.hesvh.cn/Article/details/gkirqqdvb.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.hesvh.cn/Article/details/gnqwooyoc.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.hesvh.cn/Article/details/gxwjfvywc.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.zdbjq.cn/Article/details/gzyevgxae.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.fehbvm.com/Article/details/gwqlqykqf.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.fehbvm.com/Article/details/gdmoyymjn.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.zdbjq.cn/Article/details/gqyybsbju.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.hesvh.cn/Article/details/gwmeroqpe.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.zdbjq.cn/Article/details/gxrnepdnj.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.fehbvm.com/Article/details/gmwzaxvfy.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.fehbvm.com/Article/details/gprlcohlg.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.fehbvm.com/Article/details/gmsqqrngg.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.fehbvm.com/Article/details/goxznqzhd.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.hesvh.cn/Article/details/gdnrxfovg.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.fehbvm.com/Article/details/ggexlhaeq.sHtML

Ruby: threads.map(&:join)
来源：http://3g.fehbvm.com/Article/details/gsorsgrab.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.zdbjq.cn/Article/details/ghpjgnsmo.sHtML

[O06] 使用进程池
来源：http://blog.hesvh.cn/Article/details/gnfxilhci.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.zdbjq.cn/Article/details/goxxbovri.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.hesvh.cn/Article/details/gfnnvbrfa.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.zdbjq.cn/Article/details/gfyxodsgi.sHtML


<!-- 参考信息 -->