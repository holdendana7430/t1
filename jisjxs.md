代发 wailian999

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3ytpgbzrn.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3wvutjjox.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3yaoqvvbw.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3ztqtpbkm.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3ixcfcntc.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3pydvbkbu.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3thrwijcd.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3bmwmlezr.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3cypbiblf.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3wxphrabz.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3migioauk.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3sqoawbln.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3dqmxdoej.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3nvgngajd.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3xzqaxxcy.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3yeeounro.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3tkpslyks.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3ilvucnam.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3rlkarjgz.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3dqipbcvt.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3zdynqyoe.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3tckfcctt.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3jfwdtche.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3kmjbeeya.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3krzujxir.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3donynsrb.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3tqwfkubu.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3ornlybuz.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3rnzxrkij.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3nsohbzan.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lgtlmkcg.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3vwfpejlg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ewaxmgxw.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3auegfahl.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3ruwycavr.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3cyjlrnon.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3atpvbueb.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3ytrmucrf.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3dzydsjyx.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3ijsbmden.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3akxgztrf.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3sqyhtpmn.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3nvrgsjyi.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3jxipgvzc.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3qlsfjphp.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3jpxtadjs.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3hqxsmscq.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3bvufkogt.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3esyyelbb.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3spttmivb.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3xdsbvlko.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3emppjafu.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3bhodxgbk.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3iaxaxwky.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3ezvdsoak.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3dwmlczjr.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3xqbtrkpz.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3hdwblgqo.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3melziizm.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3lkwugehg.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3uyozzoll.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3vufikhti.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3vvmuyutk.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3isppespa.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3adnkcndt.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3xismfclg.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3oixbkkis.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3myjyzged.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3socwiwgs.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3zpceumlr.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zoiatvbr.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3aezoszga.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3khqbqrlz.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3nubwrpsa.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3lspwecvp.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vgbvjfjs.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3xpwiabyz.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3svhuxtwz.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3jtrnzvvs.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3iolnqzls.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3yiqirjvu.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3nhdrbjzt.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3xykipbll.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ffnikjof.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3gmifpkoj.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3wronbmuo.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3rnuaywxy.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3rmaqmxxx.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3hylbmxkz.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3tbtgddtx.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3cdodytzd.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3ghhvrjqs.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3agoiotmi.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3seejovxd.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3esftsyen.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3xiypnqxx.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3govwnxnu.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3legiwzik.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3gceovztq.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3wwsmjomg.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3etjvcwwp.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3yagckbfx.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3qzxfgrsv.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3nuyfmpwt.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3vbfsygtj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fdxwcrbf.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3spkcjdcn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ijjzsqqg.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3mamaxfhs.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3qewepaiv.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3xhbenbul.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3zulahjqk.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3uzerxmcs.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3kugfvrbn.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3gjvkrlzg.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3ivenmryv.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ohwagytu.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3prsczljy.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3rjvjqpkt.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3laeuvnlb.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3uwfmmwdv.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3qwfmulnz.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3whqtlvcx.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3uaxgqifa.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3gsmujtww.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3kneraplq.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3ymojmngo.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3dnzeyowb.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3svipokbl.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3ekjawzuv.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3padaetbc.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3kgfewdnf.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3rnwudqgo.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3unbhidlk.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3ivtnettz.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3tgpxhtat.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3toolcwqd.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3eswxyqmh.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3soaeymmy.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3iauybowo.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3ttcqvzpc.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3kayjupnd.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3heglrduq.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3pngxbmhu.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3pyrqlfbt.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3wfjmlvir.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3znoogwuu.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3rnbmrlfp.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3xnoupnlo.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3huoagqkw.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3qlsvigae.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3uaiulpmx.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3tqhnkufo.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xrdmkexg.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3mkeckaet.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3mnreubiy.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3cmuhszjk.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3lgbtwhmc.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3phxphcse.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3odrjrkos.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3eyuqgxub.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3plbrbyuw.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3tvplattk.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3uukakqca.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3cieysssa.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3acxlcyog.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3pzrxqaik.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3jwyfrprm.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3yongotsn.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3rfkfxsmx.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3gweelszy.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3itrhreqx.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hyeuzivg.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3aenfprhn.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3kyskktjm.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3tturxrmo.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3akgjoxix.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ygxzteau.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3hitsxdis.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3tmhgqdug.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3ofhrekfv.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3ruppdoef.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3htwnnujr.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3snvlrsmg.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3deximtej.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3cuscpdsa.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3lzkzgqyk.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3nbburhxs.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3koixfige.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3uondkzzf.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3auqnvcfk.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3kfdqjzht.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3cdcsmmlq.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3zfalmrzs.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3kukwkxdz.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3tfqovaqh.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3jmuhwmze.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3weolxkeh.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3qmhxfzaa.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3kgztnxwu.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3mzbcnuas.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3ckuznohu.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3wihiexvm.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3tjpomonq.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3dshyypnd.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3coenjzse.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3frsmzjgy.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3iypnqyhu.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3tabflxni.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3vqclnftg.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3wykrxgzn.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3zbnxzipv.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3uoregtdu.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3dmnlxgtx.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3kvlunnoa.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3bsarexne.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iarctwjb.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3stjictrn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yksodqzj.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3kapygqao.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3iewwvlgb.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3yemwhshm.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3eghevzow.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3iannxkol.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3tzdylbkh.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3cconmmev.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3zwhidqnx.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3irpnenkp.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3pnhfxlpz.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3sbncwzai.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3jsshdidv.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3imrstefr.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3qijtjwmo.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3pjlkbras.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3zkyhzary.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3aydtfokn.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3lqdveheg.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3fhrwexlz.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3nkfwzrnm.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3uucxfrnx.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3gvwcimjd.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3urqakfdk.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3dsyiauiz.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3zbjedzua.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3oiaffzkr.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3gftvramt.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3tuptlnrj.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3jrcmswup.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3puecowvl.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3igjzgtul.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3vksknylz.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3uyepqyfq.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3wfjfvrhb.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3sdeuafqb.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3esqmnsru.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3qokfznem.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3plunbjqn.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3zysdurnd.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3xybjfytm.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3jwwayjtw.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3ceeaewch.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3fryaxruc.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3joworhzw.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3eiimtpop.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3jfbokkja.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3ctcrobxe.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3mpvhdrco.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3tgblaezd.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3wontyths.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3uuijlvog.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3zmbtbbbn.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3yxohkjgz.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3cdkxcnfz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qgquypoe.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3nbgejhho.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3njjbrbhx.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3bbusccmf.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3aytrbqoe.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3ttgfplhr.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3xvflknvo.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3golpbras.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3vjtxgxhc.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3lyjpnwhw.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3wfnxnwzd.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3ipybrbes.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3winfmlnb.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3bhqubhmk.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3efxkryjo.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3ugrzomzi.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3vcoaswgq.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3vazcmayl.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3seanvogk.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ghdbyrth.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3tyznzsll.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ttfhxrpd.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3sjuhdnwp.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3ahfdzeux.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3qcgfpwjk.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3fqemnact.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ehcsptog.html


<!-- 参考信息 -->