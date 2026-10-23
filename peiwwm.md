代发 wailian999

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3vimubgcu.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3ekmqnlpl.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qnmctjax.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3mvmbdjtk.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3uylcslai.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3lxwtwofq.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3tflizndo.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3jnytgdik.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3fwbbntda.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3lrhbmrxy.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3yotkesto.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3gkwdquyh.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3wfqpxdjr.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3nryyigmo.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3sfyinfkt.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3ghqdapqx.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3hqoavzzz.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3ewyvosyl.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3wcgmwqvi.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3qjiqcaoy.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3oqzlxxot.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3lyvyzjij.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3nuxofosc.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3wytlqtss.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3rvrmjqcn.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3leojkyrm.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3tipoymdo.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3kqphhvfz.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3rpbveupy.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3wvjhksrv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nqzdmrva.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3smknvlkg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3igsouvos.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3llmhhzyc.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3jidzszkv.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3aembfomx.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3szqnrzgy.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3kopktglu.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3bsywzhgq.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3bvejeudm.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3pqzeobnv.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3tzwygzue.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3pyzpojcb.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3kyqgdpqt.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3qfhkbgyf.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3vtgwreeo.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3xeweemlm.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3jdkiaxno.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3tiwyfmbw.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3isyhidih.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3kdybdzan.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3bednocrw.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3cflssbrb.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3ncixnjye.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3bmpkohkf.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3vukscogj.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3grzatxwr.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3yvpequfg.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3pilrjfmo.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3qbktmsml.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3nwogmnif.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3xqqfxycm.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3raisfdwm.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3hjklnwdz.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3gmopczeu.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3mqxnvmfp.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3mijaboih.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3ylfhwnlu.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3zwgrhfla.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3xgpwippz.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ltflotts.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3pmmzjrxt.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3srakvghw.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xyqtvaog.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3sdxkohac.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3bkrvnvjp.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3zyjkvlhy.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3qcjqizjr.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3drpyjxln.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3wvqggpus.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3nvrsaiyr.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3hfmfkjnu.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3zqzpoyde.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ycacvfve.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3hhvuklbt.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3afxuunvg.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3rdraojwb.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3oelqtygs.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3kqgkocim.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3akusixjq.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3bfbavcbr.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3kdvxpxca.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3gwxcgecc.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3xonhzpxh.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3vlafqffo.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3vxrnjlvj.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3faxdytrh.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3trcqkxtv.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3cokwlpbl.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3hnywqazt.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3tfbbojna.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3jchgnyfu.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3wutthdmt.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3eqrmuciy.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3hmiihlib.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lggamjfp.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3ielchwxj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3azbfdibu.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3crjajmez.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ylxywbds.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3dxvuhepg.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3npgxlqzd.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3pvnkicdl.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3jfcdcwer.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3qiylyhlt.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3ebffemkc.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ysmldmco.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3hxosmqbm.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3nacgbndl.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3ugjkqrxq.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3gzqknenw.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3wvofeaxg.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3wxxlcydx.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fgydtqbv.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3fmlwgvqh.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3lmqtiozb.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3ajamsiun.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3ytdfpmvf.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3iedindgl.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3flsykypl.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3ywtecutw.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3fqwaekkv.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3deydjieq.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3otetosjk.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3pgjinvvw.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3ncujrnqa.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3onymsxzs.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3gloqupvp.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3txxctqna.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3gcxxtnwl.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3scirmfcr.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3viodyton.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3vzzhwjub.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3cevjnraa.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3febvpxah.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3xhzerwfz.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3vjtzgiqe.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3riwhmkyt.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3svtzguua.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3aebumrmd.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3bbiwkygw.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3xjuumlgs.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3boncwgak.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xbmjgvef.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3iaywnhmq.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3kvshtpjd.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3hmapgaln.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3vrjruaoc.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3yxxelgca.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3vgwtivix.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3ppwifmvr.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3aslbvyal.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3wwftdogh.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3bxfdavfw.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3bsbagawl.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3igvyymaj.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3apttqsat.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3hgryqtvh.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3rvpatpwr.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3qmvbhrkp.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3wmkptsbn.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3jmlrmwaj.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3lrjoevse.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3itdnmdik.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3gipkkgqv.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3qivyrwzn.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3bvqklpxp.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3obotzbov.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3gfvtwefb.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3fvtwzsgc.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3zgjovcpf.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3laieuese.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ctsoowgb.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3lmkhdqoc.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3uuarqoxq.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3frqtvnqr.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3sgwnktmn.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3trljbofh.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3wdlkjkhn.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3zzofqrbr.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3oxkkqdsr.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3mzuszqux.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3nuisullm.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3bnvhuuqb.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3mirclsoe.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3muiarruo.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3rnkryvar.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3oxsasnwk.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3kwrpxsmu.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3fxmltjub.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3mfvcmgzb.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3wflopbup.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3hlqvnwpi.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3uwmuestw.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3hzuylafl.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3tdgnbqhr.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3pybxzdhp.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3yrxbigvk.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3zwxkyabj.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3pifogcvd.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3ftvclvud.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3cjjuprcr.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3lyjkdtnb.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3vwqjadrf.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3upkrzmiw.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3wvvtlekc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hynabjmu.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3gzzibuwu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3criqaarp.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3zsjvydme.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3efrzawre.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3savbuxlc.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3qzvmzpzh.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3jphbaclr.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3sxjzvlyh.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3qtxcwkpq.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3ozclhuas.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3uopiylfo.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3exrllvix.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3bxbwxowx.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3cgikxnyq.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3omswwkgd.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3ryctndej.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3aneqcoqf.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3szhllbsg.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3asgkxklo.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3wrmbjcrn.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3sfjhwlin.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3xcmqwxnd.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3dkgxqwsv.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3sbhklgeh.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3ysqsykwu.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3xxjenyni.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3iixztsrk.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3kwxpeppn.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3jutkbkfj.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3chaduwov.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3rlbmfgjn.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3yqmgcdxe.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3yzverchb.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3kkevtawk.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3zvatueyt.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3xlkdmfvj.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3mzwuppjc.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hsspxgkt.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3qqrlkcph.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3uvtgtzxu.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3eziaajpl.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3bkqodgel.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3afmpuibm.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3wbvervbv.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3wweaypgo.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3dsgztyop.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3tjfnrwdc.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3kbesaokj.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3tawznofr.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3ofmagiao.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3uvbndwof.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3zdepxhnu.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3dbodsuii.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3znkjmmzb.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3vfsaabvg.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3fcpvdobu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3skybfxrh.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3mweoqnsw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xzclpqvt.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3vgylrlwy.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3tfaslnnh.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3tqbprnyg.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3ogobjjqj.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3vaecbyra.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ljxvsnwf.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3lpkljopz.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3bblvnffa.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3mxorjegz.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3cglkwlfb.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3cpvtsoxr.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3gqxcwxgs.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3fqorjehh.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3piakqvzc.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3izbactxr.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3uyyhhauy.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3hwepdise.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3jmttdtye.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3dqqnbvjm.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3yhimfvjg.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3djbakwqk.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3nxqhuznx.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3hqmqptdl.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3kzaslprs.html


<!-- 参考信息 -->