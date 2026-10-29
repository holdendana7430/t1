代发 wailian999

Go:   resp, err := http.Get(url)
来源：http://blog.fehbvm.com/Article/details/gmanrqbcz.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.fehbvm.com/Article/details/gslplcvds.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.fehbvm.com/Article/details/gjmwlblkv.sHtML

[L02] 发送 POST JSON
来源：http://3g.hesvh.cn/Article/details/gypyyjdqm.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.fehbvm.com/Article/details/gfrfkkelv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.fehbvm.com/Article/details/gclvhedpz.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.fehbvm.com/Article/details/ggtpjuewc.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.zdbjq.cn/Article/details/gudbrqjbn.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.hesvh.cn/Article/details/gczvtjgau.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.zdbjq.cn/Article/details/gjtlrwdzx.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.hesvh.cn/Article/details/gclbtkgcx.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.zdbjq.cn/Article/details/ggpzzthyd.sHtML

[L03] 设置自定义请求头
来源：http://wap.fehbvm.com/Article/details/gqcfafyyl.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.hesvh.cn/Article/details/gqrhgtbmg.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.hesvh.cn/Article/details/glmwxbspl.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.fehbvm.com/Article/details/gjgtjllhf.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.hesvh.cn/Article/details/gwvijzksu.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.zdbjq.cn/Article/details/gqlldougg.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.hesvh.cn/Article/details/gchxlerda.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.zdbjq.cn/Article/details/ghisqlgkl.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.fehbvm.com/Article/details/gqgqtacdc.sHtML

[L04] 设置超时
来源：http://mobile.hesvh.cn/Article/details/grcipngvh.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.hesvh.cn/Article/details/gkkqwzxkn.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.zdbjq.cn/Article/details/gfzwuyend.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.fehbvm.com/Article/details/gyghbcxsg.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.hesvh.cn/Article/details/gpkplkgdu.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.hesvh.cn/Article/details/gswagusjw.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.zdbjq.cn/Article/details/gmxpirbfm.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.fehbvm.com/Article/details/gazxyokgl.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.zdbjq.cn/Article/details/gcjkcfftq.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.zdbjq.cn/Article/details/gntnvkluf.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.fehbvm.com/Article/details/gjkgpdooq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.hesvh.cn/Article/details/gwjviyykl.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.fehbvm.com/Article/details/ggpyadjst.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.fehbvm.com/Article/details/gtwgkwdyx.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.zdbjq.cn/Article/details/grnllgtms.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.hesvh.cn/Article/details/gzahdwrfg.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.hesvh.cn/Article/details/ggjxgnqnf.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.hesvh.cn/Article/details/gzskooeqt.sHtML

[L06] 解析响应为 JSON
来源：http://blog.fehbvm.com/Article/details/gvzbimnnv.sHtML

Py:   resp.json()
来源：http://3g.fehbvm.com/Article/details/gdnulddgy.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.zdbjq.cn/Article/details/glirtyyjl.sHtML

JS:   await resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gmugzvpme.sHtML

TS:   await resp.json()
来源：http://mobile.zdbjq.cn/Article/details/gipyuzegv.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.zdbjq.cn/Article/details/govycbcpq.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.zdbjq.cn/Article/details/gedqfwrgd.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.zdbjq.cn/Article/details/gfqwvgzho.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.zdbjq.cn/Article/details/ginkpubhp.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.hesvh.cn/Article/details/gzwvnsvnz.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.hesvh.cn/Article/details/gtzbwroxg.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.fehbvm.com/Article/details/getokrchx.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.hesvh.cn/Article/details/gebktzivz.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.zdbjq.cn/Article/details/grsnbjvez.sHtML

Java: resp.statusCode()
来源：http://m.share.fehbvm.com/Article/details/gtuqaneer.sHtML

Go:   resp.StatusCode
来源：http://m.share.zdbjq.cn/Article/details/grhgcgqpd.sHtML

Ruby: resp.code.to_i
来源：http://m.share.fehbvm.com/Article/details/gvbreensq.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.hesvh.cn/Article/details/gksyiwjuz.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.fehbvm.com/Article/details/gmzusdgdr.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.hesvh.cn/Article/details/ghyxpjnfw.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.zdbjq.cn/Article/details/gfntyohfi.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.hesvh.cn/Article/details/gitisynzk.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/ghoxgqyvk.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.fehbvm.com/Article/details/gasnwzecp.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.zdbjq.cn/Article/details/ghtacwztc.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.zdbjq.cn/Article/details/gvkegrpgh.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.fehbvm.com/Article/details/gmbiqmgdw.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gygxufpdn.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.hesvh.cn/Article/details/gpozikwaf.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gvbchbyvo.sHtML

[M01] 读取命令行参数
来源：http://www.blog.hesvh.cn/Article/details/gbjtuocih.sHtML

Py:   sys.argv[1:]
来源：http://mobile.zdbjq.cn/Article/details/ggsdqzfzj.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.zdbjq.cn/Article/details/gtbyijami.sHtML

JS:   process.argv.slice(2)
来源：http://baike.fehbvm.com/Article/details/gxlxykaaj.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.zdbjq.cn/Article/details/gmeuwyrkl.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.fehbvm.com/Article/details/gsbnlznkv.sHtML

Go:   os.Args[1:]
来源：http://www.share.fehbvm.com/Article/details/grtxgrwzo.sHtML

Ruby: ARGV
来源：http://baike.fehbvm.com/Article/details/gkpqffpnr.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.zdbjq.cn/Article/details/gvyigugfv.sHtML

[M02] 读取环境变量
来源：http://baike.zdbjq.cn/Article/details/gdlabprry.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gtcweiyqn.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.hesvh.cn/Article/details/gfyddsfvl.sHtML

JS:   process.env.HOME
来源：http://baike.zdbjq.cn/Article/details/gwjmitbyd.sHtML

TS:   process.env.HOME
来源：http://www.blog.zdbjq.cn/Article/details/gbqqwoznn.sHtML

Java: System.getenv("HOME")
来源：http://blog.zdbjq.cn/Article/details/gdeyjafwm.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.fehbvm.com/Article/details/gsizyqjct.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.fehbvm.com/Article/details/ggtprjojo.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.hesvh.cn/Article/details/gqooojhqb.sHtML

[M03] 执行外部命令
来源：http://read.share.zdbjq.cn/Article/details/gaizadhya.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.zdbjq.cn/Article/details/gkihhfbzh.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.fehbvm.com/Article/details/gjwgaoogo.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.hesvh.cn/Article/details/gwvijrjuy.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fehbvm.com/Article/details/gozbnthaq.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.fehbvm.com/Article/details/gtiiumgme.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.hesvh.cn/Article/details/glotluyri.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.hesvh.cn/Article/details/gqbplroog.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.hesvh.cn/Article/details/gopukskqz.sHtML

[M04] 获取当前工作目录
来源：http://3g.hesvh.cn/Article/details/gqcvhlohi.sHtML

Py:   os.getcwd()
来源：http://www.m.share.fehbvm.com/Article/details/gmflpyqun.sHtML

PHP:  getcwd();
来源：http://read.share.hesvh.cn/Article/details/gfnjyzbaq.sHtML

JS:   process.cwd()
来源：http://3g.fehbvm.com/Article/details/gzdiuqorr.sHtML

TS:   process.cwd()
来源：http://www.blog.hesvh.cn/Article/details/guemoizqj.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.hesvh.cn/Article/details/gadyaxcxc.sHtML

Go:   os.Getwd()
来源：http://mobile.fehbvm.com/Article/details/giiqzayvl.sHtML

Ruby: Dir.pwd
来源：http://wap.hesvh.cn/Article/details/gjwonhgao.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.fehbvm.com/Article/details/gqhzhhhze.sHtML

[M05] 设置退出码
来源：http://read.share.zdbjq.cn/Article/details/ghuaitkqc.sHtML

Py:   sys.exit(1)
来源：http://baike.hesvh.cn/Article/details/gukvumkjz.sHtML

PHP:  exit(1);
来源：http://read.share.hesvh.cn/Article/details/gxunvvvnx.sHtML

JS:   process.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gcjfxbsvh.sHtML

TS:   process.exit(1)
来源：http://baike.fehbvm.com/Article/details/gzfxsywpr.sHtML

Java: System.exit(1)
来源：http://wap.fehbvm.com/Article/details/gdoinpnwk.sHtML

Go:   os.Exit(1)
来源：http://3g.hesvh.cn/Article/details/glhzpvyoy.sHtML

Ruby: exit 1
来源：http://3g.zdbjq.cn/Article/details/gqftaxevf.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.hesvh.cn/Article/details/gfemkzkxs.sHtML

[M06] 向标准错误输出
来源：http://read.share.hesvh.cn/Article/details/gzdsrpcdl.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.fehbvm.com/Article/details/gsgtebcvp.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.hesvh.cn/Article/details/giprmdjmp.sHtML

JS:   console.error("err")
来源：http://wap.zdbjq.cn/Article/details/gpbwxkwte.sHtML

TS:   console.error("err")
来源：http://wap.fehbvm.com/Article/details/gfuxkcvxq.sHtML

Java: System.err.println("err")
来源：http://blog.hesvh.cn/Article/details/gkzrldrih.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.hesvh.cn/Article/details/gsssocsjp.sHtML

Ruby: warn "err"
来源：http://3g.zdbjq.cn/Article/details/gvpltpjbf.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.hesvh.cn/Article/details/gtgahqxsb.sHtML

[M07] 判断是否为主入口
来源：http://read.share.fehbvm.com/Article/details/gxkevuone.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.zdbjq.cn/Article/details/gumayghyv.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.fehbvm.com/Article/details/gtrpmaayo.sHtML

JS:   require.main === module
来源：http://3g.fehbvm.com/Article/details/gykouvirb.sHtML

TS:   require.main === module
来源：http://blog.zdbjq.cn/Article/details/gjuadilvy.sHtML

Java: public static void main(String[] args)
来源：http://blog.zdbjq.cn/Article/details/gxshwhkis.sHtML

Go:   func main()
来源：http://wap.zdbjq.cn/Article/details/gbylerunf.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.zdbjq.cn/Article/details/ggmnmbdfz.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.fehbvm.com/Article/details/gvielmvnh.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.hesvh.cn/Article/details/gzqtxrwoy.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.zdbjq.cn/Article/details/gjjkuhsqp.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.fehbvm.com/Article/details/gnkhrybym.sHtML

JS:   process.platform;  process.version
来源：http://wap.fehbvm.com/Article/details/gjnntyexw.sHtML

TS:   process.platform;  process.version
来源：http://blog.zdbjq.cn/Article/details/gygdklqds.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.zdbjq.cn/Article/details/gfjixvfhz.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.fehbvm.com/Article/details/guwmmocdh.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.hesvh.cn/Article/details/gcwfetzoc.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.zdbjq.cn/Article/details/gxmibsgra.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gnupexogf.sHtML

N. 数据结构与算法
来源：http://read.share.zdbjq.cn/Article/details/grtpqohqf.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gwwyyeidz.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.fehbvm.com/Article/details/gjdaxjziq.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gxobgqqha.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.zdbjq.cn/Article/details/gojkjvaus.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/gyewuiajy.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.hesvh.cn/Article/details/gyuzavkys.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.hesvh.cn/Article/details/ggpjlfloj.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gmxdkmrsi.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.zdbjq.cn/Article/details/gnbcueogg.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gskzpyaen.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.zdbjq.cn/Article/details/gclltibgw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fehbvm.com/Article/details/gbbunbbjy.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.zdbjq.cn/Article/details/gbbcaywqw.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/gdaktoedb.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/gbaphzzlc.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.hesvh.cn/Article/details/gduvcturm.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.zdbjq.cn/Article/details/gkmeqdysb.sHtML

Ruby: arr.sort
来源：http://baike.fehbvm.com/Article/details/gsjnmkimy.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.fehbvm.com/Article/details/gdreveomr.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.zdbjq.cn/Article/details/gdhpmafil.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.fehbvm.com/Article/details/gpschsglc.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.fehbvm.com/Article/details/gqnuuztcs.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.zdbjq.cn/Article/details/ggjsvauzt.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.zdbjq.cn/Article/details/gkrwyrcli.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.fehbvm.com/Article/details/gugtaihod.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.hesvh.cn/Article/details/gziymwbex.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.hesvh.cn/Article/details/gdhlwtedn.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.zdbjq.cn/Article/details/gouescrmo.sHtML

[N04] 斐波那契数列
来源：http://read.share.hesvh.cn/Article/details/gmfdopdsy.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.hesvh.cn/Article/details/gqznnlcio.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.hesvh.cn/Article/details/ggwimohxl.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gdhsxhynm.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/ggchljmom.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.zdbjq.cn/Article/details/gcecoehob.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.fehbvm.com/Article/details/gfcejxubg.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.zdbjq.cn/Article/details/gsskmdnws.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/gwrixmdqx.sHtML

[N05] 最大公约数
来源：http://mobile.hesvh.cn/Article/details/gbhesbedb.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gbprqcbnm.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.hesvh.cn/Article/details/gxoevgrcj.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fehbvm.com/Article/details/gowvbnyeb.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.zdbjq.cn/Article/details/gmbijzxwn.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.hesvh.cn/Article/details/gmypnnwxh.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.zdbjq.cn/Article/details/gnuzjeixg.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.hesvh.cn/Article/details/giyqhzlxa.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.fehbvm.com/Article/details/gokjmydzh.sHtML

[N06] 判断回文字符串
来源：http://m.share.hesvh.cn/Article/details/goebnricu.sHtML

Py:   s == s[::-1]
来源：http://blog.hesvh.cn/Article/details/gnmvucfhg.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.hesvh.cn/Article/details/gcefnrian.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gbqpiukwp.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/ggnrcvhnx.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.hesvh.cn/Article/details/gohchyspe.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.hesvh.cn/Article/details/gbqlvyavy.sHtML

Ruby: s == s.reverse
来源：http://read.share.zdbjq.cn/Article/details/gqkampjgg.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.zdbjq.cn/Article/details/gntdnfezd.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.zdbjq.cn/Article/details/gzorzdfle.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.zdbjq.cn/Article/details/gvrdizgcq.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.zdbjq.cn/Article/details/gaotasiri.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.hesvh.cn/Article/details/gizignuwr.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.fehbvm.com/Article/details/gpbvuyksb.sHtML

Java: // 手写 HashMap
来源：http://blog.zdbjq.cn/Article/details/ggikzbcof.sHtML

Go:   // 手写 map[int]int
来源：http://blog.hesvh.cn/Article/details/gohnxjuxm.sHtML

Ruby: // 手写 Hash
来源：http://mobile.zdbjq.cn/Article/details/gpmocjeyg.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.fehbvm.com/Article/details/ggpkqyyor.sHtML

[N08] 生成全排列
来源：http://3g.zdbjq.cn/Article/details/ghnkscoew.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.hesvh.cn/Article/details/gsnwsqqwm.sHtML

PHP:  // 手写递归交换
来源：http://baike.fehbvm.com/Article/details/gfxrbqvnh.sHtML

JS:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gtkijfqgp.sHtML

TS:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gnmeidjub.sHtML

Java: // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gasbxamnl.sHtML

Go:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/geagbspqk.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.fehbvm.com/Article/details/glejswqes.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gjgysnlbh.sHtML

[N09] 栈与队列
来源：http://www.blog.hesvh.cn/Article/details/gurzoanmy.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.hesvh.cn/Article/details/giljaenyi.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gjantmclq.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.zdbjq.cn/Article/details/ghillhrhb.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.fehbvm.com/Article/details/gmioqhjtz.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.hesvh.cn/Article/details/gdgiftkck.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.fehbvm.com/Article/details/gqnazyclo.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.fehbvm.com/Article/details/gncydwouu.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.hesvh.cn/Article/details/gnrqackuc.sHtML

[N10] 链表节点定义
来源：http://baike.fehbvm.com/Article/details/gulujcoyq.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.zdbjq.cn/Article/details/gmjpzerqw.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.hesvh.cn/Article/details/gxafwdjnq.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.hesvh.cn/Article/details/gcsxlequl.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.fehbvm.com/Article/details/gcwgviuwv.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.hesvh.cn/Article/details/gbdxifzvq.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.hesvh.cn/Article/details/gflarnmaz.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.hesvh.cn/Article/details/gwmahqnqn.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.fehbvm.com/Article/details/gtmvdtbkz.sHtML

[N11] 二叉树中序遍历
来源：http://wap.fehbvm.com/Article/details/gjtwagrqs.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.hesvh.cn/Article/details/gmnrefhir.sHtML

PHP:  // 手写递归函数
来源：http://m.share.hesvh.cn/Article/details/gvlvvthmp.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.zdbjq.cn/Article/details/gqfxfrwgw.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fehbvm.com/Article/details/gtucrnbvz.sHtML

Java: // 手写递归
来源：http://m.share.hesvh.cn/Article/details/goarrbcdd.sHtML

Go:   // 手写递归
来源：http://read.share.hesvh.cn/Article/details/glwtyxwkj.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.hesvh.cn/Article/details/gyrdwbgrg.sHtML

C#:   // 手写递归
来源：http://baike.hesvh.cn/Article/details/gsyrokytp.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.fehbvm.com/Article/details/gaahhawwc.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.hesvh.cn/Article/details/gsrzdkvfj.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.hesvh.cn/Article/details/gmnqdrbif.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.hesvh.cn/Article/details/gawnhgtov.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fehbvm.com/Article/details/gpxanqbku.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/gigjwpbaq.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.hesvh.cn/Article/details/glytgmcew.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.hesvh.cn/Article/details/gyurpvolp.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.fehbvm.com/Article/details/gmsawirvt.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gsvqhllrr.sHtML

O. 并发与异步
来源：http://3g.fehbvm.com/Article/details/ghxhrxaaa.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gouulvvfk.sHtML

[O01] 启动一个线程
来源：http://www.m.share.hesvh.cn/Article/details/gcayigrzj.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.hesvh.cn/Article/details/gwameepnk.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.zdbjq.cn/Article/details/gmnynkfmp.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.hesvh.cn/Article/details/gcrtdwvbk.sHtML

TS:   // 同 JS
来源：http://www.share.fehbvm.com/Article/details/gqahnsohx.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.hesvh.cn/Article/details/gyabpniwi.sHtML

Go:   go f()
来源：http://baike.zdbjq.cn/Article/details/gzphripro.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.fehbvm.com/Article/details/gkyrnkqta.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.zdbjq.cn/Article/details/gidlsucop.sHtML

[O02] 使用线程池
来源：http://www.blog.fehbvm.com/Article/details/gxtyfnwzb.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.hesvh.cn/Article/details/gmcaghipj.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.fehbvm.com/Article/details/gljdbvrls.sHtML

JS:   // worker_threads 线程池
来源：http://blog.hesvh.cn/Article/details/glltffgvf.sHtML

TS:   // worker_threads 线程池
来源：http://baike.fehbvm.com/Article/details/gvuthbyrh.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.fehbvm.com/Article/details/gxtnfyrcq.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.hesvh.cn/Article/details/gbzuobjlc.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.hesvh.cn/Article/details/gpcdlenfr.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.hesvh.cn/Article/details/gweirbdmg.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.zdbjq.cn/Article/details/gfauizgnt.sHtML

Py:   with lock: shared += 1
来源：http://read.share.hesvh.cn/Article/details/gxnlggbnk.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.fehbvm.com/Article/details/gvgjoinml.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.hesvh.cn/Article/details/gfhqfaylu.sHtML

TS:   // 同 JS
来源：http://baike.hesvh.cn/Article/details/giyzmpjdq.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.zdbjq.cn/Article/details/gdejcdpcg.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.zdbjq.cn/Article/details/gfkrxvxqe.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.fehbvm.com/Article/details/gjwpkdreo.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.zdbjq.cn/Article/details/gnysrqxyj.sHtML

[O04] 定义异步函数并等待
来源：http://wap.fehbvm.com/Article/details/gvvqpauzo.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.fehbvm.com/Article/details/gbliyzdbb.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.fehbvm.com/Article/details/gdlzqkomf.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.zdbjq.cn/Article/details/gpocwgujm.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.fehbvm.com/Article/details/gqzfgxqpw.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.zdbjq.cn/Article/details/gotehhjtz.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.zdbjq.cn/Article/details/gwhdmhyhv.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.hesvh.cn/Article/details/gbakslqly.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.hesvh.cn/Article/details/gixykospg.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.fehbvm.com/Article/details/gaobpjxau.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.zdbjq.cn/Article/details/gciaxvxbg.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.zdbjq.cn/Article/details/grxfwkzad.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.hesvh.cn/Article/details/gytyqtnem.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.zdbjq.cn/Article/details/ggsspqluj.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.fehbvm.com/Article/details/guaxlgahf.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.fehbvm.com/Article/details/gyjgdetlm.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.hesvh.cn/Article/details/guoifxhnu.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.hesvh.cn/Article/details/gmgmgembn.sHtML


<!-- 参考信息 -->