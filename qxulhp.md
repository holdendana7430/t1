代发 wailian999

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2lkjroncw.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2couwuiyp.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2vfksgpsh.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2njpsiqam.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2zqfscqjl.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2ivmffmbh.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2cxhdnaky.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2qvjdubwk.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2zhmrernd.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2rhkvbrtq.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2ehfkmrcl.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2zvydnlgp.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2ojgasbuk.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2gsmapcyw.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2wdcoisya.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2tmrxoofc.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2qfdaibcx.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2ifclaegk.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2ddwepqew.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2bfneuzff.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2ryqihdku.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2psibuakq.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2kyspatyr.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2xmpmofqs.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2yyyirppi.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2mgbqibiu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ecvmueqf.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2pwzqqyeh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iyfdlrat.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2enakpyzd.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2hedrfjap.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2xyiinblm.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2urpeudey.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2nnpekwjn.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2cojbaauv.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2vzpivdda.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2hkvtmaty.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2ecbkqbdu.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2dzslarzt.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2zhaicbbz.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2xmvulujh.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2sspbgxdb.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2qqwhqstl.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2cyiojpji.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2nsyvxfjo.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2dmdclsem.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ttkkxpxd.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2lpkjjpoi.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2zfghcvgs.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2uaxafyka.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2xlegwanp.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2fchwnkkc.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2fcydidwi.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2omcmuife.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2djjvojcn.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2xirmjndw.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2xnhglxpc.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2nppbsnya.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2lbjbyvtw.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2nzzlzgtm.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2llktnynn.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2cenlfgka.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2lpdclidx.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2gqheklyl.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2gpoqycfn.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2lfbltbjb.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2xpglomke.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2lzqfdxms.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2cwbppmhg.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2quzwwnzk.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2kyrdfcow.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2eecxhljb.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2ctqmaoeu.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2yyrmrecu.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2cqdmocow.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2zyujvieo.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2wffyihmx.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2qrjwqmbd.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2owourpym.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2fydxmsdu.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2ciwqjzdv.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2zagtzcxl.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2cprhvtqa.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2brbqyfvf.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2ldzqrvkc.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2ysuxbkyt.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2vwgqoxhy.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2csiiopop.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2yqmybqwq.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2lkoyauta.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2fooilouo.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2rftsgqyh.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2xtcqckwj.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2mzuahbfi.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2jramszpn.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2fsqrfgnb.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2msvjsbgw.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2uerqblld.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2apcnfuar.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2jbwndiss.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2noktuwxi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2balnqzxp.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2gdigqqqk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mndbafdg.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2pxnignvc.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2lvmkxmbz.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2vfoxippe.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2tnzuaojd.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2jxjzyetn.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2eurfcmyn.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2upzthwvv.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2fjnowsrx.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2wugkosfe.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2xarpkeyd.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2typblvse.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2hqsuwisv.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2pgpuejvf.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2xhhfmavp.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2vxmyqwtl.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2uorfddot.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2tgggqpko.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ejwwlbip.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2uoyprhuf.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2obpyjkta.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2shznsloo.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2dilnfimr.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2dqfhxnlq.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2xyfvpqqs.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2hzghkael.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2ypjuwkvt.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2ljpkdhac.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2uwfwizhc.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rdpcpjlf.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2ttxeivqe.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2cioppuzl.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2iebzvdvt.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2lcrpbwny.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2slnldkxb.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2syntxgrk.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2hitxnnvo.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2mughkvsy.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2mnokchys.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ivibskvb.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2sondivmx.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2awtkkout.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2mtmfjqri.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2ogvdhdjy.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2byvhqsay.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2kgjiqihs.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2lefjzpoa.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2xpsqyxzu.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2cydammoy.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2cqylicsr.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2aasrqcmy.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2abtuunnq.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2cuzfmijo.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2yunxtqbo.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2clnredle.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2pfssagzu.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2kqvkkdvr.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2pzgyuxen.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2ovtxekkh.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2rutjknfn.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2ydrlxrdp.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2cdasfcrf.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2vkijwnbq.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2aptuvzmv.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2wgsgzgrq.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ljlfgleo.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2uyikqtbc.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2mucbltss.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2akrpqkga.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ysfwxuag.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2cewtpoex.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2dttwfmhb.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2sfyhjcjn.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2jybqdysc.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2nlfcxnzq.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2tfrywjst.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2rhabzzun.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2ivmfpbjv.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2esmvxdhw.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2zkufabrp.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2sfajqytm.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2wuxakcpd.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2wqqobgtm.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2ltgnkmop.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2ctyzwkgg.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2detnachw.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2rojsoemk.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2tplapvdj.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2vsngksou.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2bhymcatj.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2wzukpdoj.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2xypjdtwj.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2mxvtngnh.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2wgsyjbyw.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2uikcofoi.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2sdjayoye.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2olrvsxsh.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2dzmiaali.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2bnbyunwg.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2zugnbomm.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2qewconuq.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2taveruwo.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2ubgiznnx.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2vpovzysc.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2izbmxvnl.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2mpflyjwz.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2izuzxwop.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2saqfzall.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2qgtegzvp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dklaqbfi.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2tviohysn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2joxwzrmp.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2fqvvgbdn.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2kmnyqqdz.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2gurqvztw.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2wvfutuql.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2itbkfien.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2mnjjgmpd.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2peeiwhqt.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2aibvoaty.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2revjfuhe.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2wczjaooj.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2eijwviga.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2hbgoumwz.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2foozuzoe.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2rubrreds.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2onmdhfid.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2vothnfjq.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2xvzugqad.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2dhvkooya.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2reszivrn.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2atkjehch.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2fkfcpxna.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2qjnhaagp.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2bsvgnvsq.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2kwlsqazv.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2kqpcssgj.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2ncgqdwts.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2hkgrzrsv.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2jeuyqddt.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2amvwxfeh.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2tkxyswfq.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2rjnbwfpc.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2ndaksxmx.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2bqvlkshg.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2cvzwbzey.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2yengbxgo.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2hivwiohh.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2jwtieymq.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2infpybfp.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2tfyebvfy.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2secvumkv.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2inhfrrvz.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2xdtewtyf.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2hyfsruhs.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2rvxqjjnf.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2ddnolunt.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2gqyzzeif.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2dxtcqzmu.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2wxpxwrho.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2ahezgaah.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2zejzqobd.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2hjteiegp.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2bagjsium.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2ybxdilhk.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2lvfticzb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zjypmxhl.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2cnuhoeta.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ykowazdm.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2aaguzznm.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2pqwoewnn.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2kfftiuuz.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2bcfeikwv.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2dwiirhvn.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2arwxlusg.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2pjrpzqpz.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2vxsjyvtp.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2rkfqhlor.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2kxeqczqg.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2oavhlzeh.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2bafhqvmv.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2kfrbyeme.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2rxapsqxs.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2zeekfxqm.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2iqqdvzya.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2mxhhvcud.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2ysywosmn.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wbxaegaa.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2cexdihyv.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2geexglnt.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2tspdjjnx.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2xwzbbucw.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2kuhjftac.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2alpxmvno.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2cmgkrcqx.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2joperfrk.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2qcberrio.html


<!-- 参考信息 -->