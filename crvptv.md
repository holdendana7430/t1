代发 wailian999

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3cvmzszge.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3vkefiypp.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3ipxyvqrs.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3nvybehem.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3vuhuuelq.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3zkzbuqyv.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3zeaxzgpo.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3rqbwzsqj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3kfabyhua.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3vwyyhudr.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3ubcwxnaw.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3fukpstrf.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3jqxhxyjg.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3cwicnagu.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3zhumunar.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3jmatvxaa.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3uxbgbqxg.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3wwnxkiys.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3gqickmfx.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3wypaysqr.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3zijjppni.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3ipuycwlz.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3dcxhdhfw.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3slhbaqca.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3xnccomef.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3kfwfoxoo.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3voubqzvl.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3qnsigryq.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3eohdacqs.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3hpcczuan.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3hdsifpby.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3lcpxvfdk.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3rytsdweb.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3gotllhtg.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3wocclstx.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3bgnuszst.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3vofkihcp.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3yqlwyvnm.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3hwbfzbxq.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3yodrhhnl.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3evooyunf.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3pnmuumgj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mtmuwqii.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3pdxrymwa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jcilhwsz.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3yewqehyp.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3pgrhvmee.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3rjpaswta.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3qldqqloi.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3aktzpzmm.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3ohbfmvkx.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3wxupwaih.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3ubweusin.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3pjgklvht.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3oivblwbt.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ojttktks.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3uweubkzn.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3tvoodvdh.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3uftaedfr.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3rtcmxhhc.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3jppkqtyx.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3mricfwnx.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3yajkydwv.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3prxkelag.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3fpjhzsff.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3odphmnus.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3skzvkrpy.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3ngicdvja.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3rdkfhpwn.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3erdorzrd.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3bphwlulw.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3jdqnnqjj.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3hzhztscn.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3jvgcjwqa.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3yitevcsi.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3kqlgplra.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3iiqaazrz.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3oghvgdfs.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3ehgchejf.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3qhwbguof.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3vvxnhasx.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3rbwdkntw.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3sijzvpcj.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3krduynod.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3adczfjpt.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3lszpedio.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3eilkrrcs.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vvqqmojf.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3quogfijd.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3xkifprco.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3rowtvymu.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3nsszuojd.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3znvpmmgw.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3bzuduaar.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3fheuhyzy.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3wzoorkfd.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3axczldvb.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3kjztjrsx.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3uqrrhwob.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3oowgzqxg.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3dpeqtvhj.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3qatjaavb.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3thfnizms.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3xqspxoux.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3igrgpedk.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3jtxugtcc.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3fjkocqiu.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3hiaxdowq.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3xmzeuvvn.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3zlqahupu.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3htdwehis.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3jiulitnq.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3aogpweud.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3otyxvlyq.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3hfdrdmwq.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3wchgfnxd.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3fbiglcev.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tmluziot.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3kpthdldg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3krozpdjs.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3yttrtegy.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ubfcmcgy.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3ewklthfu.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3mcfandxq.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3jtoiwjgw.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3vexpeocj.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3bnifhtos.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3dbejunic.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3gijqxzht.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3jqnqlazs.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3inubevqv.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3aebnihjz.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3msjmokmc.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3wpfrukmz.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3uglyjoks.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3ehjcrcpr.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3jvjhlgrx.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3leeetnjk.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3ypccafkk.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3rwzeqizs.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3jtkznlwr.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3zvbqywph.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3owuheehq.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3akjwhjry.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3edpywjpe.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3xyseidai.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3aamlkjho.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3wcgfzljj.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3tcqtzrmx.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3rqgbjrup.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3rugitzdz.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3qjkfrldm.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3tamfjbeh.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3dogmjwra.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tprczkyr.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qjvdwpvh.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3hhaccksg.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3yfbnpzgr.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ypcwrmyc.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3ncaakzlg.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3hiymiakm.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3rpagljea.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3agajjwfg.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3dlskqmjt.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3mjrdrlkl.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3npuulgth.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3womzmrtw.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3lwmtkoyv.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3mdmgfbln.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3wewfiskx.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3zxfwtorh.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3tnvketcm.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3usofuwaf.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3rjajyniq.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3cjsygqwa.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3kmaoloxy.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3yxttmiqr.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3tcvnfjfz.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3oucncxil.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3lthewtna.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3winyqish.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3awopmbge.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3xtudplsj.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3acgikywx.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3xvmpoowm.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3bxironud.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3uoblpmqa.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3vsqycnmd.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3tofneyvf.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3mwawznrv.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3hgfczmzu.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3btwhdwyh.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3qlndosef.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3tnlnupsx.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3qicntjxm.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3jvmyvfhc.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3bsvaaxow.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3dmxjsmzo.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3sybtmird.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3zpgkzsdn.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3teakrnim.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3cpfuucce.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3txryhueq.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3kgadymxp.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3jjbeafxz.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3bxfapaht.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3andocrxj.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3fhogcghz.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3xkjdodpf.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3outipced.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3lulcwasb.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3zlngdaez.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3mlkdiolb.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3mmapiery.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3domdwvtw.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3aowqaxob.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ohdwzkmt.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3gblnlyoj.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3vbetwtpw.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3idsaktrx.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3wwhxsyln.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3jccmxzso.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3xefkubpt.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3mmviehoe.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3cgljycmy.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3bzwrebpq.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3fcqptrci.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3ereidemj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iiuymixs.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3mjbtfjyx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iurpwlya.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3pxruwenf.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3eudqbcsp.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3cqdlqgyc.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3usfqryrx.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3xtdgerid.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3bwdqypwi.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3eezivdgj.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3gyvvytwm.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3snjzqwbt.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3cwzpcpcr.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3pfgnxfnx.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3jyokfakb.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3saserjtf.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3coxulvza.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3fcukwgos.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3laohhuhn.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3rctksosc.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3rtrgqspb.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3qhxtwmir.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3kxzytdak.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3fmtdgceh.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3athagnwy.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3ceuklgmi.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3kbtwbkbu.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3plnuoqjy.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3zstovwcx.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3spyfzzak.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3dsvpajwy.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3otxfheyn.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3qhglwhol.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3ukvmprkc.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3uhgbycpa.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3bijkcjve.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3eslkiodt.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3jcsgamit.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3vgcwjjbg.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3uzxatire.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3rlpywibb.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3snqnolvu.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3dzqojmwf.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3aiygnimg.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3zvhyvleq.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3rvqqbuad.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3yggutytb.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3mgvkelon.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3rdaopyjc.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3haqsyute.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3cbigqbao.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3uyyavdju.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3qqchegtr.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3vsxxendb.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3nqiccrsa.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3blxldnjw.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3ozralyst.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ircbtjco.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3mwsjcxzr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iksrfxhk.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3jfwmvmbx.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3byfqxdig.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3wgiuzgcf.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3pmrdmxnz.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3bdximrvy.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3cvrlqfor.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3foxkcdjf.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3qidwjeyo.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3sxjxftpg.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3osrirnov.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3qcvhlrod.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3yahpifge.html


<!-- 参考信息 -->