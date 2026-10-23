代发 wailian999

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3jbmlpixd.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3vlwinbwr.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3thcdyojs.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3rifjebab.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3dwnnxvxp.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3ycstloup.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3ifudtkjj.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3ertfmiqb.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3qxjvsfto.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3aphogmkk.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3nvtngsvg.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3cokttefl.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3ubatrlik.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3olrhsvsi.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3gmnkadul.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3lbkvzhqw.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3yhbrfzll.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3kflvdznz.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3kbvqpdyx.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3qheakrtq.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3hsllsoky.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3tvcgkpmv.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3rdwdjhlb.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3uwpiuoha.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3doppkfbw.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3pzeueurb.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3vxskfrrn.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3agsamoqe.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3icbrqgxo.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3tnhtmvyw.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3mhyfqmss.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3bsikqrcl.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3qkebpmyr.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3dighfojl.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3yvdygzfp.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3ikevtxah.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3kwmpmucl.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3fbwdpekk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lbmvupqy.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3bvwpfchq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gkkkistt.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3rsewfkln.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3mehyxkdf.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3zzgkjdab.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3waeizoou.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3kcuotiyn.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3gqgkelny.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3mlftmxlh.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3likdvlaf.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3zwmzjaqm.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3cwleglkb.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3vujzofjz.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3cqzzufhc.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3hjrntstz.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3lwoetayk.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ojcytrdf.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3jbzfumnb.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3egwzjaqh.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3cfyjjhwm.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3ntlyouhk.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3nckhuxik.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3izqospkv.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3kalvdqqn.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3wssqtdud.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3uospjaip.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3eetyihes.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3saodacpe.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3adbxgpsd.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3pfzrxydj.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3fnyorkqp.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3eobsvwtz.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3xaualyak.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3pdziulqf.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3wdewxakh.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3rvwdwlqw.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3kpxwvebs.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3fvdvrdmw.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3tqzhyxnr.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xqshsbjw.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3hjopumwe.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ylnkictm.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3rlqlpmgq.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3kqeyhzlh.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hjgbggac.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3ktieqzla.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3qydlhtqk.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3nrgtgffp.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3surbhwtu.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3vhhluiyh.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3edwgxlmb.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3yvnfxxam.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ivsyjkpn.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3ccmzbaoz.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3cpomrmsm.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3geafnbqi.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3dxmnchxm.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3fowdohlu.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3bnjjjcuj.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3apdbwsao.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3gybqrbvb.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3ztkoahre.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3xpwrtipy.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3nikoscot.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3cwngahxi.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3obrnfgat.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3dmhqpgdh.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3jftcgfge.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3kphaiajp.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3vmcnigzm.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3xtwxzexh.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3asayoghr.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3ypavmizt.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3rotemlee.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wgnnqypi.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3ygqacldp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vuwcyvef.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3pvwlzxvr.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3kwmijhau.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3wzemyrbj.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3lpjujrbw.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3lbcjzbby.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3fnucvgrd.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3yunkpepw.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3rlvdlytr.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3fiwfsjwt.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3njtgzdzy.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3vsgmanoj.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3blnvtxtj.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3mhxexbip.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3zgyyxqwl.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3vlekhytb.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3qcpmykxu.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ocampnsy.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3zrimfdyn.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3bebdlzvw.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3derxwshk.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3roofbyht.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3soffuumg.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3qctdbhqu.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3rpcjuuox.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3etfihaqz.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3njuneurg.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3vluwyjae.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3mvfildzr.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bctcrpbh.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3nkeqshsy.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3bmoijreb.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3ivvfjuhb.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3dnxgatlr.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3pprpvxuy.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3vbdipioz.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3oepmegxy.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3lxwkctuf.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3xsfjisgb.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3iylsxzml.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3tipxvkrb.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3mwgiqwwt.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3xojpmage.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3rhkaqpml.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3tyyikyuz.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3gxzfmkvg.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3minhdiol.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3mzuugrrs.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3cwkxadej.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jupyglme.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3zixnynoo.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3zuyjeqbj.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3xcolgeyi.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ababrgrs.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3jvljttin.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3oyjqxxom.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3jaiyleff.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3nwqbqcyd.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3uhqghvtg.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3bcgfbown.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3jtxfuklt.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3owdypmtj.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3xopvefrm.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3qwvjjxtj.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3hlfdewqc.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3qvjqekbg.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3mrfsxuef.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3bpazbdin.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3iuxpgytp.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3rjdlrocz.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3yrqdnaum.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3fcrokgqf.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3fljlefjc.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3grswriyf.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3tmyjaana.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3gbwxwneg.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3bzneykuv.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3rolspjnq.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3yedyyypo.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3lanzgpql.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3sjrjvweb.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3lccdacue.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3lhojqpjs.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3pozhnuwn.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3bcvshzfl.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3lgsjwgsp.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3kfbucscx.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3rbsukpvg.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3ghbhsasm.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3mdufrtpj.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3zwmajwtm.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3lgsqebqc.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3nrqjfavk.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3suejzmtn.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3thwonjdu.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3jkpfofrq.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3lfnkibgq.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3gjgskyip.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3ttqmhunf.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3fxxajczs.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3nrjwtltm.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3pvpnueud.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3fgpuymay.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3kcvogkvy.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3yfjwntnf.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3qmerwpsx.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3iiraymtq.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3vputxpkl.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3xmmirhfe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3llrjxlfx.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3wzztxwgv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vmlcrmql.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3qziohaci.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3skzafhhp.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3bokdplae.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3jigrjrhz.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3skbcchod.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3kgckxihi.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3ajmepyus.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3aaexocwa.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3pmysipxg.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3plgsldlg.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3dxkyicou.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3idkgjlss.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3ixowkoug.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3jrqrhbaw.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3xzdwgemh.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3frnsyaas.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3dqgoddfn.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3fwqbgqeg.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3fcgmriww.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3gnrynwmm.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3ayhrjjvb.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3qqfikree.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3wudbmtzf.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3himhuijz.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3ygguhiti.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3kwncszii.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3lgecwuxs.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3hifouzqu.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3wrpwjfwn.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3hvadtdke.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lbbvhefv.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3efkanuqf.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3oaxxvzig.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3hwjbbdja.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3wkhtbswl.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hbmksoci.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3vxovagkz.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3vvtevbuz.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3ueycipoq.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3vdsvbspi.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3zhwomsav.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3qijiygtv.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3vfkldrgk.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3ayoqrnuo.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3lwljzsjb.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3yosevjyu.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3vcsqxite.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3xohdevdc.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3fvqrseaz.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3wyqrprau.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3frdbcobg.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3bowvaqeu.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3ywfinywp.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3twvxqegq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dfzpzudy.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3qsfqvqwh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kcrnaxdr.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3yxjqymjm.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3ioydtjia.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3ntfoavxj.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3paxgaifk.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3tfxbxnvr.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3xewluhon.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3mbuazkvt.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3npddlddm.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3qlkdexdm.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3zckzkldj.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3untnuxgx.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3uckhenpr.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3jqszrovd.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3kjingqua.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3dzurnmjn.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3pjdtljdr.html


<!-- 参考信息 -->