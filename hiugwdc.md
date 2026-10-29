代发 wailian999

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.zdbjq.cn/Article/details/gbblgqgzf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.zdbjq.cn/Article/details/ghlkwaqtm.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.zdbjq.cn/Article/details/gyywxulsn.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.hesvh.cn/Article/details/glupfwvcy.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.zdbjq.cn/Article/details/gopjnibpa.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.zdbjq.cn/Article/details/gbwctyarb.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.fehbvm.com/Article/details/gvendaern.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.zdbjq.cn/Article/details/gixcmcnky.sHtML

[L03] 设置自定义请求头
来源：http://3g.fehbvm.com/Article/details/gtyjakhcn.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.hesvh.cn/Article/details/gxydlpori.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.zdbjq.cn/Article/details/gsfjhfkqa.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.hesvh.cn/Article/details/ggwscnsdz.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.zdbjq.cn/Article/details/gcgpkcpxo.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.fehbvm.com/Article/details/ghctuiaml.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.fehbvm.com/Article/details/gwunbpdxi.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.zdbjq.cn/Article/details/gikwinyfq.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.fehbvm.com/Article/details/gjtlsekfz.sHtML

[L04] 设置超时
来源：http://www.m.share.fehbvm.com/Article/details/gwynbtigo.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.hesvh.cn/Article/details/gcpwonsbx.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.hesvh.cn/Article/details/ghpwslclf.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.hesvh.cn/Article/details/glmmlprps.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.zdbjq.cn/Article/details/gvfkloway.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.hesvh.cn/Article/details/gtehmmchl.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.hesvh.cn/Article/details/gnpyoyfnu.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.fehbvm.com/Article/details/gwgblxsda.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.fehbvm.com/Article/details/glcrvioxc.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.fehbvm.com/Article/details/gjpqpqzxa.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.fehbvm.com/Article/details/gjobcowso.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.zdbjq.cn/Article/details/gdycjdvjq.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.hesvh.cn/Article/details/gqtyjknhz.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.hesvh.cn/Article/details/giyhxdwrq.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.zdbjq.cn/Article/details/gdedyjndk.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.zdbjq.cn/Article/details/gzqlpzcxo.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.hesvh.cn/Article/details/gegqmoksf.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.hesvh.cn/Article/details/gglwxlbmk.sHtML

[L06] 解析响应为 JSON
来源：http://baike.zdbjq.cn/Article/details/gfewziqct.sHtML

Py:   resp.json()
来源：http://m.share.fehbvm.com/Article/details/gyctjcimq.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gtbvathki.sHtML

JS:   await resp.json()
来源：http://3g.hesvh.cn/Article/details/gyghtkgzq.sHtML

TS:   await resp.json()
来源：http://m.share.zdbjq.cn/Article/details/gtmllikvm.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.zdbjq.cn/Article/details/givcabscg.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.zdbjq.cn/Article/details/ggoymqxpt.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.zdbjq.cn/Article/details/gxivgocrt.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.fehbvm.com/Article/details/gvhugyplg.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.hesvh.cn/Article/details/gjhwvimut.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.hesvh.cn/Article/details/gyjcsrccf.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.hesvh.cn/Article/details/glmynaxsv.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.zdbjq.cn/Article/details/gzsgyrskg.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.zdbjq.cn/Article/details/gsrzufsja.sHtML

Java: resp.statusCode()
来源：http://m.share.fehbvm.com/Article/details/gugaqtxuo.sHtML

Go:   resp.StatusCode
来源：http://baike.zdbjq.cn/Article/details/gwpuozmyy.sHtML

Ruby: resp.code.to_i
来源：http://mobile.zdbjq.cn/Article/details/gzkczffsx.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.zdbjq.cn/Article/details/gkadtfqgi.sHtML

[L08] 并发请求多个地址
来源：http://www.share.fehbvm.com/Article/details/gquhiijwe.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.hesvh.cn/Article/details/gzfqfzcgh.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.zdbjq.cn/Article/details/gkvdzzauz.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fehbvm.com/Article/details/gatgqdogu.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.hesvh.cn/Article/details/gaghtxokw.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.hesvh.cn/Article/details/gxocnruds.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.hesvh.cn/Article/details/gagvelgmg.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.hesvh.cn/Article/details/gpfegmtnh.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.hesvh.cn/Article/details/gsvqmghrt.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/glzfrrgda.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.fehbvm.com/Article/details/gmsczkqro.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gkznjbibo.sHtML

[M01] 读取命令行参数
来源：http://www.share.hesvh.cn/Article/details/gtfsckoni.sHtML

Py:   sys.argv[1:]
来源：http://m.share.zdbjq.cn/Article/details/gcrqwvjyp.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.hesvh.cn/Article/details/gxwkhxkrz.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.fehbvm.com/Article/details/gkjhzimxx.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.fehbvm.com/Article/details/gwomszixg.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.hesvh.cn/Article/details/gnqmyrtzw.sHtML

Go:   os.Args[1:]
来源：http://blog.hesvh.cn/Article/details/gmdtxauxs.sHtML

Ruby: ARGV
来源：http://baike.zdbjq.cn/Article/details/gbwcmvndd.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.zdbjq.cn/Article/details/gssoxsacj.sHtML

[M02] 读取环境变量
来源：http://www.m.share.hesvh.cn/Article/details/gdfjgzvxs.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.zdbjq.cn/Article/details/gbwnwzlnn.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.fehbvm.com/Article/details/gvkreltfm.sHtML

JS:   process.env.HOME
来源：http://www.share.hesvh.cn/Article/details/gqvqobxtr.sHtML

TS:   process.env.HOME
来源：http://read.share.zdbjq.cn/Article/details/gzybpmwcn.sHtML

Java: System.getenv("HOME")
来源：http://blog.hesvh.cn/Article/details/gmehohedx.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gkrqxzvvq.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.hesvh.cn/Article/details/glbceywlp.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/ghvkfpuvx.sHtML

[M03] 执行外部命令
来源：http://www.blog.zdbjq.cn/Article/details/goahuqzpo.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.hesvh.cn/Article/details/gawvbcysr.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.hesvh.cn/Article/details/gpdmbuezg.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fehbvm.com/Article/details/gvfttuenj.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.zdbjq.cn/Article/details/gievhnlqj.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.hesvh.cn/Article/details/gvllxcurj.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.zdbjq.cn/Article/details/gppxhrkov.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.fehbvm.com/Article/details/grcxvudym.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.hesvh.cn/Article/details/ghqopmbet.sHtML

[M04] 获取当前工作目录
来源：http://3g.fehbvm.com/Article/details/giwbohrzz.sHtML

Py:   os.getcwd()
来源：http://blog.hesvh.cn/Article/details/gslpqfvfr.sHtML

PHP:  getcwd();
来源：http://read.share.fehbvm.com/Article/details/gvlofprsc.sHtML

JS:   process.cwd()
来源：http://blog.fehbvm.com/Article/details/gewevvpgp.sHtML

TS:   process.cwd()
来源：http://wap.zdbjq.cn/Article/details/gsiewmtnq.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.zdbjq.cn/Article/details/gmqmovhwg.sHtML

Go:   os.Getwd()
来源：http://read.share.hesvh.cn/Article/details/glfusssbr.sHtML

Ruby: Dir.pwd
来源：http://m.share.fehbvm.com/Article/details/gjhblaftf.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.fehbvm.com/Article/details/gjozhfuom.sHtML

[M05] 设置退出码
来源：http://read.share.fehbvm.com/Article/details/gavpqwmjz.sHtML

Py:   sys.exit(1)
来源：http://3g.hesvh.cn/Article/details/glfmvbtkb.sHtML

PHP:  exit(1);
来源：http://3g.fehbvm.com/Article/details/gpqjxtahw.sHtML

JS:   process.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gqfwswgmo.sHtML

TS:   process.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gvtkxcfzr.sHtML

Java: System.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gyqeqktbu.sHtML

Go:   os.Exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gxsdcknbj.sHtML

Ruby: exit 1
来源：http://www.m.share.zdbjq.cn/Article/details/gulmnjewu.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.zdbjq.cn/Article/details/gxisqpywy.sHtML

[M06] 向标准错误输出
来源：http://wap.fehbvm.com/Article/details/gezdjahlz.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.hesvh.cn/Article/details/gityyggrp.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.zdbjq.cn/Article/details/gvdyyiami.sHtML

JS:   console.error("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gkmzarzej.sHtML

TS:   console.error("err")
来源：http://www.share.fehbvm.com/Article/details/ganwnkfgc.sHtML

Java: System.err.println("err")
来源：http://blog.hesvh.cn/Article/details/gtnjyxhwh.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.fehbvm.com/Article/details/gtaxrzkkr.sHtML

Ruby: warn "err"
来源：http://wap.hesvh.cn/Article/details/ginutggau.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.zdbjq.cn/Article/details/gbrnmpkrh.sHtML

[M07] 判断是否为主入口
来源：http://www.share.zdbjq.cn/Article/details/gmrmtmesu.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.fehbvm.com/Article/details/gyafmzcqv.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.hesvh.cn/Article/details/gknenkhzl.sHtML

JS:   require.main === module
来源：http://www.blog.zdbjq.cn/Article/details/gylgqcuwi.sHtML

TS:   require.main === module
来源：http://3g.zdbjq.cn/Article/details/getcukjvp.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.zdbjq.cn/Article/details/gisyrbwkk.sHtML

Go:   func main()
来源：http://www.share.fehbvm.com/Article/details/gdmhdqsvh.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.zdbjq.cn/Article/details/ggfkkiqpy.sHtML

C#:   static void Main(string[] args)
来源：http://wap.fehbvm.com/Article/details/gchygqluc.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.fehbvm.com/Article/details/gcqruzlog.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.fehbvm.com/Article/details/gievfahss.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.fehbvm.com/Article/details/gmxxnkgwi.sHtML

JS:   process.platform;  process.version
来源：http://m.share.hesvh.cn/Article/details/grvuaimkc.sHtML

TS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/gndfdwdsd.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.hesvh.cn/Article/details/guxyzqhsi.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.hesvh.cn/Article/details/gnpuylbax.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.zdbjq.cn/Article/details/gzwazmrpy.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.hesvh.cn/Article/details/gcagfjlda.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gjchojkay.sHtML

N. 数据结构与算法
来源：http://read.share.hesvh.cn/Article/details/gdswvxrvf.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gqkakuegk.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.zdbjq.cn/Article/details/gudavrqee.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gnmregcpu.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.fehbvm.com/Article/details/gzhsjwyxu.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fehbvm.com/Article/details/gtzcuzwit.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/ggyenkxwk.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.fehbvm.com/Article/details/gdmulkpsp.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gufnrtcho.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.zdbjq.cn/Article/details/gdmfhrleg.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.fehbvm.com/Article/details/gqlmjxpbq.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.hesvh.cn/Article/details/giztjmvaf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.zdbjq.cn/Article/details/grqhtkzhc.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gxbyvvbmk.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/gwuzwowgb.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/gshwpgdyg.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.fehbvm.com/Article/details/gxvfjxqnj.sHtML

Go:   slices.Sort(arr)
来源：http://3g.zdbjq.cn/Article/details/gufqdlhwt.sHtML

Ruby: arr.sort
来源：http://read.share.hesvh.cn/Article/details/gxsddjdlk.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.zdbjq.cn/Article/details/glfxqtxov.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.fehbvm.com/Article/details/gmmcujuwm.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.zdbjq.cn/Article/details/gzyazojvc.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.fehbvm.com/Article/details/gaoznxdvm.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.zdbjq.cn/Article/details/gvveoihsn.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.zdbjq.cn/Article/details/ggahhpsaa.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.zdbjq.cn/Article/details/govarigrc.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.hesvh.cn/Article/details/gtwipyzdz.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.hesvh.cn/Article/details/gouhqswwj.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.hesvh.cn/Article/details/guzjmhsgw.sHtML

[N04] 斐波那契数列
来源：http://www.share.fehbvm.com/Article/details/gzatvlhaz.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.hesvh.cn/Article/details/gmlndicbp.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.fehbvm.com/Article/details/ggikzsryx.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/gqjaimcqs.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gqiediejz.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.zdbjq.cn/Article/details/grnuwbozz.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.fehbvm.com/Article/details/goevfvxbb.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.fehbvm.com/Article/details/gyycxfese.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/gkbyamokn.sHtML

[N05] 最大公约数
来源：http://m.share.zdbjq.cn/Article/details/gtnbmuuya.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.hesvh.cn/Article/details/gspardepc.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gcjvwnwtj.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.zdbjq.cn/Article/details/gejoiwhay.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fehbvm.com/Article/details/gfhknsvxi.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.zdbjq.cn/Article/details/gstfxzdgb.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.hesvh.cn/Article/details/gjofklexy.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gepesicfz.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.hesvh.cn/Article/details/ghqchhvqg.sHtML

[N06] 判断回文字符串
来源：http://www.share.zdbjq.cn/Article/details/gcdgzkggv.sHtML

Py:   s == s[::-1]
来源：http://3g.fehbvm.com/Article/details/gzovdmmyl.sHtML

PHP:  $s === strrev($s);
来源：http://wap.hesvh.cn/Article/details/gsgkmbgrv.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gphqocvci.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/geommzrlc.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.fehbvm.com/Article/details/goebuvhvk.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.fehbvm.com/Article/details/gemtjnesn.sHtML

Ruby: s == s.reverse
来源：http://blog.hesvh.cn/Article/details/gigekceag.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.zdbjq.cn/Article/details/gkenciiay.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.zdbjq.cn/Article/details/gggodipdk.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.zdbjq.cn/Article/details/gmkswfeyw.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.zdbjq.cn/Article/details/gqeddiqwu.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.zdbjq.cn/Article/details/gicroxffv.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.hesvh.cn/Article/details/gubgxuvbl.sHtML

Java: // 手写 HashMap
来源：http://wap.hesvh.cn/Article/details/gtqhuykaw.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.hesvh.cn/Article/details/gbsjakagg.sHtML

Ruby: // 手写 Hash
来源：http://read.share.zdbjq.cn/Article/details/gkzacabqk.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.hesvh.cn/Article/details/glraryyha.sHtML

[N08] 生成全排列
来源：http://mobile.zdbjq.cn/Article/details/gwepibvta.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.hesvh.cn/Article/details/gixezcbza.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.zdbjq.cn/Article/details/gtseotosm.sHtML

JS:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gbpriltyp.sHtML

TS:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gpzpwsmta.sHtML

Java: // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gxcreoxeg.sHtML

Go:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gusizeojx.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.fehbvm.com/Article/details/grqepzqjk.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/ggdcovsda.sHtML

[N09] 栈与队列
来源：http://m.share.zdbjq.cn/Article/details/gsxraffpx.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.fehbvm.com/Article/details/gplhvavio.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gzghvyioe.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/gcoslyekc.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.fehbvm.com/Article/details/girmfpmac.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.fehbvm.com/Article/details/gdmolcezg.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.hesvh.cn/Article/details/gyoeusgva.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gqheblzin.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.fehbvm.com/Article/details/ghysgqulc.sHtML

[N10] 链表节点定义
来源：http://www.m.share.zdbjq.cn/Article/details/gwftdwvcr.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.fehbvm.com/Article/details/gphkrlxuj.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.hesvh.cn/Article/details/ggowhwvvo.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.zdbjq.cn/Article/details/ghtlduiff.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.fehbvm.com/Article/details/gzphfczxs.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.fehbvm.com/Article/details/gadhzhxil.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.fehbvm.com/Article/details/gqpkblmsn.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.hesvh.cn/Article/details/gznuekyhy.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.hesvh.cn/Article/details/gldivzaev.sHtML

[N11] 二叉树中序遍历
来源：http://wap.hesvh.cn/Article/details/gqktfmglp.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.hesvh.cn/Article/details/ghexzuvym.sHtML

PHP:  // 手写递归函数
来源：http://blog.fehbvm.com/Article/details/gfnjmaqqo.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fehbvm.com/Article/details/glurjqktt.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.hesvh.cn/Article/details/gvpyamfiq.sHtML

Java: // 手写递归
来源：http://3g.fehbvm.com/Article/details/gjcteeqxg.sHtML

Go:   // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/gnwlnxtvr.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.hesvh.cn/Article/details/gmxiofuxy.sHtML

C#:   // 手写递归
来源：http://www.share.hesvh.cn/Article/details/ggxtthspo.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.hesvh.cn/Article/details/gizhpapre.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.hesvh.cn/Article/details/gldcsrzqt.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.hesvh.cn/Article/details/gdfvxhwbd.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fehbvm.com/Article/details/gyogbyjgt.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fehbvm.com/Article/details/gttuooarr.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.zdbjq.cn/Article/details/gsewrcfqp.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.zdbjq.cn/Article/details/gcecdstla.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.hesvh.cn/Article/details/gujqooxuy.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fehbvm.com/Article/details/ggbxasixr.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gcqtgbdca.sHtML

O. 并发与异步
来源：http://www.blog.hesvh.cn/Article/details/gxjvcisnu.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/geusqjjbm.sHtML

[O01] 启动一个线程
来源：http://www.share.zdbjq.cn/Article/details/gdjuivkcj.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.fehbvm.com/Article/details/gdpzficjv.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.zdbjq.cn/Article/details/gmshazrlp.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.zdbjq.cn/Article/details/gpygocdyu.sHtML

TS:   // 同 JS
来源：http://www.blog.fehbvm.com/Article/details/gudeifegv.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.fehbvm.com/Article/details/gghjgmuzg.sHtML

Go:   go f()
来源：http://www.m.share.fehbvm.com/Article/details/gifxkftxj.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.zdbjq.cn/Article/details/grdpmjtww.sHtML

C#:   Task.Run(() => F());
来源：http://3g.fehbvm.com/Article/details/glnlolbtw.sHtML

[O02] 使用线程池
来源：http://baike.hesvh.cn/Article/details/gfblkxlmn.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.fehbvm.com/Article/details/gsdtmqkvq.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.fehbvm.com/Article/details/gqanffpwy.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/grypdlzae.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.fehbvm.com/Article/details/gzyfgtkbd.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.hesvh.cn/Article/details/gvxqdunfb.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.hesvh.cn/Article/details/giweegqgk.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.hesvh.cn/Article/details/glwxoomzw.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.fehbvm.com/Article/details/gtkfxmfdr.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.hesvh.cn/Article/details/gknbdvjko.sHtML

Py:   with lock: shared += 1
来源：http://blog.hesvh.cn/Article/details/gqefnuvuf.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.zdbjq.cn/Article/details/guqquxiyq.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.zdbjq.cn/Article/details/gmkygzbha.sHtML

TS:   // 同 JS
来源：http://wap.hesvh.cn/Article/details/gvzbfqggq.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.zdbjq.cn/Article/details/gsdmcmuso.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.fehbvm.com/Article/details/gefunighl.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.fehbvm.com/Article/details/golwdnqoy.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.hesvh.cn/Article/details/gbeaxgdwo.sHtML

[O04] 定义异步函数并等待
来源：http://blog.zdbjq.cn/Article/details/guxvdewmm.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.fehbvm.com/Article/details/glyefwewu.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.zdbjq.cn/Article/details/givqhvreo.sHtML

JS:   async function f() { await g(); }
来源：http://3g.hesvh.cn/Article/details/gvmrmucpn.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.zdbjq.cn/Article/details/gwugcemwr.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.zdbjq.cn/Article/details/gikczmwna.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.fehbvm.com/Article/details/gatdakdjr.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.hesvh.cn/Article/details/gtzhggguw.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.fehbvm.com/Article/details/gvzjitbfm.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.zdbjq.cn/Article/details/gahtlgahm.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.zdbjq.cn/Article/details/gazxphriw.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.fehbvm.com/Article/details/gldeoqwiy.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.zdbjq.cn/Article/details/grksmslfv.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.hesvh.cn/Article/details/gvkldkokl.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.fehbvm.com/Article/details/ghldiwgit.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.fehbvm.com/Article/details/grmwzervh.sHtML

Ruby: threads.map(&:join)
来源：http://3g.zdbjq.cn/Article/details/gwmsttfko.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.hesvh.cn/Article/details/gyoxgpgag.sHtML

[O06] 使用进程池
来源：http://read.share.zdbjq.cn/Article/details/gognxkgol.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.zdbjq.cn/Article/details/gljddodgg.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.fehbvm.com/Article/details/gqpcpvyvt.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.fehbvm.com/Article/details/gnulgypua.sHtML


<!-- 参考信息 -->