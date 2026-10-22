代发 wailian999

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2sckkatqs.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2pdnjmttr.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2cqsrryjh.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2mfltxpqg.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2eczixpyu.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2ncieiqgp.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2eqpptpjh.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2dxpexmmb.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2xsbpnjlu.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2hyjtyoxq.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2ouvokajw.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2arfvoqsb.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2qygptceb.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2bavourmf.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2egdavofm.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2nsbwaktb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2mqrvqahz.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2hxjrwebl.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2kyeultpi.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2kgbkwsnf.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2jeljprfq.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2xnapriyp.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xhinxjpk.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2zmwyscpb.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2upznbynj.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2rglfdvna.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2euolkrei.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2qawlfxgb.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2ltpeorhm.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2pqosiydp.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2frqttmxb.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2zspmdcjr.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2skzvdvmb.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2xmqmqmfs.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2zmkmnons.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2rluvmwpq.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2ojkuwssr.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2gmekvuaf.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2zavaqcxp.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2csvumqut.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2mzpnpnqe.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2zdotccdi.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2wuqmvvpc.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2bvsbgcxl.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2zbsxmnpk.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2othjnodt.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2rwjkvtus.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2nmwquoak.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2lbbhmnzj.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2hhaunrxu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mafxetln.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2chiyglud.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nwduwqkm.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2pcbfglug.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2kepvpdon.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2eyapqjhh.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2eikhhrtv.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2gxhffpeh.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2glzojozm.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2rhuojjzr.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2rwuicvui.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2czlhxmmt.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2mtjypogt.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2lxxlbcdu.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2rwkntzau.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2uaqjvyao.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2vgbvucfb.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2zznskimm.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2jjonaukf.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2ptxpxmkr.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2zhnulpot.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2cyefowvz.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2viyntfks.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2hxhethfw.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2mzsgkhvx.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2qnvsyjhg.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2wzsphukc.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2kpqytwqu.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2clbsvovz.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2ezbyzxen.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2onvpyjua.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2myljvsxl.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2amfzleul.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2mpohopsu.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2zalujwcq.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2ckgtnnoq.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2ymszscdk.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2ahapawhh.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2nchcxfng.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2dxpvlzws.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2warguayp.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2hmecjlhs.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2iuxnwfxu.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2clbuyqzu.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zipdsdkh.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xpnkjclo.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2jzyolmlj.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2fvtootdq.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2mseydynk.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2zacdsdtj.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2cnrciohh.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2bbfaeioo.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2xoxtznua.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2cpnkcwxj.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2qxlwfmbo.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2sqnxrnhr.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2tqeiubkc.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2rsaqibct.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2thwhupts.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2qpeqwpeh.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2fsfefjdu.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2ovckyimo.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2kvydefkk.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2zvwgxqrs.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2hjeuicnv.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2rgrohchx.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2tnbnwigs.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2fiwcbvlo.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2xvnyqrjx.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2cfxratoa.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2ikdjkaiw.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2kfrrzouc.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2kcfwenga.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2qszxrvps.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2jmbzfkip.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2scczhqez.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2mpiedgbn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vecwniii.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2gmlegdog.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2npbzoezq.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2lserssar.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2uqglivzg.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2woddjayd.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2hmnansny.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2vhjglczw.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2mfgibggh.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2hdmrbpkw.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2hacpkikf.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2soagvqnk.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2jitfvhmc.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2ehbmousa.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2ezoocfmw.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2jmraunrm.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2yqriyxln.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2riyfqqyd.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2jbxmxvgt.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2krwexxer.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2cpjibela.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2rgnbtwty.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2cfxjdvfe.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2ulhruepj.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2bjkilrnj.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2auqbgppj.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2akvcejfl.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2mvqyddhv.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2juiuiqnr.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ajohubjf.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2xjhtxacs.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2hplfkcsv.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2xwddqjmo.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2wjyobkag.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2vsthwtms.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2fdqodzvj.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2wajpjpom.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2djwbysrw.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2eaohvyiu.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2evpttubn.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2abfksuhg.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2gllgdcxb.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2zfrteiny.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2tguqmzeb.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2mlohzelm.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2xiuyjmgl.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2hnmexgll.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2eafuvnxe.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2oqrlimar.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2lpyhogeo.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2kxclciwt.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2lugbuqnw.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2vozsuulb.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2mwgdsmah.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2bsxtaxbf.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2cgnifede.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2spuzanqm.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2ucgpiozo.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2irnqamuq.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2ulfjopyz.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2idrrxabv.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2fbnydawy.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2oomuepjr.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2spdjcevt.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2grjfcytg.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2zsonsjqy.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2ricgwwxc.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2mxyreqsd.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2oylpxzmz.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ibeewvmk.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2mdnhzdpz.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2qzvojfyn.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2deramlxo.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2erjnecxs.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2peqbqppo.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2uqxwkkod.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2dxsqagbp.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2dzaupspe.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2syergsys.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2dbceazfi.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2efjbflcw.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2tfvsezsq.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2sxmbyhvc.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2cmzgaoas.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2teigjpwr.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2sjrkznfe.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2bdanxmvu.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2txyctgcd.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2wsojzrgr.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2bpcptqwt.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2gdvjfphi.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2fvzbnaqq.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2aniandas.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2bdpvdles.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2dpgovjra.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2sjehnzft.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2dpsqkecw.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2vuxprurh.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2mqgebajl.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ektxswxc.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2bkftrgkp.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2xqhrcymu.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2emtezwsy.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2biqfcrwq.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2znyffstk.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2gzmgyjna.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2drscdokx.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2tibarlzn.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2voicohwc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vfguvcfc.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2zdwceifa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2onqpdxrz.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2rkxdxocr.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2ndrvhaws.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2nsgcdvui.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2tsyeqkdf.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2fblrohjf.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2crgxoepq.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2pdswanvv.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2tgxwvrge.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2ztecmgcc.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2capuzzez.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2qsuuluke.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2jlajvoqq.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2yyxoahfy.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2clzktwbp.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2xnvmijck.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2tcsonlng.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2utfbmcxa.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2qgzydtdk.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2oflvpotm.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2burrpiqm.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2rgblupgg.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2yqycrgtb.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2afqdwylt.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2kiqgcjbg.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2eeplprmy.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2ccdtnoei.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2ehjlslbx.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2fgabnist.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2pjujujby.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2mjmtprpu.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2aiwzegaw.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2djshvgzl.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2nzyfnfja.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2dzhuzyhd.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2xchhqnda.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bnbupvyx.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2odzbvuis.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2ymrydkmf.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2ksfsfjdn.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2iilahapw.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2abkhpaos.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2ksypaywq.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2kidntmli.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2xomvdtan.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2zvxihtco.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2hmdvuygk.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2kgkehrmf.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2ueixtfeg.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2mvgjbuzy.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2taubbqiw.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2zpdvobln.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2cwpcpdgn.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2nvjjzcei.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2yleyythr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2otzrpfde.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2tduxsbag.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2utcjstvw.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2etashkgo.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2dcdcxswj.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2gemqjzlv.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2txqxehnn.html


<!-- 参考信息 -->