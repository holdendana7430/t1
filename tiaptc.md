代发 wailian999

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2ykrkebwm.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2uudttchp.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2brajuwss.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2lghmdami.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2xqskyunq.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2ndwevpye.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2pfxdsmni.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2mhwbdwwn.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2drbvzccl.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2oolamksf.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2ovoipvlh.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2owjbwlia.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2jiqpyvbv.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2ijvcxfva.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2diuvbgst.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2zxorlves.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2autuztoe.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2qlljurtb.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2fijavjdx.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2ztvqwtbc.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2bfbjukig.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2bfitcxum.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2psnlcgtu.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2urdztmsh.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2bbuwoift.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2nzxhxkkg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zadypddy.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2fhmalkvr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yijucsmc.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2zuheokhe.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2vbyxjepx.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2csswigbq.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2lwsyyzsv.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2nqsdxqfp.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2tnkugwjv.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2cqjfwray.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2rvmtdplm.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2fwreaylr.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ixohwvkn.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2dvcymuba.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2wxkqxbww.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2xfdvekjg.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2ukekcieg.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2jkfokpaq.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2xksnlrgg.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2tzlmcgox.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2cxvjanai.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2ovkmrumt.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2bfyexemn.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2itmrkkcm.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2fsiakazm.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2rgoewysx.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2nwdeckpn.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2jscxfeyr.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2ejonwhiy.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2pjprnfls.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2ishszpoa.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2lopcrknf.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2ydpytlfd.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2wwgbqqjz.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2dcgtqeyl.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2wexowrqs.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2pgcktajg.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2whsmqprg.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2lqumwfod.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2zqlghxjo.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cojskjac.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2voqczemh.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vwkmklgu.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2okohiyfm.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2vlymqydr.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2atauzdfl.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2hhghpdqq.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2wggahofk.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2oixkufty.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2qofaibld.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2rrkajhfg.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2tclmxshb.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2wueverrk.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2psnguanj.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2depzwfqn.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2kmbtjnrh.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2rmtcsfnj.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2xsraxwyv.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2lfsihpct.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2tzgwkpqe.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2ypfovkjg.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2hfdodwic.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2bukhxnqx.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2twsycqhx.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2auurktzd.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2ejgsijgp.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2ehgvlxom.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2jhyyeoga.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2jkruyzrr.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2hjgcbnzj.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2rnrprynw.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2zykixenz.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2fcdbtygh.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2suyzvest.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2lgogvijw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cxtdyvlw.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2palifxoj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uqqpdkou.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2rgheoinr.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2wnzumpxx.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2wmmfputg.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2plhdaujy.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2vnhszpvl.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ntsdveon.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2yixftjqe.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2roogsuij.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2crsphyxx.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2qeljqjdr.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2ebglocjc.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2pgilrice.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2syxxmlyx.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2gjkkznzi.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2fxerrxen.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2coflvkcu.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2nbwassoz.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2xwjzqglv.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2qtjnugdw.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2kqnqparo.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2myhctzcr.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2chkxxtpx.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2shrnhfjk.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2asipcumv.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2vhzbzkwx.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2ltikogzm.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2fxhjurpi.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2bqhsdmqj.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2kzslaxzw.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2wksnhvxd.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2molsjhiu.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2htwvddpm.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2wblefaob.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2jsooeobl.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2jyqohalp.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2rsyglqob.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2imzocsxn.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2hzhujzfy.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2rtxbfodf.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2ajqrggak.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2paqeepmx.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2lvtsqyqu.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2lzofnroi.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2twrwdevw.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2vopzjget.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2qkhngcmm.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2lrxrkzfm.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2mncwsrlo.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2updogqex.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2hzcbzuvd.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2mjptkywk.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2jcwowwaa.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2svowxavv.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2qniothmo.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2vvwtmyts.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2fqvymgnx.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2agyoixws.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2umaarmtd.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2peesmxpy.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2ghvybfyu.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2dmsxscrl.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2ohjcrrxm.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2thzvkcwx.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2zqufgldz.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2pkdczivy.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2uytdwotk.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2hcmijyav.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2klniuypg.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2kpifjqel.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2kxpdmzzu.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2wsmzfftf.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2aspvvtiz.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2lgwkdqki.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2wgiviqex.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2gunwotsr.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2qsjnwctr.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2grmzvwwg.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2pgnqrlkn.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2cpsfaznc.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2hcorxxbs.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2nrrwglon.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2hpigfiqq.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2ajadczuh.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2qqazktve.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2kydebtyo.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2btkawfst.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2oivsdgyg.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2cjikycbh.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2nutxhtsz.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2zhmnizqg.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2cpywfgtj.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2kwqkjxoe.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2komgilqx.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2gngaxjtj.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2rthaqckg.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2uodyrwzu.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2fikpdjst.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2pyylgtmg.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2sgogcudj.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2npblfnps.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2gjdiurkj.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2ceghlern.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2jrzoqrwr.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2sbnjixlg.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2kmnwrndt.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2eqnxjgiz.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2elflbboy.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2mvhgyppf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mtzdwmie.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2manrlzcv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pddnlvkm.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2phevrlfj.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2emrediac.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2zcivnarw.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2sjxoxvgq.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2tfdxqqad.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2qsqfhifn.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2yrilryrp.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2kenpgiqy.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2oavwlpuw.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2hfkjnujh.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2vtdifnna.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2fugdxqpz.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2sxyzbczu.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2zennyabi.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2yfrxthvs.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2lnbesuwz.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2jrspgoxt.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2jrsjbhpu.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2amckdynd.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2icemmxqa.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2mymwpfge.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2beqfhyzp.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2nkowozbc.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2qjmqcymc.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2lovhpcgf.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2ztpcmbmu.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2kzihuwfb.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2afzzzpns.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2uvjoowkd.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2wbeftrkv.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2adaltsrc.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2aikscdph.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2fvwjxwqh.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2ksbggekm.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2tzcsqkwx.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mypfemij.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2vrrsoske.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2qxbapbvw.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2qaxkjfwx.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2calxjnez.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2olsempuw.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2trkuwyeo.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2ukiuxgaa.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2qvdebryn.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2nwonxpcj.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2zxtjjoxc.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2fepxguqd.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2nczuozrs.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2pyjqosax.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2jdabwojf.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2wvhurlsl.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2waorourt.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2nsnbdhqe.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2mvpbpxtx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oyiazbmo.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2tnzcavdg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pzusmbfu.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2iyuurncq.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2yflonftc.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2adcejbsh.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2cnholvvk.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2ofpzrudx.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2amghbsxz.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2hevswnve.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2pwuemuoh.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2roxcgcbc.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2paojdfsr.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2kkhxoyfr.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2mmjhibsm.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2qqnvpnta.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2kxllbicl.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2iqekgqkj.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2hacdugxy.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ampihsff.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2ntaixuyo.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nqawuaea.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2gmpdeabs.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2jnwlahyo.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2awidhnew.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2zglkaris.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2cegzyrwq.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2hnqvuxsw.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2mrryotvf.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2yuqjlcav.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2lnebptyw.html


<!-- 参考信息 -->