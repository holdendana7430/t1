代发 wailian999

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3dmwqpnkm.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3ywhknggt.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3wmhjxasm.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3mraghnty.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3dargcoqj.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3pufzyedv.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3dafpedud.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3pltpxrxe.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3gfnicutl.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3fexwtotz.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3tqbulmeo.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3kauiajxf.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3qcsaqgye.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3gpylimjl.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3kcjspvtv.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3ktwymoaw.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3nblvuvdr.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3dtjnegid.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3ilhagpzq.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3eqytnbhs.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3umrehxtj.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3xisugnay.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3zjeluihx.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3jczpusyh.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3paqnluav.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3xqjovhto.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3iwhqngtc.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3yrvhbxqq.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3ncmtqeoi.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3lmbvtzaj.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3spalbgqr.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3dxtgqlzi.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3ufhjbykj.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3onqskbjf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xpczxzes.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3mhgclyuz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3owoqzkos.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3igkmunrs.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3rtjhdtmg.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3vybnqueb.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3jjxaqnli.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3jgkimoaw.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3eelmmwuj.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3gpgewwde.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3jvuyijvm.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3emjhxqwc.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3nsabxmob.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ajxoqpet.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3thofkvht.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3friiceew.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3tqgolxum.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3pziwdkjf.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3kcnubbul.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3mebtnicx.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ofeudcis.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3dgchakqb.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3oievqith.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3htxkfxgm.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3qovwffxd.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3ftiybdgw.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3ancezgkq.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3imwjfpcq.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3txysavpw.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3akpedigu.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3jxkcnsol.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3ygjogult.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3xprvubti.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3uavchagv.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3itfzioap.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3izjiibkl.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3fpgourqx.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3iekyljwv.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3ntbcwrpw.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3qcvlueuf.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3uxltmkfn.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3whvyynax.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cbwkyaia.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zmjmxhlr.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zhbsuiah.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3tovtaxre.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3zbgxutau.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3qjyprbme.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3vjejhcvr.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3xzhijgtb.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3dnqgnrmk.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3mblpnibs.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3wdarqjty.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3rhkzpkiu.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3gefudomp.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3igcrutzq.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3btjjentg.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3biaxzejc.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3emhnnjii.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3vhzbvcol.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3xcnbavuy.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3ubbdpplh.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3ktrflfqf.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3fkoguteu.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3acnhwcos.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3mtmylsgi.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3ekqkuxmd.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3ohpwijoa.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3qeldzvab.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3htaagvvq.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3fqnkqeje.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3dfsvtafp.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3ydpapdoy.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3wqrnhujg.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3giguoajs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zwuesipd.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3yoggnnnz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zlohubjs.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3qixqpoph.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3kcwveqko.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3lwvtilbj.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3rvdkplff.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3hbhbfelj.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3crzjrxhv.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3zncanjgq.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3jsrzdwiz.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3wrhznckr.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3qqriyjoh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3ujsvsqob.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ssrszzbe.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ygnlhlsv.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3uyogeofi.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3wntyjigy.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pbkcbdnv.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3crqgxfzh.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3rdephjqg.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3msyddqof.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3hmulfkhn.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3tmgjdasa.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3rrppeaje.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3enaqxfzo.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3tlfvoedg.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3rzpsqvpf.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3eaawjmtq.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3fqcqawyg.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3zaqgpaxo.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3lyolwrmj.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3jrvvahkx.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3hxxssnrk.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3cskhbema.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3opbiolrg.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3qgnordue.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3imavijfm.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3glcslnup.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3tczaplgd.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3uuhlnvpb.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3elvtuorc.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3nvhkdefc.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3uviwtnan.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3vxyyhkno.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3vqsdcuge.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3qpfmmyoo.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3cpurhclo.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3bvklnmrn.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3cslmfwxa.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3wneefphc.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3dtyzztuf.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3wsmzyhhp.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3xxravjnv.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3oompvzsq.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3foxcwfqx.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3ivgeqoyf.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3hditqpis.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3ihckjnyr.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3azhucosc.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3qddhloyo.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3kdazhdxf.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3kcnlksjm.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3sefqldci.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3aybqlbyq.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3ycywxpfg.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3xygqmjof.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3keseyqkb.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3vsqqcuzd.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3fclajjkh.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3hmbnwmsz.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3girskckc.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3zzwwooae.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3uncwqudz.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3adtyuupd.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3icnuumkv.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3bmwgcpgk.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3yxjtvsfq.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ncyysvkb.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3opzwoyjz.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3uvcrfozb.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3qjlqgbmx.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3gdgoyxgp.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3gxbooorl.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3cryshhzd.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3kgvhnhsb.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3jrolexhe.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3sthxnvcy.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3qyxvecwh.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3qgzswfkg.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3gvcfxrzg.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3bfulziqp.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3dmrvlfsm.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3jjbonayd.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3eplvakzb.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3aiqxhepm.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3cwmftxek.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3rjpsfavd.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3hvvmsfoa.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3edhkyfyy.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3cgydnpqe.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3tzhyzfma.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3ldjcvjll.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3blejxqog.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3xxiumtup.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3qgavbtgs.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3chrqxprl.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3beuxslzf.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3feectsid.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3wufbjvqj.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3lnqjyqvn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jvsthhfb.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3xuitsfjc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ezngbkqk.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3bslmbxke.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3qjhsehmx.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3zmslviqq.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3etkelzhp.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3hbcbcnej.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3mwrfstcx.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3pmmqsbrv.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3ggqpvudr.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3cnovhkqi.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3vwwqdgud.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3rovukogt.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3niykqlfz.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3vtoklsix.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3mdmekiwl.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3hzbmztpv.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3jncsmmyx.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3tanhjzdc.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3rqhuirfl.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3wfhctpsa.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3bfwfaddx.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3ppbcojfw.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3fyialwir.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3qgopbrsr.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3onhgfwsq.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3qkkqdaij.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3czpszgwt.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3vlvqxngl.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3xsqlptfr.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3qcjkzbsd.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3cwtuyvvw.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3evjcjcsb.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3zsrwaesb.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3vwviowig.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3uqqdwtld.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3plsweglf.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3olwwqxlo.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3xciqznfs.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3oantarej.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3udxsmqow.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3awkcsjru.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3mkoqlcdi.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3oigypevj.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3gggmmfeu.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3cagsrjhp.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3jvhmumys.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3jgdultsl.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3qonrjiqz.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3vrdudmby.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3zjiyktvo.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3fjgktjax.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3svhvituy.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3vwuxqrju.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3wckljdos.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3bswvrxwb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gzvvurrr.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3ykibjiov.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ltsnldxq.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3hvmdgcej.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3hytlccws.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3leyvedzp.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3bzwfnqvu.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3scahdqgt.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3fxxoifjn.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3pnvclcxj.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3jrhmgnaz.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3vhawcffc.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3yqdbrebs.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3cmkqucsl.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qedwtpsn.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3yzpnfmyz.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3ykvpudmq.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3dcupterm.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3elzbxvfk.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zbfzqzno.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3skykhvkh.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3athmzqcu.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3rgsgaxzg.html


<!-- 参考信息 -->