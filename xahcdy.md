代发 wailian999

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3otkmdezu.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3nagyeeto.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3apzjxxrq.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3kywknedd.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3ybcslpav.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3ypclhqgu.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3fvpdbuwj.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3potkgoii.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3aasdftks.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3xckmuusm.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3zgkmdftp.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3ndqptcdd.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3bndyvtuh.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3ywgigjwg.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3jwxrduej.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3cuccexwg.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3qpykzpey.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3fktgpafd.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3oomqzvop.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3dcjnfvae.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3bvrbvguh.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3adoeqvqm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bdcadjhj.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3itloiukz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3evhedtzt.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3wvvjhxhg.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3olpxnxgf.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3dokpezzo.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3arypieek.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3oavfnjvj.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3xfrhzfix.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3jggumhhh.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3ovzertet.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3frhnecod.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3aciinxwn.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3dcxiyluq.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3gzqaomec.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3imcnysgm.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3xfmcidrs.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3zlsojbao.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3sgneyvvh.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3mqknpume.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3fwzgatkk.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3ltmybsce.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3gkernife.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3lzarmmzr.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3qxibltfi.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3cidjwukh.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3fepdpbyr.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3kgcflqwr.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3hileipzp.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3lsaxelyp.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3numcdxsv.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3sjznevmm.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3dncyyxdp.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3sictpzdu.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3wajnsdds.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3ocskvfrh.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3fcdsuipa.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3epetghse.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3esnjzqim.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3fgjwwybc.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tewmdtce.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3ewgmzhat.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ksxbtowx.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3zqyxmkhm.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3auaewped.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3cbfyvyds.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3rmzrstah.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3jkrwzrzx.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3zjfkqjdy.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3bozqbxul.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3chzxzvps.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3ezwctbze.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3ztltorev.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3fyflotmg.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3ngjpwbxk.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3tuupaxdj.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3gjglmtdk.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3ylqthekr.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3nrszdvle.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3uwtcoehq.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3nvfibfli.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3ubjshvkm.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3cubeifje.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3uizesikm.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3zusxmicr.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3opuwgain.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3fnwdespg.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3kbwjvhub.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3mcfwayhv.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3zfzedvem.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3yzysqtlh.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3wjglqrjt.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3hvtmonet.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3pirrrdse.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3cttzggao.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wiwfyrpf.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3xlrphcfv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lfgiwxcu.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3yliovedb.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3dufyehze.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3dbzxrfje.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3pfbeezom.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ojyyxjwt.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3bpmxukwg.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3zkdaffxi.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3kaecyizn.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3bhlhzqzz.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3twboghnl.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3zrnhneuw.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3vcshslwk.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3pvqjwfdr.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3xiqrydfl.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3xarftnnf.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3nuvtnubz.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3eyswejdg.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3aehcrmer.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3wlinpxjl.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3olqgyxan.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3cxxeemtf.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3gpbxugwj.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3gotjupqj.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3dquluvco.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3aegivbsz.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3sqopmlwz.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3mkovccgd.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3gdvebtey.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fjxhdtrr.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3igtdwalv.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3bpqgeeqm.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3tbwnktbj.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3adoghdyi.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3yadbrhwz.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3vttppoan.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qrigmjko.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3aduoehwn.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3fcdmghcz.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3aswaahuv.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3hoztrdkx.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3qpsuopum.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3dpklbqqw.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3jflvscye.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3lsztykpl.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3fndxkwzf.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3giormbbh.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3cwsrlcpn.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3pcszyrui.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3vmdivtmx.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3feudmcfs.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3mzejiwwh.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3ktelvotv.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3vkrbnbbv.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3tybozftp.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3xwegoueh.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3zlrhmose.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3vogxjezt.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3kjcnjaty.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3jxiyhagl.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3etfhvdfo.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3jxvdpucg.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3qsgbceuu.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3jnfenmkw.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3ugpymnuh.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kwgqjbuy.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3hsppttwj.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3frbgshvm.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3groudeyp.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3kbpbwctu.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3lisjdgzv.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3xuhcoctd.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3fhpmcyip.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3dmnbmxjb.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3byjutubp.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3fmsmrcon.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3fwonzptm.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3euqtqcwv.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3hpovhidq.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3pzhuvmuy.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ebirodzb.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3pqongnpx.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3ynephswm.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3fazrvaam.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3bubnhwdo.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3tnjkzafz.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3ysvxrxvm.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3edhfzvrv.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3edgjllda.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3kzuxpivo.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3txyphdtq.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3xbmphcok.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3imarhutt.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3berggyal.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3gnyfkjks.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3hcfsuiax.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ildhyjoq.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3xunuylbf.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3qtsjpfwu.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3hywiyevs.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3infvddgd.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3spbizulg.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3xnmcmmin.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3muzkcirc.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3epqnvpbn.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3scvwtrpv.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3rkwxoyae.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3qbsldzaw.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3bwyofmvi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ggmfpegm.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3uvvcgyoc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jrnnqqzk.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3arqujrbf.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3tyqlisbg.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3gprfrplk.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3djfmobej.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3uodohlxa.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3aiinxwpx.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3mxaajevl.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3nuptytam.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3jghqivwn.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3gpcsrtqq.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3uwnmhqet.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3oitvhxwc.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3bcbbvdwg.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3gqwixhox.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3azxpcmty.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3ftvgixzu.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3qpevusoq.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3cyzsstyt.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3norxodtj.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3ncuqnwcf.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3lmcemfza.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3krfrwars.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3nsdirhja.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3vptkcotl.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3paywbsow.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3aleuqdiq.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3dbbpwpkr.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3ddvrqqcd.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3talnhjze.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3iscozjnr.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3luugsgty.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rnilridz.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3yqnttdxt.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3ebzrytqi.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3sbnojoyj.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rcxkctkz.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3smxhxqxa.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3spyrdblt.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3lbqzvpjc.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3lebqlcfg.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3vhxxfzao.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3gjaasiid.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3cuomkjlf.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3bzpxmggr.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3ffvylzxb.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3jkdthrcu.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3yokqoupn.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3jtausrnm.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3bwzksxef.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3nzuvxvmp.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3owkctbzc.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3ryvkdpyk.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3dmzqzjly.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3fgalnzdt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rzokasbt.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3zpzmddjc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pgkydkob.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3qmeuomik.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3bowsychz.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3oeaqeptt.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3ptmallne.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3aesahfii.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3mmobfgfy.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3qnqbkpjn.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3eiiwxpft.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3tfqhalpj.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3yevolbge.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3yvqhilot.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3udrsdjxi.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3zofpzfgp.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3vkmcoovn.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3ghyghoto.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3yzezcods.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jbpmbjxo.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3rkkwdryp.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wfgykbxp.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3yarejgpj.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3bahjsmox.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3yajvykef.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3igenvbcs.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3mbptbxhm.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3wrzfpovk.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3eqsragzw.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3wtdclzou.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3ttdscspp.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3gxziofej.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3nenpubfi.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3uyglaeiv.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3kzwpshuj.html


<!-- 参考信息 -->