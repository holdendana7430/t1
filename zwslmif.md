代发 wailian999

[L03] 设置自定义请求头
来源：http://mobile.fanxiaobao.xyz/Article/details/gnclaaiwg.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gizfszuwh.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.fanxiaobao.xyz/Article/details/gttnrugqq.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.fanxiaobao.xyz/Article/details/gpvkgxogt.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.fanxiaobao.xyz/Article/details/gxwbsxxij.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.fanxiaobao.xyz/Article/details/gecduudal.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.fanxiaobao.xyz/Article/details/gveqtcifo.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.fanxiaobao.xyz/Article/details/gkdtyajgf.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.fanxiaobao.xyz/Article/details/ghipxbbzj.sHtML

[L04] 设置超时
来源：http://blog.fanxiaobao.xyz/Article/details/gdudglzby.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.fanxiaobao.xyz/Article/details/gaghuyvha.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.fanxiaobao.xyz/Article/details/gvupvgqrk.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.fanxiaobao.xyz/Article/details/gyjemdrdu.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.fanxiaobao.xyz/Article/details/gnzpyuvox.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gobmeenht.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gooodnrqs.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.fanxiaobao.xyz/Article/details/gwempenyx.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.fanxiaobao.xyz/Article/details/glsmmhjjq.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.fanxiaobao.xyz/Article/details/ggybukzub.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.fanxiaobao.xyz/Article/details/gjzefzrzr.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.fanxiaobao.xyz/Article/details/gdlhkclkg.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glejyhera.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.fanxiaobao.xyz/Article/details/gstngmvlh.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.fanxiaobao.xyz/Article/details/gtfdgtfyp.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gfbwzaimk.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.fanxiaobao.xyz/Article/details/glsqreqyo.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.fanxiaobao.xyz/Article/details/ginupsoid.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/gmkgytnvq.sHtML

Py:   resp.json()
来源：http://m.share.fanxiaobao.xyz/Article/details/glcejfvaf.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gntpzqfhd.sHtML

JS:   await resp.json()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glgtpjtwc.sHtML

TS:   await resp.json()
来源：http://blog.fanxiaobao.xyz/Article/details/gczkrlcpu.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkkgfifka.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.fanxiaobao.xyz/Article/details/gutoegbnn.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.fanxiaobao.xyz/Article/details/gfjeujkxr.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.fanxiaobao.xyz/Article/details/gtuaekslp.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gepywjgzt.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.fanxiaobao.xyz/Article/details/gatribnke.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.fanxiaobao.xyz/Article/details/gnvuzctkg.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbrrorfib.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.fanxiaobao.xyz/Article/details/gbhgfngfj.sHtML

Java: resp.statusCode()
来源：http://baike.fanxiaobao.xyz/Article/details/gmcswelyn.sHtML

Go:   resp.StatusCode
来源：http://m.share.fanxiaobao.xyz/Article/details/ghozqpbna.sHtML

Ruby: resp.code.to_i
来源：http://blog.fanxiaobao.xyz/Article/details/glbxyleeq.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.fanxiaobao.xyz/Article/details/gsnbluqae.sHtML

[L08] 并发请求多个地址
来源：http://read.share.fanxiaobao.xyz/Article/details/gnumrydoc.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.fanxiaobao.xyz/Article/details/gvhgdernz.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.fanxiaobao.xyz/Article/details/gvnzsfdwz.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fanxiaobao.xyz/Article/details/ggfmnnqlf.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fanxiaobao.xyz/Article/details/gjtdppvkm.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.fanxiaobao.xyz/Article/details/gzqwlxmks.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.fanxiaobao.xyz/Article/details/gjqvrwxui.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtjmwpssk.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gggasymva.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gzcgbxvig.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghutdmeis.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/guzhsphcz.sHtML

[M01] 读取命令行参数
来源：http://blog.fanxiaobao.xyz/Article/details/gbgojuuhw.sHtML

Py:   sys.argv[1:]
来源：http://blog.fanxiaobao.xyz/Article/details/geqjwcqfu.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbwrvhtss.sHtML

JS:   process.argv.slice(2)
来源：http://wap.fanxiaobao.xyz/Article/details/gkmnjlkym.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyfoihpxc.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.fanxiaobao.xyz/Article/details/grpmwmdlo.sHtML

Go:   os.Args[1:]
来源：http://mobile.fanxiaobao.xyz/Article/details/glelszblc.sHtML

Ruby: ARGV
来源：http://wap.fanxiaobao.xyz/Article/details/gonqiuhjr.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.fanxiaobao.xyz/Article/details/gxvrlvprh.sHtML

[M02] 读取环境变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gpbxrqqeb.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.fanxiaobao.xyz/Article/details/guxktqwzj.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjrxwtrdy.sHtML

JS:   process.env.HOME
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqvptxbah.sHtML

TS:   process.env.HOME
来源：http://baike.fanxiaobao.xyz/Article/details/gqavkagor.sHtML

Java: System.getenv("HOME")
来源：http://wap.fanxiaobao.xyz/Article/details/gznyoqhik.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.fanxiaobao.xyz/Article/details/gwtzqsyev.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghzjrqiqd.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.fanxiaobao.xyz/Article/details/goczarsgi.sHtML

[M03] 执行外部命令
来源：http://mobile.fanxiaobao.xyz/Article/details/gwqtkpvjz.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.fanxiaobao.xyz/Article/details/gcuqljxel.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.fanxiaobao.xyz/Article/details/gixlelfww.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.fanxiaobao.xyz/Article/details/gqrpfqcxt.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.fanxiaobao.xyz/Article/details/gajbxduib.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwmadycmw.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghirevgep.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.fanxiaobao.xyz/Article/details/gzndnbqov.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.fanxiaobao.xyz/Article/details/gojmynvmq.sHtML

[M04] 获取当前工作目录
来源：http://mobile.fanxiaobao.xyz/Article/details/gulgzajnr.sHtML

Py:   os.getcwd()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gohrjeyxp.sHtML

PHP:  getcwd();
来源：http://wap.fanxiaobao.xyz/Article/details/gkpresqgw.sHtML

JS:   process.cwd()
来源：http://wap.fanxiaobao.xyz/Article/details/gxqrfekoq.sHtML

TS:   process.cwd()
来源：http://read.share.fanxiaobao.xyz/Article/details/gjpolzjsw.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.fanxiaobao.xyz/Article/details/gyfgckrhx.sHtML

Go:   os.Getwd()
来源：http://read.share.fanxiaobao.xyz/Article/details/gkabzsydx.sHtML

Ruby: Dir.pwd
来源：http://wap.fanxiaobao.xyz/Article/details/gegfqpquq.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.fanxiaobao.xyz/Article/details/gwjuantbp.sHtML

[M05] 设置退出码
来源：http://mobile.fanxiaobao.xyz/Article/details/gocovtukg.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkkpclywg.sHtML

PHP:  exit(1);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbbecrrbg.sHtML

JS:   process.exit(1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzdyqexsh.sHtML

TS:   process.exit(1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwofbslav.sHtML

Java: System.exit(1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghyshrvni.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzvhollsd.sHtML

Ruby: exit 1
来源：http://3g.fanxiaobao.xyz/Article/details/glustpfbx.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gysavvhjd.sHtML

[M06] 向标准错误输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gsjvloakc.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpywoohlp.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcbfetvgi.sHtML

JS:   console.error("err")
来源：http://m.share.fanxiaobao.xyz/Article/details/ghrcjjzei.sHtML

TS:   console.error("err")
来源：http://www.share.fanxiaobao.xyz/Article/details/gpvriwwro.sHtML

Java: System.err.println("err")
来源：http://mobile.fanxiaobao.xyz/Article/details/gaudhwfcf.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsgbhbkdx.sHtML

Ruby: warn "err"
来源：http://baike.fanxiaobao.xyz/Article/details/gdxuqrntj.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.fanxiaobao.xyz/Article/details/gncohrlzh.sHtML

[M07] 判断是否为主入口
来源：http://3g.fanxiaobao.xyz/Article/details/gmqisivyf.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdzhkjfsr.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.fanxiaobao.xyz/Article/details/gdztokcqu.sHtML

JS:   require.main === module
来源：http://baike.fanxiaobao.xyz/Article/details/ggwwgiiic.sHtML

TS:   require.main === module
来源：http://wap.fanxiaobao.xyz/Article/details/gaolantuq.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glozdqawc.sHtML

Go:   func main()
来源：http://blog.fanxiaobao.xyz/Article/details/gvddzxyny.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.fanxiaobao.xyz/Article/details/gyhuxqlhu.sHtML

C#:   static void Main(string[] args)
来源：http://blog.fanxiaobao.xyz/Article/details/gzkgegfql.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.fanxiaobao.xyz/Article/details/gpulwmfpv.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.fanxiaobao.xyz/Article/details/gagvazbpy.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.fanxiaobao.xyz/Article/details/gserzpaie.sHtML

JS:   process.platform;  process.version
来源：http://read.share.fanxiaobao.xyz/Article/details/gnacsopgi.sHtML

TS:   process.platform;  process.version
来源：http://baike.fanxiaobao.xyz/Article/details/gjnxjnrjd.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.fanxiaobao.xyz/Article/details/gkyeekums.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggyepnlzh.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.fanxiaobao.xyz/Article/details/ggruywdmn.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.fanxiaobao.xyz/Article/details/ghisqjfhw.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gxljllfre.sHtML

N. 数据结构与算法
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbqewvefj.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/guvqieutd.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.fanxiaobao.xyz/Article/details/gcrzbxgbf.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.fanxiaobao.xyz/Article/details/gcpeincmi.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.fanxiaobao.xyz/Article/details/gpafymybw.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fanxiaobao.xyz/Article/details/gmmbohtqg.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fanxiaobao.xyz/Article/details/gmjmklher.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gudcpqnwv.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.fanxiaobao.xyz/Article/details/guggryyao.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.fanxiaobao.xyz/Article/details/gdpvtnsba.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gaadzldmh.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.fanxiaobao.xyz/Article/details/gjosclmpi.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fanxiaobao.xyz/Article/details/gqhywiasr.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gjwuweyuv.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fanxiaobao.xyz/Article/details/gupfunmfz.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbgdtinqf.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gilzlhfyw.sHtML

Go:   slices.Sort(arr)
来源：http://blog.fanxiaobao.xyz/Article/details/gsllhnafh.sHtML

Ruby: arr.sort
来源：http://3g.fanxiaobao.xyz/Article/details/gmulgagro.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.fanxiaobao.xyz/Article/details/goxwtqvcv.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.fanxiaobao.xyz/Article/details/gpxlbbvpw.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.fanxiaobao.xyz/Article/details/gwgwsogsq.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.fanxiaobao.xyz/Article/details/gbckfylmu.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fanxiaobao.xyz/Article/details/ggzasetui.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fanxiaobao.xyz/Article/details/gymrhljpc.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.fanxiaobao.xyz/Article/details/gzemrznxe.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxxyslovp.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geubyysou.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.fanxiaobao.xyz/Article/details/gpsbcovfv.sHtML

[N04] 斐波那契数列
来源：http://www.share.fanxiaobao.xyz/Article/details/gxvzmxchn.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gihhdwxdd.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmdisdwrd.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fanxiaobao.xyz/Article/details/gthcjpuoj.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gghcfxion.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.fanxiaobao.xyz/Article/details/goybpqiua.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giecxlyok.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpztihfgy.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtpufjgjx.sHtML

[N05] 最大公约数
来源：http://www.share.fanxiaobao.xyz/Article/details/gjjkkgxxs.sHtML

Py:   math.gcd(a, b)
来源：http://wap.fanxiaobao.xyz/Article/details/gjfulapra.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggghblgkp.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gylibhzrm.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfwknkmji.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.fanxiaobao.xyz/Article/details/glbzahteh.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyqkwoxgx.sHtML

Ruby: a.gcd(b)
来源：http://mobile.fanxiaobao.xyz/Article/details/gthzsnmbn.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqzvfpkcx.sHtML

[N06] 判断回文字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gxyiydmnu.sHtML

Py:   s == s[::-1]
来源：http://m.share.fanxiaobao.xyz/Article/details/gdyvaaigl.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmpyjxjvz.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.fanxiaobao.xyz/Article/details/geiwsmboq.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.fanxiaobao.xyz/Article/details/glacxnxti.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcohdjeni.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcpfyqcob.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxsmnuovi.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.fanxiaobao.xyz/Article/details/gqkopgxwj.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.fanxiaobao.xyz/Article/details/gfqjoaijs.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.fanxiaobao.xyz/Article/details/gesfnxufg.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkjzuhchr.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.fanxiaobao.xyz/Article/details/gkssdxozk.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.fanxiaobao.xyz/Article/details/gacxwuvsa.sHtML

Java: // 手写 HashMap
来源：http://www.share.fanxiaobao.xyz/Article/details/ghgbenryk.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyyqcggeo.sHtML

Ruby: // 手写 Hash
来源：http://3g.fanxiaobao.xyz/Article/details/gcabpiaog.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.fanxiaobao.xyz/Article/details/gsurhdgwp.sHtML

[N08] 生成全排列
来源：http://blog.fanxiaobao.xyz/Article/details/gghanyqzj.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gntyxvcxo.sHtML

PHP:  // 手写递归交换
来源：http://baike.fanxiaobao.xyz/Article/details/gjhwhjylf.sHtML

JS:   // 手写回溯递归
来源：http://baike.fanxiaobao.xyz/Article/details/gkvzfbczw.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.fanxiaobao.xyz/Article/details/gycqqscjt.sHtML

Java: // 手写回溯递归
来源：http://3g.fanxiaobao.xyz/Article/details/ggrhmdqij.sHtML

Go:   // 手写回溯递归
来源：http://m.share.fanxiaobao.xyz/Article/details/gauikppuh.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.fanxiaobao.xyz/Article/details/gkhsrjqwy.sHtML

C#:   // 手写回溯递归
来源：http://baike.fanxiaobao.xyz/Article/details/grjaepnre.sHtML

[N09] 栈与队列
来源：http://blog.fanxiaobao.xyz/Article/details/goucbhdod.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.fanxiaobao.xyz/Article/details/gjtjtwsrt.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.fanxiaobao.xyz/Article/details/gslmecwmm.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.fanxiaobao.xyz/Article/details/gbxfhxlza.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.fanxiaobao.xyz/Article/details/gwcepewgv.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.fanxiaobao.xyz/Article/details/gjjlrhjsi.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.fanxiaobao.xyz/Article/details/gwnfiwsbw.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.fanxiaobao.xyz/Article/details/gmdkunies.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gykwjoiun.sHtML

[N10] 链表节点定义
来源：http://3g.fanxiaobao.xyz/Article/details/gyldlbdfb.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.fanxiaobao.xyz/Article/details/gefldtysz.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.fanxiaobao.xyz/Article/details/gsrakupgj.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxuqxeqpr.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.fanxiaobao.xyz/Article/details/glewakokn.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnlpioxek.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdujuzhfj.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.fanxiaobao.xyz/Article/details/grkuxfept.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.fanxiaobao.xyz/Article/details/ggvhpjutc.sHtML

[N11] 二叉树中序遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gykxfkpac.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.fanxiaobao.xyz/Article/details/gnfhcskrx.sHtML

PHP:  // 手写递归函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gkxiafjul.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fanxiaobao.xyz/Article/details/gebpumkva.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fanxiaobao.xyz/Article/details/gjqsmzexb.sHtML

Java: // 手写递归
来源：http://m.share.fanxiaobao.xyz/Article/details/gtvcdelcq.sHtML

Go:   // 手写递归
来源：http://m.share.fanxiaobao.xyz/Article/details/gchqgtpcg.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghfcdluwc.sHtML

C#:   // 手写递归
来源：http://mobile.fanxiaobao.xyz/Article/details/guwqtvwpn.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmcxhbhxi.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.fanxiaobao.xyz/Article/details/gcujohdgt.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.fanxiaobao.xyz/Article/details/gqikchzhn.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fanxiaobao.xyz/Article/details/gdrzfzers.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fanxiaobao.xyz/Article/details/gunphzzpg.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpcvtdlgv.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.fanxiaobao.xyz/Article/details/gqhdaqbjk.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvsfwkykg.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.fanxiaobao.xyz/Article/details/gzhtzdtsp.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/ggpdwkqhv.sHtML

O. 并发与异步
来源：http://www.share.fanxiaobao.xyz/Article/details/gvtrmxmkh.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gzynluhgp.sHtML

[O01] 启动一个线程
来源：http://3g.fanxiaobao.xyz/Article/details/gkwuzjuqo.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtgeevtbv.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghylystsi.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvmtykqfr.sHtML

TS:   // 同 JS
来源：http://baike.fanxiaobao.xyz/Article/details/gtaxeyqtf.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guefdpkwy.sHtML

Go:   go f()
来源：http://www.share.fanxiaobao.xyz/Article/details/gmqbhllcg.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdrfntlxz.sHtML

C#:   Task.Run(() => F());
来源：http://wap.fanxiaobao.xyz/Article/details/gtayzvoer.sHtML

[O02] 使用线程池
来源：http://blog.fanxiaobao.xyz/Article/details/gzpooeewu.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gokpwsmvr.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.fanxiaobao.xyz/Article/details/gyuzlxybw.sHtML

JS:   // worker_threads 线程池
来源：http://blog.fanxiaobao.xyz/Article/details/ghuxvlseb.sHtML

TS:   // worker_threads 线程池
来源：http://baike.fanxiaobao.xyz/Article/details/gsqtavbli.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.fanxiaobao.xyz/Article/details/giihzfpsh.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gevlhvlig.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.fanxiaobao.xyz/Article/details/gjqjxdire.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.fanxiaobao.xyz/Article/details/gkpdsltbx.sHtML

[O03] 加锁保护共享数据
来源：http://baike.fanxiaobao.xyz/Article/details/gayyjsevo.sHtML

Py:   with lock: shared += 1
来源：http://3g.fanxiaobao.xyz/Article/details/gcqaojteo.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.fanxiaobao.xyz/Article/details/gjiqqbvsz.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfjjtzfrj.sHtML

TS:   // 同 JS
来源：http://read.share.fanxiaobao.xyz/Article/details/ggjtycujq.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gsoqezshu.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.fanxiaobao.xyz/Article/details/gqhrtcnmm.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gulxmelcw.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gcvioiugu.sHtML

[O04] 定义异步函数并等待
来源：http://wap.fanxiaobao.xyz/Article/details/gtqgxfljm.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.fanxiaobao.xyz/Article/details/genhxewgk.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.fanxiaobao.xyz/Article/details/ggqbtwkjc.sHtML

JS:   async function f() { await g(); }
来源：http://blog.fanxiaobao.xyz/Article/details/gthxlgogw.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.fanxiaobao.xyz/Article/details/glzeuezri.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.fanxiaobao.xyz/Article/details/gylhkmloz.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.fanxiaobao.xyz/Article/details/gkyluzmaw.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.fanxiaobao.xyz/Article/details/gseuhgojd.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.fanxiaobao.xyz/Article/details/ghjprjnzh.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.fanxiaobao.xyz/Article/details/gujlxgasy.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmqovzqym.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.fanxiaobao.xyz/Article/details/glsclzorv.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glagnyktx.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gojgiounp.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.fanxiaobao.xyz/Article/details/gevvhdaxi.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gszfvhvbb.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.fanxiaobao.xyz/Article/details/gflgosjfm.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnttniyqm.sHtML

[O06] 使用进程池
来源：http://baike.fanxiaobao.xyz/Article/details/gojadvsxt.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.fanxiaobao.xyz/Article/details/giuvlbywn.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmlvyerxk.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.fanxiaobao.xyz/Article/details/gcqexkehx.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.fanxiaobao.xyz/Article/details/gstnhjlxd.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjdgundby.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.fanxiaobao.xyz/Article/details/gpclbjrrw.sHtML

Ruby: // fork 块
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giwvcbqjq.sHtML

C#:   Parallel.For
来源：http://read.share.fanxiaobao.xyz/Article/details/ghsjjcbts.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gbkekeodv.sHtML

P. 常用工具函数
来源：http://blog.fanxiaobao.xyz/Article/details/gvfrmsqrf.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gayhdvjgd.sHtML


<!-- 参考信息 -->