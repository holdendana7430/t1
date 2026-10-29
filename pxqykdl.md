代发 wailian999

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.zdbjq.cn/Article/details/gptcgppek.sHtML

JS:   await fetch(url)
来源：http://baike.zdbjq.cn/Article/details/gyluasujw.sHtML

TS:   await fetch(url)
来源：http://baike.zdbjq.cn/Article/details/goxacljvp.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.fehbvm.com/Article/details/gkwrtsycx.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.zdbjq.cn/Article/details/gpyijfpdb.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.zdbjq.cn/Article/details/garvkrgyh.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.zdbjq.cn/Article/details/gumohqvsj.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.zdbjq.cn/Article/details/gtyuepdxq.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.fehbvm.com/Article/details/gilavhbpg.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.zdbjq.cn/Article/details/gufgndqvh.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.hesvh.cn/Article/details/gvzrqvcwh.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.hesvh.cn/Article/details/gxlchzftg.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.fehbvm.com/Article/details/gxjehbvoo.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.fehbvm.com/Article/details/ghhapeeka.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.hesvh.cn/Article/details/gtvwqcqff.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.fehbvm.com/Article/details/gjstzyfkj.sHtML

[L03] 设置自定义请求头
来源：http://read.share.hesvh.cn/Article/details/gnbpljysw.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.fehbvm.com/Article/details/gyhcfyaxq.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.hesvh.cn/Article/details/ggxtujduo.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.fehbvm.com/Article/details/gbzpfiqje.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.hesvh.cn/Article/details/gvjewxxkz.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.zdbjq.cn/Article/details/glovrofzn.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.zdbjq.cn/Article/details/gcwjleexh.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.fehbvm.com/Article/details/gnutabjwf.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.fehbvm.com/Article/details/giezssyzf.sHtML

[L04] 设置超时
来源：http://www.share.hesvh.cn/Article/details/gckfcixig.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.hesvh.cn/Article/details/gmqyihtev.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.zdbjq.cn/Article/details/gwxngrphk.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.hesvh.cn/Article/details/ggamvoqys.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.zdbjq.cn/Article/details/glytqeiif.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.hesvh.cn/Article/details/gxmvtpngj.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.hesvh.cn/Article/details/gbodcwvkj.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.fehbvm.com/Article/details/gdgipnxic.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.hesvh.cn/Article/details/gqwudvxsj.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.hesvh.cn/Article/details/gmljcdriv.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.fehbvm.com/Article/details/gqjqipdxm.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.zdbjq.cn/Article/details/gvcefaohm.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.zdbjq.cn/Article/details/gsukmryhy.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.zdbjq.cn/Article/details/gmrocsffr.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.zdbjq.cn/Article/details/gyezpzuik.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.zdbjq.cn/Article/details/gqobcckha.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.hesvh.cn/Article/details/greyhtdbr.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.hesvh.cn/Article/details/gyxfwymyz.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.fehbvm.com/Article/details/gqljfoynz.sHtML

Py:   resp.json()
来源：http://blog.fehbvm.com/Article/details/gbuhbxknp.sHtML

PHP:  json_decode($body, true);
来源：http://wap.hesvh.cn/Article/details/gdcescifv.sHtML

JS:   await resp.json()
来源：http://www.m.share.fehbvm.com/Article/details/gzmhrkxxr.sHtML

TS:   await resp.json()
来源：http://www.blog.fehbvm.com/Article/details/gjbtbyiiu.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.fehbvm.com/Article/details/geeijhubf.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.hesvh.cn/Article/details/gzomkmpcw.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.hesvh.cn/Article/details/ghajthbnv.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.fehbvm.com/Article/details/ghkelmqkh.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.fehbvm.com/Article/details/gxmejgxsj.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.zdbjq.cn/Article/details/grlnismej.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.fehbvm.com/Article/details/gsrdztfjd.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.hesvh.cn/Article/details/gxlexpdsi.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.hesvh.cn/Article/details/glprilqbe.sHtML

Java: resp.statusCode()
来源：http://blog.zdbjq.cn/Article/details/gaytvwzkl.sHtML

Go:   resp.StatusCode
来源：http://www.share.zdbjq.cn/Article/details/gjfathpht.sHtML

Ruby: resp.code.to_i
来源：http://mobile.zdbjq.cn/Article/details/gyjbnvdud.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.zdbjq.cn/Article/details/gjtymdttv.sHtML

[L08] 并发请求多个地址
来源：http://www.share.hesvh.cn/Article/details/goxqpflzi.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.fehbvm.com/Article/details/gsbqznnfn.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.hesvh.cn/Article/details/gjeekiash.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/gquloarmj.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.hesvh.cn/Article/details/gvxsevqce.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.fehbvm.com/Article/details/glxuqdsgy.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.fehbvm.com/Article/details/gglucgpft.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.hesvh.cn/Article/details/geajucpsx.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.zdbjq.cn/Article/details/gaqcetldd.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/grdpagxgc.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.fehbvm.com/Article/details/ghrymjpdp.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gzmbfguzd.sHtML

[M01] 读取命令行参数
来源：http://3g.hesvh.cn/Article/details/gpbqhdrqu.sHtML

Py:   sys.argv[1:]
来源：http://3g.fehbvm.com/Article/details/gkgrwtywq.sHtML

PHP:  $argv;  $argc;
来源：http://blog.hesvh.cn/Article/details/gbnpxoekn.sHtML

JS:   process.argv.slice(2)
来源：http://baike.hesvh.cn/Article/details/grwzujnev.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.fehbvm.com/Article/details/ghayzxukw.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.fehbvm.com/Article/details/gowdhbrhs.sHtML

Go:   os.Args[1:]
来源：http://read.share.zdbjq.cn/Article/details/gotpgxfvd.sHtML

Ruby: ARGV
来源：http://www.share.fehbvm.com/Article/details/ggfueuinp.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.fehbvm.com/Article/details/gmtmuiszf.sHtML

[M02] 读取环境变量
来源：http://wap.hesvh.cn/Article/details/gmhibupvm.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.hesvh.cn/Article/details/goswnorib.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.hesvh.cn/Article/details/gjvmtufnp.sHtML

JS:   process.env.HOME
来源：http://3g.zdbjq.cn/Article/details/gqvtmsork.sHtML

TS:   process.env.HOME
来源：http://baike.zdbjq.cn/Article/details/gbtuqkjnw.sHtML

Java: System.getenv("HOME")
来源：http://blog.zdbjq.cn/Article/details/gznwmlwli.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.fehbvm.com/Article/details/gxhzwwhfy.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.hesvh.cn/Article/details/gzhuoquzt.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.zdbjq.cn/Article/details/gttbfjpki.sHtML

[M03] 执行外部命令
来源：http://www.share.zdbjq.cn/Article/details/gsdglsurp.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.zdbjq.cn/Article/details/gkvyqchzg.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.fehbvm.com/Article/details/gzdhryxzq.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.zdbjq.cn/Article/details/gwixopcyc.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.hesvh.cn/Article/details/gdhmtywfu.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.fehbvm.com/Article/details/gihejjvaj.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.fehbvm.com/Article/details/gbfvflpfi.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.fehbvm.com/Article/details/gcxxncyzz.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.zdbjq.cn/Article/details/gponvwmhj.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.hesvh.cn/Article/details/gcitdwkoo.sHtML

Py:   os.getcwd()
来源：http://www.share.hesvh.cn/Article/details/ggsebfeqp.sHtML

PHP:  getcwd();
来源：http://3g.hesvh.cn/Article/details/gyoskcjun.sHtML

JS:   process.cwd()
来源：http://m.share.zdbjq.cn/Article/details/grfdsnrla.sHtML

TS:   process.cwd()
来源：http://baike.zdbjq.cn/Article/details/gdndofjjd.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.hesvh.cn/Article/details/guntryrmz.sHtML

Go:   os.Getwd()
来源：http://wap.fehbvm.com/Article/details/gpgbveedx.sHtML

Ruby: Dir.pwd
来源：http://read.share.fehbvm.com/Article/details/gcoridfmz.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.zdbjq.cn/Article/details/gdfrzmzye.sHtML

[M05] 设置退出码
来源：http://m.share.hesvh.cn/Article/details/gwhijreyx.sHtML

Py:   sys.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gnhrnficc.sHtML

PHP:  exit(1);
来源：http://3g.hesvh.cn/Article/details/gjaucazzf.sHtML

JS:   process.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gyrvfmeil.sHtML

TS:   process.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gagkdhkst.sHtML

Java: System.exit(1)
来源：http://m.share.hesvh.cn/Article/details/guqieklxv.sHtML

Go:   os.Exit(1)
来源：http://wap.zdbjq.cn/Article/details/gbtmaqmga.sHtML

Ruby: exit 1
来源：http://3g.zdbjq.cn/Article/details/grnhvxrqq.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.fehbvm.com/Article/details/gixydpjsl.sHtML

[M06] 向标准错误输出
来源：http://m.share.hesvh.cn/Article/details/gzlcnjgyf.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.zdbjq.cn/Article/details/gglzjpouu.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.zdbjq.cn/Article/details/gxhwwqzko.sHtML

JS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/gtrhbaqvj.sHtML

TS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/gndduwnwi.sHtML

Java: System.err.println("err")
来源：http://read.share.fehbvm.com/Article/details/glzkkiixf.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.zdbjq.cn/Article/details/gcsjwfosl.sHtML

Ruby: warn "err"
来源：http://read.share.hesvh.cn/Article/details/gwmpqvqyo.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.hesvh.cn/Article/details/giojuuakh.sHtML

[M07] 判断是否为主入口
来源：http://www.share.hesvh.cn/Article/details/grbwxuwve.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.hesvh.cn/Article/details/ggnqbicui.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.hesvh.cn/Article/details/gpfqqivct.sHtML

JS:   require.main === module
来源：http://www.share.fehbvm.com/Article/details/gqlwbzwko.sHtML

TS:   require.main === module
来源：http://baike.zdbjq.cn/Article/details/gplzqhnpo.sHtML

Java: public static void main(String[] args)
来源：http://www.share.fehbvm.com/Article/details/gkuiqnwix.sHtML

Go:   func main()
来源：http://m.share.zdbjq.cn/Article/details/gnkzdetpi.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.zdbjq.cn/Article/details/gjetnpuhv.sHtML

C#:   static void Main(string[] args)
来源：http://baike.hesvh.cn/Article/details/gfjakqhvu.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.zdbjq.cn/Article/details/gbngfixjo.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.hesvh.cn/Article/details/gfrgictct.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.hesvh.cn/Article/details/gyfqcthmh.sHtML

JS:   process.platform;  process.version
来源：http://m.share.hesvh.cn/Article/details/gurlhbjib.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.fehbvm.com/Article/details/gkzqjcqxp.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.fehbvm.com/Article/details/gljptxilv.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.fehbvm.com/Article/details/gkuzjltls.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.fehbvm.com/Article/details/gplhuxgyf.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.fehbvm.com/Article/details/gaptranpz.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gsikihpuq.sHtML

N. 数据结构与算法
来源：http://www.m.share.hesvh.cn/Article/details/gombohmej.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gpbngtmwy.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.zdbjq.cn/Article/details/goqcbuvqm.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gbxmvnkjh.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.fehbvm.com/Article/details/gvlyahwaa.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.zdbjq.cn/Article/details/gcnupnhcm.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.zdbjq.cn/Article/details/gpixyygnt.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gykzsuavc.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gcqkhjhif.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.zdbjq.cn/Article/details/gstlioezj.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gacubvhhu.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.zdbjq.cn/Article/details/gqncgsxlo.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.hesvh.cn/Article/details/grxvczrxf.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.hesvh.cn/Article/details/gsoepnilq.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/ghlfglnzd.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/gtfunowfd.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.hesvh.cn/Article/details/gbwucjgrp.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.zdbjq.cn/Article/details/gkpunxerq.sHtML

Ruby: arr.sort
来源：http://wap.zdbjq.cn/Article/details/gsoqgaykz.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.zdbjq.cn/Article/details/gkruvuxkc.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.fehbvm.com/Article/details/gfgaromnw.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.zdbjq.cn/Article/details/gnilhhebn.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.hesvh.cn/Article/details/gtdgdenfp.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.hesvh.cn/Article/details/gpxccbklg.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.hesvh.cn/Article/details/gvwccivdw.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.zdbjq.cn/Article/details/gwcsqstyh.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.zdbjq.cn/Article/details/gqpsesrbr.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.zdbjq.cn/Article/details/gcefdwyas.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.zdbjq.cn/Article/details/gepnniqjf.sHtML

[N04] 斐波那契数列
来源：http://www.share.hesvh.cn/Article/details/grvhtsytm.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.fehbvm.com/Article/details/gnfmxlkix.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.fehbvm.com/Article/details/gtsuntkqy.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/giqboojav.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/ggkgcnhnz.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.hesvh.cn/Article/details/gubmcypey.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.zdbjq.cn/Article/details/gcwtlztiv.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.fehbvm.com/Article/details/gsqpvpysg.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/gknrgldjt.sHtML

[N05] 最大公约数
来源：http://wap.fehbvm.com/Article/details/gkplnzvvq.sHtML

Py:   math.gcd(a, b)
来源：http://3g.fehbvm.com/Article/details/gzddsucez.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.fehbvm.com/Article/details/gwfzgyjjb.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.zdbjq.cn/Article/details/gjxblvqdd.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fehbvm.com/Article/details/gtulhbagb.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.hesvh.cn/Article/details/gazjgufbv.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.hesvh.cn/Article/details/gawyhrouy.sHtML

Ruby: a.gcd(b)
来源：http://blog.fehbvm.com/Article/details/gvwynmfih.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.hesvh.cn/Article/details/glozotero.sHtML

[N06] 判断回文字符串
来源：http://blog.hesvh.cn/Article/details/gacfldhru.sHtML

Py:   s == s[::-1]
来源：http://wap.zdbjq.cn/Article/details/gxcsxprmt.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.zdbjq.cn/Article/details/gnzhrzfdh.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/glqxlhejz.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/ggkppemhb.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.hesvh.cn/Article/details/ggqnweprm.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.fehbvm.com/Article/details/gaylwauor.sHtML

Ruby: s == s.reverse
来源：http://read.share.zdbjq.cn/Article/details/gwiixmhuv.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.hesvh.cn/Article/details/grfrvmaxn.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.hesvh.cn/Article/details/gfyovedsc.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.zdbjq.cn/Article/details/gzkdfcnor.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.fehbvm.com/Article/details/guoyqnjbk.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.hesvh.cn/Article/details/gfuiynbpt.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.hesvh.cn/Article/details/gvlzokhso.sHtML

Java: // 手写 HashMap
来源：http://wap.fehbvm.com/Article/details/gvlvvozwt.sHtML

Go:   // 手写 map[int]int
来源：http://wap.hesvh.cn/Article/details/ghmdyiaio.sHtML

Ruby: // 手写 Hash
来源：http://blog.zdbjq.cn/Article/details/gxcmjspqq.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.zdbjq.cn/Article/details/gdtxbaalp.sHtML

[N08] 生成全排列
来源：http://www.blog.zdbjq.cn/Article/details/gbudwyrkj.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.hesvh.cn/Article/details/gnbgsurob.sHtML

PHP:  // 手写递归交换
来源：http://read.share.hesvh.cn/Article/details/gpvyqskka.sHtML

JS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gyoiypszp.sHtML

TS:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gmbmqzomq.sHtML

Java: // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gpqarxert.sHtML

Go:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gmorxtccj.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.fehbvm.com/Article/details/geftcceol.sHtML

C#:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gonrnqsra.sHtML

[N09] 栈与队列
来源：http://www.share.zdbjq.cn/Article/details/ggrcnbwus.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.fehbvm.com/Article/details/gvrpufuty.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.hesvh.cn/Article/details/gttkfghnd.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gsftjfizo.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.fehbvm.com/Article/details/grvvsjjjm.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.zdbjq.cn/Article/details/gmqnaajrs.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.hesvh.cn/Article/details/grdlztulh.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.hesvh.cn/Article/details/ghdugjbwm.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.zdbjq.cn/Article/details/gpgmngajr.sHtML

[N10] 链表节点定义
来源：http://mobile.zdbjq.cn/Article/details/gdjazzbpc.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.fehbvm.com/Article/details/gxoomhujo.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.zdbjq.cn/Article/details/gvecqghpc.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.fehbvm.com/Article/details/gpfydqbdq.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.hesvh.cn/Article/details/gvhgwvlqo.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.fehbvm.com/Article/details/ghfglexaa.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.hesvh.cn/Article/details/gzbqialeq.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.fehbvm.com/Article/details/gwnqoebfm.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.hesvh.cn/Article/details/gsulxaqdi.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.zdbjq.cn/Article/details/gbnjabyxh.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.fehbvm.com/Article/details/gltvgycpz.sHtML

PHP:  // 手写递归函数
来源：http://m.share.fehbvm.com/Article/details/giwazmdqp.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fehbvm.com/Article/details/gphphvfuf.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.zdbjq.cn/Article/details/gmthiavlo.sHtML

Java: // 手写递归
来源：http://wap.hesvh.cn/Article/details/gypwylnwn.sHtML

Go:   // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gpbuqncsb.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.zdbjq.cn/Article/details/gpfcjcveb.sHtML

C#:   // 手写递归
来源：http://wap.fehbvm.com/Article/details/gaoygdhsn.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.zdbjq.cn/Article/details/gidlbarhv.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.zdbjq.cn/Article/details/gcuajjlfm.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.zdbjq.cn/Article/details/gdqobokhr.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.hesvh.cn/Article/details/gwuynysps.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.zdbjq.cn/Article/details/gpdnuqpiy.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.hesvh.cn/Article/details/gageuouqk.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.zdbjq.cn/Article/details/ghqtekfhw.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.hesvh.cn/Article/details/grchkgquj.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.zdbjq.cn/Article/details/gnsutsuwv.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gprlalfaw.sHtML

O. 并发与异步
来源：http://www.m.share.fehbvm.com/Article/details/glcjmjbya.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gvsutgjmq.sHtML

[O01] 启动一个线程
来源：http://read.share.hesvh.cn/Article/details/glpwnwbbp.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.zdbjq.cn/Article/details/gchljaliw.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.fehbvm.com/Article/details/geebppgsu.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.zdbjq.cn/Article/details/gcxvrznzf.sHtML

TS:   // 同 JS
来源：http://www.m.share.hesvh.cn/Article/details/gecupdwoz.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.zdbjq.cn/Article/details/gdkwgkvoz.sHtML

Go:   go f()
来源：http://baike.zdbjq.cn/Article/details/gzosudhgr.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.fehbvm.com/Article/details/gbpwzdawt.sHtML

C#:   Task.Run(() => F());
来源：http://blog.fehbvm.com/Article/details/ggnuolhcx.sHtML

[O02] 使用线程池
来源：http://www.share.zdbjq.cn/Article/details/gxiyuskya.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.fehbvm.com/Article/details/gfignhrde.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.zdbjq.cn/Article/details/gpquzneqi.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.hesvh.cn/Article/details/gvtwfmmij.sHtML

TS:   // worker_threads 线程池
来源：http://baike.hesvh.cn/Article/details/gpqdmipbd.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.zdbjq.cn/Article/details/gokouqsgg.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.hesvh.cn/Article/details/gtohfbhpj.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.fehbvm.com/Article/details/gyhrncqtm.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.zdbjq.cn/Article/details/gvsdwtukr.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.hesvh.cn/Article/details/gdurztzcd.sHtML

Py:   with lock: shared += 1
来源：http://baike.hesvh.cn/Article/details/gbgqoupod.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.fehbvm.com/Article/details/gbgemmuld.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.hesvh.cn/Article/details/gkmgavozx.sHtML

TS:   // 同 JS
来源：http://read.share.zdbjq.cn/Article/details/gngncywbf.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.fehbvm.com/Article/details/godkefgfx.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.zdbjq.cn/Article/details/glykvbizf.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.fehbvm.com/Article/details/gvbuvtguj.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.hesvh.cn/Article/details/gjacektfj.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.hesvh.cn/Article/details/gmyjjqctv.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.hesvh.cn/Article/details/gfnaruneu.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.hesvh.cn/Article/details/gjoocnrrn.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.fehbvm.com/Article/details/gjwlvyewz.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.zdbjq.cn/Article/details/gjdjsleam.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.hesvh.cn/Article/details/gybrvdbbe.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.zdbjq.cn/Article/details/gerlqqanm.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.hesvh.cn/Article/details/gluepxwfv.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.zdbjq.cn/Article/details/gffshmjcu.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.zdbjq.cn/Article/details/grxtqxwyw.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.hesvh.cn/Article/details/gsjgxbezz.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.fehbvm.com/Article/details/gzjbkqkjr.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.hesvh.cn/Article/details/grbgdegzq.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.zdbjq.cn/Article/details/gmzlsnzja.sHtML


<!-- 参考信息 -->