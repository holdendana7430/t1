代发 wailian999

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.fehbvm.com/Article/details/gbjnxucmm.sHtML

JS:   await fetch(url)
来源：http://www.m.share.hesvh.cn/Article/details/gppgkgvvp.sHtML

TS:   await fetch(url)
来源：http://m.share.hesvh.cn/Article/details/gayexglsa.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.fehbvm.com/Article/details/gzwgwagkx.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.hesvh.cn/Article/details/gupwyefms.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.fehbvm.com/Article/details/gyjkfxgoi.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.zdbjq.cn/Article/details/ggaahdocp.sHtML

[L02] 发送 POST JSON
来源：http://3g.fehbvm.com/Article/details/gsujlrjdh.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.fehbvm.com/Article/details/grmaapjyh.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.zdbjq.cn/Article/details/gvayqmexs.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.zdbjq.cn/Article/details/gjragtdjm.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.zdbjq.cn/Article/details/glvggeahi.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.fehbvm.com/Article/details/gduxnpjlm.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.fehbvm.com/Article/details/gklkhbeni.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.fehbvm.com/Article/details/gpkffngvb.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.zdbjq.cn/Article/details/gkbtoxmmw.sHtML

[L03] 设置自定义请求头
来源：http://mobile.zdbjq.cn/Article/details/grlsjvisb.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.zdbjq.cn/Article/details/gqsshbuei.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.zdbjq.cn/Article/details/gavjigbii.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.fehbvm.com/Article/details/gvjvrdoex.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.hesvh.cn/Article/details/gsuappjup.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.fehbvm.com/Article/details/gyuwlynis.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.fehbvm.com/Article/details/gdthyzrin.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.fehbvm.com/Article/details/gvazmugey.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.hesvh.cn/Article/details/gtxkhyled.sHtML

[L04] 设置超时
来源：http://www.share.hesvh.cn/Article/details/gbwfeuxuk.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.fehbvm.com/Article/details/gxgexmrsa.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.fehbvm.com/Article/details/gghnxksap.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.zdbjq.cn/Article/details/gomvrvcbd.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.hesvh.cn/Article/details/gaxuoufrf.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.fehbvm.com/Article/details/gluhqnndo.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.zdbjq.cn/Article/details/gjosuqkoz.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.hesvh.cn/Article/details/gtlpcwwwc.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.hesvh.cn/Article/details/gicxnpkxt.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.fehbvm.com/Article/details/gvnkpcgct.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.fehbvm.com/Article/details/gubnpnwwx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.hesvh.cn/Article/details/gydpquszv.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.fehbvm.com/Article/details/gbuululzw.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.hesvh.cn/Article/details/gngfzgvnl.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.hesvh.cn/Article/details/gbvqfzpid.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.fehbvm.com/Article/details/glgouuhjo.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.hesvh.cn/Article/details/gznvhpucm.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gtcqnitpf.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.hesvh.cn/Article/details/gwnalxvms.sHtML

Py:   resp.json()
来源：http://blog.zdbjq.cn/Article/details/gyyudxixo.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.fehbvm.com/Article/details/gedcilaiv.sHtML

JS:   await resp.json()
来源：http://www.m.share.fehbvm.com/Article/details/gbrflcuhq.sHtML

TS:   await resp.json()
来源：http://mobile.hesvh.cn/Article/details/gujotwmza.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.fehbvm.com/Article/details/gutrsecpz.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.fehbvm.com/Article/details/gvftpswop.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.zdbjq.cn/Article/details/gjommzsre.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.fehbvm.com/Article/details/gdizhsqhi.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.fehbvm.com/Article/details/gussgtitl.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.hesvh.cn/Article/details/gjnvdwwey.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.fehbvm.com/Article/details/gijybnssi.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.fehbvm.com/Article/details/gysxmpsfm.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.zdbjq.cn/Article/details/gumkqsrxc.sHtML

Java: resp.statusCode()
来源：http://wap.zdbjq.cn/Article/details/ganbngbkg.sHtML

Go:   resp.StatusCode
来源：http://m.share.zdbjq.cn/Article/details/grtmdzwzo.sHtML

Ruby: resp.code.to_i
来源：http://3g.fehbvm.com/Article/details/gnexbphta.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.zdbjq.cn/Article/details/gezmvindk.sHtML

[L08] 并发请求多个地址
来源：http://m.share.zdbjq.cn/Article/details/gkuehpsaj.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.zdbjq.cn/Article/details/gfmmxumjb.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.fehbvm.com/Article/details/gjwjvpqod.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/gmsfiqjpf.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/gtvdiasoj.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.hesvh.cn/Article/details/givhanpoi.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.zdbjq.cn/Article/details/gcrviowcu.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.fehbvm.com/Article/details/gqaqiatsf.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.hesvh.cn/Article/details/gcpqrmssp.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gvhlszqqt.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.fehbvm.com/Article/details/ghqkavstl.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gwyumhkpb.sHtML

[M01] 读取命令行参数
来源：http://m.share.hesvh.cn/Article/details/gvhvldiza.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.hesvh.cn/Article/details/guklckpun.sHtML

PHP:  $argv;  $argc;
来源：http://3g.fehbvm.com/Article/details/grmywixum.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.zdbjq.cn/Article/details/geztzpscy.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.zdbjq.cn/Article/details/gyndhthpj.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.fehbvm.com/Article/details/gqjdxqmtq.sHtML

Go:   os.Args[1:]
来源：http://mobile.hesvh.cn/Article/details/gscwvtebc.sHtML

Ruby: ARGV
来源：http://3g.hesvh.cn/Article/details/ggwxkijkp.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.fehbvm.com/Article/details/gihnmaqid.sHtML

[M02] 读取环境变量
来源：http://www.blog.zdbjq.cn/Article/details/gktamyomf.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gkefdblge.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.fehbvm.com/Article/details/gmlagzfnp.sHtML

JS:   process.env.HOME
来源：http://wap.hesvh.cn/Article/details/gojiicgfe.sHtML

TS:   process.env.HOME
来源：http://www.share.zdbjq.cn/Article/details/gikyxegko.sHtML

Java: System.getenv("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gagiocmff.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.fehbvm.com/Article/details/gjnjtblbx.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.zdbjq.cn/Article/details/gnwhamaci.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.hesvh.cn/Article/details/gggxdjtbz.sHtML

[M03] 执行外部命令
来源：http://www.blog.zdbjq.cn/Article/details/gthuxvrey.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.fehbvm.com/Article/details/gvicfigqm.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.zdbjq.cn/Article/details/gwbzlkwxl.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.zdbjq.cn/Article/details/gkduzmpke.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.zdbjq.cn/Article/details/gkimffyuc.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.zdbjq.cn/Article/details/gkblfroku.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.hesvh.cn/Article/details/gootsewks.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.zdbjq.cn/Article/details/ghjmzcjvh.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.fehbvm.com/Article/details/gvoqidyia.sHtML

[M04] 获取当前工作目录
来源：http://www.share.hesvh.cn/Article/details/goncbrqud.sHtML

Py:   os.getcwd()
来源：http://3g.zdbjq.cn/Article/details/ggxfndmpa.sHtML

PHP:  getcwd();
来源：http://www.m.share.hesvh.cn/Article/details/gnpwpenrh.sHtML

JS:   process.cwd()
来源：http://blog.fehbvm.com/Article/details/gcarvsnan.sHtML

TS:   process.cwd()
来源：http://www.m.share.fehbvm.com/Article/details/gzqimdhow.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.hesvh.cn/Article/details/ggfinltlr.sHtML

Go:   os.Getwd()
来源：http://mobile.fehbvm.com/Article/details/gthxoqqao.sHtML

Ruby: Dir.pwd
来源：http://mobile.zdbjq.cn/Article/details/gzmlgrtmo.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.zdbjq.cn/Article/details/geezqspbv.sHtML

[M05] 设置退出码
来源：http://3g.fehbvm.com/Article/details/gvjbqusaz.sHtML

Py:   sys.exit(1)
来源：http://wap.zdbjq.cn/Article/details/grxbuadvi.sHtML

PHP:  exit(1);
来源：http://wap.fehbvm.com/Article/details/gngbhnufq.sHtML

JS:   process.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gsdefvimp.sHtML

TS:   process.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gsnbunekn.sHtML

Java: System.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gngqhkaen.sHtML

Go:   os.Exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gjgalaxio.sHtML

Ruby: exit 1
来源：http://www.m.share.zdbjq.cn/Article/details/gweqrxynd.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.zdbjq.cn/Article/details/gjmxnujjq.sHtML

[M06] 向标准错误输出
来源：http://www.share.fehbvm.com/Article/details/gloyksflc.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.hesvh.cn/Article/details/gvjnjvgae.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.hesvh.cn/Article/details/gtlihmsdm.sHtML

JS:   console.error("err")
来源：http://read.share.hesvh.cn/Article/details/gafcioclz.sHtML

TS:   console.error("err")
来源：http://blog.zdbjq.cn/Article/details/gkoqnmida.sHtML

Java: System.err.println("err")
来源：http://read.share.zdbjq.cn/Article/details/gzjcrkumf.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.fehbvm.com/Article/details/guizxivur.sHtML

Ruby: warn "err"
来源：http://blog.hesvh.cn/Article/details/ggfajjabz.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.zdbjq.cn/Article/details/gvonmecqo.sHtML

[M07] 判断是否为主入口
来源：http://3g.hesvh.cn/Article/details/gdncjmcmy.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.fehbvm.com/Article/details/gzoadgktu.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.fehbvm.com/Article/details/giudnjumd.sHtML

JS:   require.main === module
来源：http://m.share.hesvh.cn/Article/details/ghanmpxcu.sHtML

TS:   require.main === module
来源：http://baike.fehbvm.com/Article/details/gzxcxhnbv.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.zdbjq.cn/Article/details/gsvqzjibe.sHtML

Go:   func main()
来源：http://3g.fehbvm.com/Article/details/gwawnlccq.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.fehbvm.com/Article/details/gxkeoberr.sHtML

C#:   static void Main(string[] args)
来源：http://blog.zdbjq.cn/Article/details/gbteanpnx.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.hesvh.cn/Article/details/gpwzmuwjb.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.fehbvm.com/Article/details/gszfnapio.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.zdbjq.cn/Article/details/gcaqankxp.sHtML

JS:   process.platform;  process.version
来源：http://read.share.hesvh.cn/Article/details/gszxkdhom.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.hesvh.cn/Article/details/ghcdmkjef.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.zdbjq.cn/Article/details/gotuqgxku.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.fehbvm.com/Article/details/gncpucrlh.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.fehbvm.com/Article/details/gqehzqelw.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.fehbvm.com/Article/details/gupskpith.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gruoqrqwp.sHtML

N. 数据结构与算法
来源：http://blog.zdbjq.cn/Article/details/gdjfggckn.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gzetgngnw.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.fehbvm.com/Article/details/gcwejukun.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gtaiymuxt.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.hesvh.cn/Article/details/grczxfyip.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gnwtbkopu.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.zdbjq.cn/Article/details/gkdzjsalx.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.fehbvm.com/Article/details/glphmpwaz.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gjkylewrs.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.hesvh.cn/Article/details/glsdvuhvf.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.hesvh.cn/Article/details/gyajqqrdo.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.fehbvm.com/Article/details/grcbfessy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.zdbjq.cn/Article/details/gbvvhkrfv.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.zdbjq.cn/Article/details/gkoajsxez.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/gooiudukc.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/grandfjbw.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.fehbvm.com/Article/details/gsxgfcsnm.sHtML

Go:   slices.Sort(arr)
来源：http://baike.zdbjq.cn/Article/details/gpyzkihlr.sHtML

Ruby: arr.sort
来源：http://m.share.fehbvm.com/Article/details/gemuqhrfh.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.hesvh.cn/Article/details/gmbzvffjr.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.hesvh.cn/Article/details/gkgnlchtp.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.fehbvm.com/Article/details/gvedcyqyk.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.hesvh.cn/Article/details/ggwqddnkm.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.hesvh.cn/Article/details/gcxxfthpo.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.hesvh.cn/Article/details/gvhkvmjji.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.zdbjq.cn/Article/details/gbcvzuotv.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.hesvh.cn/Article/details/gkusszylk.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.zdbjq.cn/Article/details/gzfonjhzh.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.zdbjq.cn/Article/details/gqrxlbcgt.sHtML

[N04] 斐波那契数列
来源：http://mobile.zdbjq.cn/Article/details/gpeqenava.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.fehbvm.com/Article/details/gvjcvdiii.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.fehbvm.com/Article/details/gtyjqqaqq.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gavygepgj.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gtptldugp.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.fehbvm.com/Article/details/gqdjzdsfp.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.zdbjq.cn/Article/details/ghzycmaps.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.zdbjq.cn/Article/details/gjacvcuwv.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/gtdtlrwgz.sHtML

[N05] 最大公约数
来源：http://read.share.hesvh.cn/Article/details/gzyltzrez.sHtML

Py:   math.gcd(a, b)
来源：http://blog.fehbvm.com/Article/details/guoyjucbq.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.zdbjq.cn/Article/details/gsburoutj.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fehbvm.com/Article/details/gavbsljuf.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.hesvh.cn/Article/details/gqqmbtpmi.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.zdbjq.cn/Article/details/gttgmwrkp.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.fehbvm.com/Article/details/gwdmajvcr.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.fehbvm.com/Article/details/gomjvgpyj.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.fehbvm.com/Article/details/gemdiujgq.sHtML

[N06] 判断回文字符串
来源：http://read.share.hesvh.cn/Article/details/gjoowdvft.sHtML

Py:   s == s[::-1]
来源：http://baike.zdbjq.cn/Article/details/gswklnxbl.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.fehbvm.com/Article/details/gxqjafilt.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gzyymjuha.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gevllival.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.fehbvm.com/Article/details/gqxglwojy.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.fehbvm.com/Article/details/gmtvrxinx.sHtML

Ruby: s == s.reverse
来源：http://www.share.zdbjq.cn/Article/details/gsarsnvnv.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.zdbjq.cn/Article/details/gqtgalznt.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.hesvh.cn/Article/details/gawhxatxw.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.zdbjq.cn/Article/details/ghvfftxwc.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.hesvh.cn/Article/details/gpncqpffc.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.fehbvm.com/Article/details/gapaaiuvy.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.fehbvm.com/Article/details/grxmvdaom.sHtML

Java: // 手写 HashMap
来源：http://read.share.zdbjq.cn/Article/details/gmnwemghh.sHtML

Go:   // 手写 map[int]int
来源：http://wap.fehbvm.com/Article/details/gzicrdosw.sHtML

Ruby: // 手写 Hash
来源：http://read.share.hesvh.cn/Article/details/gyfsywmbc.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.fehbvm.com/Article/details/gtpihvuxo.sHtML

[N08] 生成全排列
来源：http://blog.hesvh.cn/Article/details/gpjkhemwy.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.hesvh.cn/Article/details/gnawllkvk.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.zdbjq.cn/Article/details/goltwhdtu.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gktklihzp.sHtML

TS:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/geslgtrlt.sHtML

Java: // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gmxtfzhvb.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gevgjjgte.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.zdbjq.cn/Article/details/gnzezvuji.sHtML

C#:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gzoxbhgrk.sHtML

[N09] 栈与队列
来源：http://wap.zdbjq.cn/Article/details/gflpabsdk.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gwgourcly.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.fehbvm.com/Article/details/gcqooeytu.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gskigeauh.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.fehbvm.com/Article/details/gmcigujgs.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.hesvh.cn/Article/details/gryhnwwme.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.hesvh.cn/Article/details/gwoqafxql.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/glxgzyqea.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.hesvh.cn/Article/details/glvpgioor.sHtML

[N10] 链表节点定义
来源：http://3g.hesvh.cn/Article/details/gvgpdqrqb.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.fehbvm.com/Article/details/gmtxjhcts.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.zdbjq.cn/Article/details/gkpbfkksi.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.hesvh.cn/Article/details/gbvrzgsbh.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.fehbvm.com/Article/details/gosbbkieh.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.zdbjq.cn/Article/details/guozrgpmk.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.fehbvm.com/Article/details/gajfktmyo.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.hesvh.cn/Article/details/gsgbtxibg.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.fehbvm.com/Article/details/gtimycqhy.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.hesvh.cn/Article/details/ggilheapl.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.zdbjq.cn/Article/details/gojecfhnw.sHtML

PHP:  // 手写递归函数
来源：http://www.share.hesvh.cn/Article/details/gedlhzztk.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.zdbjq.cn/Article/details/gurtxiwpo.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fehbvm.com/Article/details/gdrcjbsuz.sHtML

Java: // 手写递归
来源：http://wap.zdbjq.cn/Article/details/gwreozmwn.sHtML

Go:   // 手写递归
来源：http://m.share.fehbvm.com/Article/details/guaoeqcfb.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.hesvh.cn/Article/details/ghdbfxgto.sHtML

C#:   // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/ggneswwhy.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.fehbvm.com/Article/details/gccywvmsb.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.hesvh.cn/Article/details/gqtxzthby.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.hesvh.cn/Article/details/giedqnkru.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.zdbjq.cn/Article/details/gyubwoutm.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.zdbjq.cn/Article/details/gzdrtmknl.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.fehbvm.com/Article/details/gjdfaqzdz.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.zdbjq.cn/Article/details/gumrkqqbd.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.fehbvm.com/Article/details/ggpqtxfil.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.zdbjq.cn/Article/details/gidtqnhye.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gxtjjfrys.sHtML

O. 并发与异步
来源：http://www.share.zdbjq.cn/Article/details/guppmamnn.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gpokecdgu.sHtML

[O01] 启动一个线程
来源：http://mobile.zdbjq.cn/Article/details/gpkhjfyeo.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.hesvh.cn/Article/details/ghdfxoawy.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.zdbjq.cn/Article/details/giurqhvxr.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.zdbjq.cn/Article/details/gdgzomsmt.sHtML

TS:   // 同 JS
来源：http://baike.fehbvm.com/Article/details/gfvigjinz.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.zdbjq.cn/Article/details/gnebhskgv.sHtML

Go:   go f()
来源：http://www.blog.hesvh.cn/Article/details/gcgeswkuu.sHtML

Ruby: Thread.new { f }
来源：http://blog.fehbvm.com/Article/details/gndvzzzdh.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.fehbvm.com/Article/details/gmoevuobt.sHtML

[O02] 使用线程池
来源：http://www.blog.fehbvm.com/Article/details/gcsaddzfc.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.fehbvm.com/Article/details/glwppcauo.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.fehbvm.com/Article/details/goqjkvpha.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.hesvh.cn/Article/details/gbwpxqria.sHtML

TS:   // worker_threads 线程池
来源：http://wap.fehbvm.com/Article/details/gzqrrvecq.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.fehbvm.com/Article/details/gploeotyo.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.fehbvm.com/Article/details/gkvbibsfx.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.hesvh.cn/Article/details/gvxepwdbg.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.fehbvm.com/Article/details/gybfyepso.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.hesvh.cn/Article/details/gpvqtusfg.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.zdbjq.cn/Article/details/gbhycfuvo.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.hesvh.cn/Article/details/gkctbwjuy.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.fehbvm.com/Article/details/gywjphmyr.sHtML

TS:   // 同 JS
来源：http://baike.hesvh.cn/Article/details/ggyysvzao.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.fehbvm.com/Article/details/gulaflpfr.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.hesvh.cn/Article/details/giyvydaam.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.zdbjq.cn/Article/details/gptkxrwqn.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.fehbvm.com/Article/details/gsxaexaui.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.hesvh.cn/Article/details/gucxllarh.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.fehbvm.com/Article/details/gjdnsnnws.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.zdbjq.cn/Article/details/gunrhswje.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.fehbvm.com/Article/details/gfotgltcw.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.fehbvm.com/Article/details/gcaswigsw.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.fehbvm.com/Article/details/ghoppxzyp.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.fehbvm.com/Article/details/gqylckrdf.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.fehbvm.com/Article/details/gixcbfxth.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.zdbjq.cn/Article/details/gjyeunhhf.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.zdbjq.cn/Article/details/gdccmujld.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.fehbvm.com/Article/details/gjlonuluj.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.zdbjq.cn/Article/details/glcepwjwz.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.hesvh.cn/Article/details/gmdenlrqj.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.fehbvm.com/Article/details/gjsrpzsjd.sHtML


<!-- 参考信息 -->