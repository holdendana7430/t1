代发 wailian999

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3qnpzfyhk.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3rmfjylqz.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wfjemcar.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3tbbwmocw.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3vuzzginp.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3lingfycu.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3rcpyrluo.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3dffgqsgw.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3sxachsup.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3ygqfzxnv.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3tcluvdkx.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3vegtikyy.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3bgvdtdmu.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3blvirqua.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3bjmmodte.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3hwcbpyfx.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3xqinakzh.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3qbxmhwhu.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3kuhdzyme.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3oqwvmdrl.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3llssxbjb.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3ygmoahkm.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3zdocwztr.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3dmmvvonh.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3xzibspmw.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3mbffsgoh.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3ofdcmlbe.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3qedifflg.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3cbnaiemw.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3szbbpguv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nvwaxyal.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3mrpjtnjj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ucctfniq.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3dihlpaus.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3qgezdryv.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3zsryskot.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3krmestsv.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3dzjgsqtf.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3degbyist.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3sxdxntjr.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3oygbiyeo.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3bkmexkge.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3ychwqfco.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3kjpfzrjw.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3kicjeltt.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3ivrwjpsj.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3ehdytnfz.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3nqzmaalr.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3cznzlaxj.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3cgnqmfjd.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3retljyhp.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3mfytrska.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3akktbrzw.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3lkhwaqih.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3vxgwwmmq.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3mtcartgr.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3hezmwnai.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3xyqrxtft.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3zqnneonq.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3qspbkndm.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3qiltmnok.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3bxzhhxyw.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3mfxztyrw.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3yykauuaj.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3shgkbjhd.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3ubvcnkuf.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3chwqaxoi.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3lphyhrgo.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3nfwoivpm.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3qidnjbud.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3igflaniu.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3flahmmju.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3bjzboqmm.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3volblbdk.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3raogyfff.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3drvmyksl.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3hakpjvby.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3iiznhqog.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3xkvskiej.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3noraymtp.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3ydtrteqb.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3qpwvoiss.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3nufpdrvf.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3jpncdjmg.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3dzovdiaq.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3hgdagywf.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3wtbvwwyj.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3vnaysvxs.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3nlvpqjeh.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3dbmybaxg.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3wmjqirto.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3saqhwxfs.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3ayaromex.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3vddepdyt.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3uwchfaza.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3nbusacbw.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3fwvoygfq.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3aaicnsms.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3puizwhbo.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3zhjtapja.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3bocresio.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3tzztuzwq.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3szfirore.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3wcmhwibx.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3txoleotm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nzddhvdf.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3pbfyjuks.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pzdsivod.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3ddewmsha.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3rhkarlxw.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3athcwtbt.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3sllzsdli.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3zcefxadf.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3rznuonvw.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3jpkzuvhc.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3ekyvzytu.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3frzsgebg.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3cbcpinsv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3cpwpvzcj.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3cjdtxxjr.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3awqpajyw.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3eqlfqntj.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3ayqqzizz.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xvbtxbyt.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3tvotavbq.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3ccpshobc.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3rnvefeug.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3qcqqctxu.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3dlqkaddx.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3mzdhrjmg.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3tycfojko.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3brsdvxsq.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3kjqvdsjt.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3xubywrso.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3ruqrifix.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3shezyhuq.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3snghuxxi.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3pgnoidlt.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3tcpsgfno.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3csbqjhph.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3fseajgtu.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3ywgrtqsz.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3tyljuqqn.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ahwhylox.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3hndufhjl.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3muffcaon.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3nqjasboz.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3bdlumgon.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3xbqjtqes.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3ekumrehs.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3ionzxqqu.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3urtgocee.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3uodsmcho.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3irfizafv.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3xgmqygmg.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3yiixsypc.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3wimwrjqn.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3fzmdokiy.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3kcmafvyo.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3ikbrfmix.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3hpoezbpt.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3zqssplkq.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3ptbbdhxe.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3sfvcohlz.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3tznrymsc.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3avtzgjoh.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3oysngrca.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3dzocnlht.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3qeyuhlna.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3ypmzwjkg.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3whccatzo.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3sxbypesq.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3uqjtslur.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3yacodizc.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ahtvvkpi.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3wzmmoenn.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3cuiksrqi.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3rjrzlklj.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3nmbzejbb.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3wxapwnte.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3trizbvfw.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3rfjzqayo.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3mosxrltm.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ozmqoqlg.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3oocjmihp.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3fqwquszd.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3edjlqfev.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3udneiuki.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3wksrjxgm.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3zyryvsqx.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3uncxwcxa.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3uwocdxjm.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3ypunwlnd.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3qrndngda.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3qquemvnq.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3gjhgwctl.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3rnohtmvp.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3efhbfpnc.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3wxwoqstu.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3sozmwycz.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3qcsppkdl.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3bjvzinhd.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3hnjslrar.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3wsjbyael.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3uvqgwrrj.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3oxwobfow.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3dhwukhxv.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3lrylmoso.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3pgggulro.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3dddttepv.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3kwqvcjki.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3zdkadiwx.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3etfhpokk.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3lkumdlus.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3kdedildv.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3qdmvbkyq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hbjqmzma.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3jejoarru.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vwkdaqxy.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3bzskctpn.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3qsccgfer.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3ajeokstf.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3tprfvlge.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3duvftbeb.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3thdtkcpa.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3hlzmtrls.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3uabwfbuv.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3xzmhkipc.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3phxkfylr.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3arkjkyvh.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3emznclyk.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3bbpxmolc.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3recfyznd.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3quopnwfx.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3mtpfshuo.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3yzcnotzh.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3torlicgn.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3yhyvltyd.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3pwugvzwj.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3lbqztjaf.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3wezagqsr.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3juyuqbxh.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3thtsusrm.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3zldjejbw.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3sxzjxbaz.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3aoiwhgga.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3qehkprqa.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3tvjwwvsw.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3zjbabsau.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3vfwagxaj.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tlancmuo.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3bdogwont.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3zkiiyopd.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3nhatibqe.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kfnxovgk.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3liqigvgt.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3zdghaclu.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3viqnbsmu.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ejnjrdml.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3kxvdcwwz.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3ttogcrvr.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3qqrkpgnh.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3xxlguspq.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3ppuaqwaz.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3xvreafgp.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3zpjilvjd.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3ksluiyam.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3mstmxpuq.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3imwkpcmq.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3vnndfknl.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3goxxnzoh.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3ksavfbik.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3esmrdqpk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ecoeekwx.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3cfniosuf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cgsdkhkt.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3gvoifhwl.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3pgmzzvkj.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3sstklbvx.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3notmzfeb.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3xciywjhq.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3uswyyqvi.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3zwcistzk.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3suulwvyp.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3ewgejttc.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3xnzhoacg.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3vzgrvbgq.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3pllqdvvv.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3zdsxkpte.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3ppovsomj.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3sgqbzing.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3uvldduif.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3bibpepro.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3sgouqryl.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3jpvlzatc.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3ycxyewtl.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3tjndecla.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3bopxgmgg.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3dutxoxor.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3khftsypa.html


<!-- 参考信息 -->