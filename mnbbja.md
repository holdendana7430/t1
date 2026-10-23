代发 wailian999

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3gibppkle.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3fcqobrsz.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3xjrkufxq.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3elgbcrmn.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3cknkhljm.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3ysdgzroj.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3ljvixkpj.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3fvxewcsc.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3dpxszgzg.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3xjnfulyh.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3qdwuycya.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3koxwljyg.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3ciyxgyxt.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3mjsetmts.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3inpnsguj.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3zskponry.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3iitcdemu.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3loaxdbso.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3waaxeccw.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3whprheoq.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3dyjqjfnv.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3buwclipb.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3zwwuwwtd.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3vmxmotao.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3wccpwmat.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3gfhnqaxy.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3alrxjxxa.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3clhadwma.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3tiziwpmb.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3nfwqmjdr.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3wriiapmg.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3syizfrxw.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3syziyfmw.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3auvvrrvi.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xvupubfx.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3vgmamddw.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3zvrateku.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3prlqtxfd.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3rfjhimos.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3ksegfgim.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3vockvftv.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3tzylwwym.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3voqqywsc.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3iqsslxtm.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3zmfemmdq.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3qpjyymiu.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3zfihihwu.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3mufhknjx.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3cwcoqqfm.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3kooaiejt.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3nvdmyowb.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3zvujtlpx.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3lvbtrvjf.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3upqcljgz.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3qcexdxxd.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3rcpmretx.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3snweztjo.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3heolpzis.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3izgcbbal.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3ahdvqvgc.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3znjjozbv.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3qrszfhtr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3plsvmiyt.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3qxvfdrhh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sfvkvtuc.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3cahkgzhb.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3omzqtxxp.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3keopdgrp.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3qprlwgtr.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ipwjjwic.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3upfkaheb.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3sigcettw.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3wrxtbqae.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3pdzbxoyz.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3pvgovmln.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3onrqjruc.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3shxqmois.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3kpuyvobt.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3gyygvibv.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3kezmkeea.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3rasazkxp.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3qqwfoxze.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3wivbsoip.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3nqewkkal.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3rxriugjz.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3feolrfjh.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3mqwznspo.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3yijphnos.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3aeznplio.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3aefkclgl.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3iancsmaz.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3ixgkmnht.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3ysntpcin.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3erpyjqbb.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3junhmthd.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3xfkyjrcc.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3micbnsxk.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3himtmzde.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3xfahgbbs.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3xvpcbbrz.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3xjvfzzvm.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3ufbesvmy.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mjsyhziz.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3rpjffgth.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3aywhtxbu.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zygzrgja.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ozxfxbdm.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nzdndaol.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3qlehhgzs.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3laogjabi.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3wwsevfex.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3cqgdxjhe.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3fnerbfpi.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3kuwljvte.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3lraliciw.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3nuqeovbc.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3unvcwxra.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3jmxbqrol.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3kxyghwmt.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3pibnoakh.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3yvfnjtlp.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3undovnql.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3rygfmxwj.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3wwptstjh.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3gbcqdhty.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3zpqzqudi.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3zjjfvmhh.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3czueothv.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3sxvmqdgs.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3gmhivkdy.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3gfcaztpp.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3visfaxjc.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3jeeemupk.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3rgowaezq.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3evgaeikf.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3pbbetovy.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3cvpypvpu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xgarcmol.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3qoiqvytv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cartaguo.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3utlvhygl.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3zuemmrfp.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3vbmuphec.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3vuecyzsa.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3kqmqhmog.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3zqfyrsye.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3nkejxyfk.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3olvgrulb.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3nedrpioa.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3gmdfifpw.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3yghobchc.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3conafozs.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3eavqghsa.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ghxbtiyd.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3nnthxftx.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jebxznlr.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3apoydrya.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3ayiqwmtt.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3bleeztyt.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3fkowvelk.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3gtoaorro.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3qmcbdvik.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3tunxaice.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3txizwqug.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3wvipoeso.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3ifgwjbfi.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3efsufefb.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3bbmmuesp.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nhfbceoq.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3bdwgmgne.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ovpbjbgd.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3qahtvwqx.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3goavakfg.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3lwiwtcqi.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3ilqanvhq.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3ttaiihxu.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3fkpifjfd.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3wfxfbkoz.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3hpsexmkk.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3wjrtmrdv.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3miohsvkz.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3ofjvfwnu.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3gmohthad.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3typsppnm.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3riwfdsiv.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3vpfxqtgu.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3pqcpcdnn.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3zndrtpfq.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3dwrhscbx.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rpkdbndv.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3urfagreb.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3dehapvgn.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3jzapttav.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3rzzfdwbh.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3ziqmfmye.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3ztxqvcte.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3brzvoans.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3tfhegkby.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3jvczpqdo.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3acohtszu.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3uhkgdtec.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3xpwslyfa.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3jefpkrlp.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3gayjiblv.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ovnxyxnw.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3vwmwpaaz.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3knhalajm.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3xhqipxgx.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3wsuknbsf.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3mxylhkgx.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3jpwqofqi.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3pwfxomvc.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3tqvxvpza.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3smkdpwdg.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3joaaqltb.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3cbrstscv.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3tiqzlnhy.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3opfuebbu.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3nfqxcabc.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3hnjrjmqr.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3kvrtyoed.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3lszidnof.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3bwkyedas.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3yjonemqu.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3puesfloo.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3lzujwbhu.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3grivdocj.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3injntdga.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3eozlczdy.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3jkvpuwww.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3vjcfjrvq.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3wemqyovj.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3mtyrcaxd.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3sbhuooob.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3zgskwnir.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ouvipyhf.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3bkfjzxlr.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3dlenvfmz.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3tncjyfpj.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3ayyfgsac.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3aagvnroi.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3grulbyua.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3xudjycig.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3ogykjois.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3onjlhhoo.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3fofbkmjd.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3xmudfeyd.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3hywhlogg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mxgiogge.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3tkfkeaic.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ophxrqyn.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3dizgixpb.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3xdotsdij.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3mrsckqtr.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3qltiqrtq.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3nmapwnxv.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3wdzhbfkj.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3qgucxltj.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3xnbwpiyd.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3srvduaud.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3yqzznele.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3pbnovcqu.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3oaqqysno.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3zbbodwhk.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3uyqjggos.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3oakheldr.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3eerosgrm.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3tmpobmgh.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3fljdoovy.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3yrpgntuh.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3vqeftozl.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3mhynxwbl.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3frjotkug.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3qgxhrvun.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3wcmmkrpn.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3gjyqclqn.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3uckmtmrg.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3slnontdp.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3ylujbpnh.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3olxajail.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3ufoszkzh.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3pyqndovt.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3aypayhrv.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3uoxmgrnz.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3aoryxbja.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3kdspqkzs.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3wfermmwk.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3lbnfyckq.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3jvxedphf.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3fkewfbvt.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ffijcfiu.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3itdxutql.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3yvsjugea.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3yydazlqe.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3bgcefaor.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3czntagut.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3ksksyntb.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3riekodsr.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3srcffkna.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3wprtxahf.html


<!-- 参考信息 -->