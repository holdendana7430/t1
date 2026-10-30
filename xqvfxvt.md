代发 wailian999

Py:   resp.json()
来源：http://baike.fehbvm.com/Article/details/gpxwuqeqq.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.fehbvm.com/Article/details/gnnagpdkg.sHtML

JS:   await resp.json()
来源：http://blog.fehbvm.com/Article/details/gmcmmjkct.sHtML

TS:   await resp.json()
来源：http://m.share.hesvh.cn/Article/details/gitnixvrg.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.zdbjq.cn/Article/details/gmuilnskt.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.zdbjq.cn/Article/details/grqovhnfi.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.zdbjq.cn/Article/details/gzggpxrsr.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.fehbvm.com/Article/details/gbpawdzys.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.hesvh.cn/Article/details/gtxsswjus.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.hesvh.cn/Article/details/gvushuzrx.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.zdbjq.cn/Article/details/gsquyfgfk.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.fehbvm.com/Article/details/guntmszmb.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.zdbjq.cn/Article/details/gyyfilmae.sHtML

Java: resp.statusCode()
来源：http://wap.hesvh.cn/Article/details/gwzxbgvxq.sHtML

Go:   resp.StatusCode
来源：http://www.blog.fehbvm.com/Article/details/gxyktacas.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.zdbjq.cn/Article/details/gmwolwcvo.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.fehbvm.com/Article/details/grojvlhod.sHtML

[L08] 并发请求多个地址
来源：http://3g.zdbjq.cn/Article/details/gnbraipah.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.fehbvm.com/Article/details/glfkqaicp.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.hesvh.cn/Article/details/gxerklxmo.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/gvdenjzoz.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/glacvoreg.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.fehbvm.com/Article/details/gceurvacm.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.fehbvm.com/Article/details/gsnozkccr.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.hesvh.cn/Article/details/gdqxvjbhq.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.hesvh.cn/Article/details/gcdthtnmp.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gauyqdxyz.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.zdbjq.cn/Article/details/gqgwxgjjp.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gafnmvuil.sHtML

[M01] 读取命令行参数
来源：http://3g.hesvh.cn/Article/details/gzplsmfrz.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.hesvh.cn/Article/details/grdcdssjo.sHtML

PHP:  $argv;  $argc;
来源：http://baike.fehbvm.com/Article/details/ggjsspqdh.sHtML

JS:   process.argv.slice(2)
来源：http://baike.zdbjq.cn/Article/details/gixnkabvh.sHtML

TS:   process.argv.slice(2)
来源：http://3g.zdbjq.cn/Article/details/gdsrmovsu.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.fehbvm.com/Article/details/gdbsyeqac.sHtML

Go:   os.Args[1:]
来源：http://m.share.fehbvm.com/Article/details/gtbafxenb.sHtML

Ruby: ARGV
来源：http://www.share.fehbvm.com/Article/details/grkcapbvh.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.zdbjq.cn/Article/details/goqnuhpou.sHtML

[M02] 读取环境变量
来源：http://wap.fehbvm.com/Article/details/gjvhlkpfe.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.fehbvm.com/Article/details/ghpghzhze.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.fehbvm.com/Article/details/gmecdjqhl.sHtML

JS:   process.env.HOME
来源：http://read.share.fehbvm.com/Article/details/gbevvdagr.sHtML

TS:   process.env.HOME
来源：http://www.share.hesvh.cn/Article/details/gbflmmdcp.sHtML

Java: System.getenv("HOME")
来源：http://read.share.hesvh.cn/Article/details/groplntix.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.hesvh.cn/Article/details/ghnwlqrgz.sHtML

Ruby: ENV["HOME"]
来源：http://baike.hesvh.cn/Article/details/gusladsri.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/ghhwdqeri.sHtML

[M03] 执行外部命令
来源：http://www.blog.hesvh.cn/Article/details/gzobzkytg.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.hesvh.cn/Article/details/guyyohxmj.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.fehbvm.com/Article/details/gmjtykkqr.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fehbvm.com/Article/details/gfltlznem.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.hesvh.cn/Article/details/gglabmcyp.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.fehbvm.com/Article/details/gtebwcpip.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.hesvh.cn/Article/details/gfuiyrplo.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.fehbvm.com/Article/details/gfuzugpkw.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.hesvh.cn/Article/details/gcfwyfhmd.sHtML

[M04] 获取当前工作目录
来源：http://blog.zdbjq.cn/Article/details/gumcyqjyc.sHtML

Py:   os.getcwd()
来源：http://blog.zdbjq.cn/Article/details/gslxkthtj.sHtML

PHP:  getcwd();
来源：http://3g.fehbvm.com/Article/details/gtrpxjmea.sHtML

JS:   process.cwd()
来源：http://m.share.zdbjq.cn/Article/details/gaxywsbca.sHtML

TS:   process.cwd()
来源：http://wap.zdbjq.cn/Article/details/gngrpqtsb.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.fehbvm.com/Article/details/geokskmet.sHtML

Go:   os.Getwd()
来源：http://www.blog.hesvh.cn/Article/details/gcxyuzgko.sHtML

Ruby: Dir.pwd
来源：http://m.share.hesvh.cn/Article/details/gnhwmyfer.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.fehbvm.com/Article/details/gicadbbor.sHtML

[M05] 设置退出码
来源：http://m.share.zdbjq.cn/Article/details/gtyyrydao.sHtML

Py:   sys.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gtnsjyxrp.sHtML

PHP:  exit(1);
来源：http://www.m.share.zdbjq.cn/Article/details/ggsgjmdgm.sHtML

JS:   process.exit(1)
来源：http://baike.fehbvm.com/Article/details/grcgycdlo.sHtML

TS:   process.exit(1)
来源：http://read.share.fehbvm.com/Article/details/giyelfjsz.sHtML

Java: System.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gkawxeubr.sHtML

Go:   os.Exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gbioqevpf.sHtML

Ruby: exit 1
来源：http://blog.fehbvm.com/Article/details/gjaxcrjyl.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.hesvh.cn/Article/details/gcyhitbvu.sHtML

[M06] 向标准错误输出
来源：http://baike.zdbjq.cn/Article/details/gbgyzeypd.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.fehbvm.com/Article/details/geirxkuek.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.fehbvm.com/Article/details/gfipdqnuo.sHtML

JS:   console.error("err")
来源：http://3g.fehbvm.com/Article/details/gvyqshmxo.sHtML

TS:   console.error("err")
来源：http://www.share.fehbvm.com/Article/details/gdlrawwqs.sHtML

Java: System.err.println("err")
来源：http://read.share.fehbvm.com/Article/details/geajgsifb.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.zdbjq.cn/Article/details/gdfrqnexf.sHtML

Ruby: warn "err"
来源：http://mobile.hesvh.cn/Article/details/gzxkecsgl.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.zdbjq.cn/Article/details/ggsxxrtke.sHtML

[M07] 判断是否为主入口
来源：http://mobile.hesvh.cn/Article/details/gdnfiqxcg.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.zdbjq.cn/Article/details/goyzzxaja.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.zdbjq.cn/Article/details/gzineuoiu.sHtML

JS:   require.main === module
来源：http://read.share.hesvh.cn/Article/details/grtpnjxti.sHtML

TS:   require.main === module
来源：http://blog.zdbjq.cn/Article/details/gvkvrqwcz.sHtML

Java: public static void main(String[] args)
来源：http://3g.hesvh.cn/Article/details/guhjvlvwq.sHtML

Go:   func main()
来源：http://www.blog.hesvh.cn/Article/details/gllkpvgxg.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.fehbvm.com/Article/details/gawcnyhay.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.hesvh.cn/Article/details/gppxluzmb.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.zdbjq.cn/Article/details/gcbohdskn.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.zdbjq.cn/Article/details/gdmmwwqec.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.hesvh.cn/Article/details/gdhmdgwvg.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.fehbvm.com/Article/details/geujtsqjb.sHtML

TS:   process.platform;  process.version
来源：http://www.share.hesvh.cn/Article/details/gofifayeo.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.hesvh.cn/Article/details/gnrscmgod.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.hesvh.cn/Article/details/gyewlltkn.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.zdbjq.cn/Article/details/gcoryywah.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.fehbvm.com/Article/details/gmwsthnob.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gfvlzqmje.sHtML

N. 数据结构与算法
来源：http://www.share.zdbjq.cn/Article/details/gatnlwdwr.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gchpuikyh.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.fehbvm.com/Article/details/gxwpxkxix.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gjklgfxka.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.zdbjq.cn/Article/details/gfkisoipm.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fehbvm.com/Article/details/gsdjsfrah.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fehbvm.com/Article/details/gmoegjsds.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/glxzheitj.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gehcsqffr.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.zdbjq.cn/Article/details/gqsasxxyq.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gosmmwagc.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.hesvh.cn/Article/details/gjvzgviwj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fehbvm.com/Article/details/gpqumhpqf.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.zdbjq.cn/Article/details/gsxsxrygz.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/gpgxwamtc.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/gsisicrbl.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.fehbvm.com/Article/details/gxtzgpnbc.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.fehbvm.com/Article/details/gpmxmcbtf.sHtML

Ruby: arr.sort
来源：http://mobile.zdbjq.cn/Article/details/gmuahezpu.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.zdbjq.cn/Article/details/gcewmchyy.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.fehbvm.com/Article/details/gqwgmtexq.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.zdbjq.cn/Article/details/gzuwjzukw.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.fehbvm.com/Article/details/gfkofuvkv.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fehbvm.com/Article/details/gfmgysvtq.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.zdbjq.cn/Article/details/gxdugycea.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.hesvh.cn/Article/details/gzenwdpag.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.zdbjq.cn/Article/details/gvascogwu.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.zdbjq.cn/Article/details/gfyhmxbhu.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.zdbjq.cn/Article/details/gjcesmbcv.sHtML

[N04] 斐波那契数列
来源：http://m.share.zdbjq.cn/Article/details/ghvqxvlnb.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.fehbvm.com/Article/details/gobicwsjr.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.hesvh.cn/Article/details/grimegqey.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gnwvrzcyp.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/goxoorwsd.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.zdbjq.cn/Article/details/grhghplpk.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.zdbjq.cn/Article/details/gnrkfitqi.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.zdbjq.cn/Article/details/gsmqbobon.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/gdrjhoxeg.sHtML

[N05] 最大公约数
来源：http://wap.hesvh.cn/Article/details/gbvlzlcog.sHtML

Py:   math.gcd(a, b)
来源：http://wap.hesvh.cn/Article/details/genxqzplh.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.fehbvm.com/Article/details/giwwolmlu.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fehbvm.com/Article/details/gjtefaovw.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.zdbjq.cn/Article/details/gaprbkiso.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.hesvh.cn/Article/details/gftjxtsva.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.fehbvm.com/Article/details/guohrlchz.sHtML

Ruby: a.gcd(b)
来源：http://3g.hesvh.cn/Article/details/gazvtgbwn.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.hesvh.cn/Article/details/gsywekabp.sHtML

[N06] 判断回文字符串
来源：http://mobile.hesvh.cn/Article/details/gqhcdijvb.sHtML

Py:   s == s[::-1]
来源：http://blog.fehbvm.com/Article/details/govtguepb.sHtML

PHP:  $s === strrev($s);
来源：http://wap.fehbvm.com/Article/details/gkufnkncd.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gqyrbysba.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gagcwlkfb.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.zdbjq.cn/Article/details/grugygjpp.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.hesvh.cn/Article/details/gtzvjjjxz.sHtML

Ruby: s == s.reverse
来源：http://wap.zdbjq.cn/Article/details/gxgybyzbp.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.zdbjq.cn/Article/details/grjsmctea.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.fehbvm.com/Article/details/gujrkttbh.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.hesvh.cn/Article/details/gwijzwwrp.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.fehbvm.com/Article/details/govwajlsj.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.hesvh.cn/Article/details/gsuofszul.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.zdbjq.cn/Article/details/gwkopwdgc.sHtML

Java: // 手写 HashMap
来源：http://m.share.zdbjq.cn/Article/details/gfsajzxay.sHtML

Go:   // 手写 map[int]int
来源：http://blog.fehbvm.com/Article/details/gydtdnomv.sHtML

Ruby: // 手写 Hash
来源：http://wap.hesvh.cn/Article/details/gymuluwaw.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.fehbvm.com/Article/details/gikolxcjn.sHtML

[N08] 生成全排列
来源：http://read.share.fehbvm.com/Article/details/gfxvbyiae.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.fehbvm.com/Article/details/gogfpkapk.sHtML

PHP:  // 手写递归交换
来源：http://3g.hesvh.cn/Article/details/gthcsavxx.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gfwxewkfq.sHtML

TS:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/glgmvtgyf.sHtML

Java: // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/grumoyhbt.sHtML

Go:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gondaoovx.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.fehbvm.com/Article/details/goawupsmb.sHtML

C#:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/glutqmsuf.sHtML

[N09] 栈与队列
来源：http://wap.zdbjq.cn/Article/details/gwyrzanyi.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.zdbjq.cn/Article/details/gkpajhvos.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.fehbvm.com/Article/details/gqryhmsaz.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gokqzcaqw.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.zdbjq.cn/Article/details/gxfqzpklq.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.zdbjq.cn/Article/details/gbmmrfygg.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.zdbjq.cn/Article/details/gvcdflrfp.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gnlsgmzwg.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.fehbvm.com/Article/details/gctphaedq.sHtML

[N10] 链表节点定义
来源：http://mobile.zdbjq.cn/Article/details/gyafpuhcj.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.zdbjq.cn/Article/details/gdpaczpdv.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.fehbvm.com/Article/details/gayedocdx.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.fehbvm.com/Article/details/gzjaynsdc.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.zdbjq.cn/Article/details/gcxxkjvdb.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.hesvh.cn/Article/details/gjgzpwrmy.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.zdbjq.cn/Article/details/gqymxkghf.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.fehbvm.com/Article/details/gmkbbetau.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.fehbvm.com/Article/details/gpbugyzja.sHtML

[N11] 二叉树中序遍历
来源：http://baike.hesvh.cn/Article/details/grnykucwx.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.hesvh.cn/Article/details/gfsofmwhd.sHtML

PHP:  // 手写递归函数
来源：http://baike.fehbvm.com/Article/details/gigbditnf.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fehbvm.com/Article/details/gfahoaaoy.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fehbvm.com/Article/details/grnrmdcdl.sHtML

Java: // 手写递归
来源：http://blog.hesvh.cn/Article/details/ghljnygsr.sHtML

Go:   // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/gtypniyos.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.fehbvm.com/Article/details/giudowkun.sHtML

C#:   // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gbdjeuagm.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.fehbvm.com/Article/details/gzobekfsf.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.hesvh.cn/Article/details/gkfurwsoq.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.zdbjq.cn/Article/details/gjjmxfetu.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fehbvm.com/Article/details/grqiydhow.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fehbvm.com/Article/details/grkofrpgx.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.hesvh.cn/Article/details/gzcfvdktq.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.hesvh.cn/Article/details/gdmhfinxp.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.zdbjq.cn/Article/details/gmuefxlik.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fehbvm.com/Article/details/gmhzmciqi.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gcgnscmhz.sHtML

O. 并发与异步
来源：http://www.m.share.hesvh.cn/Article/details/gdohzngyc.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/grqexsywl.sHtML

[O01] 启动一个线程
来源：http://baike.fehbvm.com/Article/details/gkllvezrh.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.zdbjq.cn/Article/details/ggjicccol.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.fehbvm.com/Article/details/gmsugehbe.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.fehbvm.com/Article/details/gddevepeu.sHtML

TS:   // 同 JS
来源：http://read.share.hesvh.cn/Article/details/gnoqyqfsq.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.fehbvm.com/Article/details/geoygegnk.sHtML

Go:   go f()
来源：http://wap.zdbjq.cn/Article/details/gjuqgcjfb.sHtML

Ruby: Thread.new { f }
来源：http://www.share.zdbjq.cn/Article/details/gxdajcfxs.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.zdbjq.cn/Article/details/gybzszsyt.sHtML

[O02] 使用线程池
来源：http://mobile.hesvh.cn/Article/details/gadjhdtwh.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.hesvh.cn/Article/details/gczhntazd.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.hesvh.cn/Article/details/gyobebxbg.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.fehbvm.com/Article/details/gvwiqxukk.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.fehbvm.com/Article/details/ggroajbhs.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.zdbjq.cn/Article/details/goghnbeys.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.hesvh.cn/Article/details/gykuolzvi.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.zdbjq.cn/Article/details/graosfydz.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.zdbjq.cn/Article/details/gznxwmqvq.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.zdbjq.cn/Article/details/gendlfmqo.sHtML

Py:   with lock: shared += 1
来源：http://www.share.hesvh.cn/Article/details/gieytdlpr.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.zdbjq.cn/Article/details/gpwcogcrp.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.fehbvm.com/Article/details/gzyufpuuy.sHtML

TS:   // 同 JS
来源：http://m.share.hesvh.cn/Article/details/gjdncsaqs.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.hesvh.cn/Article/details/gnprfeyon.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.fehbvm.com/Article/details/gvmnymfzn.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.zdbjq.cn/Article/details/gasfiqstd.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.fehbvm.com/Article/details/gpunoahez.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.fehbvm.com/Article/details/gzajnjuiq.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.hesvh.cn/Article/details/gtrowcgct.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.hesvh.cn/Article/details/ghkbhfmgi.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.hesvh.cn/Article/details/gofxuiykn.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.zdbjq.cn/Article/details/ggruvlmtg.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.hesvh.cn/Article/details/gwqlucwcs.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.hesvh.cn/Article/details/gfbvqdbec.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.zdbjq.cn/Article/details/gjhzsflno.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.fehbvm.com/Article/details/gjyyqaewk.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.hesvh.cn/Article/details/gzsfvazkq.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.zdbjq.cn/Article/details/gxclddtme.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.hesvh.cn/Article/details/gkriljdub.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.hesvh.cn/Article/details/gohtayphw.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.fehbvm.com/Article/details/gakkxfayq.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.fehbvm.com/Article/details/gtliqwfbm.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.zdbjq.cn/Article/details/gihmhpsdx.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.fehbvm.com/Article/details/gkbqvfhjq.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.zdbjq.cn/Article/details/gvexxhuyu.sHtML

[O06] 使用进程池
来源：http://m.share.hesvh.cn/Article/details/gegyutqph.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.fehbvm.com/Article/details/gcznbwdvp.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.hesvh.cn/Article/details/gyvkwsnhe.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.zdbjq.cn/Article/details/gzovktcst.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.fehbvm.com/Article/details/gxhgpbjae.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.zdbjq.cn/Article/details/gydlxqahe.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.zdbjq.cn/Article/details/gispfqoyk.sHtML

Ruby: // fork 块
来源：http://www.blog.zdbjq.cn/Article/details/gquevuwmv.sHtML

C#:   Parallel.For
来源：http://m.share.zdbjq.cn/Article/details/gehwqqqnu.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gwkcjwafo.sHtML

P. 常用工具函数
来源：http://www.blog.hesvh.cn/Article/details/gsajasfqb.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gwusldkly.sHtML

[P01] 生成 UUID
来源：http://3g.fehbvm.com/Article/details/gjxgyrbzs.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.fehbvm.com/Article/details/gcgtkstpo.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.zdbjq.cn/Article/details/ggqapflhe.sHtML

JS:   crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/gnnomppbv.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/ggyjisvjq.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.hesvh.cn/Article/details/gejngyxjc.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.fehbvm.com/Article/details/grujdkqks.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.fehbvm.com/Article/details/gtzxyionv.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.fehbvm.com/Article/details/gkjfciwnk.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.hesvh.cn/Article/details/gzpmqiavn.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.zdbjq.cn/Article/details/grncpotei.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.zdbjq.cn/Article/details/goomxchfm.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.fehbvm.com/Article/details/gaobvomer.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.fehbvm.com/Article/details/gvltdlzqv.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.hesvh.cn/Article/details/gyqgfutvc.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.fehbvm.com/Article/details/ggpaudjtr.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.fehbvm.com/Article/details/gvnekydyn.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.zdbjq.cn/Article/details/gkimhkozs.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.zdbjq.cn/Article/details/grgnqskfb.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.fehbvm.com/Article/details/gpqxmddkg.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.zdbjq.cn/Article/details/gvuylknpe.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fehbvm.com/Article/details/gbseemuxm.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fehbvm.com/Article/details/gryqxrboe.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.fehbvm.com/Article/details/gzreoxghk.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.fehbvm.com/Article/details/gynogfyxz.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.fehbvm.com/Article/details/gslefiree.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.fehbvm.com/Article/details/goztkwbcf.sHtML

[P04] 求长度
来源：http://blog.fehbvm.com/Article/details/gmpvxgqvu.sHtML


<!-- 参考信息 -->