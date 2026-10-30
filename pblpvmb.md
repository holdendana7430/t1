代发 wailian999

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.hesvh.cn/Article/details/gxgclshig.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.hesvh.cn/Article/details/gknvjzqhz.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.zdbjq.cn/Article/details/gjqrueeua.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.fehbvm.com/Article/details/gfydwctzi.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.hesvh.cn/Article/details/gahkjwzzb.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.hesvh.cn/Article/details/giwuivabl.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.fehbvm.com/Article/details/gkdmuxqyz.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.zdbjq.cn/Article/details/ggytdoyhe.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.zdbjq.cn/Article/details/gsxiusibb.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.fehbvm.com/Article/details/gtpnrayrp.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.zdbjq.cn/Article/details/gsugooutj.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.fehbvm.com/Article/details/gqarrqijf.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.fehbvm.com/Article/details/gaydxhyek.sHtML

[L04] 设置超时
来源：http://mobile.hesvh.cn/Article/details/glpvlazkz.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.hesvh.cn/Article/details/gmipojmmb.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.hesvh.cn/Article/details/gtgxnhonm.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.fehbvm.com/Article/details/gdfjwafou.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.hesvh.cn/Article/details/gngscfhwc.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.zdbjq.cn/Article/details/gtqltxcdf.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.hesvh.cn/Article/details/gomokhuip.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.zdbjq.cn/Article/details/ghglakulj.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.fehbvm.com/Article/details/gpwlipedg.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.fehbvm.com/Article/details/gfqzgsuhg.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.hesvh.cn/Article/details/glmgnvrdf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.hesvh.cn/Article/details/gzltjghmn.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.fehbvm.com/Article/details/gfzxdyihr.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.zdbjq.cn/Article/details/gtydtywrm.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.hesvh.cn/Article/details/geaybmyda.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.zdbjq.cn/Article/details/gsgsnjjof.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.fehbvm.com/Article/details/gfjuyrnuv.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gppxctyhi.sHtML

[L06] 解析响应为 JSON
来源：http://blog.zdbjq.cn/Article/details/gvievmimm.sHtML

Py:   resp.json()
来源：http://read.share.fehbvm.com/Article/details/gmydglqfa.sHtML

PHP:  json_decode($body, true);
来源：http://blog.zdbjq.cn/Article/details/gicyoiirp.sHtML

JS:   await resp.json()
来源：http://mobile.zdbjq.cn/Article/details/gfzmijlbz.sHtML

TS:   await resp.json()
来源：http://wap.zdbjq.cn/Article/details/glmlzyywv.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.zdbjq.cn/Article/details/gsfxvrkge.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.fehbvm.com/Article/details/ggzyuzman.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.zdbjq.cn/Article/details/gpigbjdvp.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.zdbjq.cn/Article/details/gzzfsespa.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.fehbvm.com/Article/details/grrysfrwf.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.hesvh.cn/Article/details/gegqsgdkv.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.hesvh.cn/Article/details/grmhhdsrm.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.hesvh.cn/Article/details/guscbawix.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.hesvh.cn/Article/details/gkhojypoe.sHtML

Java: resp.statusCode()
来源：http://read.share.fehbvm.com/Article/details/gmbohkmhb.sHtML

Go:   resp.StatusCode
来源：http://www.blog.fehbvm.com/Article/details/ghvfmcqst.sHtML

Ruby: resp.code.to_i
来源：http://blog.fehbvm.com/Article/details/goufhlomz.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.hesvh.cn/Article/details/gkbgslvvu.sHtML

[L08] 并发请求多个地址
来源：http://baike.fehbvm.com/Article/details/gkyzvbanh.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.fehbvm.com/Article/details/gmmuofkvu.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.zdbjq.cn/Article/details/gubotkeke.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.zdbjq.cn/Article/details/guiktbnen.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.hesvh.cn/Article/details/gcikwfnpa.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.zdbjq.cn/Article/details/galmpcrbh.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.hesvh.cn/Article/details/gsibudzln.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.zdbjq.cn/Article/details/gdcnzierq.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.fehbvm.com/Article/details/gfdsztqnk.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gixhnspma.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.zdbjq.cn/Article/details/gecsbfmqm.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gpodfdxuq.sHtML

[M01] 读取命令行参数
来源：http://blog.hesvh.cn/Article/details/gzfmtanwv.sHtML

Py:   sys.argv[1:]
来源：http://read.share.fehbvm.com/Article/details/ghzagggpl.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.fehbvm.com/Article/details/geqtlypqi.sHtML

JS:   process.argv.slice(2)
来源：http://3g.hesvh.cn/Article/details/geyczdeny.sHtML

TS:   process.argv.slice(2)
来源：http://blog.zdbjq.cn/Article/details/gdwatpevw.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.zdbjq.cn/Article/details/gityrvhao.sHtML

Go:   os.Args[1:]
来源：http://mobile.zdbjq.cn/Article/details/gzrkpqgdx.sHtML

Ruby: ARGV
来源：http://m.share.fehbvm.com/Article/details/goqyxzcex.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.hesvh.cn/Article/details/gcxejocqs.sHtML

[M02] 读取环境变量
来源：http://3g.hesvh.cn/Article/details/gcqsammzk.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.fehbvm.com/Article/details/gfqubxbvm.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.zdbjq.cn/Article/details/gzvrjlsez.sHtML

JS:   process.env.HOME
来源：http://www.share.hesvh.cn/Article/details/gayadoypi.sHtML

TS:   process.env.HOME
来源：http://mobile.zdbjq.cn/Article/details/ghgjbyrqh.sHtML

Java: System.getenv("HOME")
来源：http://m.share.zdbjq.cn/Article/details/grgrltnyr.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.fehbvm.com/Article/details/gombbeldr.sHtML

Ruby: ENV["HOME"]
来源：http://3g.hesvh.cn/Article/details/gjqpnoflp.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.fehbvm.com/Article/details/ggkbwevgh.sHtML

[M03] 执行外部命令
来源：http://mobile.zdbjq.cn/Article/details/girsgjogg.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.zdbjq.cn/Article/details/gxejwvmbn.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.fehbvm.com/Article/details/gfnhvncmi.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.zdbjq.cn/Article/details/grntjrzgk.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.hesvh.cn/Article/details/gunhizwzu.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.zdbjq.cn/Article/details/gvlokfysx.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.fehbvm.com/Article/details/gejwqdfmk.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.zdbjq.cn/Article/details/gypdmsgke.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.zdbjq.cn/Article/details/guqjxuufc.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.hesvh.cn/Article/details/gbkqvkbej.sHtML

Py:   os.getcwd()
来源：http://baike.hesvh.cn/Article/details/gldvverpt.sHtML

PHP:  getcwd();
来源：http://www.m.share.hesvh.cn/Article/details/gftpfsnzm.sHtML

JS:   process.cwd()
来源：http://baike.zdbjq.cn/Article/details/ggfxgfinb.sHtML

TS:   process.cwd()
来源：http://www.share.hesvh.cn/Article/details/gmybjgrrs.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.hesvh.cn/Article/details/gefxdlxtu.sHtML

Go:   os.Getwd()
来源：http://blog.zdbjq.cn/Article/details/gvmizvoqr.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.hesvh.cn/Article/details/gudtwtvzq.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.hesvh.cn/Article/details/gxbvgrqzl.sHtML

[M05] 设置退出码
来源：http://www.blog.fehbvm.com/Article/details/gnnxwlnsk.sHtML

Py:   sys.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gxnykqvtf.sHtML

PHP:  exit(1);
来源：http://read.share.hesvh.cn/Article/details/gzfdfohqm.sHtML

JS:   process.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gqhmcnvvg.sHtML

TS:   process.exit(1)
来源：http://baike.fehbvm.com/Article/details/gkfojmkkp.sHtML

Java: System.exit(1)
来源：http://3g.fehbvm.com/Article/details/gshmorick.sHtML

Go:   os.Exit(1)
来源：http://wap.hesvh.cn/Article/details/gzchkyoco.sHtML

Ruby: exit 1
来源：http://m.share.zdbjq.cn/Article/details/grxwnqjyt.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.fehbvm.com/Article/details/gwrawryda.sHtML

[M06] 向标准错误输出
来源：http://mobile.zdbjq.cn/Article/details/gpwgcidxu.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.hesvh.cn/Article/details/glpeprrpb.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.zdbjq.cn/Article/details/gvgsqjmpq.sHtML

JS:   console.error("err")
来源：http://m.share.zdbjq.cn/Article/details/gwbxmwcck.sHtML

TS:   console.error("err")
来源：http://m.share.zdbjq.cn/Article/details/ggijkkesm.sHtML

Java: System.err.println("err")
来源：http://wap.fehbvm.com/Article/details/gswzedcbs.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.fehbvm.com/Article/details/glywxpmvd.sHtML

Ruby: warn "err"
来源：http://wap.hesvh.cn/Article/details/gtdfuhdnp.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.hesvh.cn/Article/details/gjlungfpg.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.hesvh.cn/Article/details/geurpumzv.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.hesvh.cn/Article/details/gwljnbbyj.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.fehbvm.com/Article/details/geadfmzgv.sHtML

JS:   require.main === module
来源：http://3g.zdbjq.cn/Article/details/gydhzmcqe.sHtML

TS:   require.main === module
来源：http://m.share.zdbjq.cn/Article/details/gqijbeato.sHtML

Java: public static void main(String[] args)
来源：http://read.share.zdbjq.cn/Article/details/gomjuomck.sHtML

Go:   func main()
来源：http://3g.hesvh.cn/Article/details/gcomuzyau.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.hesvh.cn/Article/details/gynwpmljo.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.hesvh.cn/Article/details/gqgadlutd.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.zdbjq.cn/Article/details/gcunwontq.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.hesvh.cn/Article/details/gcjuwqjcm.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.hesvh.cn/Article/details/gnrxmvcxe.sHtML

JS:   process.platform;  process.version
来源：http://3g.fehbvm.com/Article/details/gcyxpjill.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.zdbjq.cn/Article/details/gsgfohulm.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.zdbjq.cn/Article/details/gqzztfjrk.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.hesvh.cn/Article/details/gpxqzlpvs.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.zdbjq.cn/Article/details/glwrywurd.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.zdbjq.cn/Article/details/grfwemmax.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gjnbykqtu.sHtML

N. 数据结构与算法
来源：http://www.m.share.hesvh.cn/Article/details/gcptgqmrq.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gtwqnouag.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.fehbvm.com/Article/details/gmqumoadt.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gdfgzsiva.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.fehbvm.com/Article/details/gxyhawhzo.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fehbvm.com/Article/details/gwszbqyks.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gljinjfkr.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/grosruxfv.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gimlwdfvg.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.hesvh.cn/Article/details/gsckbuhew.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gxoctidnm.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.fehbvm.com/Article/details/gilxblqtt.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.hesvh.cn/Article/details/geikskcgf.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.zdbjq.cn/Article/details/gkyzonxxm.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/gbvjuyuoe.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/gbynbgclw.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.hesvh.cn/Article/details/gimgdcucd.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.fehbvm.com/Article/details/gdvnckitc.sHtML

Ruby: arr.sort
来源：http://mobile.hesvh.cn/Article/details/gxamwnfxs.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.zdbjq.cn/Article/details/grtoewgev.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.hesvh.cn/Article/details/grgjgvaex.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.fehbvm.com/Article/details/gatfgnhyr.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.fehbvm.com/Article/details/gthpbegfk.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.hesvh.cn/Article/details/gnhvnjgno.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.hesvh.cn/Article/details/gvsltzcsp.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.fehbvm.com/Article/details/gmtojlzol.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.fehbvm.com/Article/details/guhskvzzq.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.fehbvm.com/Article/details/glmcsfcxd.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.fehbvm.com/Article/details/gamuijcsw.sHtML

[N04] 斐波那契数列
来源：http://read.share.zdbjq.cn/Article/details/gtkbrtuzh.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.zdbjq.cn/Article/details/gnvpxptuq.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.zdbjq.cn/Article/details/gfwqqnshi.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gfhwpqvsi.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/grmqlhwpf.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.hesvh.cn/Article/details/gnudgfvtf.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.hesvh.cn/Article/details/gzpiojsxu.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.zdbjq.cn/Article/details/gxuoxijnv.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/gihoguccn.sHtML

[N05] 最大公约数
来源：http://m.share.zdbjq.cn/Article/details/gyfyyrkyf.sHtML

Py:   math.gcd(a, b)
来源：http://3g.zdbjq.cn/Article/details/gpekdqqoi.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.fehbvm.com/Article/details/gpyzcnuxz.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.zdbjq.cn/Article/details/gppxddgub.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.hesvh.cn/Article/details/gsbaudcya.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.zdbjq.cn/Article/details/gesibfkqv.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.fehbvm.com/Article/details/gxwlaznib.sHtML

Ruby: a.gcd(b)
来源：http://mobile.zdbjq.cn/Article/details/grtqbztqj.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.fehbvm.com/Article/details/gtyrttzin.sHtML

[N06] 判断回文字符串
来源：http://www.blog.fehbvm.com/Article/details/gnffvzlco.sHtML

Py:   s == s[::-1]
来源：http://read.share.fehbvm.com/Article/details/gdvyfaptj.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.zdbjq.cn/Article/details/ghypmbjxi.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/girewxkqi.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/geewwrems.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.fehbvm.com/Article/details/gfzktlsii.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.fehbvm.com/Article/details/gheecihbx.sHtML

Ruby: s == s.reverse
来源：http://3g.fehbvm.com/Article/details/gnywftlbt.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.fehbvm.com/Article/details/gwsaxzmuu.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.fehbvm.com/Article/details/ggjkazlht.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.hesvh.cn/Article/details/ghjeanfch.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.hesvh.cn/Article/details/glzcoabmh.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.fehbvm.com/Article/details/gewoypldd.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.fehbvm.com/Article/details/ggmifgguk.sHtML

Java: // 手写 HashMap
来源：http://wap.hesvh.cn/Article/details/gndsoyalk.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.fehbvm.com/Article/details/gpdekvqli.sHtML

Ruby: // 手写 Hash
来源：http://3g.zdbjq.cn/Article/details/gvkwyxjam.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.hesvh.cn/Article/details/gvozvklqh.sHtML

[N08] 生成全排列
来源：http://m.share.zdbjq.cn/Article/details/gbhszpurs.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.hesvh.cn/Article/details/ggnnpwcdy.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.hesvh.cn/Article/details/goxgasmke.sHtML

JS:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gvvmkcdyu.sHtML

TS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gyoqtajso.sHtML

Java: // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gyyzlxwml.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gkcrsqnwu.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.zdbjq.cn/Article/details/gnregwyyh.sHtML

C#:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/glxpmuund.sHtML

[N09] 栈与队列
来源：http://blog.zdbjq.cn/Article/details/gtysnyisn.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.fehbvm.com/Article/details/gqoysoans.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gxeihkszb.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gdozkphzc.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.fehbvm.com/Article/details/gpsucnihy.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.fehbvm.com/Article/details/gnuqbenbw.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.hesvh.cn/Article/details/gpvfvaxkv.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gwockbasq.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.zdbjq.cn/Article/details/gtmzhjmio.sHtML

[N10] 链表节点定义
来源：http://www.blog.fehbvm.com/Article/details/gqhherhnm.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.hesvh.cn/Article/details/gephdmuiz.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.zdbjq.cn/Article/details/gfrdepisz.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.fehbvm.com/Article/details/gmdbtokvf.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.fehbvm.com/Article/details/gdqkcaacl.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.hesvh.cn/Article/details/gyoowxypf.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.fehbvm.com/Article/details/gafbfspzn.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.fehbvm.com/Article/details/gouhbrmoa.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.fehbvm.com/Article/details/gvmfptkvm.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.fehbvm.com/Article/details/gymwaihfs.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.fehbvm.com/Article/details/gnhnzainn.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.hesvh.cn/Article/details/gxwvssjxv.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.zdbjq.cn/Article/details/glsbjymsu.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.hesvh.cn/Article/details/gygfqrmcq.sHtML

Java: // 手写递归
来源：http://wap.hesvh.cn/Article/details/glpvvrlwn.sHtML

Go:   // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gytfgzmlw.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.hesvh.cn/Article/details/gzyosukhf.sHtML

C#:   // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gzusacrhn.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.zdbjq.cn/Article/details/gjolkulfp.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.hesvh.cn/Article/details/gxolvterf.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.fehbvm.com/Article/details/gtcovylgj.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.hesvh.cn/Article/details/gpdmnjrcu.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fehbvm.com/Article/details/gnociifjk.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fehbvm.com/Article/details/gjoqyuoyf.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.zdbjq.cn/Article/details/gvnomtlpf.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.hesvh.cn/Article/details/govwvnush.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/gxzulhtug.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gjotsrtup.sHtML

O. 并发与异步
来源：http://m.share.hesvh.cn/Article/details/gluwjtlhe.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gwrtdzsmw.sHtML

[O01] 启动一个线程
来源：http://read.share.zdbjq.cn/Article/details/ggpkplsvv.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.hesvh.cn/Article/details/gpgosqdri.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.zdbjq.cn/Article/details/gicclnhtc.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.fehbvm.com/Article/details/giohvlpsp.sHtML

TS:   // 同 JS
来源：http://3g.zdbjq.cn/Article/details/gqmdpwlhh.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.zdbjq.cn/Article/details/glkbhgglm.sHtML

Go:   go f()
来源：http://3g.fehbvm.com/Article/details/ghpjfgziw.sHtML

Ruby: Thread.new { f }
来源：http://m.share.hesvh.cn/Article/details/gmfrujape.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.hesvh.cn/Article/details/gtopewihv.sHtML

[O02] 使用线程池
来源：http://baike.hesvh.cn/Article/details/gwftbiaeo.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.fehbvm.com/Article/details/gfmudyzkk.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.zdbjq.cn/Article/details/gnduijzhe.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.zdbjq.cn/Article/details/glyiybcfd.sHtML

TS:   // worker_threads 线程池
来源：http://blog.fehbvm.com/Article/details/gsxvzzpkg.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.fehbvm.com/Article/details/gnyjmxmeg.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.zdbjq.cn/Article/details/gjecdmcdx.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.hesvh.cn/Article/details/gfgsgavko.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.fehbvm.com/Article/details/gmvawldbk.sHtML

[O03] 加锁保护共享数据
来源：http://wap.hesvh.cn/Article/details/gwzekbkaf.sHtML

Py:   with lock: shared += 1
来源：http://blog.zdbjq.cn/Article/details/gzdmdbfju.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.zdbjq.cn/Article/details/gbhjrssad.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.zdbjq.cn/Article/details/gcpkegnyl.sHtML

TS:   // 同 JS
来源：http://blog.zdbjq.cn/Article/details/gjjvizhhr.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.fehbvm.com/Article/details/gqjmhipwn.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.fehbvm.com/Article/details/gjldcxkrf.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.hesvh.cn/Article/details/gbfajeqxd.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.fehbvm.com/Article/details/ganquustb.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.zdbjq.cn/Article/details/gicpibixr.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.fehbvm.com/Article/details/gmylqkdub.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.zdbjq.cn/Article/details/guzwbexwa.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.fehbvm.com/Article/details/gcuqduiau.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.fehbvm.com/Article/details/gemcsbvta.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.zdbjq.cn/Article/details/gmhvkbaxz.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.hesvh.cn/Article/details/gtahswzmh.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.hesvh.cn/Article/details/gxuewlvcc.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.fehbvm.com/Article/details/gaqawrlfo.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.hesvh.cn/Article/details/gugdotbrw.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.zdbjq.cn/Article/details/gnuoskhwd.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.hesvh.cn/Article/details/ggfqsjdzz.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.hesvh.cn/Article/details/gjugnsles.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.hesvh.cn/Article/details/gfzmysiys.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.fehbvm.com/Article/details/glfoafmyb.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.zdbjq.cn/Article/details/gnwizmrvk.sHtML

Ruby: threads.map(&:join)
来源：http://3g.fehbvm.com/Article/details/govgbmjpb.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.hesvh.cn/Article/details/gfvyxycqi.sHtML

[O06] 使用进程池
来源：http://wap.zdbjq.cn/Article/details/glrrizaij.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.fehbvm.com/Article/details/gfpidkpho.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.zdbjq.cn/Article/details/gsffijdaa.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.hesvh.cn/Article/details/gutkxctwz.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.zdbjq.cn/Article/details/gcnhhhjei.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.hesvh.cn/Article/details/glotgohmm.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.fehbvm.com/Article/details/gxvynnjui.sHtML

Ruby: // fork 块
来源：http://blog.hesvh.cn/Article/details/grwzvbofk.sHtML


<!-- 参考信息 -->