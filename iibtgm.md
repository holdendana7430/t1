代发 wailian999

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.shzxlz.cn/gtsfvnyqbu.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.zycfv.cn/gtrmuchvyl.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.shzxlz.cn/gtksbzmtut.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.hnxiangtu.top/gtkoswcsmh.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.nwbrower.top/gtnmepkilh.html

[L04] 设置超时
来源：http://hz.xuanzx.com/gtscwmzwzv.html

Py:   requests.get(url, timeout=5)
来源：http://hz.fengsongda.top/gtljwnnmko.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.hnqzz.top/gtphwckolg.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jianghu66.top/gtzdyizvql.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jinghuilouyu.cn/gtmqrttzgk.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.zycfv.cn/gtaeeyaumg.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.cdnleiting.top/gtsfmzxliu.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.birdmap.top/gtsnqejhho.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.guannengcc.top/gtauhrooly.html

[L05] 上传文件（multipart）
来源：http://hz.cqqwz.cn/gtydycqebx.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.gzhubu.top/gtcglsxojw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.wangdashe.top/gtgryxhkiy.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.fzhhl.top/gtkmotoivs.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.wangdashe.top/gtosqvjqtn.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.yonumen.top/gtqfbwmxog.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.yvedp.cn/gtotuhvjat.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.daxiang520.top/gtctygmxue.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.hammf.cn/gtponstuio.html

[L06] 解析响应为 JSON
来源：http://hz.hnqzz.top/gtackxecwf.html

Py:   resp.json()
来源：http://hz.guannengcc.top/gtvxijevav.html

PHP:  json_decode($body, true);
来源：http://hz.jiagoushi.top/gtptgqkmoq.html

JS:   await resp.json()
来源：http://hz.shangyingyoupin.top/gtokxkemqw.html

TS:   await resp.json()
来源：http://hz.shangyingyoupin.top/gttkfmxvfk.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.c1oappe.top/gtjyfbntqj.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.aizwys.cn/gtgpkeccsy.html

Ruby: JSON.parse(resp.body)
来源：http://hz.jyoumei.cn/gtimhlenpo.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.ppjwa.cn/gtsjsqpkud.html

[L07] 处理 HTTP 状态码
来源：http://hz.316326.xyz/gtzxazqxlv.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.jinqigfzy.top/gtorijwyho.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.yonumen.top/gtbhuusvjq.html

JS:   resp.ok;  resp.status
来源：http://hz.zhengqikj.top/gtuakhidef.html

TS:   resp.ok;  resp.status
来源：http://hz.hnxiangtu.top/gtshzolqjg.html

Java: resp.statusCode()
来源：http://hz.jlsjyb.cn/gtrkrlkuua.html

Go:   resp.StatusCode
来源：http://hz.ehwqpu.com/gtkkspguew.html

Ruby: resp.code.to_i
来源：http://hz.wangdashe.top/gtdjaiokzs.html

C#:   (int)resp.StatusCode
来源：http://hz.52xcode.cn/gtdovuheju.html

[L08] 并发请求多个地址
来源：http://hz.hnxiangtu.top/gtqsebvdjr.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.tian-w.cn/gtfigwfcvi.html

PHP:  curl_multi_init() 系列
来源：http://hz.xuanzx.com/gtryexsdxp.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.aibaodan.cn/gtbncnsftf.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jianghu66.top/gtwknzmtrb.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.daxiang520.top/gtztmqstqc.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.chenzaomai.com/gtaulqgwbs.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.sweek.top/gtjzbhtrgn.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.yj20258.top/gtbfgdloks.html

================================================================================
来源：http://hz.nanxuanxn.top/gtanyzzkfy.html

M. 命令行 / 进程 / 环境
来源：http://hz.hammf.cn/gtueulejdl.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtqemdpapj.html

[M01] 读取命令行参数
来源：http://hz.smart0.xyz/gtchffukck.html

Py:   sys.argv[1:]
来源：http://hz.shangyingyoupin.top/gtayfbvkph.html

PHP:  $argv;  $argc;
来源：http://hz.daxiang520.top/gtolgwntyl.html

JS:   process.argv.slice(2)
来源：http://hz.ehwqpu.com/gtdtevkaky.html

TS:   process.argv.slice(2)
来源：http://hz.zhengqikj.top/gtbkzortmn.html

Java: args 数组（main 方法参数）
来源：http://hz.jiagoushi.top/gtsdiwkzcc.html

Go:   os.Args[1:]
来源：http://hz.hfpthk.cn/gtqvoflqne.html

Ruby: ARGV
来源：http://hz.wangdashe.top/gteoqplndu.html

C#:   args 数组（Main 方法参数）
来源：http://hz.kuanghao11.cn/gtzfssdxjo.html

[M02] 读取环境变量
来源：http://hz.kuanghao11.cn/gtyulnhqbq.html

Py:   os.environ.get("HOME")
来源：http://hz.nwbrower.top/gtixegbnco.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.tanke756.top/gtxbhkehbp.html

JS:   process.env.HOME
来源：http://hz.andypj.xyz/gtxxybxdcd.html

TS:   process.env.HOME
来源：http://hz.chenlongwang.top/gtmjcenexj.html

Java: System.getenv("HOME")
来源：http://hz.hfpthk.cn/gtsufqmvee.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.kuanghao11.cn/gthhfqkkev.html

Ruby: ENV["HOME"]
来源：http://hz.tianlin.xyz/gtflhqaqno.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.yuanzhike.top/gtluwqorhv.html

[M03] 执行外部命令
来源：http://hz.chenlongwang.top/gtscckzbyb.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.hywenlv.cn/gthgzazvie.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.feifeiyinyue.top/gtsbengouc.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.yongpay.top/gtqziemfjs.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.xingfuxueyuan.xyz/gtmfcjrblx.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.yuanzhike.top/gtzhlxrbbo.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.ywan-chungtsiang.top/gtbmuobjid.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.bjfxy.top/gtpjqfdzqs.html

C#:   Process.Start("ls", "-l");
来源：http://hz.shanyushiyangkeji.top/gtymrnkelg.html

[M04] 获取当前工作目录
来源：http://hz.snrcjt.cn/gteiqjncyc.html

Py:   os.getcwd()
来源：http://hz.chenlongwang.top/gtwxpnypgf.html

PHP:  getcwd();
来源：http://hz.ydzc1.top/gtzphzhjtc.html

JS:   process.cwd()
来源：http://hz.hnqzz.top/gtcpnujvmk.html

TS:   process.cwd()
来源：http://hz.yuanzhike.top/gtgeiprfee.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.316326.xyz/gtlbiuxtue.html

Go:   os.Getwd()
来源：http://hz.zhongyouzk.top/gtyxlhnwvz.html

Ruby: Dir.pwd
来源：http://hz.snrcjt.cn/gtcsmfwbfh.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.xinyue.icu/gtzyvnkxum.html

[M05] 设置退出码
来源：http://hz.andypj.xyz/gtprxgonjy.html

Py:   sys.exit(1)
来源：http://hz.sweek.top/gtveklcjgs.html

PHP:  exit(1);
来源：http://hz.0kj1m.cn/gtakilxmub.html

JS:   process.exit(1)
来源：http://hz.zhengqikj.top/gtpiiphqci.html

TS:   process.exit(1)
来源：http://hz.yanxiufei.cn/gttijimvjq.html

Java: System.exit(1)
来源：http://hz.ydzc1.top/gtpqlluanq.html

Go:   os.Exit(1)
来源：http://hz.aibaodan.cn/gtxelpyevv.html

Ruby: exit 1
来源：http://hz.fzhhl.top/gtdbmwrsun.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.dashuyun.cn/gtguipnwjg.html

[M06] 向标准错误输出
来源：http://hz.chenzaomai.com/gtfbaqkcks.html

Py:   print("err", file=sys.stderr)
来源：http://hz.daria6918.cn/gtgxylzjct.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.guowangkeji.top/gtffflhtqm.html

JS:   console.error("err")
来源：http://hz.shzxlz.cn/gtocpgvhmw.html

TS:   console.error("err")
来源：http://hz.ehwqpu.com/gtqxlvqyqt.html

Java: System.err.println("err")
来源：http://hz.svipenyu.cn/gtlkhzyipq.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.zhoulong.xyz/gtrghltlxe.html

Ruby: warn "err"
来源：http://hz.haohaochexian.top/gtlqefxdhx.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.shzxlz.cn/gtsgdrappn.html

[M07] 判断是否为主入口
来源：http://hz.hongshengwenyu.top/gtfcrcjeke.html

Py:   if __name__ == "__main__":
来源：http://hz.chenlongwang.top/gtfmooxmif.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.aibaodan.cn/gtvwvjgfxb.html

JS:   require.main === module
来源：http://hz.xylfe.cn/gtnfdbqfac.html

TS:   require.main === module
来源：http://hz.fengsongda.top/gtxtyguqah.html

Java: public static void main(String[] args)
来源：http://hz.chenjidiqi.icu/gtycfcavrb.html

Go:   func main()
来源：http://hz.pengpengdd.cyou/gthuxojyjf.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.jinghuilouyu.cn/gtoxkwsuod.html

C#:   static void Main(string[] args)
来源：http://hz.yvedp.cn/gtnmgqbpmu.html

[M08] 获取系统与运行时信息
来源：http://hz.fengsongda.top/gtohzolzth.html

Py:   platform.system();  platform.python_version()
来源：http://hz.zhoulong.xyz/gtrqnhruwo.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.hnqzz.top/gthrsauryl.html

JS:   process.platform;  process.version
来源：http://hz.sweek.top/gtfeloyrsl.html

TS:   process.platform;  process.version
来源：http://hz.dashuyun.cn/gtgbuqlxiu.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.fzhhl.top/gtmiuqdqep.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.xinyue.icu/gtanezkdlk.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.sysykeji.top/gtlvbjfrfi.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.ybcxt.top/gtmumlfzwx.html

================================================================================
来源：http://hz.c1oappe.top/gtxbotmolo.html

N. 数据结构与算法
来源：http://hz.yj20258.top/gtewfdpgep.html

================================================================================
来源：http://hz.ydzc1.top/gtpdxyyetm.html

[N01] 二分查找（有序数组）
来源：http://hz.yvedp.cn/gtxxsetezw.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.xingfuxueyuan.xyz/gtzrithbhz.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.zycfv.cn/gthpkebbat.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.guowangkeji.top/gtonfepryb.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.hongshengwenyu.top/gtensscbqq.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.sysykeji.top/gtvoycgvvc.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.ybcxt.top/gtjigosnok.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.meibo888.top/gtubargqfb.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.aibaodan.cn/gtlplpkscj.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.snrcjt.cn/gtooqcaaif.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.guowangkeji.top/gtwybtwrmt.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.jqgfzy.top/gtdxusgphb.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yvedp.cn/gtiiqjkejl.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.sufxvd.cn/gtpbonqsho.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.tian-w.cn/gtnqgloeqi.html

Go:   slices.Sort(arr)
来源：http://hz.snrcjt.cn/gtwpvwypjt.html

Ruby: arr.sort
来源：http://hz.jiagoushi.top/gtjrbqrhcq.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.daria6918.cn/gtibuomezm.html

[N03] 快速排序（分治示例）
来源：http://hz.hfpthk.cn/gteddfhwhu.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.jinqigufen.top/gtdbbjfvvf.html

PHP:  // 递归实现，或用 usort
来源：http://hz.gzhubu.top/gttzebnsnj.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.9152youxi.cn/gtuuczrbdp.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.shzxlz.cn/gtjwilwhze.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.cqqwz.cn/gtbdgdfuhg.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.yuanzhike.top/gtcofyzbgv.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.ybcxt.top/gtsdbxagma.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.yj20258888.top/gtvfxhfwwd.html

[N04] 斐波那契数列
来源：http://hz.gogol.net.cn/gtrduwseuk.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.jinqigfzy.top/gtxltypvcs.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.sxryk.cn/gtxfzuodmd.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.zhaomingkeji.xyz/gtrriqcqfn.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.daria6918.cn/gtgrzqzorf.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.jianghu66.top/gtsqabbidz.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.aizwys.cn/gtbnqhanov.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.shuidangran.top/gtprpglxmb.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.ydzc1.top/gtxkhyzawm.html

[N05] 最大公约数
来源：http://hz.zhengqikj.top/gtoewsznsd.html

Py:   math.gcd(a, b)
来源：http://hz.gaohongyu789.top/gthztruelz.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.gzhubu.top/gtodgqlajk.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.nanxinkj.top/gtyvqqoajv.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.meibo888.top/gtmzxgtzlf.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.quarkkingdee.top/gtyunsiphl.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.snrcjt.cn/gtvdxecvte.html

Ruby: a.gcd(b)
来源：http://hz.hfpthk.cn/gtevnsbiwb.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.9152youxi.cn/gtzdoqgdvw.html

[N06] 判断回文字符串
来源：http://hz.yanxiufei.cn/gtbmwqweid.html

Py:   s == s[::-1]
来源：http://hz.cheryme.top/gtrtpvnakc.html

PHP:  $s === strrev($s);
来源：http://hz.yj202588.top/gtqvvtuqkz.html

JS:   s === [...s].reverse().join("")
来源：http://hz.mhx1999.top/gtyergtzfx.html

TS:   s === [...s].reverse().join("")
来源：http://hz.andypj.xyz/gtcluvtwox.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.dashuyun.cn/gtmktvqets.html

Go:   // 双指针从两端比较
来源：http://hz.bjfxy.top/gtrzzmuhts.html

Ruby: s == s.reverse
来源：http://hz.sysykeji.top/gtyhbghsll.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.yangfankeji.com/gtdlomovrt.html

[N07] 两数之和（返回下标）
来源：http://hz.chenjidiqi.icu/gtzqpzvnkr.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.nanxinkj.top/gtoihnipqj.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.gzhubu.top/gtdznjioxk.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.gaohongyu789.top/gthyyurvjh.html

TS:   // 手写 Map<string, number>
来源：http://hz.sweek.top/gtfiidfrhf.html

Java: // 手写 HashMap
来源：http://hz.ehwqpu.com/gtoebkwjec.html

Go:   // 手写 map[int]int
来源：http://hz.cashguo.top/gtldzpxuab.html

Ruby: // 手写 Hash
来源：http://hz.daxiang520.top/gtjecwobal.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.shuidangran.top/gthxgcpauf.html

[N08] 生成全排列
来源：http://hz.sysykeji.top/gtehwxvcgs.html

Py:   itertools.permutations(arr)
来源：http://hz.shangyingyoupin.top/gtvmxblwlf.html

PHP:  // 手写递归交换
来源：http://hz.gzhubu.top/gtwedsyhfd.html

JS:   // 手写回溯递归
来源：http://hz.52xcode.cn/gtclrhdqxw.html

TS:   // 手写回溯递归
来源：http://hz.hysaishi.cn/gtrqdotwtp.html

Java: // 手写回溯递归
来源：http://hz.aizwys.cn/gtgowdhqob.html

Go:   // 手写回溯递归
来源：http://hz.kuanghao11.cn/gtjelaiogy.html

Ruby: arr.permutation.to_a
来源：http://hz.sysykeji.top/gtxesraevi.html

C#:   // 手写回溯递归
来源：http://hz.nanxuanxn.top/gtoascitly.html

[N09] 栈与队列
来源：http://hz.ehwqpu.com/gtigytheir.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.ydjk.org.cn/gthgsctgsy.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.hysaishi.cn/gtyeuhyotx.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.hnqzz.top/gtzcdnyago.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.yvedp.cn/gtjfierfsc.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.wangdashe.top/gtnazbkgzw.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.nanxinkj.top/gtokffdhbh.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.jyoumei.cn/gtbucxykho.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.yueranfly.top/gtwwmiplqw.html

[N10] 链表节点定义
来源：http://hz.cdnleiting.top/gtyjmcbaau.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.gogol.net.cn/gtomimlwor.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.xuanzx.com/gtnulptidu.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.jinqigufen.top/gtcppadpvj.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.hongshengwenyu.top/gtbeutccdt.html

Java: class Node { int v; Node next; }
来源：http://hz.fengsongda.top/gtdodjcyul.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.zhengqikj.top/gturdmfynn.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.meibo888.top/gtjwkncvzo.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.gaohongyu789.top/gtcuupbsty.html

[N11] 二叉树中序遍历
来源：http://hz.tanke756.top/gtczhgrszd.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.yanxiufei.cn/gtqwpmyweo.html

PHP:  // 手写递归函数
来源：http://hz.redwolf501.top/gtgrpwofbx.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yonumen.top/gtzqmnnlit.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.zhoulong.xyz/gtraveeabr.html

Java: // 手写递归
来源：http://hz.fengsongda.top/gtrdwhvndq.html

Go:   // 手写递归
来源：http://hz.shanyushiyangtech.top/gtowyoqjlc.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.aibaodan.cn/gthhfqpghx.html

C#:   // 手写递归
来源：http://hz.birdmap.top/gtjmvbliwp.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.zhongyouzk.top/gtufzkmkxh.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.sysykeji.top/gttmbopzek.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.zycfv.cn/gtogmlfsbv.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jqgfzy.top/gtrkxxnjfl.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.zhaomingkeji.xyz/gtlfwffono.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yangfankeji.com/gtwbabbryt.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.tanke756.top/gtspkxcltd.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.hnqzz.top/gtwlvjysol.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yj202588.top/gtaaiknczq.html

================================================================================
来源：http://hz.zhijiandao.cn/gtuvclmwng.html

O. 并发与异步
来源：http://hz.jinqigfzy.top/gtngqjizbc.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtiryrhdze.html

[O01] 启动一个线程
来源：http://hz.daria6918.cn/gtqnxrjvau.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.shanyushiyangkeji.top/gtovrccfir.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.dashuyun.cn/gtqecbwdxc.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.sweek.top/gtopzuuvjg.html

TS:   // 同 JS
来源：http://hz.daria6918.cn/gtvyrhviqs.html

Java: new Thread(() -> f()).start()
来源：http://hz.zhongyouzk.top/gtblxpzalm.html

Go:   go f()
来源：http://hz.birdmap.top/gtqwylogpd.html

Ruby: Thread.new { f }
来源：http://hz.ehwqpu.com/gtbhklgovn.html

C#:   Task.Run(() => F());
来源：http://hz.52xcode.cn/gtqtenkroe.html

[O02] 使用线程池
来源：http://hz.zhiwuduotai.top/gtnzgedhci.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.kuanghao11.cn/gteaxmryzd.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.ivvv.top/gtpggwgavu.html

JS:   // worker_threads 线程池
来源：http://hz.ydjk.org.cn/gtvidmffmr.html

TS:   // worker_threads 线程池
来源：http://hz.yj202588.top/gtiynxjwvy.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.sysykeji.top/gtogwpfzqs.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.zdqjudy.top/gtiqagbbbz.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.zhiwuduotai.top/gtpxixjdib.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.gotoacloud.top/gtjtdbxgkl.html

[O03] 加锁保护共享数据
来源：http://hz.ivvv.top/gtmavmszlu.html

Py:   with lock: shared += 1
来源：http://hz.jqgufenzy.top/gtidwclbjo.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.cqqwz.cn/gtculkzneh.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.hysaishi.cn/gtwcjhfxqs.html

TS:   // 同 JS
来源：http://hz.9152youxi.cn/gtrmnnpykz.html

Java: synchronized (this) { shared++; }
来源：http://hz.jinqigfzy.top/gthakksehq.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.ywan-chungtsiang.top/gticigxekw.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.cashguo.top/gtwbdaaoqr.html

C#:   lock (gate) { shared++; }
来源：http://hz.jianghu66.top/gtnqlcdawa.html

[O04] 定义异步函数并等待
来源：http://hz.yvedp.cn/gtkgbydbgw.html

Py:   async def f():⏎    await g()
来源：http://hz.gotoacloud.top/gtmrljbwcj.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.dianchejie.cn/gtbubazuaw.html

JS:   async function f() { await g(); }
来源：http://hz.andypj.xyz/gthwqwtshv.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.ydzc1.top/gtgwwwtkbe.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.zhiwuduotai.top/gtwiywqiaa.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.shanyushiyangtech.top/gtgtofkwbf.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.hammf.cn/gtshzbsduc.html

C#:   async Task F() { await G(); }
来源：http://hz.xziqi.cn/gtbwswpzqd.html

[O05] 并发执行并等待全部完成
来源：http://hz.yj202588.top/gtdmigzima.html

Py:   asyncio.gather(*tasks)
来源：http://hz.dianchejie.cn/gtmhnvrfue.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.shanyushiyangkeji.top/gtttcjvqef.html

JS:   await Promise.all(tasks)
来源：http://hz.chenzaomai.com/gtucftnqlu.html

TS:   await Promise.all(tasks)
来源：http://hz.9152youxi.cn/gtjqfxnxep.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.hnxiangtu.top/gtkhtysvgs.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.snrcjt.cn/gtgmqrolsa.html

Ruby: threads.map(&:join)
来源：http://hz.tanke756.top/gtigpxuiyn.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.snrcjt.cn/gtowxicgfx.html

[O06] 使用进程池
来源：http://hz.hywenlv.cn/gtdenurabc.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.chenzaomai.com/gtxbpuxrwt.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.cheryme.top/gtouracvgu.html

JS:   // child_process / cluster 模块
来源：http://hz.chenlongwang.top/gtfspwpxmm.html

TS:   // child_process / cluster 模块
来源：http://hz.jlsjyb.cn/gtqdpicqgy.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.316326.xyz/gtopbcwlon.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.svipenyu.cn/gtchoqking.html

Ruby: // fork 块
来源：http://hz.hammf.cn/gthdsapxqy.html

C#:   Parallel.For
来源：http://hz.guannengcc.top/gtfpycrmht.html

================================================================================
来源：http://hz.chenzaomai.com/gtpytmfmzz.html

P. 常用工具函数
来源：http://hz.guannengcc.top/gtcxmyggxo.html

================================================================================
来源：http://hz.guannengcc.top/gtgkeurmqk.html

[P01] 生成 UUID
来源：http://hz.yongpay.top/gtezsfblno.html

Py:   str(uuid.uuid4())
来源：http://hz.wangshuangyany.cn/gtksgvwzku.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.hongshengwenyu.top/gtmxfgqhgp.html

JS:   crypto.randomUUID()
来源：http://hz.mhx1999.top/gtzexphifu.html


<!-- 参考信息 -->