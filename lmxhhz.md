代发 wailian999

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3hnppjyve.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3dfpujwna.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3utchfdlh.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3optomhrz.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3etdsqxvj.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3frirrxrz.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3uuclhxly.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3fqmdptlr.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3kopjkdzh.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3ubwtcvul.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3qzsfnxhx.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3ubceobza.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3eezlamen.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3obaeilfk.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3hqzvllmm.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3abhhohyf.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3ddkwqvhy.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3cjibhuyh.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3jasztzbr.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3akkknfyh.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3nbqoklwb.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3wgokwibo.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3emdvfoiz.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3gxysxbie.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3vcjrcoef.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3mpziyiql.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cyrvmqdt.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3gzzaagqe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lbnscjbx.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3pwwiabax.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3bkejfzea.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3umeukyaw.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3ixwiuakb.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3qslqnyhy.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3moqofcyi.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3fklmdspc.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3zixbcmfx.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3fkgqsawl.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3treopbxb.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3leuxybzd.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3nsuetxzc.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3jxbyuuaj.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3sgjxvslo.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3zevquimj.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3cqrzfjpl.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3nbxarnpp.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3qfrjtsde.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3mkczrpih.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3uwricjkc.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3vklwwzui.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3nbovihat.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3bxzpmxiy.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3qrkokacf.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3ctqztwdx.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3mbfbjgrf.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3pdwvqyyz.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3eaitvlxo.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3jxovyukc.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3tqjyscqk.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3epricxhk.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3vhdgvrpb.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3bhfdkhbn.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3zoyhjlja.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3polaueec.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3bguxtfzy.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3gryrvdji.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3sipmbgpq.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3qqpkjmjq.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3zgsuordo.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bcrxpvld.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3quvijsjv.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zfcxuwpu.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3rmxoafmr.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3kxcakori.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3qpoqztbs.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3huaeesif.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3vwcksqfz.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3eqfranbq.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3abdobpse.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3bsycxflf.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3gvsjcqld.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3fvhwxuok.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3olsdykcl.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3hrdwbkzm.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3xfuagcug.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3xwgvwzcj.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3vcmjrkms.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3vdlzgjji.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3peptvboi.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3uhldrizj.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3jdyqnlpu.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3vodznkzn.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3yzplouob.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3ixvkivsm.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3yyqrdwaq.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3enxzabzz.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3ictyrxvj.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3lpzfrkfn.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3kkrqkuix.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3cxppssgm.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3jpqgjpld.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qdgkciwo.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3dmrnmfxz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qckzhnvb.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3rlnejust.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3brmnrdrg.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3qokgwurx.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3akisxtor.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3gbkkziao.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3rjglihhc.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3qhktzybt.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3zphklzjp.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3sdachwmf.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3panhlcnb.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3bemyxzik.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ndqcuvmp.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3hvyplnbw.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3ozhyqaan.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3dnfzxqdn.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3nsijpgnk.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3jkonzkib.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3yoomuyvq.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3rhzveybs.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3isvijxez.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3ythiased.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3gisdvoaa.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3fxiecfzm.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3uheqewiu.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3zrgijihz.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3oawfxogm.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3ovkcrmkn.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3eaanoqvn.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3labsabyq.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3iagbcfhn.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qxcuohlk.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3vksgiatg.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3owzstfri.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3xjhbvppp.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dtzeaewq.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3mfixnzls.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3trkaxorh.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3itdjihum.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3frvgzygt.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3zuvkwfab.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3kygyukpy.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3xkvhafto.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3kkicoxpk.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3mlkbmmlt.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3rkmswtht.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3sjakscaz.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3szufqzgn.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3crixhvrg.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3kmakjlbd.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3rnfcibqd.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3bfuhxgoj.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3huaxxoqz.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ugzlrlky.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3cxvumtcw.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3jewrtplp.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3npvvovsv.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3tgxohtmu.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3rjiykmxq.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3lpzzkoxt.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3mnmjvaiu.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3ksutwwsa.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3msvfvcpo.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3pcywrkiw.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3ucovrqcq.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jiaamrka.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3wccclift.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3gvuaegaj.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3grcldpxp.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3pwahuxsk.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ybucnmvf.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3eklqjvmd.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3zevjsafl.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3ldjtrlkg.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3hykwvwzy.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ylwwhklo.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3tihopatf.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3dgeveqrs.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3zrdkkgif.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3ougzhkbq.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3tnxvdrtg.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3mwxwwecg.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3glppivca.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3qqemffup.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3znycuddv.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3vpwcpqyx.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3kimuyelz.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3wcjwqpfi.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3cthfmqda.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3xrljpoam.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3lyokbdpl.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3hyrlohpt.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3tizlakpp.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3jaipvthz.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3jemkjued.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3kofnxguu.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3oohqeocf.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3boswaqnj.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3etkrkynk.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3duttwvwo.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3byxtxdhh.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3bssboalw.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3holpnqcx.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3byahcrfh.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3cxjmsgln.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3pajwvckj.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3vflganky.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3twrjommg.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3kvlgeubx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3roxalhok.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3cvhktrvj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aleedexd.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3hnatzoii.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3eddqibof.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3owqignsp.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3nussrncn.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3riypoauf.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3hknfihrn.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3padrbisx.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3mulkfivd.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3ezcghtod.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3qyjzypoq.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3yhjtmaud.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3xxotrbdz.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3khkjpucp.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3rcevojas.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3ufdzjrtj.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3cupadjmp.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3ebwftxpt.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3wafdfrwf.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3zhyoyguw.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3swtxikkj.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3ccvoikha.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3nssluoza.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3wjnqvheo.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3esjfqtms.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3mfmcrncj.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3lxlqmkhu.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3zirxaxcq.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3gwujzwoq.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3wkyfdzvk.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3eywzzlox.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3xgbkxlpk.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pfmbmoqb.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3ujbezrkf.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3obrectsh.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3jrnvdnka.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lrkumvys.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3twnyxbkf.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3npnxyqbb.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3wdncfxbb.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3dbasidlh.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3ycqmtmoq.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3mtpgooji.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3jkpsvdhb.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3mztdkdyj.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3tfzzexkt.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3zkspbaqy.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3rnuqjtvj.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3qoapavco.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3welcmzex.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3rfhccdlx.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3jvjvpkxn.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3frbdjslr.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3tagekllq.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3ahlxbpna.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tnuaaysw.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3bkhwzyxz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lmhummpt.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3ynclqxly.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3dnrxzmmt.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3ipdxuwfb.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3dyiilcxa.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3hukmtmjx.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3flnjtnpl.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3knujjkun.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3lyuoulbc.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3hjzeigym.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3loitdmef.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3woegmmti.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3anicntfk.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3rphtqvli.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3vyffgpfa.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3frhblzpv.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3ukfxuknp.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3zcgsqknd.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3lccnytxw.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mtdmnhtj.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3bczamehu.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3qtdntbmg.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3zwazdihn.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3arsmthpd.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3atbgbjii.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3vveajqsw.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3ymockzcg.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3kjshkcjw.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3ndgcgcld.html


<!-- 参考信息 -->