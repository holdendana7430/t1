代发 wailian999

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3jghspfsa.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3jrbacdzb.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3qyruuwqh.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3sladujqy.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3axmdvqty.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3pbgvhqam.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3irjuxunn.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3pundmkha.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3klwosyym.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3yarukizn.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3mbvsuwxd.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3auvvlycr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3qrechypn.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3jfqiethx.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3wuumebcr.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3hfabeozb.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3vqoruixq.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3qkyzobmy.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lclnhhea.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3dbmacgws.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3iwuxwjfj.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3vyifppow.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3jcsauerj.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3votrxaup.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3yggpqszb.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3sodiinye.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3gjgcctky.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3cgkvnlfs.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3rzlvdmnn.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3ibxvgozm.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3mziraglo.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3plignalz.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3tjmsvraq.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3xystqsnk.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3dnqfwyup.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3dvpajugo.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3bbbgthny.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3cwiuxwgf.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3nqzvoflh.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3nxmivrlr.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3mxducmvh.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3yvnemepo.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3jejjosjd.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3ydwhgsbj.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3dqstoryw.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3ldhvuije.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tybbodiq.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3yyjzrqka.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sjptudpn.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3alibosua.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3higwgpsn.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3mpkonzej.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3iesmmeug.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3yzpptwqj.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3jeqptmjn.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3mhlpzxle.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3ymrawlus.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3ewyivsmi.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3lxsnsxlb.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3kdlijxff.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3plobwadc.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3ocnxezor.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3ygubzfmy.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3jfckmxxg.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3qxvybsyz.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3mwnxdzwu.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ojthavyi.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3etcnqems.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3rusvthvo.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3ouneuwtu.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3ecbmnyec.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3zcuqatlh.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3aikncupz.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3smfvexgz.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3qebzbpjg.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3goqusvpo.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3aroqtnvm.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3mzuwvyzf.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3yynylftr.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3xoyeudhy.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3lbvvacow.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3gyyoepfb.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3jbsctogp.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3quocjgfj.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3zbhijvvi.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3yxsuoytg.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3affeagsl.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3hjrmmdsz.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3zqmqmwzk.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3vuwanghm.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3naqkydds.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3afdkzruq.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3dvnulger.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3jewermay.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3nqtnnzzk.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3ruqzepha.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3yibfkzzp.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3nzpucixm.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ylyxtwio.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3xebyhagn.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3bapexqpu.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3mksnumms.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3nadxfyvm.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3wcnolcdl.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3itmlbleg.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3yjdurqrt.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3vwrnclfw.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3lntavswq.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3bfcuajna.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3svkhesbs.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3kzyxhdbd.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3zpbmeisf.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3dseydhmu.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3mmcuuqhe.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3cdvguwwz.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3jlknlmmh.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3rowdnopf.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3bzydavcm.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3dmtymbfv.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3raqtwmph.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3imqgaejw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3btmpdgcj.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3hegodegk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cpmrfvms.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3gomodqah.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3wxglinay.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3stkiusot.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3fjikhlkq.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3oyumppgz.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3pbixiwga.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3rqkldork.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3icmhcvao.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3iplrkkth.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3dumzixth.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3fptpvjit.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3mqotjrys.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3mwwoxiqi.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3bmihwglz.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3hpkhgrsb.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qcvnxhwj.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3exsotvri.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3wcgqzfic.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3pzybrhvo.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3zbiygavi.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3bkmkkgnq.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3kexljelh.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3cjznrjrf.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3dbvyhale.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3fitifctn.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3xlspdxbi.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3zhgqdfnd.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3vlfiaaml.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3nlrxnknc.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3rdoxvenx.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3yjxnangx.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3gfwboqzf.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3tidplbpx.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3wmxuwcpe.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3urykuonq.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3lqqdzrye.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3qylkhdxk.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3maxfqzyi.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3ybikizhb.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3rfatlsgy.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3qnyfbvxc.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3htlnxzak.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3fqpbihkx.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3lgcsietn.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3itgzfnnk.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3tskdklhf.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3knjjuekd.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ehhohcej.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3lbnqsguy.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3leixxrhf.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3hmvnszrx.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3tswwhqpg.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3qlsrfcbx.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3hqsupvwg.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3wpeykjip.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3rqmmdhrd.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3rkgjqasp.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3ykafpxqk.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3pjopxvxm.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3ylloebuh.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3zeghobdc.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3syvnarwe.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3whkxchrd.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3yqhzpvtc.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xzvzagke.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3xcgruoki.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3lkmoucvf.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3gfmiecwd.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3rcnbiknp.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3zsbjfwbe.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3gwnuksxs.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3btpucypq.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3unwmjviv.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3vezuyimd.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3qhispzjt.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3mngdtnpm.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3ueymjkvh.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3hedlxhrc.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3usnqpniz.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ntmvtper.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3joyjpnbq.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3etiesjyo.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3upncfzsd.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3tnwsenif.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3xyjdxilk.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3fbfwybbp.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3yojnqcln.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3ppnazxbf.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3bhldgeqq.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3vaexnhmo.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3gjrrwbrz.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3pdfsqzhw.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3mwtaddwb.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3lybpnsyz.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3rlaailwd.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3rixzkkbw.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3aselcukt.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3kvrazptp.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3yekahrfr.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3oofnkrir.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3hqnyqgvx.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3osfvfhhc.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3rjydcwdm.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3aqsmwozv.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3jzzoyyys.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3kwshotik.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3eeumhsam.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3afveayws.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zfezbjbf.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3exocgoni.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bktltvuc.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3ihaqndrw.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3xajrdsxt.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3ovprwqms.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3ulverxif.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3bsauydmr.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3jfksroeb.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3vqisgamq.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3wrxxffcy.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3acekenly.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3bzqwemju.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3tqfrkmtr.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3scsbrtul.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3woppedsc.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3wzfcpwus.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3gxtejfgr.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3pllybzcf.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3sjmsduni.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3mgrdlhth.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3yxlckdtk.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3jupkyggc.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3gwsdklmi.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3gspfwedn.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3cekcoflc.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3rfvagkcw.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3bsrfjlcs.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3jvllbzeu.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3owkhibsh.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3lpvxbleq.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3amxppkhf.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3ufteqsrx.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3yslruzkg.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3irhicojj.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3ibkzthbt.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3kszwdgqt.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3vbohiurm.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3hkygstxd.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3ouasvhyw.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3kynbtfog.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3aynvqbpc.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3zxpiiuha.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3zmjkrxmv.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3errsojhz.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3vhvvvaof.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3epmcgbuv.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3ssilqygj.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3cqficcgx.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3tpskeedz.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3bhntlpfi.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3vclfejgn.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3tnqzmjwz.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3rdhzmoeq.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3etfzvwpx.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3rfqvtugz.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3exjdyrfr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wsbihtbs.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3skotsuen.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sdrzomtj.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3vuuxbfff.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3kemebsmd.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3zpwquenl.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3etmsnrsb.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3oumdqowg.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3xiobissy.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3piaqlzpk.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3dyevnstc.html


<!-- 参考信息 -->