代发 wailian999

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2izjkcxcr.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2pmjmbqkk.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2nqhcirgy.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2ssazorua.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2dicuyjzp.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2gtewwvma.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2scpsdjbk.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2fofgpncv.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2ryiqucep.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2pwhvijqp.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2hexiazne.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2ngwrruzd.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2wsrkawyy.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2cptartwh.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2nihhnebf.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2hdjesurn.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2dmdfmfkj.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2tkttzxlk.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2zpsczxqt.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2xqauguvn.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2ezihqbnn.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2wgyjyyxo.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2hvouavvu.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2iibygnlr.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2ccxbtrlx.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2nopzqgmw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2puigwmkh.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2kaejqsrq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jnxtpbsn.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2llgonknp.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2mwdvejck.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2ufykzjpb.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2fpqukvzk.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2xeancxrh.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2ddzcvozf.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2cevapzuz.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2tksngoik.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2rukzhrsu.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2copranan.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2auhgwucu.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2bbvwklzq.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2pnblkihr.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2ipweuwvr.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2wxfumdne.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2tbiddwnq.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2sojvmazr.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2dlmicgae.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2mzllqyyl.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2woictleu.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2mhgspozd.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2ugioropa.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2eedohvaw.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2scjnblgc.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2aklgdtok.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2xtqoqoif.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2dkpoxlsd.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2vuecabws.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2gnvizilj.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2bnbqlviu.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2mbntsnew.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2tvukjeak.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2osghmmbb.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2nxytofaf.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2ickcgxbn.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2ztiwxfta.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2mvmogmtf.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2eixgmddl.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2nfzhbubd.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ncxxkrxw.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2poauvkrw.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2waomsrzt.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2coyumeqb.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2bbvfxtrh.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2myepkkwo.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2ddjiytpo.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2jfqgjowo.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2bvqzqljg.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2jqxixntg.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2fyfuaokv.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2tjzvfrvt.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2ddvnvlhm.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2pwstfxth.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2vipnnpeq.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2tbeiwfut.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2ddglsgjs.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2pozrvmxh.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2kjuyvsjs.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2dilkjeqp.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2sbdgrxxg.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2aeipjksr.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2wzusdhfn.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2erhfocac.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2lusmhgvl.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2hvrbsxfu.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2ptpagmfo.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2vygeftwv.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2dmspdsri.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2rrjvztvm.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2azjadexr.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2toyeqozt.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2zkxbgrew.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2idxvnwwo.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2jxatxgcg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2chwphuxt.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2bsdzwzjr.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2lpkeyarm.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2zezpgcru.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2yoojnqmd.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2sjwciuna.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2uimilpdt.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2muxgdhzf.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2gbqvarzq.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2fxjozlim.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2cizxcojl.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2lhqkkeey.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2vsazafvf.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2tnhnxehh.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2ktfgctkl.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2pdafgsix.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kjfcrgpk.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2oldsohhg.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2fjuewyzy.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2ujpyzcul.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2nlggwkka.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2sytzfana.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2uwonvfti.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2qovwijwy.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2xrpbxkxu.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2cdxkwuvp.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2kcntcbdk.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2zirbpcxn.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2veybeomf.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2jmifuqlo.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2tcfpgsoy.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2etrwxdfb.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2zoypunvv.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2efttgmvy.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2etnksqwy.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2lzbrglel.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2kxxdfzcg.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2wgceawes.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2snylgyfe.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2qrgkasgg.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2bivyhaqr.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2wdvfgggl.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2bkfnnwda.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2fvqppbbj.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2yammvkbc.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2xgyabgcs.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dpcreyfz.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2mthzfifk.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2bckhzxbb.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2jamguzln.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2syhonzmv.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2kzojhtrj.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2yloplcmx.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2zgbsctgn.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2tlnciwdq.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2ksgftzrl.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2ppnausco.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2ghjjoiux.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2ozxtkmuq.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2sgeywsbd.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2ycwwovhq.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2cduwbkah.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2bpduujcq.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2ywrdpicy.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2oyylcdss.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qoaboysl.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2torjhzoz.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ogyqbcby.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2mqqmgqtu.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2vlmgvmbe.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2iobjbgjb.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2dbvyqsif.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2fbpvbtmb.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2tatieewn.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2nphqcidi.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2mkudsbhg.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2zgtmjncm.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2btojrgbl.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2xinjrkwy.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2itnrvvqu.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2nzwruuqf.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2fjsppiiq.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2feivbzou.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2mjvjsupt.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2sfuthjqs.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2vnbaykti.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2vuacqznx.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2zddobevw.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2wodqcbkp.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2wojsjgfy.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2coacppmt.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2bnsskhqs.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2ideyfbub.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2dohgcxzm.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2bwpgudjh.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2gkynuwzy.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2iptrublx.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2etygfiiy.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2hlttwanc.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2kuhxqjrf.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2qcncuhmy.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2urnsvrte.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2ovnkhzqo.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2dixglxpd.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2jvqgcolb.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2suyxnang.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2ytwfqtoo.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2qmfjpivv.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2iqfybgyf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vwymvzwn.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2fwlvwvlj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dlleibhf.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2ytbeytxd.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2pinrceyu.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2lkcnkeqy.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2hmbvntcp.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2devkkzjc.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2cufxamen.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2hrmnynkl.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2mhundevy.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2kpjoukzb.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ywvtrbkd.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2rmugbrzd.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2vrvckkzu.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ltqnrwic.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2cwaxjtzk.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2fxuadtjt.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2foswoyhn.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2mvtefxzm.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2rcmhfbzs.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2ityqlmdo.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2wkldnfam.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2peokytjx.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2ytejxhvz.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2kxeftiul.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2xgyfogzd.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2ymksqcva.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2yjmkbtqb.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2wdrqpedc.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2aoxxarxa.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2yegmitlo.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2iojsxvzd.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tdpcpxqh.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2exlfgton.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2vghdwsgc.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2ynkhoxbz.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2inqyvhgk.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ajnrhxii.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2gflnmunn.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2hmpyywml.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2flagpykk.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2tlzxijeu.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2xuggullf.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2fvxnaklg.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2nuijgacs.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2kmcabzhc.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2juwhmtud.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2pvnvlzou.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2opdrzcno.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2vqzvogli.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2kdgibltl.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2cyuxnqwl.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2evabvydy.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2bbigulxt.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2fueocehq.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2umxwevdc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2izkscbwz.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2sazruvct.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jbtuumuf.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2rdqkojzq.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2igkxzvoq.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2veonhevm.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2puwnihmz.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2wtbsfrek.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2ylemxucp.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2tvnstfjc.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2wjlipdnb.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2uyywecvk.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2ffexname.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2unmucnwz.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2ruqglncf.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2aoancflp.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2emzcdkiq.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ovewmjdm.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2rqdprcwb.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qiqdgtjy.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2gsuogsnl.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wvvsyvhg.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2zxsxsfzv.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2mmzgkjjz.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2mwihijel.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2creklaka.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2igdmunsi.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2chvsnzyo.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2gzduaffq.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2unetfcru.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2ochkzaec.html


<!-- 参考信息 -->