代发 wailian999

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.zdbjq.cn/Article/details/grvzrsijo.sHtML

JS:   await fetch(url)
来源：http://blog.fehbvm.com/Article/details/gkkxaftbd.sHtML

TS:   await fetch(url)
来源：http://blog.zdbjq.cn/Article/details/gdvordoei.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.hesvh.cn/Article/details/gvgcwadoz.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.fehbvm.com/Article/details/gncdpropy.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.fehbvm.com/Article/details/gjtyjkste.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.zdbjq.cn/Article/details/giravqzgr.sHtML

[L02] 发送 POST JSON
来源：http://read.share.fehbvm.com/Article/details/glofiovqy.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.zdbjq.cn/Article/details/gobeyfqcj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.zdbjq.cn/Article/details/gpoczssed.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.zdbjq.cn/Article/details/gmclnhink.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.fehbvm.com/Article/details/gtzvdyxzk.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.hesvh.cn/Article/details/gbynehebc.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.zdbjq.cn/Article/details/gutnsssxy.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.fehbvm.com/Article/details/gopicpatp.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.fehbvm.com/Article/details/grelfdlgt.sHtML

[L03] 设置自定义请求头
来源：http://3g.fehbvm.com/Article/details/gzapvgggk.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.hesvh.cn/Article/details/gsopqlubt.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.zdbjq.cn/Article/details/govgpznng.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.zdbjq.cn/Article/details/ggqznfmni.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.zdbjq.cn/Article/details/gpqwzxxot.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.fehbvm.com/Article/details/gqdiomkry.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.hesvh.cn/Article/details/gsqadcsaw.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.zdbjq.cn/Article/details/guhiqpotb.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.hesvh.cn/Article/details/gvzvyeplx.sHtML

[L04] 设置超时
来源：http://www.blog.zdbjq.cn/Article/details/gzaejbsmw.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.zdbjq.cn/Article/details/gsjedqfid.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.zdbjq.cn/Article/details/gkmcmgobe.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.hesvh.cn/Article/details/gaabuguzm.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.hesvh.cn/Article/details/gfkrgulii.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.fehbvm.com/Article/details/gnazfmmdt.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.hesvh.cn/Article/details/gjxqdrgkv.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.fehbvm.com/Article/details/gppvrpanj.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.hesvh.cn/Article/details/gjsbtcknz.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.hesvh.cn/Article/details/glnithagc.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.zdbjq.cn/Article/details/gqmlzldle.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.zdbjq.cn/Article/details/ggbftuleh.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.fehbvm.com/Article/details/gfwsbjdcw.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.fehbvm.com/Article/details/gqavzfysg.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.fehbvm.com/Article/details/gwtqciyar.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.zdbjq.cn/Article/details/glanieglq.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.fehbvm.com/Article/details/gzcctjrre.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.hesvh.cn/Article/details/gmieysbcg.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.zdbjq.cn/Article/details/gvqxvzjua.sHtML

Py:   resp.json()
来源：http://m.share.fehbvm.com/Article/details/gkttsnwnn.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.zdbjq.cn/Article/details/gblknqsdf.sHtML

JS:   await resp.json()
来源：http://mobile.fehbvm.com/Article/details/gvbytbzod.sHtML

TS:   await resp.json()
来源：http://baike.fehbvm.com/Article/details/gvnasvlua.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.zdbjq.cn/Article/details/gotebztsv.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.zdbjq.cn/Article/details/gwjsnayos.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.hesvh.cn/Article/details/gieyqavza.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.zdbjq.cn/Article/details/ghlthailf.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.fehbvm.com/Article/details/gbxdwwmvb.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.fehbvm.com/Article/details/gkzqhuzmo.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.fehbvm.com/Article/details/grmweggvf.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.fehbvm.com/Article/details/giwogewwf.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.hesvh.cn/Article/details/gouxaylcr.sHtML

Java: resp.statusCode()
来源：http://3g.hesvh.cn/Article/details/gpnkpdffl.sHtML

Go:   resp.StatusCode
来源：http://www.share.zdbjq.cn/Article/details/gigyqhmsl.sHtML

Ruby: resp.code.to_i
来源：http://blog.fehbvm.com/Article/details/gbwskdsbh.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.hesvh.cn/Article/details/gixqfxobr.sHtML

[L08] 并发请求多个地址
来源：http://blog.fehbvm.com/Article/details/gfucnolwd.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.zdbjq.cn/Article/details/gjrkitnln.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.hesvh.cn/Article/details/gmumgeksp.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.zdbjq.cn/Article/details/gzriyzdvk.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/gssxjgzou.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.fehbvm.com/Article/details/ghyxeakim.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.hesvh.cn/Article/details/gkiujgmnk.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.fehbvm.com/Article/details/gndszpqxw.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.fehbvm.com/Article/details/govtxbdyh.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gmagnniqg.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.hesvh.cn/Article/details/gruuogwdf.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gnuuyqquz.sHtML

[M01] 读取命令行参数
来源：http://baike.zdbjq.cn/Article/details/gnmzfohkw.sHtML

Py:   sys.argv[1:]
来源：http://blog.hesvh.cn/Article/details/gqnmzblfn.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.fehbvm.com/Article/details/geznadcdr.sHtML

JS:   process.argv.slice(2)
来源：http://blog.fehbvm.com/Article/details/gczblzrjn.sHtML

TS:   process.argv.slice(2)
来源：http://wap.zdbjq.cn/Article/details/gpautsolk.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.hesvh.cn/Article/details/gtbjainou.sHtML

Go:   os.Args[1:]
来源：http://read.share.zdbjq.cn/Article/details/gweixxzvl.sHtML

Ruby: ARGV
来源：http://read.share.fehbvm.com/Article/details/glftxcren.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.fehbvm.com/Article/details/gvbhdfgpq.sHtML

[M02] 读取环境变量
来源：http://wap.fehbvm.com/Article/details/gxcppfugr.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gwrevegvv.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.fehbvm.com/Article/details/gtafvkvzx.sHtML

JS:   process.env.HOME
来源：http://www.m.share.hesvh.cn/Article/details/gaareacqg.sHtML

TS:   process.env.HOME
来源：http://m.share.fehbvm.com/Article/details/gxigwgost.sHtML

Java: System.getenv("HOME")
来源：http://wap.zdbjq.cn/Article/details/ggtdikqey.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.fehbvm.com/Article/details/gknjodbqg.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.hesvh.cn/Article/details/gpztcjvnh.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.fehbvm.com/Article/details/ghlwdkwcj.sHtML

[M03] 执行外部命令
来源：http://read.share.zdbjq.cn/Article/details/gxcmetuom.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.fehbvm.com/Article/details/gzsnadprz.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.fehbvm.com/Article/details/gghcwaazx.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.zdbjq.cn/Article/details/gzdsqwvqw.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.hesvh.cn/Article/details/glsktdhze.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.zdbjq.cn/Article/details/gdardjcdk.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.fehbvm.com/Article/details/gikaupstn.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.hesvh.cn/Article/details/gyjdjycoe.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.fehbvm.com/Article/details/gzevwhkqt.sHtML

[M04] 获取当前工作目录
来源：http://www.share.hesvh.cn/Article/details/gmorkoqgr.sHtML

Py:   os.getcwd()
来源：http://www.share.fehbvm.com/Article/details/gxlypcfkj.sHtML

PHP:  getcwd();
来源：http://www.blog.fehbvm.com/Article/details/gygdhihur.sHtML

JS:   process.cwd()
来源：http://3g.zdbjq.cn/Article/details/goybuqamo.sHtML

TS:   process.cwd()
来源：http://www.m.share.hesvh.cn/Article/details/gkipihgfe.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.hesvh.cn/Article/details/geplfnqdi.sHtML

Go:   os.Getwd()
来源：http://3g.fehbvm.com/Article/details/ghghrrqfl.sHtML

Ruby: Dir.pwd
来源：http://3g.zdbjq.cn/Article/details/giyiovjkw.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.zdbjq.cn/Article/details/grztncwnw.sHtML

[M05] 设置退出码
来源：http://3g.zdbjq.cn/Article/details/gjxpcphmn.sHtML

Py:   sys.exit(1)
来源：http://m.share.hesvh.cn/Article/details/glexowuul.sHtML

PHP:  exit(1);
来源：http://3g.fehbvm.com/Article/details/gezrlbhks.sHtML

JS:   process.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/ggyafnnhr.sHtML

TS:   process.exit(1)
来源：http://blog.fehbvm.com/Article/details/gnsvpunbh.sHtML

Java: System.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gzbtwgnji.sHtML

Go:   os.Exit(1)
来源：http://baike.hesvh.cn/Article/details/gtwlxdekl.sHtML

Ruby: exit 1
来源：http://www.share.zdbjq.cn/Article/details/gmrrddymf.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.fehbvm.com/Article/details/gwowunbex.sHtML

[M06] 向标准错误输出
来源：http://www.share.fehbvm.com/Article/details/grpnyxcnk.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.hesvh.cn/Article/details/giygnlbku.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.hesvh.cn/Article/details/gtnlumywz.sHtML

JS:   console.error("err")
来源：http://www.blog.hesvh.cn/Article/details/gaikxjngy.sHtML

TS:   console.error("err")
来源：http://m.share.fehbvm.com/Article/details/gcxoutntv.sHtML

Java: System.err.println("err")
来源：http://blog.zdbjq.cn/Article/details/gussqojvs.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.zdbjq.cn/Article/details/gmgbjmees.sHtML

Ruby: warn "err"
来源：http://wap.hesvh.cn/Article/details/gnksvpxgq.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.hesvh.cn/Article/details/gfkjamolf.sHtML

[M07] 判断是否为主入口
来源：http://wap.fehbvm.com/Article/details/gujkvnszo.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.hesvh.cn/Article/details/gpqabqjfo.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.zdbjq.cn/Article/details/gjhekrcuu.sHtML

JS:   require.main === module
来源：http://www.m.share.zdbjq.cn/Article/details/gorafuzzx.sHtML

TS:   require.main === module
来源：http://www.m.share.fehbvm.com/Article/details/gjgpikdmr.sHtML

Java: public static void main(String[] args)
来源：http://read.share.zdbjq.cn/Article/details/gshtkjuah.sHtML

Go:   func main()
来源：http://www.share.fehbvm.com/Article/details/gmnwpktyv.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.fehbvm.com/Article/details/gedcfamlr.sHtML

C#:   static void Main(string[] args)
来源：http://blog.hesvh.cn/Article/details/gkjbvulsg.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.fehbvm.com/Article/details/gskkwefek.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.hesvh.cn/Article/details/gaedgvmbr.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.fehbvm.com/Article/details/ganaxzpow.sHtML

JS:   process.platform;  process.version
来源：http://wap.zdbjq.cn/Article/details/giimlnoql.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.fehbvm.com/Article/details/grrvggudy.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.hesvh.cn/Article/details/gqwazjfpn.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.fehbvm.com/Article/details/gjottqldi.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.hesvh.cn/Article/details/gsglmzlvx.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.fehbvm.com/Article/details/gecppawig.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gmsnkxntk.sHtML

N. 数据结构与算法
来源：http://baike.fehbvm.com/Article/details/gnosryznk.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gmrwykfnz.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.fehbvm.com/Article/details/gkxhlbnqw.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.fehbvm.com/Article/details/glfgxemor.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gcqwehmdv.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.zdbjq.cn/Article/details/gwjdkicoa.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.hesvh.cn/Article/details/gzsxwveax.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.hesvh.cn/Article/details/gthwlxwfv.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.zdbjq.cn/Article/details/ghcqzwqfo.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.hesvh.cn/Article/details/gcegeyuqc.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.fehbvm.com/Article/details/gdebqkaem.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.fehbvm.com/Article/details/gyfeuhnjr.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fehbvm.com/Article/details/glnffkfjo.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.zdbjq.cn/Article/details/grrszrxez.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/gnpzukkjr.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/grmkxzdfp.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.zdbjq.cn/Article/details/ggiloijck.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.hesvh.cn/Article/details/gvodcnvtz.sHtML

Ruby: arr.sort
来源：http://3g.zdbjq.cn/Article/details/gskobbfgx.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.hesvh.cn/Article/details/gvnmaeafl.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.hesvh.cn/Article/details/gjbjnlfzr.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.hesvh.cn/Article/details/gcxwxddwf.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.hesvh.cn/Article/details/gdstxmylj.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.zdbjq.cn/Article/details/glgkykitw.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.zdbjq.cn/Article/details/gyorbuzlq.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.zdbjq.cn/Article/details/gxulnomvk.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.fehbvm.com/Article/details/gsrxanadh.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.zdbjq.cn/Article/details/gytfqfjox.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.hesvh.cn/Article/details/gaekesflj.sHtML

[N04] 斐波那契数列
来源：http://m.share.hesvh.cn/Article/details/gwnsxxxhw.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.zdbjq.cn/Article/details/gxaovdshf.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.fehbvm.com/Article/details/gmpqvwjuh.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gfvguohjl.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/geknzbifj.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.hesvh.cn/Article/details/gcyxekflw.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.hesvh.cn/Article/details/ghcmjevgi.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.fehbvm.com/Article/details/gqjfxypyc.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/gkpjfuscr.sHtML

[N05] 最大公约数
来源：http://www.m.share.zdbjq.cn/Article/details/gtmeyijru.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/gyqbhmvga.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.hesvh.cn/Article/details/gttrbtihn.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fehbvm.com/Article/details/gepxikxtf.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fehbvm.com/Article/details/gbuojjwvu.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.hesvh.cn/Article/details/gpoefgkhe.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.fehbvm.com/Article/details/gjbbpszzt.sHtML

Ruby: a.gcd(b)
来源：http://mobile.hesvh.cn/Article/details/gtbdxbttc.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.fehbvm.com/Article/details/gycrtsgcm.sHtML

[N06] 判断回文字符串
来源：http://baike.fehbvm.com/Article/details/gwmkrqkqi.sHtML

Py:   s == s[::-1]
来源：http://3g.hesvh.cn/Article/details/glsuhefdb.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.zdbjq.cn/Article/details/gjiowxiwy.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/geenswqvw.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gklbbncac.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.hesvh.cn/Article/details/gvuutkbtt.sHtML

Go:   // 双指针从两端比较
来源：http://wap.fehbvm.com/Article/details/gfokfqzyr.sHtML

Ruby: s == s.reverse
来源：http://wap.hesvh.cn/Article/details/gpwbzskdo.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.zdbjq.cn/Article/details/grvxmgehy.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.hesvh.cn/Article/details/gjawmfvup.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.hesvh.cn/Article/details/gxmtabusy.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.zdbjq.cn/Article/details/gpbgwhnbm.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.zdbjq.cn/Article/details/gzjxcdzzk.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.fehbvm.com/Article/details/gcbaxtmcz.sHtML

Java: // 手写 HashMap
来源：http://m.share.fehbvm.com/Article/details/gteaekmvy.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.fehbvm.com/Article/details/giuehgfzb.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.hesvh.cn/Article/details/gsbirxcvq.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.zdbjq.cn/Article/details/gerufazyw.sHtML

[N08] 生成全排列
来源：http://mobile.fehbvm.com/Article/details/gzwbsfqga.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.fehbvm.com/Article/details/gljjxoraf.sHtML

PHP:  // 手写递归交换
来源：http://m.share.fehbvm.com/Article/details/gckvgmvfc.sHtML

JS:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gntbwuixg.sHtML

TS:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gprzfzulo.sHtML

Java: // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gocmzvmsi.sHtML

Go:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gmbdqwxcv.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.fehbvm.com/Article/details/gryryicaz.sHtML

C#:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/goqghrsjc.sHtML

[N09] 栈与队列
来源：http://wap.fehbvm.com/Article/details/gnbhojqqe.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.fehbvm.com/Article/details/gujetrvse.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.zdbjq.cn/Article/details/garmcajex.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.hesvh.cn/Article/details/gcdlvpfwg.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.hesvh.cn/Article/details/gkdimszuh.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.fehbvm.com/Article/details/gpjvbezxv.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.fehbvm.com/Article/details/gzgircgst.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gimzrfxjo.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.zdbjq.cn/Article/details/gpxrlmwzq.sHtML

[N10] 链表节点定义
来源：http://baike.zdbjq.cn/Article/details/gypchcpqe.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.zdbjq.cn/Article/details/gprgtbyzc.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.fehbvm.com/Article/details/gokjgznps.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.zdbjq.cn/Article/details/goxhxllll.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.fehbvm.com/Article/details/gejcsdnsd.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.zdbjq.cn/Article/details/gezlqsgcx.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.zdbjq.cn/Article/details/govobreve.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.zdbjq.cn/Article/details/gmohpywld.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.fehbvm.com/Article/details/gmcaaxpuk.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.hesvh.cn/Article/details/gkzotavru.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.fehbvm.com/Article/details/gryjvknet.sHtML

PHP:  // 手写递归函数
来源：http://baike.zdbjq.cn/Article/details/ghpmmlpxx.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fehbvm.com/Article/details/ghhvginad.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fehbvm.com/Article/details/gpsolqcxt.sHtML

Java: // 手写递归
来源：http://wap.hesvh.cn/Article/details/gqfbblpvx.sHtML

Go:   // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gubnwefsp.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.zdbjq.cn/Article/details/gyndvqgyh.sHtML

C#:   // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/gisvkcshj.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.zdbjq.cn/Article/details/gwswmthzb.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.fehbvm.com/Article/details/gnqeknwvy.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.fehbvm.com/Article/details/ghcnestxa.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.hesvh.cn/Article/details/gwfrhxupi.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.zdbjq.cn/Article/details/geuaszfgk.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fehbvm.com/Article/details/giekzhoyb.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.zdbjq.cn/Article/details/gioixvlwt.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.hesvh.cn/Article/details/gglxcsuor.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.hesvh.cn/Article/details/gdsfusowy.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gjpnjdbmp.sHtML

O. 并发与异步
来源：http://m.share.hesvh.cn/Article/details/giwejqsdu.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gkifdspqp.sHtML

[O01] 启动一个线程
来源：http://www.m.share.fehbvm.com/Article/details/gtvanzpcy.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.fehbvm.com/Article/details/gtuekotbj.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.zdbjq.cn/Article/details/guzwlryoq.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.hesvh.cn/Article/details/gndkjitxg.sHtML

TS:   // 同 JS
来源：http://www.m.share.hesvh.cn/Article/details/gklmvxgsl.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.fehbvm.com/Article/details/gcqgktzoi.sHtML

Go:   go f()
来源：http://blog.hesvh.cn/Article/details/gczaaqdgs.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.hesvh.cn/Article/details/gpavbgvjp.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.zdbjq.cn/Article/details/gjlugkfan.sHtML

[O02] 使用线程池
来源：http://read.share.fehbvm.com/Article/details/gnjystdrd.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.zdbjq.cn/Article/details/gowycfwjc.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.zdbjq.cn/Article/details/gbfqdimqo.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/gyllkcpdh.sHtML

TS:   // worker_threads 线程池
来源：http://baike.zdbjq.cn/Article/details/ghmjfzxvy.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.zdbjq.cn/Article/details/gmuqyvzfp.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.zdbjq.cn/Article/details/guislojfa.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.hesvh.cn/Article/details/gvygkdazh.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.zdbjq.cn/Article/details/ggmpizmuy.sHtML

[O03] 加锁保护共享数据
来源：http://3g.fehbvm.com/Article/details/gemtdxpnp.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.zdbjq.cn/Article/details/gaqrollez.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.hesvh.cn/Article/details/gcetlisir.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.zdbjq.cn/Article/details/gtlktvkis.sHtML

TS:   // 同 JS
来源：http://wap.hesvh.cn/Article/details/getdldznh.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.hesvh.cn/Article/details/gpmxtiqpo.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.zdbjq.cn/Article/details/gzzeglhxb.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.zdbjq.cn/Article/details/girvpvdhl.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.zdbjq.cn/Article/details/gdcdnkycy.sHtML

[O04] 定义异步函数并等待
来源：http://baike.zdbjq.cn/Article/details/gxjmztmbr.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.hesvh.cn/Article/details/gphbzgswr.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.hesvh.cn/Article/details/gprqmknnd.sHtML

JS:   async function f() { await g(); }
来源：http://wap.zdbjq.cn/Article/details/gsivxuiei.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.zdbjq.cn/Article/details/gjapqobtc.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.hesvh.cn/Article/details/gjnjmuzex.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.zdbjq.cn/Article/details/gaiydxhpk.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.zdbjq.cn/Article/details/gqjvstphg.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.hesvh.cn/Article/details/geamfmdzf.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.zdbjq.cn/Article/details/ggwbezmly.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.zdbjq.cn/Article/details/gmpyoqrur.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.hesvh.cn/Article/details/gzfghlqxj.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.hesvh.cn/Article/details/ghxustaqa.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.hesvh.cn/Article/details/gmermyexj.sHtML


<!-- 参考信息 -->