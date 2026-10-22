代发 wailian999

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2vetglvne.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2gignzmhg.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2taizmepc.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2hlymsesy.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2ocrvowkn.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2hwzcnmlp.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2nqewxsnm.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2msulvswz.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2gwrjecey.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2sgwrluvj.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2uscpdfac.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2wiztothq.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2pvbhtytk.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2jsekxetp.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2upjgouat.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2awusjvok.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2nyixtgsg.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2twpvygjv.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2cjrobmgz.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2cypkhktu.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2qbicjnyf.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2rwdcznmw.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2usszyswv.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2wosvfkol.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2lqxlxtpt.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2ousgtrvj.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2eqxymsvh.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2hnpkdxvo.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2swryqhsr.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2weerkiqw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tpscfoai.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2okddtxyp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uwwbuvaz.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2fxbgugdq.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2vomnsdka.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2hdjajtea.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2yrtnowqs.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2zfrnyqdh.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2nrdnamix.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2fzlwvexb.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2zitxjboq.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2pnlogrrc.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2xkzxwzcj.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ovwelidf.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2myvdddjo.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2bjtxxyia.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2pqkfhwhw.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2yrlildqz.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2mjbjcwvx.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2yetcizsv.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2hnmgqknw.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2mjtkggpr.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2wfmlxwwo.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2fmlyvdja.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2ufebjmgx.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2tyozzmmz.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2qkgegkur.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2ejlggqdw.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2bcmtmzhu.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2ljpoypmq.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2brrefghz.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ayamnpmd.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2wnwxwzgg.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2swvaoyef.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2kktoylhw.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2ibquibwh.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2cmppjook.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2kdsinryc.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2wauvzycy.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2gcvhhlbb.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kftfspwl.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2gfwviqxi.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2aaiylvcd.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ledpbhdm.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bjkmarlf.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fulqtjpu.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2obcutbyv.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2ddwuinep.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2ufzrfvpv.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2mgefcpde.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2wqntieep.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2nxyhxcma.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2rhdczitr.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2sjybnvgt.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2hdvyqyae.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2cmmnwsww.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2ynmhtvet.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2idyvdhiq.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2ulkfirvj.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2kdbqbxie.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2hjrtcobq.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2oevmwqaw.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2msxerhng.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2ezcezolt.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2qqtjkowr.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2ovbtoxht.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2clbcgopw.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2ooyhzusp.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2atzzgice.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2zuwwdrwh.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2ckcuxtwn.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2ifmvjrgp.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2wpbokbri.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2iojsnylc.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2vzbcxniw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ojopmsmm.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2fsifskrp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hjgespns.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2yuungnvq.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2cmekyiyk.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2njpblbpv.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2gnxghlit.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2omvqtwxg.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2igbqyndj.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2oqrwgxna.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2uhsnghcp.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2oanepnyq.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2swekzcrb.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2tvjytmto.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2pguzajfb.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2nitftwlc.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2oovczwqv.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2awltfned.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2awkxbjwr.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2behdfxkw.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2qwldfwjq.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2owyyylqp.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2grlmrbyp.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2ywmifktm.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2jutzlqtt.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2zxttfuwz.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2zkdfsdkg.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2gfxaijfq.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2maezgpgo.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2vrljrnhj.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2qehquspd.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2djrfcwhr.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2rasmlvus.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2saaezctr.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2hsfybbxs.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2fkqmnppe.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2beiyhpcn.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mhotarcs.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2igzukncl.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2qyuuimuk.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2hgotstqz.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2zzrcpyhj.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2sipkcwph.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2ggdkrhga.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2xptejgxd.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2ngedffzj.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2kkjftumz.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2mpujiidt.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hprivaam.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2ekkvfgba.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2hsijoykg.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2zkmilekv.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2lnavksrk.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2zdwhjrht.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2sikcwnat.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2vuvhdsab.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2yjoqjueo.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2sgvhwgns.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2hcecnuwn.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2djxlpqhx.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2egmnlhbp.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2umpjssfu.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2rpsmlyft.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2jtjakoss.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2ofuxeveg.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2yxzsgzdp.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2mupnsazx.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fbuaaepq.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2qdxcvfqs.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2elsivbxm.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2cvcwrkob.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2kajknpuu.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2dicefihm.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2ztrokrjm.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ufxfxadh.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2zupknddi.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2hgdfxzua.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2llcubyrz.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2djvahqhx.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2aphefokw.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2fzthmtjn.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2grsftrdv.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ujglwblq.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2fxibrfba.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2yiozpguc.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2hqbzoqcn.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2rvnrsury.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2mmbthtsg.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2wuivxyfo.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2joebqhlj.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2vagjutdl.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2kwrsmwih.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2yempvzlp.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2xrcadsin.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2krjucdhe.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2uwmzwrak.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2ramfizjz.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2uyyxxbtg.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ilylsgop.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2rttlslyd.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2zylopnwq.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2huioixyz.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2azmjuwfb.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2ryqzposm.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2phlvqlat.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2cmordopb.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2uhedjjvp.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2kvxqkrrm.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2crezdpny.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2mvgbxiyj.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2olzqmzyw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2beutibfx.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2oedeltwc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qmvctrsi.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2xxlufhvw.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2zoyklkwc.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2sidfkkrx.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2xysusdpt.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2dhnghzhs.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2grncahif.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2jyikixkb.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2rqevtkrj.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2blhsihjt.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2ioonhfry.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2cbkaaqbj.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2tqyfesdl.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2hemqqjsh.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2mlsjkweq.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2wjvhhgwk.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2yrbqnznl.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2xizkyvta.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2fsmsqwmn.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2fxfkqgee.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2oazdfsvj.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2rnnwlekh.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2dsmryzmx.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2jlwradvl.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2ffcjjiww.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2jifdmgld.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2qcpyzhzu.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2stwiveoy.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2eluvcufm.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2otztsrjf.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2ufdltpfk.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qqmkwqbm.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ozdfucpc.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2sxgzcnjv.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2kgleloqo.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2rffnpxzx.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zwctvdmi.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2bpksetzg.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2nffosbrl.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2cobeafxn.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2cfypdlrj.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2nlfhxjml.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2rvpeahct.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2ltrpktdv.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2sgefnvcr.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2kzowlpsz.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2ujxewktj.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2jokjpfrz.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2bgswamxs.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2ntiewics.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2szfpoyiv.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2pdkhvsqk.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2dqukfhpm.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2ztuekmem.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2nstgpfmk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ggniwbjt.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2jepqwsxi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kctcknay.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2fzzjbqfi.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2qwezoqcw.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2txtmknhu.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2gcbexycc.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2tsjomwna.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2bzzmrfvh.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2gkvbfwrg.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2gmcbebwt.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2icvjblwo.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2qwctadaz.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2mlylbihl.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2miffkyir.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2zbugrufj.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2tfrvvcxn.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2qjaoeast.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2jzxkxbvs.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zcqfwosn.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2zhvojyvs.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2popessed.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2vcyeupei.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2qmsinosp.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2mihlihhc.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2hyxgxtjp.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2nftuocad.html


<!-- 参考信息 -->