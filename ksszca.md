代发 wailian999

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3dshskloz.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3dxspknli.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3huirckzv.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3dcjojprw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3hhjhcphs.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3bfqrxwgw.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3jouwwsbu.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3heevjfga.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3vdeigynl.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3ycplsqcv.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ohfqgxfw.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3vqydenjx.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3eejiiegb.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3amxzhvxv.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3hlovyvuj.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3ntxnitxo.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3gclnfygn.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3rxjlxadb.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3ufkyhooz.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3xiwiprin.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3otvuozbu.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3okhsoelk.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3ysfgpreq.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3xsjpolsd.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3lolejpfw.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3hifaloqs.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3zdsufwgy.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3qyzdfbgo.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3toxleodf.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3yxxgypms.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3njbcxivw.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3knhdvnqk.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3nqgwseft.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3vvwpcdiq.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3pqploctb.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3dlcppusm.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3ebvlrnxe.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3lgopeqqe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pxotfopq.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3wbtropqa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ryiiefxf.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3bxjgghdo.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3vpucxnsd.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3tbcgaeor.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3gxczurwc.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3gunyasuh.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3wlbgqzpx.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3frjbodeu.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3qrmrhagu.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3zsvyhgmc.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3ukynlvil.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3mxdnwztc.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3xdhdfmco.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3qeaxuycy.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3gnjbvvnk.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3dpeargki.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3kdpmegnc.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3tgnzwsbi.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3wmikscpy.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3hplxoczf.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3gdgzvvrj.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3quglfdoa.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ygmfldnm.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3qhgqoxgc.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3fcihuzbc.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3vqduvnmq.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3njamtdwn.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3ptwyaitr.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3ndehjaer.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3mfdhxmgh.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3hwfvaidz.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3jbsxgkte.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3onjlciwb.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3pyrnuvso.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3tmnjlytn.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3knkwuxyd.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3bvsipbzh.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3laplsjyn.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ifvrhraq.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3syjybpvp.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yoixyftt.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hwpehmeq.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3jqmysrrl.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3waxvbrye.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3qpenrfnz.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3gstzquaf.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3nimkrtjk.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3dgckkykk.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3cvtexrxv.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3qlusumhp.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3ndxcddgs.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3gouxuudp.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3mrqempgq.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3kaorhtqh.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3efplsoyd.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3weeosjyn.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3zlovqija.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3qbqbwtog.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3wrcjycxh.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3ammfnvyh.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3ufirtgpr.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3bnushryu.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3ayymdxmp.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3duouxbzf.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3rrquhcfh.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3hxerriis.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3divfkgoa.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3bvblhjxc.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3stwwloon.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3kbplunrd.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3bsfgqduy.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3cbcnkxlp.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3lnhbhvse.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pazckefx.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3ieqrucqx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3havamzyj.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3phmxfkrt.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ctfqjvny.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3hedhdums.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3uhfvezgl.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3tjeyobpz.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ehsegdck.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3pysdqiuk.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3zpisyncb.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3fkacouha.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3imztlklt.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3xrmnlmdf.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3iotkftxs.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3higggaoz.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ccvsiint.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3hdntthpg.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3nlwronpz.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3dejbbyye.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3xdudkjjx.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3yvmnlezg.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3cgizyflh.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3lzawekgs.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3mbovkypn.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3ksbtczwh.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3pawjboad.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3pbvivzva.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3dcxqtful.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3yfarmelz.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3akshncax.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3ijbnqwrx.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3knsoxbmc.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3uryrgyso.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3kgpurfsr.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3gftlxxsu.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3rbwlikuz.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3axqnpqqi.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3zqhdwtgj.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3rrxljjdz.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3gtuzvrlw.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ngfynxvq.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3cubimiac.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3azqvrkgc.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3ksksdnca.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3wngnwjkb.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3vswthirc.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3kwafdvnm.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jsxspstl.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3euhpsorc.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3rcwkggyj.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3svrycljo.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3tfxklatb.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3ujqzfuke.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3hiffrmyp.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3dztnrzki.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3wlpomhhx.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3uadcreep.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3juesqvuf.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3zfqrkhdp.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3btrvcqqf.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3czozgvtx.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3cxjucyan.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3nxqwmurw.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3wdewpoan.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3wyzaknif.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3wybsnpfk.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3xleapxdr.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3wgudgqvi.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3yskovhva.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ulfzvjgv.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3mqhihyrf.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ruhfidgv.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3nftpajya.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3iwuahxif.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3ewfrbxbo.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3xxurjxdk.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ubrmqbuu.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3jlizxvrk.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3tlkiufwz.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3udoaxyuu.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3lrgnqvrv.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3nshqgixt.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3isftsbkr.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3rmpfmcpo.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3bzdefhvk.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3qebvlodb.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3erfnjsqo.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3zdtdzlgz.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3fnpfmrpr.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3wlykwcoa.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3mcqefbbw.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3boehouab.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3luakkxgs.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3fqketiyo.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3zrdmrzsi.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3rbjzuwmh.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3zpuihyks.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3mclhdcnk.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3seoeyfmr.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3kcffjpib.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3hfecbdll.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3dhrjlisr.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3whorubap.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3vdmeyzms.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3hwwjkywm.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3xwvwjbiu.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3diamvges.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3tslxogwr.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3fxxmriim.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3kojinbmr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3euuamgyj.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3ninonsgk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kcgextdu.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3lmeeqmhk.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3ntqzpoie.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3ptrjbbro.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3nlujdqek.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3sqrgbzkf.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3qqwzbusl.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3xdvgwfxl.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3dagdnaiw.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3pswpclsv.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3jsvhxgoe.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3gvbjttwd.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3hhgrtfco.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3ickmxmgx.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3umjbcfmz.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3meqmumdz.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3gbgpdewf.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3omudqjtu.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3djoiobai.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3prhxiiya.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3viupxfac.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3ngdfcfhv.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3miealoce.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3caisxzcs.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3gafvbtfi.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3kqaovpzs.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3beuzdrbz.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3vleybqfs.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3cybmkyxr.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3fydclpwb.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3wjscblxq.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3gowzxjbq.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3sfrsekhp.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3iutsftti.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3wvowgvyx.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3pmgumpva.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pujhorty.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3wmahmgix.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3hkuhbchs.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3jpryqfll.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3ezbrokax.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3wdsmknob.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3wzzcufof.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3knncwlmz.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3thrshwnd.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3khpbnxbu.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3hhoobrcl.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3jbfwmemh.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3gtjxgsgg.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3woqvtvuw.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3whwydqtt.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3tcjyryrb.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3edttgxtz.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3fqziiken.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3obznpdcc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dovhhksk.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3inknsexe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tyswwsyq.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3lbkqvqon.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3fwsdvghm.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3eyfphfwq.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3hfeicihh.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3sqmgywcc.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3lurpimkc.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3dwrxgktz.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3tlqydjxn.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3mkspryzb.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3eapkqzxa.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3tfwyinwh.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3dqawkopy.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3tyxdlgkz.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3mzcbtafr.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3ccvcicah.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3pxpfdulm.html


<!-- 参考信息 -->