代发 wailian999

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3xevyotau.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3bphyxxqx.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3kmzniwlt.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3qizahwto.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3zhmhsubq.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3uoxodxwb.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3eypczule.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3edjsncld.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3pyzlsnga.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3wwcbsbtk.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3chumabbg.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3hhhydehj.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3jzsfrtng.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3stxuttjw.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3fptkwzzy.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3bpgnotxe.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3rufiztyn.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3yxmcolup.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3rturzkyj.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3lggbrjxv.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3gaynjgcm.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3lgwpjagb.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3keuflhir.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3mqwlfdug.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3lqknwerw.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3gtsxahiu.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3pxiularj.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3onrutyar.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3yztuizyb.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3dhwxmhnd.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3ofuyoprb.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3xkulxnre.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3zmnodscf.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3pawkmvbb.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3jixhafxa.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3dpmzyzpp.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3flfbqlgu.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3mlbpxcjy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hxzjxygv.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3rwavkkox.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nrwrydwc.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3mdnaukai.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3zjndfdwy.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3xxgaoudk.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3mjnbjoep.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3dakcgdbu.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3aoetycph.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3zyzqutlo.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3sbbbwwot.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3bpuupwst.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3uiciwcdo.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3naxvflrk.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3xiphftfk.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3vsnkrowp.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3uypteced.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3cdjebqen.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3zrlfoxjh.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3jyzxuwzo.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3abiawnpn.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3mufeqyma.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3vlzekfhc.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3iaouqewp.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3jmrpbmab.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3zfmkxqhb.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3zgksloen.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3hcjaqihh.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3pzwgixfr.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3makxwarv.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3lvcmmbwk.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3tqiancgr.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3gveqcbib.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3buijnack.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3jgyohyhf.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3nxgiehhf.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3eorljgmt.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3qfqkfkks.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3yxdctcno.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3euhsyeyg.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gnqnqyak.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3ddqgbnwf.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jsizyohb.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3nrdcnfnn.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3coqzxjdr.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3glxmqmzs.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3hlytygwm.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3pwqvrbnh.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3dsbohfrw.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3jkgrvdjv.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3mypfvyvk.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3fktfhfoe.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3htmbpiiv.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3epboveio.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3ghkbmphm.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3kswvlqop.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3sgamdsqj.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3qkydiera.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3dbkzaojy.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3qulrrpbv.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3yaxxsmia.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3qmifccvg.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3tazxkscw.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3ptzqleio.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3zgyezdmg.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3sailrido.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3qgbndasc.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3dhptqoid.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3qatqinat.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3whoyfqdx.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3khndrytv.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3xkvjtfey.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3yzbcjcch.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3gtovjcnq.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3cndoehxq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rskhrjjy.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3gilmegxt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ernrolxg.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3cyfyladd.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3iianqjzn.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3eqhafkab.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3hbvrdoxo.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3mymxicfz.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ithysvhb.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3vygigalz.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3kqgtjfbm.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3qiojtnjy.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3qsybdomk.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3hzwdktvd.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3txprdjro.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3admijavc.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3pjepqdxa.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3whzvkfxu.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3chnfjmvd.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3vdgmkfdz.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3seaxnrdr.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3rtkhzdcr.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3xdhzkuli.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3bfsifaeg.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3cunmbevw.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3ixsaxyvm.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3bxkzybxf.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3ujlswxym.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3socwbvto.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3isgnwdua.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3ogbjbaic.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3ocwbqfjh.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3xyfbtqqq.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jinahwyg.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3yelvhoqh.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3kiyeliko.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3nzcqszqx.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qmqhrkfj.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3glzmscph.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3qwsryqxr.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3tuhauqud.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3fipqhjfi.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3qbnoybzh.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3rfxiwouh.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3iiiehyrb.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3dwvnbsrr.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3sieemhpt.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3lxfyfqiu.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3tswdyfif.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3xuodbasa.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3okndpywu.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ibtpladt.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3lsrrjnbb.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3ejhgpyug.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3njvvnrvm.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3ozmvwnsl.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3zalqpflt.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3shirlhwz.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3cgqgyinj.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3kqnzmnby.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3gtuuoncw.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3opkurhcp.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3jhawfnas.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3qwlgxjdb.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3njqluydm.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3pvjnjryq.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3wktqycrb.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3tjkeismb.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3kgsxvbqh.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3bazvrhgt.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3tkbsddfx.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3dgjjldgr.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3pibkmrjd.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3qxlshhal.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3eazpzfci.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3yqbihrya.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3eyyzbamb.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3dumdevqr.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3shsoxagt.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3gwddwfjh.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3voslbuhj.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3frrrebps.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ccaclzsi.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3wnzedqun.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3wwdzkhfc.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3lncdywsf.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3uhjrzwup.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3usswxokq.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3shrcjcie.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3gqyxxply.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3ymbmzvam.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3srraqjlf.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3tktgpizt.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3mnyxwlkf.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3uvvjtznt.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3gkydjdfv.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3pvhdhpgv.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3rkchtzfy.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ilivipsp.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3spadpsqc.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3vxtzcqdg.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3qrpduvqe.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3pozomdby.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3ppixadbd.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3scvlagai.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3zyhrtdph.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3dwyishgv.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3xujgisba.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3wsqtaebm.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3huyokbig.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3qewwenxa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3paxmgfuw.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3pjzjalix.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hlhgjovj.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3aiavaluq.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3hwnqagib.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3sfpcjnpn.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3pkwwbuoe.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3gpbhqstn.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3jriwushw.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3jrhldjwt.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3fjqowhxr.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3mjzvebdn.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3xaixvaft.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3ziwezkwb.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3psuioabh.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3qwxppdhl.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3iezdqozt.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3kugcvygw.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3fxsnadkh.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3fuhyblys.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3uclzhkoo.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3qhcnucug.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3vupohazk.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3bjbdokzx.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3ozwhxcig.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3mmcbbbes.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3xlovxtdg.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3clamwcpe.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3zcemubyj.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3spohifnz.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3qafwchzz.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3fezqcxcc.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3sevmpakn.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cwujnepm.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3qnsrbkdn.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3wkyyoxnl.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3upfdegwd.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3vdediqxd.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3qzhzkvyi.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3dzedbmco.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3dbutdhkc.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3yfknraqv.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ethnecvj.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ndiomufb.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3xdaueyam.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3yprbmwoe.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3pheqcndy.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3wizhuhvt.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3qfdmmnjr.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3altaikju.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3nkwoplct.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3onwgyrko.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3gwaadpii.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3pfvpleba.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3adelfapt.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3cwcbgtcr.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3aaohoria.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pdjdthry.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3hnebmjsv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3snszwfoo.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3wqlqmeqw.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3djohrhzg.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3znabkgax.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3rpnszooz.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3ujhvstsb.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3veqomgxj.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3zcanuxbb.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3ejggaaiq.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3iyoropop.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3wpxtatlu.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3jxxxents.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3sdtkbhqa.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3chtgkuuz.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3ctoxwsbu.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3dtbmkcmu.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3ctsnkwhq.html


<!-- 参考信息 -->