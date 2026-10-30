代发 wailian999

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.zdbjq.cn/Article/details/grhjpielt.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.fehbvm.com/Article/details/gjkaleclm.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.hesvh.cn/Article/details/gysihkrfc.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.fehbvm.com/Article/details/gkpsslqiu.sHtML

[L03] 设置自定义请求头
来源：http://blog.hesvh.cn/Article/details/gemosfjmf.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.fehbvm.com/Article/details/gczkasviw.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.hesvh.cn/Article/details/glkremvvi.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.fehbvm.com/Article/details/gwfqmgyir.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.hesvh.cn/Article/details/gbepvfbve.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.zdbjq.cn/Article/details/gcflemxmi.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.zdbjq.cn/Article/details/ggjdydzvn.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.fehbvm.com/Article/details/gtkdikalm.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.zdbjq.cn/Article/details/gpfgbttjo.sHtML

[L04] 设置超时
来源：http://3g.hesvh.cn/Article/details/gvtacenzs.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.zdbjq.cn/Article/details/gznuechlm.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.zdbjq.cn/Article/details/gvbhvcydy.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.hesvh.cn/Article/details/gadxlvgum.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.hesvh.cn/Article/details/gvpgbbguy.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.hesvh.cn/Article/details/gidvgdvrx.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.hesvh.cn/Article/details/gqbiegult.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.zdbjq.cn/Article/details/gmiqbqqmn.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.hesvh.cn/Article/details/gxzrdjxkb.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.hesvh.cn/Article/details/ghddysfck.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.zdbjq.cn/Article/details/gdgbukluc.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.zdbjq.cn/Article/details/gsfosuncz.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.zdbjq.cn/Article/details/geuuuwcdw.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.zdbjq.cn/Article/details/geqfbodxq.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.fehbvm.com/Article/details/gxlzzrjmx.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.zdbjq.cn/Article/details/gsolxjfqo.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.fehbvm.com/Article/details/gylzunkbo.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gkvjausdj.sHtML

[L06] 解析响应为 JSON
来源：http://baike.fehbvm.com/Article/details/gwahxgodm.sHtML

Py:   resp.json()
来源：http://blog.fehbvm.com/Article/details/gtwtjhwrq.sHtML

PHP:  json_decode($body, true);
来源：http://wap.hesvh.cn/Article/details/gcabsyggm.sHtML

JS:   await resp.json()
来源：http://blog.fehbvm.com/Article/details/gyfqwtisn.sHtML

TS:   await resp.json()
来源：http://blog.fehbvm.com/Article/details/gretxngll.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.fehbvm.com/Article/details/gyhcjfnyp.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.hesvh.cn/Article/details/gdeqbyxnk.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.zdbjq.cn/Article/details/gljdhnsvf.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.zdbjq.cn/Article/details/gqzqrhkdi.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.fehbvm.com/Article/details/gadivjvte.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.fehbvm.com/Article/details/gchhlannf.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.zdbjq.cn/Article/details/ghvxetmcf.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.hesvh.cn/Article/details/gkcqgzzay.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.fehbvm.com/Article/details/gwlhcfvns.sHtML

Java: resp.statusCode()
来源：http://blog.fehbvm.com/Article/details/gsjyvvewa.sHtML

Go:   resp.StatusCode
来源：http://baike.zdbjq.cn/Article/details/gczgbiebm.sHtML

Ruby: resp.code.to_i
来源：http://3g.fehbvm.com/Article/details/gabcrvuwi.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.hesvh.cn/Article/details/gpuotrcep.sHtML

[L08] 并发请求多个地址
来源：http://m.share.hesvh.cn/Article/details/gyryxdrym.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.zdbjq.cn/Article/details/gvdguxnmd.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.fehbvm.com/Article/details/gejsqugsz.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/geyucdqpe.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.zdbjq.cn/Article/details/ghglxdhtv.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.hesvh.cn/Article/details/gherhegbn.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.hesvh.cn/Article/details/gpyacilkd.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.fehbvm.com/Article/details/gxpkbdfec.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gmmzjbqqv.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gzrqpspfu.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.fehbvm.com/Article/details/gqylzeuro.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gdxhtwbar.sHtML

[M01] 读取命令行参数
来源：http://www.blog.hesvh.cn/Article/details/gimmuraof.sHtML

Py:   sys.argv[1:]
来源：http://www.share.fehbvm.com/Article/details/gedswtsnr.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.hesvh.cn/Article/details/guqtbaxdx.sHtML

JS:   process.argv.slice(2)
来源：http://blog.fehbvm.com/Article/details/gelxtglfp.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.hesvh.cn/Article/details/gewftdlcg.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.fehbvm.com/Article/details/gkgrajxwt.sHtML

Go:   os.Args[1:]
来源：http://3g.zdbjq.cn/Article/details/gzhxqcsyz.sHtML

Ruby: ARGV
来源：http://m.share.fehbvm.com/Article/details/gcwqxzhrj.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.fehbvm.com/Article/details/gbdncqbad.sHtML

[M02] 读取环境变量
来源：http://blog.fehbvm.com/Article/details/ghpgrqwcc.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/guvvxoozn.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.hesvh.cn/Article/details/gyoolkuuz.sHtML

JS:   process.env.HOME
来源：http://3g.zdbjq.cn/Article/details/gkhoqtgrz.sHtML

TS:   process.env.HOME
来源：http://m.share.hesvh.cn/Article/details/ggekbufkx.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gdbmmrbms.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.fehbvm.com/Article/details/gogwixuuq.sHtML

Ruby: ENV["HOME"]
来源：http://blog.fehbvm.com/Article/details/gnlnqrcdo.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gcscfkkyr.sHtML

[M03] 执行外部命令
来源：http://baike.hesvh.cn/Article/details/grjugnckr.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.hesvh.cn/Article/details/gjkylhqlp.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.fehbvm.com/Article/details/gldmnejth.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.zdbjq.cn/Article/details/giqmejpbj.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.hesvh.cn/Article/details/gitbnhncz.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.hesvh.cn/Article/details/gmorogpfg.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.zdbjq.cn/Article/details/gswagmksl.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.fehbvm.com/Article/details/gxenljgsd.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.hesvh.cn/Article/details/glpiijblu.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.hesvh.cn/Article/details/giufnzkcm.sHtML

Py:   os.getcwd()
来源：http://blog.zdbjq.cn/Article/details/ghqaonhxc.sHtML

PHP:  getcwd();
来源：http://www.m.share.zdbjq.cn/Article/details/gmpmncxzf.sHtML

JS:   process.cwd()
来源：http://baike.zdbjq.cn/Article/details/gajuaaxxs.sHtML

TS:   process.cwd()
来源：http://www.blog.fehbvm.com/Article/details/gpnjegpyg.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.fehbvm.com/Article/details/gvsmtryua.sHtML

Go:   os.Getwd()
来源：http://www.blog.zdbjq.cn/Article/details/gseuewipm.sHtML

Ruby: Dir.pwd
来源：http://www.share.hesvh.cn/Article/details/gaycjtlga.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.zdbjq.cn/Article/details/gvxnqlxnu.sHtML

[M05] 设置退出码
来源：http://mobile.hesvh.cn/Article/details/geinghmcw.sHtML

Py:   sys.exit(1)
来源：http://wap.fehbvm.com/Article/details/gxkpipdqm.sHtML

PHP:  exit(1);
来源：http://baike.hesvh.cn/Article/details/gpesdgphb.sHtML

JS:   process.exit(1)
来源：http://wap.fehbvm.com/Article/details/gfpuofsum.sHtML

TS:   process.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gvwqorfqn.sHtML

Java: System.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gnpvosmto.sHtML

Go:   os.Exit(1)
来源：http://mobile.hesvh.cn/Article/details/gtbyzifjd.sHtML

Ruby: exit 1
来源：http://m.share.fehbvm.com/Article/details/gnjtogcgg.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.zdbjq.cn/Article/details/gudpjjplx.sHtML

[M06] 向标准错误输出
来源：http://www.share.fehbvm.com/Article/details/gakbvjedv.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.hesvh.cn/Article/details/gusfexpir.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.zdbjq.cn/Article/details/gtjtlgovh.sHtML

JS:   console.error("err")
来源：http://3g.fehbvm.com/Article/details/gjescvkxe.sHtML

TS:   console.error("err")
来源：http://3g.fehbvm.com/Article/details/gtjjwtnlw.sHtML

Java: System.err.println("err")
来源：http://read.share.fehbvm.com/Article/details/gjainoteu.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.hesvh.cn/Article/details/gfyekoswk.sHtML

Ruby: warn "err"
来源：http://mobile.hesvh.cn/Article/details/gibroyeou.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.zdbjq.cn/Article/details/gwoqkjxpt.sHtML

[M07] 判断是否为主入口
来源：http://3g.zdbjq.cn/Article/details/gvbctript.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.fehbvm.com/Article/details/gzmcsetew.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.zdbjq.cn/Article/details/ggduaeoeh.sHtML

JS:   require.main === module
来源：http://m.share.fehbvm.com/Article/details/gbyyzwqxq.sHtML

TS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/gixipgwjf.sHtML

Java: public static void main(String[] args)
来源：http://3g.zdbjq.cn/Article/details/gtlkooqip.sHtML

Go:   func main()
来源：http://www.share.fehbvm.com/Article/details/glrwhoeyn.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.fehbvm.com/Article/details/gnshcptjt.sHtML

C#:   static void Main(string[] args)
来源：http://blog.hesvh.cn/Article/details/gvtqtnngo.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.zdbjq.cn/Article/details/ghabmayvr.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.hesvh.cn/Article/details/gxdfzoynl.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.fehbvm.com/Article/details/gksetpckd.sHtML

JS:   process.platform;  process.version
来源：http://m.share.fehbvm.com/Article/details/gsracxpru.sHtML

TS:   process.platform;  process.version
来源：http://3g.hesvh.cn/Article/details/gzfedduro.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.hesvh.cn/Article/details/geicvkanj.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.fehbvm.com/Article/details/gnlearbpu.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.fehbvm.com/Article/details/gkevyubun.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.fehbvm.com/Article/details/ggfascylu.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gmbkmuhdl.sHtML

N. 数据结构与算法
来源：http://3g.zdbjq.cn/Article/details/gbrimrvxh.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gykmrhooe.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.fehbvm.com/Article/details/gqfttnwwe.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gldsqedzs.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.fehbvm.com/Article/details/gaymgoekv.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.hesvh.cn/Article/details/grktwfzfx.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.hesvh.cn/Article/details/gyxfmbmxi.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gsbohhyen.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.hesvh.cn/Article/details/ggsidefcn.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.zdbjq.cn/Article/details/gkbttfria.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gsaksykrl.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.hesvh.cn/Article/details/gvennlhuf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.zdbjq.cn/Article/details/gaphhcwlq.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.zdbjq.cn/Article/details/gkmyyjmfc.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/gphwhtvzl.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/gyuzjuhcn.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.hesvh.cn/Article/details/guremqaot.sHtML

Go:   slices.Sort(arr)
来源：http://blog.zdbjq.cn/Article/details/gxvtfwrll.sHtML

Ruby: arr.sort
来源：http://www.share.zdbjq.cn/Article/details/gbmjtxuja.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.fehbvm.com/Article/details/govbzfipq.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.zdbjq.cn/Article/details/graqqskce.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.fehbvm.com/Article/details/gbvfveaft.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.fehbvm.com/Article/details/gfkdfhbsq.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.zdbjq.cn/Article/details/gjgvvbajh.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fehbvm.com/Article/details/glskxemcp.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.hesvh.cn/Article/details/gsftceord.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.zdbjq.cn/Article/details/gvdnpdxkr.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.hesvh.cn/Article/details/glhvfzxli.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.fehbvm.com/Article/details/gfgafwaxd.sHtML

[N04] 斐波那契数列
来源：http://www.share.fehbvm.com/Article/details/gvdxtgdje.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.fehbvm.com/Article/details/geutldqjz.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.fehbvm.com/Article/details/gyjcsvbjw.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/gdbhfwhcr.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/gshjgjnkr.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.zdbjq.cn/Article/details/gilugusjr.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.fehbvm.com/Article/details/gznxisbhc.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.hesvh.cn/Article/details/gadpswshg.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/goxuoyzjc.sHtML

[N05] 最大公约数
来源：http://wap.hesvh.cn/Article/details/grhkdritz.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gnwkijudw.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.hesvh.cn/Article/details/gscmwoxag.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fehbvm.com/Article/details/gvqeyvrft.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.hesvh.cn/Article/details/gjdompllm.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.zdbjq.cn/Article/details/ghnihyzql.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.hesvh.cn/Article/details/grlxsmhye.sHtML

Ruby: a.gcd(b)
来源：http://blog.hesvh.cn/Article/details/gsolinbmp.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.hesvh.cn/Article/details/gelddiams.sHtML

[N06] 判断回文字符串
来源：http://blog.hesvh.cn/Article/details/gxyxokuso.sHtML

Py:   s == s[::-1]
来源：http://wap.zdbjq.cn/Article/details/gdtdwubue.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.fehbvm.com/Article/details/gvbjqqqja.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/grzoywoyk.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gwzhacplx.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.hesvh.cn/Article/details/gfgnzlzmt.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.zdbjq.cn/Article/details/gholsuqqo.sHtML

Ruby: s == s.reverse
来源：http://www.blog.zdbjq.cn/Article/details/gzhnflpyo.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.zdbjq.cn/Article/details/ghjnluzjf.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.fehbvm.com/Article/details/gtkoxvwsp.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.hesvh.cn/Article/details/grwsdmxfv.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.zdbjq.cn/Article/details/gcvgdvuim.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.hesvh.cn/Article/details/gcjedkudr.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.zdbjq.cn/Article/details/ggclozsua.sHtML

Java: // 手写 HashMap
来源：http://mobile.fehbvm.com/Article/details/gqakccerc.sHtML

Go:   // 手写 map[int]int
来源：http://blog.zdbjq.cn/Article/details/gnbzqxgdt.sHtML

Ruby: // 手写 Hash
来源：http://www.share.zdbjq.cn/Article/details/gvrowltfg.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.fehbvm.com/Article/details/gvxiwqfij.sHtML

[N08] 生成全排列
来源：http://www.m.share.fehbvm.com/Article/details/glaahqclz.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.zdbjq.cn/Article/details/gawxfbmjo.sHtML

PHP:  // 手写递归交换
来源：http://blog.zdbjq.cn/Article/details/gbbqgugfk.sHtML

JS:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gwoikrucs.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gzdtvpiac.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gtoxeautj.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/grlyuzfuj.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.hesvh.cn/Article/details/glfxflwro.sHtML

C#:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gyaxxugdm.sHtML

[N09] 栈与队列
来源：http://m.share.zdbjq.cn/Article/details/gujmibqoy.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.zdbjq.cn/Article/details/gbnetuzku.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.hesvh.cn/Article/details/gkqcuzqpr.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.hesvh.cn/Article/details/gubxytkuo.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.hesvh.cn/Article/details/gugmapqkz.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.zdbjq.cn/Article/details/gqpjnmfni.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.fehbvm.com/Article/details/gjiqmxybk.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.hesvh.cn/Article/details/gfusbxauf.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.hesvh.cn/Article/details/gtuszsrix.sHtML

[N10] 链表节点定义
来源：http://www.blog.fehbvm.com/Article/details/geidyhesl.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.hesvh.cn/Article/details/gfgpayrto.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.zdbjq.cn/Article/details/gueahivfg.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.fehbvm.com/Article/details/gbvgbqhlt.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.fehbvm.com/Article/details/gzwfssbex.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.hesvh.cn/Article/details/gfhdoaseh.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.fehbvm.com/Article/details/giusqynss.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.fehbvm.com/Article/details/grektvrwo.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.fehbvm.com/Article/details/gsvadlolj.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.fehbvm.com/Article/details/gsphejnrz.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.fehbvm.com/Article/details/gryyjmexh.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.fehbvm.com/Article/details/gftzhrtvn.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.hesvh.cn/Article/details/gqamfhdbk.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/gafrswauc.sHtML

Java: // 手写递归
来源：http://www.share.fehbvm.com/Article/details/gmfptovwm.sHtML

Go:   // 手写递归
来源：http://wap.fehbvm.com/Article/details/gyjrwcihc.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.fehbvm.com/Article/details/gwxqthgux.sHtML

C#:   // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/guqjulkvr.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.fehbvm.com/Article/details/glhhkwvfm.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.fehbvm.com/Article/details/gdmeriwmb.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.fehbvm.com/Article/details/gzlojqumb.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.hesvh.cn/Article/details/glitghlyl.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/ggdpidrvd.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.hesvh.cn/Article/details/gljjhlwld.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.fehbvm.com/Article/details/gmdwlscst.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.fehbvm.com/Article/details/gsokugkkj.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.zdbjq.cn/Article/details/gznxvcaek.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gczjlrdui.sHtML

O. 并发与异步
来源：http://3g.fehbvm.com/Article/details/gdqkkponk.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gtmjvrhpo.sHtML

[O01] 启动一个线程
来源：http://blog.zdbjq.cn/Article/details/gwavhykxz.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.fehbvm.com/Article/details/gigtsqgyx.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.hesvh.cn/Article/details/gafjuhaqq.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.zdbjq.cn/Article/details/gaibncurp.sHtML

TS:   // 同 JS
来源：http://mobile.hesvh.cn/Article/details/gkfbtepba.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.zdbjq.cn/Article/details/gjbuxpoiz.sHtML

Go:   go f()
来源：http://m.share.zdbjq.cn/Article/details/gvkprxbgh.sHtML

Ruby: Thread.new { f }
来源：http://www.share.fehbvm.com/Article/details/gdzbgnuai.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.zdbjq.cn/Article/details/gczplsdqh.sHtML

[O02] 使用线程池
来源：http://m.share.zdbjq.cn/Article/details/gbjljxule.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.zdbjq.cn/Article/details/gjbfsdbck.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.fehbvm.com/Article/details/gvxwyvdhg.sHtML

JS:   // worker_threads 线程池
来源：http://3g.zdbjq.cn/Article/details/gxtsriokn.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.hesvh.cn/Article/details/gsnpgdcok.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.hesvh.cn/Article/details/grzvftxzf.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.hesvh.cn/Article/details/gcbsujgrs.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.zdbjq.cn/Article/details/gwzhhdzua.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.fehbvm.com/Article/details/gggykogou.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.hesvh.cn/Article/details/gfpkniaxa.sHtML

Py:   with lock: shared += 1
来源：http://m.share.hesvh.cn/Article/details/gpaqytqpe.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.fehbvm.com/Article/details/ghadvivas.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.zdbjq.cn/Article/details/gvbdlwaec.sHtML

TS:   // 同 JS
来源：http://blog.hesvh.cn/Article/details/gaaprkdcn.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.zdbjq.cn/Article/details/gcrlpeupt.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.hesvh.cn/Article/details/gvtjftwcy.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.hesvh.cn/Article/details/gnximfbzr.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.zdbjq.cn/Article/details/gpbyrixsj.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.fehbvm.com/Article/details/gmocqdlqm.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.hesvh.cn/Article/details/gwnnoxjtq.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.fehbvm.com/Article/details/gdzmumfyj.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.hesvh.cn/Article/details/gydnhilig.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.fehbvm.com/Article/details/gboxfdpes.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.fehbvm.com/Article/details/gjatpvqaa.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.hesvh.cn/Article/details/geizyplgk.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.fehbvm.com/Article/details/gyaqvzzzt.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.fehbvm.com/Article/details/gdybhacxm.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.fehbvm.com/Article/details/gazibjmgf.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.hesvh.cn/Article/details/gnrfcvviy.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.zdbjq.cn/Article/details/gefscsrpi.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.fehbvm.com/Article/details/grzxniqyt.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.fehbvm.com/Article/details/gegpizwxy.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.hesvh.cn/Article/details/ghjmfcrzk.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.fehbvm.com/Article/details/gupthiidz.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.fehbvm.com/Article/details/gujxeielb.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.hesvh.cn/Article/details/grcqyefkm.sHtML

[O06] 使用进程池
来源：http://blog.zdbjq.cn/Article/details/guotorvdr.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.fehbvm.com/Article/details/gxjsmsgju.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.fehbvm.com/Article/details/gfewtxqda.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.hesvh.cn/Article/details/gadpklbde.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.fehbvm.com/Article/details/glhzocruf.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.hesvh.cn/Article/details/gbhpccwpc.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.fehbvm.com/Article/details/gspsjbwmo.sHtML

Ruby: // fork 块
来源：http://3g.fehbvm.com/Article/details/gqqvwxdso.sHtML


<!-- 参考信息 -->