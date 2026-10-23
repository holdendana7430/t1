代发 wailian999

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3kyjqfbrj.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3rqxpwoyi.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3jngatylu.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3acyvrcbu.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3iswfnzoz.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3afmhgdle.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3memsohvg.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3eptjhnre.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3dnwfiuen.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3eohjletf.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3gfqlagnu.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3lmayljyp.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3vojhcbji.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3scmgqzgh.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3dqlezzzt.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3bfmcfrso.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3vzhsvqjt.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3vulqshev.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3nrnealpj.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3zwkggkhy.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3cyxlvdgv.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3njthcrum.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3mmjtzqyg.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3kenyaxat.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3wokzzqoe.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3donqcwun.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ujbsankw.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3qngcqgcj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zihfxyjh.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3jcflanjg.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3hklflnwa.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3hvnztesr.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3yeldoytf.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3ynudtwqr.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3qqrwbnps.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3rosubdge.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3ykvqatmf.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3otchddzk.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3omonbcvw.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3doohctbe.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3ohglnueu.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3telbfmtj.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3xgxyvjcw.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3pvzfnpna.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ubnszaln.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3uruchjrv.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ejcnlxlf.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3hxifrgol.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3yzuresfw.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3teekwsef.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3conjytqd.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3bewsumzm.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3mviwanvv.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3revoxvda.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3mvgwtevk.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3ttltnxtm.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3wbqiydin.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3vyhnsecd.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3qfupxmpd.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ualvnsth.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3hbrokjhu.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3uksxodsu.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3dylvhovl.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3xwfbjaxu.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3aqtdaejk.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3kfbsbpwu.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3dqqxtlbo.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3qqtnuixw.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ozwgorxh.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ioddbphf.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kqwhsyyp.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3snvofhmr.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3zbbscafu.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3njtmpzjs.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3tiabibdy.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3xbjmjavw.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3wcpievij.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3tzsjczfy.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3jygxivvo.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3ckpnypja.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3itluhmbl.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3vewsqtxk.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3utuotgqz.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3gbmkexht.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3uqfgrzwe.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3pgdgixgs.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3fjmaxqvx.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3cronsfcd.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3krcjiolu.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3uajleimn.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3mokyxzeh.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3aiuxfawz.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3dqkeovll.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3txtrayjc.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3onwmdyqt.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3yqyfeujv.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3oymlsfxl.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3cyprbwef.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3bxurlmzu.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3artgczun.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3glrxnivs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nymguohc.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3wudawvcv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cevrfuwd.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3haqgghfu.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3smzsuhnz.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3eogkinxa.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3hfxtldsw.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3yevoagvz.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3mrkjavuk.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3hgdtlvaa.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3youggsii.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3hrpknprg.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3cccztdcu.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3censswmc.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3bnnxnyvl.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3occagkhh.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3fkqdanqm.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3sktzppnz.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qftxycgb.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3xsxowzxp.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3hctmunvp.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3kizbfsty.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3yyqdiayn.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3hxjwzbhd.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3fgoejrxd.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3vxorflly.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3apkiwuvc.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3zmitrzxs.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3bgznebkf.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3jfvbxbar.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3bwivnlvf.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3pxrrsedp.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3xkhbrwji.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3enonzwnr.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3grvpamal.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3omittqmu.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3llkboboe.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3rfmpexdi.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jbydyurh.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3gsqauqwt.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3faqnxqlq.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3wqvqzqxt.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3lfkcceeo.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3vepqhgvi.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3ipajvxvl.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3xyixrcam.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3bfcicrsw.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3qxxldjrp.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wzprrnpv.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3iotosofr.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3iaerfzed.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3wxitblwl.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3yrjgxjdz.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3jwsfhouf.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3xeyhwppm.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3zsmyjukr.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3gzshlstp.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3ujznhqop.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3xcrjpwvf.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3czwjxyei.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3lzootsgo.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3zmmrguoe.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3bgtftimc.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3ukfgopek.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3pcwrpfgo.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3wzgshpjj.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3urhllckk.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yyaepqmx.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3ieiipuka.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3tcpezylf.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3qytnlojd.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3nezqvipj.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3giyphldq.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3gpjnemgz.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3tzcyfqlh.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3qwljpwrj.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3lpkeijap.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3frqodkwv.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ttnsmvcb.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3vmwgyqmw.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3xdkjrrtb.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3ldlwwkta.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3qsgalute.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3hwinmlzs.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3cxbufgvk.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3sfgfplvd.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3tnissitt.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3nrgkjysj.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3lbfmtxod.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3gwubesim.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3zxtnyypd.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3cgydaevb.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3jfmuhmwf.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3wfrwabnx.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3qigpanrj.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3dahjwnmm.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3jvfztivd.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3rmprdqaf.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3bpmyevmw.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3zqckordg.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3oqflvzjt.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3qqwlraej.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3gqnbjlzq.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3lurxdorc.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3qyvskjqg.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3vkczdtdw.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3nqoknsqa.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3ynworuxa.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3nvoswgtt.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3tfhkmizp.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3kdxdjxzi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ranenogm.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3xqjpghdn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kvakdcvx.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3lghthsps.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3swbhbdie.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3xfytpuhp.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3tbrbjcyr.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3flmptmyz.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3jyhfslth.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3fusxmabn.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3eeitpglm.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3blfvrpeo.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3xkkmxiku.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3itjcdior.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3bmmyifsl.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3tndvpnml.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3pgakspvs.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3rbnhcbuj.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3yezaraiu.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3hydqkxpe.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3djtoeqqo.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3lhtkapzq.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3oxzivupm.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3decowllu.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3tmfnbljm.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3meekqdqu.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ycewswxk.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3uaqiqlhr.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3wmijmggt.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ertnneer.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3wqptfvzj.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3yeugspxi.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3whvmkgel.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3relktmsu.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3htbvmccf.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3ihhyunkd.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3stocdbgy.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3jebhozwp.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3awlrvecd.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3ydhhfngn.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3gzvnazng.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3plgtscrn.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3pbyamhns.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3nvjdoxyw.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3lzljfvic.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3obatlitd.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3yuknwrtn.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3pyawpteb.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3erelpvpq.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3yywtpcey.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3idoffuco.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3vfgjalbz.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3ejpaifnf.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3ggfeavug.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3pklujtvo.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3epqtzdai.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3jfpuuhwq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cfcdgntt.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3ozyrltmy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kgoammah.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3qvotupvc.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3kzyrizau.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3klpdwvoq.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3oknbbrah.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3mwkgonzl.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3rjdtggjf.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3wcikvfrw.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3icjcjnls.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3mhhswrge.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3jluqeabv.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3tddmjpis.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3xtqcagfu.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3weoifhuo.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3aqlxuxsc.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3jlrunwqw.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3uzcmnuvk.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ajesemgw.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3nxdfnjxm.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ajdxwzmc.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3gclxhkei.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3ejkaxkav.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3vomhuyku.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3eynvzoth.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3tjbxiiqs.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3jqiwmesc.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3imtzeejd.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3imfknaja.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3aqsmlvyh.html


<!-- 参考信息 -->