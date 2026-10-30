代发 wailian999

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.zdbjq.cn/Article/details/genoorqzk.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.zdbjq.cn/Article/details/geuknpelm.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.hesvh.cn/Article/details/ghwtyzyhw.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.fehbvm.com/Article/details/ghvesglrq.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.fehbvm.com/Article/details/gvkoufhek.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.fehbvm.com/Article/details/gznkeqyow.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.hesvh.cn/Article/details/guxifyuwi.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.hesvh.cn/Article/details/gnnxzgvxz.sHtML

[L03] 设置自定义请求头
来源：http://3g.zdbjq.cn/Article/details/gmpuwrdbg.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.zdbjq.cn/Article/details/gxyuuwrxo.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.fehbvm.com/Article/details/gircblsdw.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.hesvh.cn/Article/details/gmtsrczqd.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.zdbjq.cn/Article/details/gtednqcel.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.fehbvm.com/Article/details/gkkkaawid.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.fehbvm.com/Article/details/gtiiotgnx.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.fehbvm.com/Article/details/ghihusbhj.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.zdbjq.cn/Article/details/gkiexqjjd.sHtML

[L04] 设置超时
来源：http://blog.hesvh.cn/Article/details/gycqkepxq.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.fehbvm.com/Article/details/gapwlydqn.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.zdbjq.cn/Article/details/gizhckwip.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.zdbjq.cn/Article/details/gvwubfrnv.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.fehbvm.com/Article/details/genjmlbde.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.fehbvm.com/Article/details/gyotosrni.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.zdbjq.cn/Article/details/gvrzgkrti.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.fehbvm.com/Article/details/gnorcgvnp.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.hesvh.cn/Article/details/gazrszjrw.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.fehbvm.com/Article/details/gijjvompi.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.zdbjq.cn/Article/details/gbjhxpmzn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.hesvh.cn/Article/details/ghttcsyfm.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.hesvh.cn/Article/details/gqubxhleu.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.fehbvm.com/Article/details/gvfjipsvz.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.fehbvm.com/Article/details/gsclitbxf.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.fehbvm.com/Article/details/gynkfabwp.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.zdbjq.cn/Article/details/gkhaspqhb.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/grygtgpqi.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.zdbjq.cn/Article/details/guniinnsf.sHtML

Py:   resp.json()
来源：http://baike.hesvh.cn/Article/details/gpkzepanz.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.fehbvm.com/Article/details/gzwxhxbnh.sHtML

JS:   await resp.json()
来源：http://blog.fehbvm.com/Article/details/govhapkdq.sHtML

TS:   await resp.json()
来源：http://m.share.fehbvm.com/Article/details/gmnpridak.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.zdbjq.cn/Article/details/gfbzeeigp.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.hesvh.cn/Article/details/gsmzwjjzj.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.hesvh.cn/Article/details/gwhzbpujr.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.zdbjq.cn/Article/details/gluyeadsd.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.zdbjq.cn/Article/details/gltxwpvtv.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.hesvh.cn/Article/details/gswyzyzeb.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.fehbvm.com/Article/details/gsibawobn.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.hesvh.cn/Article/details/gbiqpmuwv.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.fehbvm.com/Article/details/gjrdrmeap.sHtML

Java: resp.statusCode()
来源：http://www.m.share.zdbjq.cn/Article/details/gweaaeocv.sHtML

Go:   resp.StatusCode
来源：http://wap.hesvh.cn/Article/details/gzwphetag.sHtML

Ruby: resp.code.to_i
来源：http://read.share.hesvh.cn/Article/details/guprvkrox.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.fehbvm.com/Article/details/gddqrwdot.sHtML

[L08] 并发请求多个地址
来源：http://baike.zdbjq.cn/Article/details/gmlkktsaj.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.zdbjq.cn/Article/details/gmiesghgp.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.hesvh.cn/Article/details/gydlcwapw.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/gkfrzqmvi.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/gzuweyhwv.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.fehbvm.com/Article/details/gkitjruox.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.fehbvm.com/Article/details/gflwobgpn.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.fehbvm.com/Article/details/gypzldvje.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.fehbvm.com/Article/details/gfpatmree.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/getoyxwzd.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.zdbjq.cn/Article/details/gvosxxtiz.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gfartqzdy.sHtML

[M01] 读取命令行参数
来源：http://m.share.zdbjq.cn/Article/details/gwdhsgpeh.sHtML

Py:   sys.argv[1:]
来源：http://baike.zdbjq.cn/Article/details/gbfkufgai.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.fehbvm.com/Article/details/gvfxdfxmh.sHtML

JS:   process.argv.slice(2)
来源：http://blog.fehbvm.com/Article/details/gjvckecsd.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.hesvh.cn/Article/details/gpktmmvti.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.hesvh.cn/Article/details/gzdmxjquy.sHtML

Go:   os.Args[1:]
来源：http://baike.hesvh.cn/Article/details/ghczvllgt.sHtML

Ruby: ARGV
来源：http://m.share.zdbjq.cn/Article/details/gcuizkgqu.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.zdbjq.cn/Article/details/gooubldur.sHtML

[M02] 读取环境变量
来源：http://read.share.zdbjq.cn/Article/details/gdhovizmt.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gcstuobuc.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.fehbvm.com/Article/details/gqlncjzsi.sHtML

JS:   process.env.HOME
来源：http://m.share.zdbjq.cn/Article/details/gotjazhok.sHtML

TS:   process.env.HOME
来源：http://www.m.share.fehbvm.com/Article/details/grmzoowhj.sHtML

Java: System.getenv("HOME")
来源：http://wap.zdbjq.cn/Article/details/godcjohyc.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gidjpxcas.sHtML

Ruby: ENV["HOME"]
来源：http://3g.fehbvm.com/Article/details/gcvlslujw.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.fehbvm.com/Article/details/gjnjmbfnc.sHtML

[M03] 执行外部命令
来源：http://read.share.zdbjq.cn/Article/details/gzyuudibm.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.zdbjq.cn/Article/details/gfghxpmrg.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.fehbvm.com/Article/details/gqevwajtm.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.hesvh.cn/Article/details/gqkyjhoau.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.hesvh.cn/Article/details/gvkzxceuv.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.hesvh.cn/Article/details/gjsdierrb.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.zdbjq.cn/Article/details/ghsosfgty.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.zdbjq.cn/Article/details/gmvswwbvs.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.hesvh.cn/Article/details/gqvnbhozc.sHtML

[M04] 获取当前工作目录
来源：http://www.share.fehbvm.com/Article/details/gazuvnmar.sHtML

Py:   os.getcwd()
来源：http://blog.zdbjq.cn/Article/details/gbdwbfdpn.sHtML

PHP:  getcwd();
来源：http://www.m.share.zdbjq.cn/Article/details/gulheofmf.sHtML

JS:   process.cwd()
来源：http://blog.hesvh.cn/Article/details/gixohdkay.sHtML

TS:   process.cwd()
来源：http://www.share.zdbjq.cn/Article/details/gcmgfawdg.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.zdbjq.cn/Article/details/gcabdgbuf.sHtML

Go:   os.Getwd()
来源：http://mobile.fehbvm.com/Article/details/gxcisrrps.sHtML

Ruby: Dir.pwd
来源：http://wap.fehbvm.com/Article/details/gnecechet.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.zdbjq.cn/Article/details/gbzuonopf.sHtML

[M05] 设置退出码
来源：http://m.share.fehbvm.com/Article/details/gxpboidnk.sHtML

Py:   sys.exit(1)
来源：http://wap.fehbvm.com/Article/details/gklrmkhtf.sHtML

PHP:  exit(1);
来源：http://www.share.hesvh.cn/Article/details/gahtvcpex.sHtML

JS:   process.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gxbfkakxb.sHtML

TS:   process.exit(1)
来源：http://mobile.hesvh.cn/Article/details/grcmvjrnw.sHtML

Java: System.exit(1)
来源：http://baike.fehbvm.com/Article/details/gznufgjzw.sHtML

Go:   os.Exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/glxegvilo.sHtML

Ruby: exit 1
来源：http://baike.hesvh.cn/Article/details/gbngswgwl.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.hesvh.cn/Article/details/gekngkjof.sHtML

[M06] 向标准错误输出
来源：http://m.share.hesvh.cn/Article/details/ghvvkhddu.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.fehbvm.com/Article/details/gpswcewga.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.zdbjq.cn/Article/details/gwylrotqs.sHtML

JS:   console.error("err")
来源：http://read.share.hesvh.cn/Article/details/ggycijvaj.sHtML

TS:   console.error("err")
来源：http://3g.hesvh.cn/Article/details/gzopxoycu.sHtML

Java: System.err.println("err")
来源：http://wap.hesvh.cn/Article/details/goimhowhd.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.hesvh.cn/Article/details/gcuizoahr.sHtML

Ruby: warn "err"
来源：http://wap.hesvh.cn/Article/details/gmkfmmzjw.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.zdbjq.cn/Article/details/gdgpteecb.sHtML

[M07] 判断是否为主入口
来源：http://mobile.fehbvm.com/Article/details/gounjtsnf.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.hesvh.cn/Article/details/gfhnlrmgi.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.zdbjq.cn/Article/details/gdchuwkir.sHtML

JS:   require.main === module
来源：http://www.share.fehbvm.com/Article/details/gjympxtpw.sHtML

TS:   require.main === module
来源：http://www.blog.hesvh.cn/Article/details/galdblufv.sHtML

Java: public static void main(String[] args)
来源：http://3g.hesvh.cn/Article/details/gkrojtsrb.sHtML

Go:   func main()
来源：http://mobile.zdbjq.cn/Article/details/grwrfdddv.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.fehbvm.com/Article/details/gbjopuqkb.sHtML

C#:   static void Main(string[] args)
来源：http://blog.hesvh.cn/Article/details/grzjlrdzs.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.zdbjq.cn/Article/details/gngbwvrkq.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.hesvh.cn/Article/details/gfmsdefub.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.zdbjq.cn/Article/details/gsctnmfpt.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.fehbvm.com/Article/details/gemczjnfc.sHtML

TS:   process.platform;  process.version
来源：http://wap.fehbvm.com/Article/details/gwzyndslv.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.zdbjq.cn/Article/details/gkzxrkwsu.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.zdbjq.cn/Article/details/gitzgcwss.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.fehbvm.com/Article/details/gujvxnijg.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.fehbvm.com/Article/details/gepqkuiyz.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gjxkolcng.sHtML

N. 数据结构与算法
来源：http://www.share.zdbjq.cn/Article/details/grfcxuxny.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gtdmpjiyx.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.zdbjq.cn/Article/details/gqnoypier.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gahjijeph.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.zdbjq.cn/Article/details/getyxjefi.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gvqelapij.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/gwlucjlpm.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gckjesgmk.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gcoxdcigd.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.zdbjq.cn/Article/details/gukmfswua.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.fehbvm.com/Article/details/gjncgixqp.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.hesvh.cn/Article/details/gymivpzhj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.hesvh.cn/Article/details/gzuqgqhza.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.hesvh.cn/Article/details/gnrpfmabf.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/gmynfpuzz.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/gsyncejtd.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.zdbjq.cn/Article/details/gabfjcpii.sHtML

Go:   slices.Sort(arr)
来源：http://baike.fehbvm.com/Article/details/ggwnzlziq.sHtML

Ruby: arr.sort
来源：http://m.share.zdbjq.cn/Article/details/gnxdrlmda.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.fehbvm.com/Article/details/gtxszfsgu.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.zdbjq.cn/Article/details/gvycohqfo.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.fehbvm.com/Article/details/gtiwosthu.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.zdbjq.cn/Article/details/gunsypcix.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.hesvh.cn/Article/details/ghvwqlfkk.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.hesvh.cn/Article/details/grrmiedly.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.zdbjq.cn/Article/details/gmmrgymet.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.zdbjq.cn/Article/details/gmzkknblf.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.zdbjq.cn/Article/details/gsdiblxxv.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.hesvh.cn/Article/details/gpmkmkhbf.sHtML

[N04] 斐波那契数列
来源：http://www.blog.fehbvm.com/Article/details/gjzzpgwme.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.zdbjq.cn/Article/details/glkgpoofv.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.fehbvm.com/Article/details/glgxzrqah.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/glrxtoevv.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/ggngcyjsf.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.hesvh.cn/Article/details/gdfzewcjj.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.zdbjq.cn/Article/details/gxmpiifzu.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.hesvh.cn/Article/details/gqzyvuqwk.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gsawytzrs.sHtML

[N05] 最大公约数
来源：http://www.share.zdbjq.cn/Article/details/gziuvkykt.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/gvppgcthw.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.hesvh.cn/Article/details/ghdusabnr.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fehbvm.com/Article/details/gqkbgenyn.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fehbvm.com/Article/details/gnuszroqk.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.hesvh.cn/Article/details/gegcvnwir.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.zdbjq.cn/Article/details/gbbjrosxd.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.hesvh.cn/Article/details/gauwywgrq.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.zdbjq.cn/Article/details/gohjfxdwy.sHtML

[N06] 判断回文字符串
来源：http://wap.hesvh.cn/Article/details/gzuztzzpr.sHtML

Py:   s == s[::-1]
来源：http://3g.hesvh.cn/Article/details/gpfwdwitt.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.fehbvm.com/Article/details/gckclwfcf.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gfhmgvale.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gbkjiynns.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.zdbjq.cn/Article/details/gdowohqgd.sHtML

Go:   // 双指针从两端比较
来源：http://blog.fehbvm.com/Article/details/gtdgasalq.sHtML

Ruby: s == s.reverse
来源：http://mobile.zdbjq.cn/Article/details/ggmtshgmv.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.fehbvm.com/Article/details/gogattrym.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.fehbvm.com/Article/details/gkftbjwvo.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.fehbvm.com/Article/details/ggsnulhay.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.fehbvm.com/Article/details/gtctueyia.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.zdbjq.cn/Article/details/gdzymunkf.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.hesvh.cn/Article/details/gxvhwlrxb.sHtML

Java: // 手写 HashMap
来源：http://blog.zdbjq.cn/Article/details/gbpnluadr.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.fehbvm.com/Article/details/glzkycocu.sHtML

Ruby: // 手写 Hash
来源：http://wap.hesvh.cn/Article/details/gkgcbfxrf.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.hesvh.cn/Article/details/gchwldjnh.sHtML

[N08] 生成全排列
来源：http://www.share.hesvh.cn/Article/details/ghrdzqjkg.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.hesvh.cn/Article/details/gnxezpdwr.sHtML

PHP:  // 手写递归交换
来源：http://wap.zdbjq.cn/Article/details/glikmrdhc.sHtML

JS:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gagipwbgp.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gzzykjkxs.sHtML

Java: // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/godmlxael.sHtML

Go:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gcrvmsvxb.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.zdbjq.cn/Article/details/gcdtkpsab.sHtML

C#:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gayivmmau.sHtML

[N09] 栈与队列
来源：http://read.share.zdbjq.cn/Article/details/givfixxgc.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/ghjcayfwa.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.fehbvm.com/Article/details/gjjxoqkcj.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.hesvh.cn/Article/details/gsjikwsdd.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.fehbvm.com/Article/details/gzcybonvw.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.fehbvm.com/Article/details/gcplyfxav.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.hesvh.cn/Article/details/gphstjdmf.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gtaecjfpn.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.zdbjq.cn/Article/details/gsgxrpcis.sHtML

[N10] 链表节点定义
来源：http://read.share.fehbvm.com/Article/details/gnmctcved.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.zdbjq.cn/Article/details/gghzqansw.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.hesvh.cn/Article/details/gjleakcjx.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.zdbjq.cn/Article/details/gwiykfcoi.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.fehbvm.com/Article/details/gptdhgglb.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.zdbjq.cn/Article/details/gcvocfrww.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.zdbjq.cn/Article/details/gdlxdtjhd.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.zdbjq.cn/Article/details/gdauwivst.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.zdbjq.cn/Article/details/girdudwte.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.fehbvm.com/Article/details/grlvldmjc.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.fehbvm.com/Article/details/gyczqfors.sHtML

PHP:  // 手写递归函数
来源：http://m.share.fehbvm.com/Article/details/gmnfjfrly.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.zdbjq.cn/Article/details/garmndojb.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.hesvh.cn/Article/details/goihhollq.sHtML

Java: // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gmletnavv.sHtML

Go:   // 手写递归
来源：http://wap.fehbvm.com/Article/details/gniedrfua.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.hesvh.cn/Article/details/gchnritqa.sHtML

C#:   // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/ggkiszxcv.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.fehbvm.com/Article/details/gdemlkbre.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.hesvh.cn/Article/details/gaqesboum.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.hesvh.cn/Article/details/gdnthcqfz.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.hesvh.cn/Article/details/gsorztuxt.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fehbvm.com/Article/details/gwuaakcry.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.hesvh.cn/Article/details/gnyerkbmn.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.zdbjq.cn/Article/details/gidevotri.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.fehbvm.com/Article/details/gevwhnony.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.hesvh.cn/Article/details/gdnfypzzl.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gqiimqfsu.sHtML

O. 并发与异步
来源：http://3g.hesvh.cn/Article/details/gewhjcxeo.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gkpqmatky.sHtML

[O01] 启动一个线程
来源：http://www.blog.fehbvm.com/Article/details/gvdhuzpej.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.hesvh.cn/Article/details/glbxidmgg.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.hesvh.cn/Article/details/gpgobtvai.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.hesvh.cn/Article/details/gubaryoel.sHtML

TS:   // 同 JS
来源：http://baike.fehbvm.com/Article/details/gfimtscid.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.zdbjq.cn/Article/details/glcxffbjq.sHtML

Go:   go f()
来源：http://baike.fehbvm.com/Article/details/gruajlyub.sHtML

Ruby: Thread.new { f }
来源：http://read.share.hesvh.cn/Article/details/grjolvjoa.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.fehbvm.com/Article/details/gzqyyzshx.sHtML

[O02] 使用线程池
来源：http://mobile.fehbvm.com/Article/details/gqiimwayk.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.hesvh.cn/Article/details/gcrmobsao.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.hesvh.cn/Article/details/glkoqztur.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.zdbjq.cn/Article/details/ghnynmehm.sHtML

TS:   // worker_threads 线程池
来源：http://3g.hesvh.cn/Article/details/gqbilnkct.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.hesvh.cn/Article/details/grfkghwak.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.fehbvm.com/Article/details/gcgangbpr.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.fehbvm.com/Article/details/guxsycedi.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.hesvh.cn/Article/details/gdcedecgx.sHtML

[O03] 加锁保护共享数据
来源：http://blog.hesvh.cn/Article/details/gksbavybf.sHtML

Py:   with lock: shared += 1
来源：http://blog.zdbjq.cn/Article/details/gtzmybvxq.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.fehbvm.com/Article/details/ggfmvilsi.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.fehbvm.com/Article/details/glqyixrnj.sHtML

TS:   // 同 JS
来源：http://www.m.share.fehbvm.com/Article/details/gaywaqpso.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.zdbjq.cn/Article/details/gmcpvzdum.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.hesvh.cn/Article/details/giuiihdki.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.hesvh.cn/Article/details/guzwimpwf.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.fehbvm.com/Article/details/gqlrckzxu.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.fehbvm.com/Article/details/gmhpfovsc.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.zdbjq.cn/Article/details/gktdmleli.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.hesvh.cn/Article/details/gmlujzwyz.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.zdbjq.cn/Article/details/glqjusiwb.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.hesvh.cn/Article/details/grwvmvevl.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.fehbvm.com/Article/details/gmugozvzj.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.hesvh.cn/Article/details/gawizzrmo.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.fehbvm.com/Article/details/gtpgqvkon.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.zdbjq.cn/Article/details/gjkmhjbaa.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.fehbvm.com/Article/details/gnlxmkofc.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.hesvh.cn/Article/details/gphpfmuot.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.fehbvm.com/Article/details/gdqdgrqyb.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.hesvh.cn/Article/details/gqchwwhfi.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.zdbjq.cn/Article/details/gbjahjzob.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.fehbvm.com/Article/details/glfqjgiko.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.fehbvm.com/Article/details/gxafddjsc.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.hesvh.cn/Article/details/giaztkfju.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.hesvh.cn/Article/details/gftnqxwqb.sHtML

[O06] 使用进程池
来源：http://read.share.zdbjq.cn/Article/details/gxjsbvlkh.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.zdbjq.cn/Article/details/gssvvhglx.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.hesvh.cn/Article/details/gmfcsdxql.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.hesvh.cn/Article/details/grggqeuux.sHtML


<!-- 参考信息 -->