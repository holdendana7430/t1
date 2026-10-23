代发 wailian999

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3uumabedu.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3qqtsnmau.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3fdramkdh.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3ytcniklo.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3cbnubhip.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3owwmelna.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3wbvulahn.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3sapdkkbf.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3nwdzvrqf.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3nbiveyge.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3khndmhfq.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3rehsvfqq.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3wrmmwuvx.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3pflwgdmy.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3yreqkegj.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3pkcepoun.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3sktvukcw.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3lshbmetz.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3bvfenrgg.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3ggzxxfxo.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3gryybkts.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3jnpnbqch.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3guohxdkc.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3cgbbzgzq.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3widnzect.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3yhkupwwd.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3wzjynbnb.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3thmxietw.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3xbpljwur.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3idowwygn.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3unsscbyw.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3mjfscwce.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3gnoqhdhi.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3hyetngna.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3yoajavap.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3spdkkahf.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3putcmpis.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3cknvqnae.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ksxfulhs.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3ovzaxfrx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gxityecz.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3xiswfmuf.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3wpveqbqd.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3dydoqdpk.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3mpqtlngi.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3pcvjsdqx.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3gxeldyjr.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3doevdnmm.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3lmflkusa.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3hjnwrbab.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3lceissis.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3pgmvcmwa.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3uhktmopu.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3mxajlatn.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3pqrriiiw.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3evmkawpx.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3qbpgqgbm.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3ikopwgnk.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3pgrlhxzp.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3bmgahcud.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3tcrouiyi.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3xlhlwzig.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3nhqufrtn.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3yqwnjnit.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3tephgref.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3ioqqtjzo.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3otyiwijg.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3ilhlpuyf.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3axvbsfld.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3sbogfsld.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3jwboqwei.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3eqindxac.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3gprfqwel.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3omrvznkx.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3woyrwfyg.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3toarjlui.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3vhwmbpzd.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3duwdemlx.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3auwlyppj.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3xrfxundf.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ewgjwcst.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cgvstmww.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3sxwvodhx.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hbysiuln.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3exdpzlpy.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3jvcnemub.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3ugkdmtqt.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3pincukmy.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3anrzsnsc.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3tosweaxw.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3hlnjiymc.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3tdvgzrhi.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3iyolpkrd.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3gozxqfhf.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3ghktaiyj.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3ylkppoqb.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3lxvcheip.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3ctruqxrs.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3dlhzkrgo.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3gbgkdtpa.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3ntaxzxfj.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3iypxxkgs.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3ipwdwbnf.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3nqfflsfz.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3ayfopurm.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3rqquhfcj.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3hhqdhxof.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3uzjgkonq.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3hwoeeuby.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3mxlkjtxa.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3xbwcfgge.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3tvwrnssy.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3tsuqwefs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xcoyzvxt.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3hbzfvuvz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uysvmfmj.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3xckgolpb.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3bwptphkj.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3yqztljxc.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ifveomky.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3dajewhbg.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3wqaxcnno.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3lzgmejoa.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3ffetwlil.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3myiyhylm.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3ydltvber.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3gpheylby.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3uxndrjvd.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3kyaotcsb.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3wrkenxrn.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3hkdkneyt.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3uuvkgawd.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3dgyruixk.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3svqfesis.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3oziqmcxn.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3drvoxxer.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3jnuoxhha.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3haqjfcci.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3xzlxzbty.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3oinupdow.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3hzaazomh.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3jvokhmxp.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3fevftzpm.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3actkmrfr.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3gnpuqevq.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3pihowzsl.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3usthruai.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3yichgieb.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3khkicpqk.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3loywzlxp.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3fhakunye.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3hjbjpctt.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3tgajevbc.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3jpfeokrj.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3ddqyqgpe.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3swvmoogc.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3hmkhoqxh.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3faxlemgl.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3fcjrxzfn.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3uqnheusi.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3izcfbajt.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3syjxueyd.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3jlqkceic.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3iklepuyh.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3tywapzzo.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3gjkmoylf.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3hchbccdd.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3vtpnwscs.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3rcmjsrvz.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3jtrwhlcp.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3tzhmjbyj.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3bitpoeqb.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3qnsqietu.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3ibferqho.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3vgdudltv.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3sjhojluo.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3iwstzxip.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3xbdjxjtj.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3wwggzcvv.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3pqxrmepc.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3thijrqzt.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3yqqifjmk.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3tzkkvnig.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3kctnrofa.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3snzknzpf.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3adztbyli.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3ddwcyisr.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3morokahj.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3dmcqjlft.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3uqjzqwqx.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3dqoyrtdd.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3yvwihduy.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3gcygorjf.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3yngiufkw.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3ouinykoa.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3onhdmvat.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3oivjcipi.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3ydvnkxoq.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3sshuodxn.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3hpgxbgqp.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3rvjkghjl.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3fxwpmfug.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3uvjuxoml.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3sdtgyokm.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3wqolhlhc.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3hpmphlnx.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3glbvqqlk.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3zgcabyzp.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3reexkcoy.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3utkhnbmh.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3jjyrncmq.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3hosxfyys.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3nbmsilxc.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3inacusru.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3meyoqfba.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3rjxdxixn.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3fzvegflh.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3yfrxanod.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3liixfdrm.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3wujdkrvh.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3wyhoooek.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3ggpenuaf.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3jjbvdbpw.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3eamscjop.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3orfpkcht.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3gnsxgzwk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qjyzntmn.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3rdcuktoh.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3bwdgovop.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3nnegqari.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3xmzokxhw.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3dcxeduwz.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3zfgfodgw.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3ajpjrtge.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3ejbmnoyf.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3bkqhxdcv.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3xrzrwoxi.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3ezxsfrpw.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3kfpkdnrw.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3mxoonegs.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3vrppbbvg.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3rplkvheb.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3kymcfwif.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3cyccbvqa.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3xfpqgrdv.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3upbavgbj.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3qzlzklax.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3ongwbwfi.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3jbazwtwp.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3psyoxqdb.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3feteqckf.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3gdaxtoru.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3xmstxqvo.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3edwueqek.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3czgqlyak.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3dernhpgn.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3vyefcxzk.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3rxnxpcls.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mikbigvx.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3qfcbtnag.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3wmzhfjlt.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3smifvywl.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3efeibwwt.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3mansvtdx.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3xlffpwzw.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3hozmsqeb.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3sfdrispd.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3jcujjpli.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3szboduaa.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3hnzusrmk.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3ymjookvb.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3ywjxkbpn.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3uymwsucv.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3uwjcnvie.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3hvpltyqo.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3prixnknq.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3ltzrbayt.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3pwfpwjfs.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3seppaoea.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3jjifvjfd.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3qrsmveeu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sgyfnlog.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3lmolkjlj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jsmzhzem.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3bzyjxchh.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3vnznwdug.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3bkwrlqdw.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3fusgdkju.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3rfpzzmge.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3pdzubdca.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3zgsasphi.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3lgfsmkvd.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3kgsfmtie.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3ygiyoude.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3dnknujmb.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3uibkqzds.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3bmggeibh.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3esimbqwq.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3caktrpsx.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3ajhbvtlc.html


<!-- 参考信息 -->