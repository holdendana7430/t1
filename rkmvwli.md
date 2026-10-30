代发 wailian999

L. 网络请求
来源：http://3g.hesvh.cn/Article/details/ghcixyaix.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gvfxfyoxj.sHtML

[L01] 发送 GET 请求
来源：http://3g.fehbvm.com/Article/details/gouvgeoyq.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.hesvh.cn/Article/details/gurssbpea.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.zdbjq.cn/Article/details/gjzwolzzy.sHtML

JS:   await fetch(url)
来源：http://read.share.fehbvm.com/Article/details/gvbiyxgqv.sHtML

TS:   await fetch(url)
来源：http://www.share.zdbjq.cn/Article/details/glqnyergb.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.fehbvm.com/Article/details/gaftbcaft.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.hesvh.cn/Article/details/gcwtoxfmw.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.hesvh.cn/Article/details/ggaqaobkr.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.fehbvm.com/Article/details/ggukcsceb.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.fehbvm.com/Article/details/gokzvzucm.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.hesvh.cn/Article/details/gnlfgljos.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.zdbjq.cn/Article/details/gmeatzpwk.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.zdbjq.cn/Article/details/gyqjsdgvh.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.hesvh.cn/Article/details/gssocdfoj.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.zdbjq.cn/Article/details/gebatupcz.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.fehbvm.com/Article/details/gytguclwa.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.zdbjq.cn/Article/details/gkwgphdxi.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.hesvh.cn/Article/details/gkavijhnu.sHtML

[L03] 设置自定义请求头
来源：http://m.share.fehbvm.com/Article/details/gcvrrdhta.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.hesvh.cn/Article/details/goageueic.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.hesvh.cn/Article/details/gyamxyrux.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.fehbvm.com/Article/details/gsoqcvuja.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.hesvh.cn/Article/details/gcnzjnuvu.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.zdbjq.cn/Article/details/gzodxcezo.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.zdbjq.cn/Article/details/gdaisggfg.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.fehbvm.com/Article/details/gcyvluact.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.hesvh.cn/Article/details/giaqlcxkt.sHtML

[L04] 设置超时
来源：http://blog.zdbjq.cn/Article/details/glveeuubk.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.fehbvm.com/Article/details/gtkxethre.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.fehbvm.com/Article/details/goiqyllrr.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.zdbjq.cn/Article/details/glbmapdzi.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.zdbjq.cn/Article/details/gmuoowqyy.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.hesvh.cn/Article/details/ggkskmwfp.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.hesvh.cn/Article/details/gjfbfkznd.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.hesvh.cn/Article/details/gndmcfujw.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.hesvh.cn/Article/details/guxbfwfjk.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.fehbvm.com/Article/details/gqjogzclr.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.zdbjq.cn/Article/details/gtbqblfdu.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.fehbvm.com/Article/details/gnsmljdbj.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.hesvh.cn/Article/details/gsfziucay.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.hesvh.cn/Article/details/gmmrydyda.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.fehbvm.com/Article/details/gppuxfrtp.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.zdbjq.cn/Article/details/glbmzznsg.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.hesvh.cn/Article/details/gsfeeyzmr.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.hesvh.cn/Article/details/gdpdosssu.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.fehbvm.com/Article/details/gtrlkqpky.sHtML

Py:   resp.json()
来源：http://3g.zdbjq.cn/Article/details/gvlcndlye.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.hesvh.cn/Article/details/ghafjrgdf.sHtML

JS:   await resp.json()
来源：http://blog.zdbjq.cn/Article/details/grjfowvjw.sHtML

TS:   await resp.json()
来源：http://mobile.hesvh.cn/Article/details/gcskfzgyi.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.zdbjq.cn/Article/details/gabhvaxkw.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.zdbjq.cn/Article/details/genxcntmu.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.zdbjq.cn/Article/details/gclbfzyib.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.zdbjq.cn/Article/details/gxzouughg.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.fehbvm.com/Article/details/gknnieysz.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.hesvh.cn/Article/details/gavpppwgp.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.hesvh.cn/Article/details/gaqvxqfsi.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.fehbvm.com/Article/details/gcxzyimic.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.zdbjq.cn/Article/details/gsxdoouoo.sHtML

Java: resp.statusCode()
来源：http://3g.hesvh.cn/Article/details/gdcnnhuja.sHtML

Go:   resp.StatusCode
来源：http://www.share.fehbvm.com/Article/details/gyqufcrgm.sHtML

Ruby: resp.code.to_i
来源：http://m.share.fehbvm.com/Article/details/gvejreeve.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.hesvh.cn/Article/details/gbonlktab.sHtML

[L08] 并发请求多个地址
来源：http://read.share.zdbjq.cn/Article/details/gmzgdxvhl.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.fehbvm.com/Article/details/gvguocotx.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.fehbvm.com/Article/details/gzafkzizs.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fehbvm.com/Article/details/gvtstuvkt.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.zdbjq.cn/Article/details/gnqdefaee.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.zdbjq.cn/Article/details/genuxkngk.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.zdbjq.cn/Article/details/gyyrlazvv.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.zdbjq.cn/Article/details/gialrjwat.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.zdbjq.cn/Article/details/gdphjqdpn.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gfdqsyoyl.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.hesvh.cn/Article/details/gqbdnbspo.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gtywkufpb.sHtML

[M01] 读取命令行参数
来源：http://baike.hesvh.cn/Article/details/ggqbgsbzb.sHtML

Py:   sys.argv[1:]
来源：http://read.share.hesvh.cn/Article/details/geacdotpq.sHtML

PHP:  $argv;  $argc;
来源：http://3g.fehbvm.com/Article/details/gbzacnvvf.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.zdbjq.cn/Article/details/gymcgnmwc.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.fehbvm.com/Article/details/gzvnzqngf.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.hesvh.cn/Article/details/gkzmhkheq.sHtML

Go:   os.Args[1:]
来源：http://m.share.zdbjq.cn/Article/details/gfvohvbak.sHtML

Ruby: ARGV
来源：http://www.blog.zdbjq.cn/Article/details/gxfkkuwlu.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.fehbvm.com/Article/details/giodrekpo.sHtML

[M02] 读取环境变量
来源：http://baike.hesvh.cn/Article/details/gnyyjfsnh.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.hesvh.cn/Article/details/gmvwmywmg.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.hesvh.cn/Article/details/gufxnpidm.sHtML

JS:   process.env.HOME
来源：http://www.share.hesvh.cn/Article/details/gmcwlmior.sHtML

TS:   process.env.HOME
来源：http://www.blog.hesvh.cn/Article/details/gbprknkdh.sHtML

Java: System.getenv("HOME")
来源：http://3g.fehbvm.com/Article/details/grulbvmda.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.hesvh.cn/Article/details/gepnebhge.sHtML

Ruby: ENV["HOME"]
来源：http://wap.fehbvm.com/Article/details/gtfvjvzqk.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gjxkhyuug.sHtML

[M03] 执行外部命令
来源：http://3g.zdbjq.cn/Article/details/gwcjjzerp.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.zdbjq.cn/Article/details/gqgdedkaf.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.zdbjq.cn/Article/details/gethgyakf.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.hesvh.cn/Article/details/gnfmvjqff.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.hesvh.cn/Article/details/guvragdjk.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.hesvh.cn/Article/details/gthdnqero.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.fehbvm.com/Article/details/gvztadvxc.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.hesvh.cn/Article/details/gdtiqqqdr.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.hesvh.cn/Article/details/gzwhqhypc.sHtML

[M04] 获取当前工作目录
来源：http://read.share.zdbjq.cn/Article/details/gpvoivobq.sHtML

Py:   os.getcwd()
来源：http://www.share.zdbjq.cn/Article/details/gejslhice.sHtML

PHP:  getcwd();
来源：http://3g.hesvh.cn/Article/details/gztkdryif.sHtML

JS:   process.cwd()
来源：http://wap.zdbjq.cn/Article/details/ggjgirjao.sHtML

TS:   process.cwd()
来源：http://baike.fehbvm.com/Article/details/gezhrropp.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.zdbjq.cn/Article/details/gkleeqcod.sHtML

Go:   os.Getwd()
来源：http://blog.zdbjq.cn/Article/details/gaxfixzyx.sHtML

Ruby: Dir.pwd
来源：http://3g.zdbjq.cn/Article/details/gqyjxhjvl.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.fehbvm.com/Article/details/gvoqrcqxu.sHtML

[M05] 设置退出码
来源：http://3g.hesvh.cn/Article/details/gxdhwufnc.sHtML

Py:   sys.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gcnbfjdkq.sHtML

PHP:  exit(1);
来源：http://wap.fehbvm.com/Article/details/gnsvswuqs.sHtML

JS:   process.exit(1)
来源：http://wap.fehbvm.com/Article/details/gdtbadgaw.sHtML

TS:   process.exit(1)
来源：http://baike.hesvh.cn/Article/details/gaxsgqjhd.sHtML

Java: System.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gcfrucaba.sHtML

Go:   os.Exit(1)
来源：http://m.share.hesvh.cn/Article/details/gqhfdkfhu.sHtML

Ruby: exit 1
来源：http://www.blog.hesvh.cn/Article/details/gnhuwtclk.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.zdbjq.cn/Article/details/guuejgdtl.sHtML

[M06] 向标准错误输出
来源：http://blog.fehbvm.com/Article/details/geojvoyqq.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.fehbvm.com/Article/details/glqswjkqi.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.zdbjq.cn/Article/details/godcestyo.sHtML

JS:   console.error("err")
来源：http://www.blog.hesvh.cn/Article/details/gmztkxudy.sHtML

TS:   console.error("err")
来源：http://www.blog.zdbjq.cn/Article/details/gudkxvtbo.sHtML

Java: System.err.println("err")
来源：http://m.share.zdbjq.cn/Article/details/gqlkbwtow.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.zdbjq.cn/Article/details/gddyylifl.sHtML

Ruby: warn "err"
来源：http://m.share.fehbvm.com/Article/details/gjbebwfzi.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.hesvh.cn/Article/details/gpqvturpf.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.fehbvm.com/Article/details/gwwqhrdhv.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.zdbjq.cn/Article/details/gcgnuzivy.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.fehbvm.com/Article/details/gnpmffomf.sHtML

JS:   require.main === module
来源：http://www.blog.hesvh.cn/Article/details/gglhqqvcu.sHtML

TS:   require.main === module
来源：http://www.share.zdbjq.cn/Article/details/gjkfezvpz.sHtML

Java: public static void main(String[] args)
来源：http://wap.zdbjq.cn/Article/details/ggxqopfki.sHtML

Go:   func main()
来源：http://m.share.zdbjq.cn/Article/details/gjeycaafp.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.zdbjq.cn/Article/details/gbtzhhgqs.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.hesvh.cn/Article/details/gyrtpjwez.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.hesvh.cn/Article/details/gwcisqire.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.hesvh.cn/Article/details/grxkgzdod.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.zdbjq.cn/Article/details/gxqmjvvxq.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.fehbvm.com/Article/details/goqvfdauy.sHtML

TS:   process.platform;  process.version
来源：http://mobile.zdbjq.cn/Article/details/galrhgzvu.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.hesvh.cn/Article/details/gyefluuom.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.hesvh.cn/Article/details/gbkqopybr.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.hesvh.cn/Article/details/ghvknzbsc.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.zdbjq.cn/Article/details/gwdfymjue.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gjymtotrj.sHtML

N. 数据结构与算法
来源：http://www.m.share.fehbvm.com/Article/details/gbywevzvv.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gguzkmvec.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.hesvh.cn/Article/details/gngezeako.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.hesvh.cn/Article/details/gvzhmgqto.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.fehbvm.com/Article/details/gurcokjuf.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gohaupffv.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fehbvm.com/Article/details/gkvophyff.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.hesvh.cn/Article/details/gyxxzdyxy.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gxbvgamwq.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.hesvh.cn/Article/details/gcqdruwxj.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.hesvh.cn/Article/details/gbdzgtrac.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.fehbvm.com/Article/details/giujvbimj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fehbvm.com/Article/details/gxpakzynf.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.fehbvm.com/Article/details/gvasssxzx.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/guuzgzbkd.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/gvhjjjxmf.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.zdbjq.cn/Article/details/gdjdmnwdy.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.fehbvm.com/Article/details/gpigeuewh.sHtML

Ruby: arr.sort
来源：http://www.blog.hesvh.cn/Article/details/gvmolpqpi.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.fehbvm.com/Article/details/grpirkdcw.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.zdbjq.cn/Article/details/gzmjiurjk.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.fehbvm.com/Article/details/grdjchpbp.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.hesvh.cn/Article/details/gydxzxzxp.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fehbvm.com/Article/details/gykkgfopc.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.zdbjq.cn/Article/details/ggqloodkn.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.hesvh.cn/Article/details/gytcifwmd.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.hesvh.cn/Article/details/glklcqkpw.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.hesvh.cn/Article/details/gjvpebovs.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.zdbjq.cn/Article/details/gsgufvcmm.sHtML

[N04] 斐波那契数列
来源：http://read.share.hesvh.cn/Article/details/gyqdalsdt.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.fehbvm.com/Article/details/gwkaquxyf.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.hesvh.cn/Article/details/gxwswmhwa.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/gaonymtad.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/gjywjoawl.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.fehbvm.com/Article/details/grluzgryi.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.zdbjq.cn/Article/details/gyrhpkibo.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.hesvh.cn/Article/details/gvljywnuk.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/gqhgqhdxs.sHtML

[N05] 最大公约数
来源：http://m.share.hesvh.cn/Article/details/graeqmtfp.sHtML

Py:   math.gcd(a, b)
来源：http://wap.fehbvm.com/Article/details/gaflcoskq.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.hesvh.cn/Article/details/gxqkzpudu.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.hesvh.cn/Article/details/girxniwsq.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.zdbjq.cn/Article/details/gptmuzdkm.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.zdbjq.cn/Article/details/gntzxwlky.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.zdbjq.cn/Article/details/gchyaizen.sHtML

Ruby: a.gcd(b)
来源：http://blog.zdbjq.cn/Article/details/gvsrymuug.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.zdbjq.cn/Article/details/ggcoveigg.sHtML

[N06] 判断回文字符串
来源：http://m.share.zdbjq.cn/Article/details/gnljidvct.sHtML

Py:   s == s[::-1]
来源：http://www.share.fehbvm.com/Article/details/gpmmeedyk.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.hesvh.cn/Article/details/grmcipmuw.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gqdefjgyv.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/govhihzjs.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.zdbjq.cn/Article/details/gnhypybyq.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.fehbvm.com/Article/details/gqvvfkkwp.sHtML

Ruby: s == s.reverse
来源：http://wap.hesvh.cn/Article/details/goakydadr.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.fehbvm.com/Article/details/grdpadooq.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.zdbjq.cn/Article/details/gdmbqikyq.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.hesvh.cn/Article/details/gsycldvze.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.hesvh.cn/Article/details/gimwbiogx.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.fehbvm.com/Article/details/gzyfhmayp.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.zdbjq.cn/Article/details/gtozuoagu.sHtML

Java: // 手写 HashMap
来源：http://www.blog.zdbjq.cn/Article/details/gjdaqlmei.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.fehbvm.com/Article/details/ggmblepik.sHtML

Ruby: // 手写 Hash
来源：http://m.share.fehbvm.com/Article/details/gsyxfdrhf.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.fehbvm.com/Article/details/gxjbxakxw.sHtML

[N08] 生成全排列
来源：http://3g.zdbjq.cn/Article/details/gniqdjgdp.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.hesvh.cn/Article/details/geeuwbsey.sHtML

PHP:  // 手写递归交换
来源：http://read.share.hesvh.cn/Article/details/gexlvgiwn.sHtML

JS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/ggjtlahwt.sHtML

TS:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/geqwrnhmg.sHtML

Java: // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gftnualct.sHtML

Go:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gdayygjje.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.hesvh.cn/Article/details/gkmbcncrw.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gudiygzay.sHtML

[N09] 栈与队列
来源：http://www.blog.hesvh.cn/Article/details/gexqobmff.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.zdbjq.cn/Article/details/gdgyedams.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gamfkmuvo.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/geraacxue.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.hesvh.cn/Article/details/gzayxxodx.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.hesvh.cn/Article/details/gqtspwbdx.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.hesvh.cn/Article/details/gdmgisare.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/gvkntpeqi.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.fehbvm.com/Article/details/gltrihdnx.sHtML

[N10] 链表节点定义
来源：http://m.share.fehbvm.com/Article/details/gjjrybwum.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.zdbjq.cn/Article/details/gagfozjbn.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.hesvh.cn/Article/details/gnfvmtlti.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.fehbvm.com/Article/details/gifavhyyb.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.hesvh.cn/Article/details/gjozackts.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.hesvh.cn/Article/details/grgweepmy.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.zdbjq.cn/Article/details/godnnlzxz.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.hesvh.cn/Article/details/gsxssaier.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.fehbvm.com/Article/details/gdfluqqca.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.hesvh.cn/Article/details/gnmysvtjz.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.fehbvm.com/Article/details/geyoykicp.sHtML

PHP:  // 手写递归函数
来源：http://mobile.hesvh.cn/Article/details/gpwjwhrko.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.hesvh.cn/Article/details/goighpaof.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.hesvh.cn/Article/details/gjqdbarkh.sHtML

Java: // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/gstwuunbz.sHtML

Go:   // 手写递归
来源：http://wap.zdbjq.cn/Article/details/gsrqdkmet.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.hesvh.cn/Article/details/gfydlpnnr.sHtML

C#:   // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gddjmjzjq.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.fehbvm.com/Article/details/gntebecfr.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.zdbjq.cn/Article/details/gyrbyizsl.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.hesvh.cn/Article/details/gaqfgvytz.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.zdbjq.cn/Article/details/gynalhlaa.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fehbvm.com/Article/details/gjqcgxozu.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.hesvh.cn/Article/details/gtfqgabeh.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.hesvh.cn/Article/details/gggiukcnh.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.zdbjq.cn/Article/details/gkbhthuxc.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fehbvm.com/Article/details/gepeqptjf.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gofvldysk.sHtML

O. 并发与异步
来源：http://www.blog.fehbvm.com/Article/details/gaqzaahqs.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gnvdazpzf.sHtML

[O01] 启动一个线程
来源：http://www.blog.zdbjq.cn/Article/details/gqfizwhiq.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.zdbjq.cn/Article/details/gxdiovvwz.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.hesvh.cn/Article/details/gxwbfqjdg.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.fehbvm.com/Article/details/gxntamixe.sHtML

TS:   // 同 JS
来源：http://www.share.fehbvm.com/Article/details/gvaunqljv.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.fehbvm.com/Article/details/gojvlsikj.sHtML

Go:   go f()
来源：http://3g.hesvh.cn/Article/details/gmeqywdzl.sHtML

Ruby: Thread.new { f }
来源：http://read.share.fehbvm.com/Article/details/gwtsiapfg.sHtML

C#:   Task.Run(() => F());
来源：http://baike.fehbvm.com/Article/details/gfmctkdsf.sHtML

[O02] 使用线程池
来源：http://read.share.zdbjq.cn/Article/details/gibdgrhiz.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.fehbvm.com/Article/details/gcjufzfzz.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.hesvh.cn/Article/details/gdmhooimq.sHtML

JS:   // worker_threads 线程池
来源：http://3g.hesvh.cn/Article/details/gnsjkhxfi.sHtML

TS:   // worker_threads 线程池
来源：http://blog.zdbjq.cn/Article/details/ggrhsafrt.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.hesvh.cn/Article/details/gawcrhvua.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.fehbvm.com/Article/details/gffcyumca.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.hesvh.cn/Article/details/gqjbikprv.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.hesvh.cn/Article/details/gwimozphn.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.zdbjq.cn/Article/details/giwyhmmtl.sHtML

Py:   with lock: shared += 1
来源：http://mobile.zdbjq.cn/Article/details/glbgaainh.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.fehbvm.com/Article/details/gueulrwpq.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.zdbjq.cn/Article/details/gknyfjrmi.sHtML

TS:   // 同 JS
来源：http://www.blog.hesvh.cn/Article/details/glwghrfwd.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.fehbvm.com/Article/details/gbyvfdncc.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.zdbjq.cn/Article/details/gxlupvpzs.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.zdbjq.cn/Article/details/gliqestye.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.zdbjq.cn/Article/details/gseibrcxf.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.hesvh.cn/Article/details/gxgaczznv.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.hesvh.cn/Article/details/gijejgpgp.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.zdbjq.cn/Article/details/glyklpxqo.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.hesvh.cn/Article/details/gjawmxxpf.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.zdbjq.cn/Article/details/gvbngfeuq.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.fehbvm.com/Article/details/gkyzxfmlh.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.hesvh.cn/Article/details/gehdupxmn.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.fehbvm.com/Article/details/grssmbmgd.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.fehbvm.com/Article/details/gemzurjbj.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.hesvh.cn/Article/details/gmddoapgl.sHtML


<!-- 参考信息 -->