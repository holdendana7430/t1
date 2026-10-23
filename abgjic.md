代发 wailian999

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3iljfceon.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3vqfzjgis.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3gtifxmrv.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3vkntagvb.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3ilsdvefx.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3urdcxlye.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3grxoclnh.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3mdqsvxpu.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3ljwniqgy.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3zloumanz.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3dtktcyot.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3rvokmsuf.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3dxkpdank.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3qdatudiv.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3vnuecbjx.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3vnbwgoxz.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3bqxoskli.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3jrlrcebc.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3ideoqdzp.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3wqikybvn.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3lgaykmue.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3kkuibsfv.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3bkguutyv.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3rkdhphcn.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3djnslpsp.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3sjvgpquh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zmfqildp.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3vomziinb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3asdulhpt.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3jnlvvkaa.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3vsedrhip.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3qdwrewcb.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3hlecuywq.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3daeoqzow.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3zcjsyjdk.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3segvlqak.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3ftjfpeup.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3ovpfyohb.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ytdgrqai.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3svbjiwkz.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3enxwqvus.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3wgsnrwgw.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3mnbevilg.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3tlwjfzib.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3nnpbgmng.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3utcaphkq.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ureqbjap.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3aepzmvuv.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3qcfwuqvb.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3hhjcilhf.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3hmkvaufd.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3trfxcjdn.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3vmbjlgmv.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3mkuwkllm.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3sngbrvva.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3qknzdesg.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3sqwqgmms.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3zvnjcysz.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3kbzhhjpc.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3afbsndrr.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3eurkvtyp.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3ocullell.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3qpybzenw.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3zmkvjcoj.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3zgzbzsdm.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3izqrrxbg.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ctwtddwx.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3qeiqigbt.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kqzutvgt.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dueatnji.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xorjnmin.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3jcbqgtul.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3cogzcrfv.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3qqrbbpre.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3dcjllfby.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3fytsvxrj.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3vwnwlvbe.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3najsdyjk.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3zunhgtqp.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3wiqpoecz.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3qhmljabt.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3mmhpbiak.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3myzvapeo.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3mzjrfxhs.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3bxqpmgtz.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3iktayhbh.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3otewrrfk.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3dwnrhqbr.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3tbwqqqcb.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3qghyeqnz.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3ncqrftwd.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3zzbstiax.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3gocapyjn.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3usctgxuc.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3blhcbegy.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3hhajljqe.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3ghggikgi.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3bvhgslpo.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3qdjpskhd.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3qahtscil.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3qycdsozc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eruefbcc.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3qgvhetbt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kldzizwj.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3tvzruhde.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3fukyoweg.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3xvgbqcbh.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3soctoxgu.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3pxjhqxuu.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ecpsxzjt.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3afglafrf.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3bwrqotgu.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3hgpuovdw.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3rsyyncol.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3wtlhvwkg.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3anuqarqg.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3doowmeuf.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3exacmjaz.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3lflamsbb.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vbfmckvj.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3mhcrllow.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3uprheomi.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3hcknhcyn.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3flyljher.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3srvcqgks.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3ughwjsgz.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3knsmuoli.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3wwpfvnvp.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3zsgkrgzd.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3nstlmlkd.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3oqhqyeue.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3sgvzhebn.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hcwinckd.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3hjtoqtjo.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3pmymlnmp.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3opficwfo.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3gnrlwbbh.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3zxryerbk.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zdcilril.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3mkjssvzc.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3yoptdmid.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3yliwruxr.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3hztlxudh.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3mwtnfwpc.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3xnyrwvdl.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3brsyvupr.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3tmmbsrjo.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ittliyps.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3vgncduer.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3mrjfnxzy.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3eeglugce.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3datzxqfs.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3evbkwett.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3vmpohtty.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3nokyrnsr.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3zgewasez.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3slnravsm.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3onnvwfxj.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3fodnzjgg.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3wwyytldd.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3lybnotzf.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3xlygbjyk.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3ykcekife.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3kispgdip.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3gtxsyaal.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3bbuypsdd.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3asohjwat.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3dgwbqrmi.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wskmyfft.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3pdwnidfo.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3xbyilzsk.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ppgiacql.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3nviyomdp.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3vbgehqiu.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3dlcscqxn.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3uvmjgciv.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3nezusyuz.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3nbsfmnvl.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ebpejatt.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3rzdpvodp.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3iogmihdm.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3ckoqehbz.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3ykdmkrba.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3gdejfzkq.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3ybxhsqzv.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3fxwqjqzy.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3cvgqvyrm.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3bavxwvnp.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3truwgrdu.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3lvkmdmza.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3kdscjawb.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3navczdyv.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3rsdjonui.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3jlfvffis.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3zdpcihha.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3mcgzbmrs.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3ejtnbunh.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3gjlxpyda.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3exjbtmqj.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3yrpijeng.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3hxomwkql.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3bdpyplds.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3kfpsrabj.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3jnkswcuh.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3wjruutde.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3hwlepsvc.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3jfwhunjb.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3srusqggb.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3rlwmwcpe.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3xzuljplb.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3hlbskhlx.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3fjykukfz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ssfsmlei.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3mautvmud.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vnlzclog.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3cxxjocuz.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3nvoeybnh.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3thsaxruj.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3rawqtgaf.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3jtlqfjgp.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3boeorrrj.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3crnrefnz.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3cvzgufim.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3juwzhexa.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3uthwmqgf.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3xyvvkhrb.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3csxudbly.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3ruhpsypy.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3fysxoyec.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3obrgheyy.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3jqzrouro.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3rmfhcjnm.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3iefdwxnu.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3kxuykrdi.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3mznhednj.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3qnhwjxra.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3slrqzqwy.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3pyoqefqu.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3bkwwxjwt.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3fqpvhpna.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3yfakpirk.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3vnrtyphk.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3wiwwdmfe.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3eimsmacc.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3qtrwjpql.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ighmupkm.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3zqojprny.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3hzeghklz.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3dpruhcap.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3msnzknht.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3wsnedmkm.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3ykraefoy.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3btaopssk.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3zcrwnyzi.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3txcoesav.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3bludqxwz.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3ynlayrdq.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3iqnagpeu.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3btaorddk.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3zzbzsgli.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3xcbahsdc.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3kotxxtlb.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3zsubjpfe.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3dghrqfzs.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3betijyuv.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3rycoquhj.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3jsbjqaps.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3wxqjkkjy.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3fpflapeu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vctdgmdw.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3uyvsqetd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gcrolspo.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3yirssaam.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3hhihrqcd.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3izblpgon.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3yrnypncf.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3gvqwfqyr.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3pjeptgwq.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3clwvxhzv.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3ukwolzhq.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3apigjynv.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3sbxyebjv.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3itajpicd.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3fmwbbmzh.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3nsewkqgm.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3faltmbdc.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3pzykdoca.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3ljhxxsma.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dotkmcds.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3sqwvfglk.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3uslqjpet.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3xuhzpkck.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3fzlkijds.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3nhhwjmxf.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jnoxpueu.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3lisdmwwx.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3jwjwdkzs.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3aofytnni.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3jnefpnlu.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3dhgarvbt.html


<!-- 参考信息 -->