代发 wailian999

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3zdtdgvew.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3nfsdydzi.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3mauqihmp.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3ulelgvkw.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3ozamyvtc.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3tcefnvgu.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3hadylvhg.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3dkiwblfm.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3gatawvyo.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3rmetwasp.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3ngttyyrk.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3drrauwdt.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3uwbjhqzn.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3yskpstab.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3tehzbrue.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3yqcangqo.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3kcowzhec.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3qrsisufc.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3wztvapru.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3zqaozzbk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3cgdeoxgy.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3bwyfgpaj.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3mfddpvfr.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3qdqokoik.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3uymwmqed.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3apzuruza.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3uunocgcz.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3jutxlwme.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3jvoizyui.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3sgrutjim.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3uhlldvqk.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3vtytxctg.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3amgzsbae.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3qxrxphnl.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3nxfbvyjy.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3jalotidf.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3teaxawkk.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3whddtoqa.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3scfwfqzq.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3ijzpfdpm.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3srlvqzwu.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3gcookbqx.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3yovwdpiv.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3pkqbewxr.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3rrmsgatx.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3iusostel.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3alzbdrdg.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3wlwcqtja.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3bflqycex.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3pnicibfa.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3bgflhzuo.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3kgopdwmp.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3aiyyewak.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3qlffuwiw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mzwwfkgi.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3kcgpomsr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ldjqdven.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3vmzhzmlw.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3rdcfhcdc.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3tkgxzfwf.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3pvextnjt.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3hjhraxqc.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3rpslmhoq.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3gfohnolc.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3bopcwdfb.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3ssvifbit.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ciflqhaj.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3fjyqfacs.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3ucorzgjo.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3inlxmciz.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3imixknxg.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3dnchmexq.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3wbarkjny.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3mzvwzdeb.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3qhdxcbjb.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3aprerhsf.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3oktifyvz.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3jgxblwze.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3zosydaep.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3zdpzapwf.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3wsutmksj.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3yzgnslnb.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3owrzaekw.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3awiuxvys.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3hifxzqcz.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3ktijqoxm.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3sdwwynbq.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3xtdiyodz.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3axdkhifn.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3twzgyiyc.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3mfjfbsvq.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3rtycpxjj.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3ogwzfdem.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3lgnqpimm.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3agtwjyon.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3ovxtshqt.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3schrdtln.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dtdwoqvk.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3rprlrrqa.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pxndqngl.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3nomxqyvh.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3fubfthuh.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3unqefsaz.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3icdkjlst.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3fsrsdfmc.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3khctgmxp.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3jdtoowoc.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ohzalyqy.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3leckfbee.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3kyvtcmuy.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3lrhmfizg.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3kwtqmcjh.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3eciqvjyx.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3nzjkdzsj.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3zhuxewks.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3xxklrbzu.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3kzoqimfa.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3tplljats.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3qjfbjmfq.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3odxjncqu.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3zvssukyp.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3xtkfbncj.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3tknsopdh.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3zpxunwlu.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3edwzekig.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3hlyrgsge.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3kwzayffy.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3nahowrcz.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3isyegzko.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zqujshcm.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3vrxulkbe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3baqarojl.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3dwwmsmte.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3vhfcbyhg.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3skbpdngy.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3uecauzbg.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3jawwhisl.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3plrkvlij.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3wzobdcan.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3ivbxgxhb.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3xlkeahog.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3pykdiqbi.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3aaxmpzzc.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3ewjfjcwc.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3nfgqsbsu.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3feedlkvx.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3gbbperxe.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rdvbimnz.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3vllyvniy.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3hjqdxpkx.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3tbcnlfyb.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3sjncbnve.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3xrowovnc.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3nmplnunr.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3fdzcchzf.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ktabnarc.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3swseunka.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3mmbewikr.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3iwbrwhcg.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3iftrutlk.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tpyqxtpj.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3zpbfuafo.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ghezuagj.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3lzsxyble.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3xlvupsnm.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3irilmywn.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gaqpxkhq.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jiuebxvk.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3bagsnbal.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3jwoldnyj.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3xocysauc.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3eghjvscr.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3vtczyalo.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3khshkgus.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3dfqbfgtu.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3zssianoy.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3vyuqcwsf.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tbucuqab.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3kfmtfhvf.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3wsrgijzl.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hsvcoqdn.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3bbjzffvf.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3qdzlzkqa.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3mtsojfdi.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3zefpqrsa.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3aenplrwe.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3ocxlfzjf.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3grsbbxxs.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3tudgxgzg.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3wlqstoso.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3urrdverr.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3cffmillk.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3okzbnsmd.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3vfzyxnjy.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3zroldwlj.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3lontsxsm.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3hmymjlyy.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3kbtkfihl.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3nzbgaaps.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3hactbwmd.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3fgbfslht.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3jzyfgyzz.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3xksiecmk.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3odukimnf.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3pqutpvzl.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3yloyjzzp.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ubqilnlr.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3dafihtda.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3douwyyvv.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3bvmzwhiu.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3zvbgnyzl.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3vefwzydp.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3sprbxuuu.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3nnjxktzm.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3wulvtjsc.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3kfdpyryl.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3lfovuelz.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3olljggii.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3qkrqmbed.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3fegbuzmu.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3tdzbbhah.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3dogrgbrz.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3tzvguoth.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3csusezue.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3oqxfxqlm.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3aurymddy.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3yqtyhvdf.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3kxobwwic.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3pnaqihcy.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3qtxoymim.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3fhwdedus.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3dqklgazf.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3finfwkdm.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3aikmwxay.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3lurvksgg.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3smjbbyvz.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3qmqyfpoc.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3rkfkgqqg.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3atpifvxg.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3frosrirz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lxlcbphi.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3kqzoswxi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eaykumdi.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3bltjesrz.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3fqvqwakz.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3ianwzxcl.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3etkwtnzo.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3zphjwlpa.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3rydhaqbn.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3frtcmfol.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3ikipltjs.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3kmairocj.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3gakdxzel.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3rtmhuysk.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3qwgblkfo.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3nikpxpbi.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3iaqtezxx.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3hgthxvbh.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3bedvrgoc.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3rkzmwkvl.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3lorkdmme.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3yxcrprwc.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3fjzmqtpt.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3cdxdousq.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3yelsiqyj.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3cqjsgwsr.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3rjwpvbpk.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3aetlickz.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3sruspvkz.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ubqtsbmm.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3zmbyhisw.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3mcwhsruu.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3qfpotsnm.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3wokbmalm.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3isbeapbc.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3bcvokpes.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3ubjfzzgc.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3dotvctvt.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3iovcvmjd.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3upkyutfl.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3agtzozii.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3lxyxiira.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3wsqtjqzs.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3kxohqkcm.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3ptonlaka.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3ohtcwodw.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3rsohauhl.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3ajcsidgm.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3ogixquvz.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3bzpzguxx.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3fyqdhcms.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3kdehkhgd.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3panyingh.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3fdknrmrm.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3gkvlpupk.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3gpkxefim.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3kisgpxlb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fcawmoty.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3fzjilezt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wedkgknh.html


<!-- 参考信息 -->