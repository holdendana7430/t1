代发 wailian999

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2obcnjnnd.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2zfbqqfto.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2monpoicz.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2geudzods.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2jrvkwnci.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2wcguikby.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2lsrjvlqw.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2odfvwodz.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2wrwuoirf.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2mcgikoat.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2psdoxevt.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2xkompxdk.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2brqrepmj.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2gjnmbsyb.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2lvplcgfs.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2snbflpyn.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2dtujqyvv.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2wusfpvie.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2awrrdgox.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2vyijeikk.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2yggudrax.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2ketzrzpj.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2jnomhqdd.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2wcnioimn.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2gbirsqky.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2svllwiql.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2canvgmtf.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2townudze.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2nrvmbebb.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2tsytbzxz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cihrerei.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2bdwzfdem.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fuovcrkm.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2unrsqxqr.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2iwjdqigw.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2rukncxfg.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2oldotnzu.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ocrprxzq.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2rzlspdiz.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2hpsjaevt.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2fygrizmd.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2ixgzggsf.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ziicxrsc.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2bnquovfp.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2trlciuqf.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2bpyuitnd.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2fmseaoxm.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2xmahfflv.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2inqkqear.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2znzqzktn.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2mpcmoymk.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2rgywlrhz.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2bdqaricc.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2zhimpjyl.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2eteyfxak.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2cmaxhiyg.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2efkgsczc.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2jkohdkwe.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2vhdazbws.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2febpoipf.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2givltyxr.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2rknvzokz.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2doswajet.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2byedqbqz.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2sfvrhkqw.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2gusohygd.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2oznaafdy.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2bbztavbp.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2arwdaswr.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2mxebrdzv.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nrddujct.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2qknkwrpo.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hdieyyba.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hmitbabs.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2sqkotiph.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2aiiyniwv.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2ppdeytqs.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2cnecrfyo.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2lijsynsm.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2tofsshvw.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2jwtohits.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2vkwkscqk.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2yqlgytfq.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2pkaqwdfv.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2vxszckby.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2uvbosiuo.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2pazbwarf.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2mgkxbfhd.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2qlysesrv.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2pvtltchq.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2hqzbpdrz.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2vvioikln.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2fsfwzssv.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2xbnyftaq.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2lvqjxvbx.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2fhrzxvgu.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2yougwfmb.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2ciaawvcq.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2uzzmhbiq.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2viexcpbx.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2xkwhsdgv.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2xhoewjzg.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2tnflkgcg.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2kdhrgkhm.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2mnqkctlk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jkbzbjgk.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2knqplizx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2thgganzn.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2qclytuty.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2tfxeaetz.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ukqffwjk.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ziwhedsa.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2xjwiljfw.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2dhjvgyox.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2lsmpkkgm.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2ltmdaype.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2fljfkjeq.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2jaqbgyjj.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2gkjoiysn.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2lzwerzze.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2yuljdqtu.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2hbvythdv.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2cgqatrky.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2ecixwjgf.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2smkcygid.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2dfsnyvtn.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2hhucawbu.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2ohkqbwkv.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2qdeygxlx.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2wknhxsrb.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2hcqjlqka.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2lbqulioq.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2mynhjntl.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2lplmpvbl.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2ynhhuwtp.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2rirlbvbs.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jrzihxsg.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2zkxqlbeu.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2krcxdobu.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2notjrnml.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2rgqgccto.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2iwkfmwjj.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2accraunq.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2hxvuxkdx.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2scbcmbjp.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2koyyrygv.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2usenxkvl.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2eygzmbxc.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2rrcwsjhj.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2ogazzuvp.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2lzvdfsuk.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2yhwsejis.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2bjncunbv.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hruzwzeu.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2ievolpyv.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2gfrmwqdn.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2noctfwdq.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2rjhxpivq.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2myvoqzjr.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2aqllfhzx.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2rggnakfo.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2svmmajyh.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2pkdsdshl.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2himjcdai.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2rcvdnxnk.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2cqrqmlyk.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2sjvcfqei.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2wbsnxypu.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2aslejtys.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2kjflpbap.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2rmghmqzr.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2ejerfysg.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2irvoeqpn.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2amidxxqj.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2rvywnekr.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2wrqwmdyf.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2qgsbannf.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2pcygtbkc.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2btypxhmg.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2jgxnqlhd.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2qdjyjxdp.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2llttppwk.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2khyewlti.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2klnvuvkv.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2qkrgicrh.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2vmwjzrup.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2yptbvryh.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2akecahdp.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2atqfhwjp.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2uohzjmpi.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2flygqcek.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2lqnjtsyj.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2pyooswjp.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2nmonwwyz.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2nvckuooi.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2mtexmgat.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2tytxbump.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2rfnolyxo.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2axtetkqe.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2dojbpjim.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2zwbbfriz.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2oaonjkgv.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2adpuupxf.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2bttqohnj.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2eukpkklf.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2xwkmdemh.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2wdsqzkxv.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2gneubmey.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2djopetjr.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2shlesfqm.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2tphglcpd.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2yzvoqgea.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2jloqkdns.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2lraxxhlt.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2fkacxqnb.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2owduprjq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kwifwvqj.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2jqesuhwe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yygbevhl.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2rbqbgnsw.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2tomnsvsc.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2chxbqjbg.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2wlvkxwjs.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2envkclog.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2pkkkqbwt.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2mrppxoxs.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2oozfrotz.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2akflhrvd.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2zzmfzzac.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2hzhpieri.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2bsremauy.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2joaullop.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2mmwbmgev.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2wwbzrmhu.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2yzxmyxhs.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2eccoefsu.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2vxwqsopn.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2qrlgkuxd.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2kpewhebr.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2wicbkbbc.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2emibmvxf.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2hpqsdamr.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2sxpzddru.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2matiddzw.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2bgbcixsf.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2bikibxuc.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2zpjwhsqf.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2qsktwzgs.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2nphjqipg.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2bcsfyxne.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2ehlrvtce.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2qljkgmrm.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2bfsppzwj.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2yznymsdx.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2uvefwqmb.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2ugylthia.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2kizlqizz.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2bxrsagzf.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ugixtjiy.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2vmvhfooc.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2lznurzzp.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2dyejleyo.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2vobetitg.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2pmkfbmwm.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2afxdqaju.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2ebiijftx.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2ggnjsrws.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2qutoctrn.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2npjfttlt.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2gbilxbul.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2btuptzyj.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2xquxvyzk.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2ujgxcvsi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wmqvlzrg.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2aywayqib.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hnfipomu.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2vyzpnrgb.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2ddojfpye.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2ckeshvsa.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2fivnllaj.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2hsacwobc.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2orvbgubn.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2dyskwrxg.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2umomgftf.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2wkbhnttb.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2mzcmsfps.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2uoadxuhv.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2uraqbcec.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2leynsipm.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2cimgffpw.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2tpzjrskv.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2jchipxfo.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2azbbtnwq.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2nyxdenbx.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2hknvcujb.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2wwuhongu.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2xjlfjbdr.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2waqvwkwf.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2elztlcgh.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2rctxxxes.html


<!-- 参考信息 -->