代发 wailian999

Py:   resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/gevkvkrhl.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.zdbjq.cn/Article/details/gcabreboi.sHtML

JS:   await resp.json()
来源：http://read.share.hesvh.cn/Article/details/gvtvelnuy.sHtML

TS:   await resp.json()
来源：http://mobile.zdbjq.cn/Article/details/gdbekfike.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.hesvh.cn/Article/details/glhatlkcp.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.hesvh.cn/Article/details/ggfqftafi.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.fehbvm.com/Article/details/gwgejmplh.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.hesvh.cn/Article/details/gkbwyjyjw.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.hesvh.cn/Article/details/gshqezbqw.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.zdbjq.cn/Article/details/gxmescaqh.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.zdbjq.cn/Article/details/gshblzhoo.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.fehbvm.com/Article/details/gagdbzkde.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.zdbjq.cn/Article/details/gstsxfapt.sHtML

Java: resp.statusCode()
来源：http://wap.hesvh.cn/Article/details/gbahybplw.sHtML

Go:   resp.StatusCode
来源：http://blog.hesvh.cn/Article/details/ggaszowgt.sHtML

Ruby: resp.code.to_i
来源：http://blog.zdbjq.cn/Article/details/guqtccuwj.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.hesvh.cn/Article/details/gqwrntykd.sHtML

[L08] 并发请求多个地址
来源：http://wap.hesvh.cn/Article/details/gygrtkjan.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.fehbvm.com/Article/details/gdqplakwb.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.hesvh.cn/Article/details/grzvalozd.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fehbvm.com/Article/details/gwuuzgczt.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/gbuszlcsi.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.hesvh.cn/Article/details/gkcjzsizi.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.zdbjq.cn/Article/details/gluhdvogg.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.hesvh.cn/Article/details/gervrqcvn.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.hesvh.cn/Article/details/gbjhxflwp.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gxzvqeymb.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.fehbvm.com/Article/details/gvhbvsmtr.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gxpbpkoeu.sHtML

[M01] 读取命令行参数
来源：http://3g.zdbjq.cn/Article/details/gdeylarja.sHtML

Py:   sys.argv[1:]
来源：http://wap.fehbvm.com/Article/details/gdwnkhfch.sHtML

PHP:  $argv;  $argc;
来源：http://blog.fehbvm.com/Article/details/glcmnpkta.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.zdbjq.cn/Article/details/guesegfin.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.zdbjq.cn/Article/details/gwzeogvmm.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.zdbjq.cn/Article/details/guakjymmy.sHtML

Go:   os.Args[1:]
来源：http://wap.hesvh.cn/Article/details/gxosqgzoq.sHtML

Ruby: ARGV
来源：http://wap.fehbvm.com/Article/details/ggbnihdmw.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.zdbjq.cn/Article/details/gthbltmok.sHtML

[M02] 读取环境变量
来源：http://baike.hesvh.cn/Article/details/gjeodkzzb.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.hesvh.cn/Article/details/gkazokcju.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.hesvh.cn/Article/details/geiumrwib.sHtML

JS:   process.env.HOME
来源：http://www.share.hesvh.cn/Article/details/gynwodubh.sHtML

TS:   process.env.HOME
来源：http://3g.fehbvm.com/Article/details/gdflnorlp.sHtML

Java: System.getenv("HOME")
来源：http://wap.zdbjq.cn/Article/details/ghwysbekl.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.hesvh.cn/Article/details/ganyfjnvr.sHtML

Ruby: ENV["HOME"]
来源：http://blog.hesvh.cn/Article/details/gppcfgsmv.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.hesvh.cn/Article/details/gssxedpwv.sHtML

[M03] 执行外部命令
来源：http://3g.zdbjq.cn/Article/details/gdfwdblcp.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.hesvh.cn/Article/details/gkmnbtdcv.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.fehbvm.com/Article/details/gxtxazmew.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.fehbvm.com/Article/details/gzjlaudfr.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.fehbvm.com/Article/details/gvuaykhzy.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.fehbvm.com/Article/details/galhacvtt.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.zdbjq.cn/Article/details/ggcazqivt.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.hesvh.cn/Article/details/gzbxrszmd.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.fehbvm.com/Article/details/gidonljel.sHtML

[M04] 获取当前工作目录
来源：http://mobile.hesvh.cn/Article/details/gwqaqfqhp.sHtML

Py:   os.getcwd()
来源：http://read.share.fehbvm.com/Article/details/gbzefsfnf.sHtML

PHP:  getcwd();
来源：http://3g.fehbvm.com/Article/details/gdmceunbd.sHtML

JS:   process.cwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gbqgvwomz.sHtML

TS:   process.cwd()
来源：http://www.share.zdbjq.cn/Article/details/gggvkkkzs.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.zdbjq.cn/Article/details/gwmeecnwt.sHtML

Go:   os.Getwd()
来源：http://www.m.share.fehbvm.com/Article/details/gnxnzrdno.sHtML

Ruby: Dir.pwd
来源：http://blog.fehbvm.com/Article/details/gcgvmvaia.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.fehbvm.com/Article/details/gtgvalbta.sHtML

[M05] 设置退出码
来源：http://baike.fehbvm.com/Article/details/gjwdfbiuh.sHtML

Py:   sys.exit(1)
来源：http://wap.fehbvm.com/Article/details/gynexnkuj.sHtML

PHP:  exit(1);
来源：http://www.m.share.hesvh.cn/Article/details/gizqhpgef.sHtML

JS:   process.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gxmwwxiuu.sHtML

TS:   process.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gkflynlaf.sHtML

Java: System.exit(1)
来源：http://baike.fehbvm.com/Article/details/gtzwdnfep.sHtML

Go:   os.Exit(1)
来源：http://baike.hesvh.cn/Article/details/gphvlilky.sHtML

Ruby: exit 1
来源：http://m.share.zdbjq.cn/Article/details/gnawrcxfn.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.fehbvm.com/Article/details/gwrazqpaf.sHtML

[M06] 向标准错误输出
来源：http://read.share.fehbvm.com/Article/details/gbhkgliuk.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.zdbjq.cn/Article/details/grjkvrizg.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.fehbvm.com/Article/details/gzannmxim.sHtML

JS:   console.error("err")
来源：http://blog.zdbjq.cn/Article/details/gdiamukdq.sHtML

TS:   console.error("err")
来源：http://www.blog.fehbvm.com/Article/details/gyftbonqg.sHtML

Java: System.err.println("err")
来源：http://mobile.fehbvm.com/Article/details/gjjnvrlka.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.fehbvm.com/Article/details/gmyuxagqv.sHtML

Ruby: warn "err"
来源：http://m.share.hesvh.cn/Article/details/gtfrryxaa.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.fehbvm.com/Article/details/gajducctj.sHtML

[M07] 判断是否为主入口
来源：http://www.share.fehbvm.com/Article/details/gmnglzltj.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.zdbjq.cn/Article/details/gquoavgcx.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.hesvh.cn/Article/details/gedwxjqpo.sHtML

JS:   require.main === module
来源：http://3g.zdbjq.cn/Article/details/gokybmulr.sHtML

TS:   require.main === module
来源：http://baike.zdbjq.cn/Article/details/ggijonpdt.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.fehbvm.com/Article/details/gapduomzw.sHtML

Go:   func main()
来源：http://3g.fehbvm.com/Article/details/gjgniracn.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.hesvh.cn/Article/details/gaxbvqotr.sHtML

C#:   static void Main(string[] args)
来源：http://blog.hesvh.cn/Article/details/gpfeajdzh.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.hesvh.cn/Article/details/ggedjycsf.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.zdbjq.cn/Article/details/gpdyiezet.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.hesvh.cn/Article/details/gwngghwzu.sHtML

JS:   process.platform;  process.version
来源：http://m.share.fehbvm.com/Article/details/girfsziga.sHtML

TS:   process.platform;  process.version
来源：http://3g.fehbvm.com/Article/details/gxpridgmr.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.hesvh.cn/Article/details/gftkeznvo.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.hesvh.cn/Article/details/giqbscyet.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.fehbvm.com/Article/details/gsdxqnvyu.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.hesvh.cn/Article/details/gtdrtwvzk.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gquatpsro.sHtML

N. 数据结构与算法
来源：http://www.blog.fehbvm.com/Article/details/gwrddvldz.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gggewphea.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.hesvh.cn/Article/details/gdccglvye.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gpdykyvyv.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.hesvh.cn/Article/details/gohzqvhed.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.hesvh.cn/Article/details/gaoxqilut.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.hesvh.cn/Article/details/gjmtfdvdg.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gksjarugk.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gabywmscj.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.fehbvm.com/Article/details/gjgisvnru.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gzjrxkjwj.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.zdbjq.cn/Article/details/gxskgtlrx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fehbvm.com/Article/details/gkowxdfkt.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.hesvh.cn/Article/details/gjywytenu.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/gtbjmctib.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/gofmtscbd.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.hesvh.cn/Article/details/guhqraine.sHtML

Go:   slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/gpyamcznx.sHtML

Ruby: arr.sort
来源：http://baike.fehbvm.com/Article/details/gvabgfdtx.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.fehbvm.com/Article/details/gnuvyvnrr.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.fehbvm.com/Article/details/gnsdorxzq.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.zdbjq.cn/Article/details/guwvecvlz.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.zdbjq.cn/Article/details/gklaakoit.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.zdbjq.cn/Article/details/ghxcwrult.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.hesvh.cn/Article/details/gqhlfebus.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.fehbvm.com/Article/details/githwdvkw.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.fehbvm.com/Article/details/gmbizpkee.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.hesvh.cn/Article/details/gsfmtihhq.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.hesvh.cn/Article/details/glxitktob.sHtML

[N04] 斐波那契数列
来源：http://www.blog.fehbvm.com/Article/details/gumiojrrh.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.zdbjq.cn/Article/details/gljfusqlj.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.fehbvm.com/Article/details/grleqcbpf.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/gtfjocspl.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/gkcyibkgy.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.hesvh.cn/Article/details/gphklxqfl.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.hesvh.cn/Article/details/gqkkmwjtf.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.hesvh.cn/Article/details/gillzsxsx.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/gwulcvkqc.sHtML

[N05] 最大公约数
来源：http://baike.fehbvm.com/Article/details/gprrybcmm.sHtML

Py:   math.gcd(a, b)
来源：http://wap.hesvh.cn/Article/details/gqwrkuolh.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.fehbvm.com/Article/details/gnzznmnly.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fehbvm.com/Article/details/gcopsbnuw.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fehbvm.com/Article/details/gbftnlgrl.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.fehbvm.com/Article/details/gkxekpsct.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.hesvh.cn/Article/details/gapdeaarj.sHtML

Ruby: a.gcd(b)
来源：http://read.share.zdbjq.cn/Article/details/gwdfrjnvw.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.fehbvm.com/Article/details/gnniftgke.sHtML

[N06] 判断回文字符串
来源：http://baike.hesvh.cn/Article/details/gyjamkmer.sHtML

Py:   s == s[::-1]
来源：http://3g.zdbjq.cn/Article/details/gvhomdukn.sHtML

PHP:  $s === strrev($s);
来源：http://wap.hesvh.cn/Article/details/gyjojwhqq.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/galxsxdrt.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/guoconkds.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.zdbjq.cn/Article/details/glhpymacw.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.hesvh.cn/Article/details/gdfawwvgm.sHtML

Ruby: s == s.reverse
来源：http://www.share.fehbvm.com/Article/details/gkcpqnnik.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.hesvh.cn/Article/details/gpmziqvnz.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.hesvh.cn/Article/details/geabfxlwi.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.fehbvm.com/Article/details/gbgcipwvw.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.fehbvm.com/Article/details/ghuqodlxt.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.zdbjq.cn/Article/details/ggrnoodbk.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.hesvh.cn/Article/details/gpbqttzpt.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.fehbvm.com/Article/details/girwnbegl.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.fehbvm.com/Article/details/gzocuykht.sHtML

Ruby: // 手写 Hash
来源：http://read.share.zdbjq.cn/Article/details/gzhkudngx.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.fehbvm.com/Article/details/gqbarlzhr.sHtML

[N08] 生成全排列
来源：http://www.share.fehbvm.com/Article/details/gmfznhteb.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.zdbjq.cn/Article/details/giyatascc.sHtML

PHP:  // 手写递归交换
来源：http://baike.hesvh.cn/Article/details/goisfqvji.sHtML

JS:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gamwvznyo.sHtML

TS:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gnnoycoft.sHtML

Java: // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gpeuiicke.sHtML

Go:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gtoxxgwkl.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.fehbvm.com/Article/details/gtzmryjrr.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/grxtoxjed.sHtML

[N09] 栈与队列
来源：http://blog.hesvh.cn/Article/details/ghwgtvkfj.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.zdbjq.cn/Article/details/gcfvazyhw.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gzusfrqvb.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.fehbvm.com/Article/details/gifdtnbmp.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.hesvh.cn/Article/details/gulrfuvfq.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.zdbjq.cn/Article/details/gsbmszmfz.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.hesvh.cn/Article/details/gnkxvwwzf.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gyhorxjje.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.hesvh.cn/Article/details/glyxvcgnb.sHtML

[N10] 链表节点定义
来源：http://www.blog.fehbvm.com/Article/details/ggxqfymsq.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.hesvh.cn/Article/details/ggrvszqyx.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.zdbjq.cn/Article/details/gfcdtzcia.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.fehbvm.com/Article/details/gvwgswiyc.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.zdbjq.cn/Article/details/gqdoqvfwx.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.zdbjq.cn/Article/details/gvmtymkql.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.hesvh.cn/Article/details/ghadtzsdd.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.hesvh.cn/Article/details/ggzoytekb.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.fehbvm.com/Article/details/gtwvqyprq.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.hesvh.cn/Article/details/gqyeeejju.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.zdbjq.cn/Article/details/guzutfkln.sHtML

PHP:  // 手写递归函数
来源：http://3g.hesvh.cn/Article/details/gnxxqslan.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/gsiuocqrm.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.zdbjq.cn/Article/details/gvvggafws.sHtML

Java: // 手写递归
来源：http://3g.zdbjq.cn/Article/details/gaahnvkoy.sHtML

Go:   // 手写递归
来源：http://3g.fehbvm.com/Article/details/gwoyceask.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.fehbvm.com/Article/details/gfclfmghr.sHtML

C#:   // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gonenyqsc.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.fehbvm.com/Article/details/gwhupncmp.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.zdbjq.cn/Article/details/ggktguzsz.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.fehbvm.com/Article/details/gfzphzanu.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/gbexssuer.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.zdbjq.cn/Article/details/gdzbyrfuj.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.zdbjq.cn/Article/details/gxcjzaler.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.fehbvm.com/Article/details/gplbepwxy.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.fehbvm.com/Article/details/gbwdslady.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.hesvh.cn/Article/details/garholckh.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gwijfljve.sHtML

O. 并发与异步
来源：http://3g.zdbjq.cn/Article/details/gnjqmdcxy.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gjlebthly.sHtML

[O01] 启动一个线程
来源：http://www.m.share.zdbjq.cn/Article/details/guqhwhybp.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.hesvh.cn/Article/details/gasyohzvg.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.fehbvm.com/Article/details/gkplxjhit.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.hesvh.cn/Article/details/gprumuuxe.sHtML

TS:   // 同 JS
来源：http://www.blog.fehbvm.com/Article/details/ghbwlgres.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.hesvh.cn/Article/details/gaszsslct.sHtML

Go:   go f()
来源：http://read.share.fehbvm.com/Article/details/gcisrbdvc.sHtML

Ruby: Thread.new { f }
来源：http://blog.fehbvm.com/Article/details/gzrgnlzqx.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.zdbjq.cn/Article/details/gdepulikv.sHtML

[O02] 使用线程池
来源：http://www.m.share.zdbjq.cn/Article/details/gyuxkodeh.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.hesvh.cn/Article/details/gtazpxzxr.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.fehbvm.com/Article/details/gpdbnstue.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.zdbjq.cn/Article/details/gthpxkvzh.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.zdbjq.cn/Article/details/gexclkogg.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.zdbjq.cn/Article/details/grdwsdlvh.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.fehbvm.com/Article/details/gvndtqslv.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.zdbjq.cn/Article/details/gkewwvzfl.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.hesvh.cn/Article/details/gnhokiapq.sHtML

[O03] 加锁保护共享数据
来源：http://baike.zdbjq.cn/Article/details/gxeztjzjd.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.fehbvm.com/Article/details/gotgmguls.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.fehbvm.com/Article/details/gymacjdiy.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.zdbjq.cn/Article/details/ggusjbqff.sHtML

TS:   // 同 JS
来源：http://www.blog.hesvh.cn/Article/details/gmrrdjbaq.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.zdbjq.cn/Article/details/gvhokcmxl.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.hesvh.cn/Article/details/gaknfkuuz.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.hesvh.cn/Article/details/gnnfbsuei.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.fehbvm.com/Article/details/gkrqkigwf.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.fehbvm.com/Article/details/gsdiklwoh.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.fehbvm.com/Article/details/geloockqu.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.hesvh.cn/Article/details/ggpylaumq.sHtML

JS:   async function f() { await g(); }
来源：http://3g.zdbjq.cn/Article/details/goargvtbk.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.fehbvm.com/Article/details/gcitxkolg.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.hesvh.cn/Article/details/gajinnopm.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.fehbvm.com/Article/details/gnwdcplet.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.zdbjq.cn/Article/details/guutvqqmk.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.hesvh.cn/Article/details/gpapkkpam.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.zdbjq.cn/Article/details/glvduzdvk.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.zdbjq.cn/Article/details/gjfgywdrr.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.zdbjq.cn/Article/details/gmcqougyi.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.fehbvm.com/Article/details/gnphufkqp.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.fehbvm.com/Article/details/glrarayef.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.fehbvm.com/Article/details/gewnaeucz.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.fehbvm.com/Article/details/goezxnurz.sHtML

Ruby: threads.map(&:join)
来源：http://wap.fehbvm.com/Article/details/gdtsmpgnf.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.fehbvm.com/Article/details/gzlecdket.sHtML

[O06] 使用进程池
来源：http://wap.zdbjq.cn/Article/details/gryqikrqh.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.hesvh.cn/Article/details/ghkbmylfx.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.fehbvm.com/Article/details/gxxgyflxt.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.fehbvm.com/Article/details/giyjukpmi.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.hesvh.cn/Article/details/gvbfsljeu.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.fehbvm.com/Article/details/ghialuyrz.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.zdbjq.cn/Article/details/ggblqfihz.sHtML

Ruby: // fork 块
来源：http://blog.fehbvm.com/Article/details/ggerrtuuk.sHtML

C#:   Parallel.For
来源：http://3g.fehbvm.com/Article/details/gpltvzprj.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gurunmlgm.sHtML

P. 常用工具函数
来源：http://blog.zdbjq.cn/Article/details/gdgnhmsqc.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gioruhzwk.sHtML

[P01] 生成 UUID
来源：http://www.blog.fehbvm.com/Article/details/gdfjtcscj.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.zdbjq.cn/Article/details/gobnoqgqy.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.fehbvm.com/Article/details/ggrughaet.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/gvpoonqeh.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/ghddzqxyb.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.zdbjq.cn/Article/details/gqsjkvegc.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.zdbjq.cn/Article/details/gxxsihwur.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.fehbvm.com/Article/details/gyqtelnyf.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.zdbjq.cn/Article/details/gkutqrvgj.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.fehbvm.com/Article/details/gdyujwpxg.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.fehbvm.com/Article/details/gudwowdkv.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.zdbjq.cn/Article/details/grezmeaba.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.zdbjq.cn/Article/details/gnlxcmrph.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.zdbjq.cn/Article/details/gnxbrrlea.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.fehbvm.com/Article/details/gffkkkjnt.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.hesvh.cn/Article/details/gdyrmlorg.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.zdbjq.cn/Article/details/gtvmjavby.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.zdbjq.cn/Article/details/gtabniwwu.sHtML

[P03] 生成短随机字符串
来源：http://www.share.zdbjq.cn/Article/details/glypocijp.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.zdbjq.cn/Article/details/gtseftqza.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.hesvh.cn/Article/details/gfucihiho.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.zdbjq.cn/Article/details/gtjqpgzwb.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.zdbjq.cn/Article/details/gfivwelin.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.hesvh.cn/Article/details/gqdndgwwo.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.hesvh.cn/Article/details/gehajszfp.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.fehbvm.com/Article/details/gafkhbapl.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.hesvh.cn/Article/details/gmxxunerz.sHtML

[P04] 求长度
来源：http://3g.fehbvm.com/Article/details/gqtzufgty.sHtML


<!-- 参考信息 -->