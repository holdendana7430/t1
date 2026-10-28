代发 wailian999

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.jqgfzy.top/gtcjtgbceu.html

[L04] 设置超时
来源：http://hz.jlsjyb.cn/gtrzxhcljg.html

Py:   requests.get(url, timeout=5)
来源：http://hz.ydzc1.top/gtxicebrqg.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.ywan-chungtsiang.top/gtllfipajb.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.52xcode.cn/gtruewpspv.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.cqqwz.cn/gtkyejmtfu.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.yj20258.top/gtmfrakcwr.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.sweek.top/gtjsvqcvuu.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.aibaodan.cn/gtahtehptg.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.yangfankeji.com/gtlncwrovd.html

[L05] 上传文件（multipart）
来源：http://hz.yj202588.top/gtoyusrhae.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.mhx1999.top/gtfrtyfbjn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.shanyushiyangkeji.top/gteuozlsip.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.316326.xyz/gtvpusbikl.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.316326.xyz/gtjfxocnbv.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.snrcjt.cn/gthbqmmeck.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.yvedp.cn/gtcwncsiof.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.shzxlz.cn/gtglpcdmqn.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.ppjwa.cn/gtyoqvdqkl.html

[L06] 解析响应为 JSON
来源：http://hz.gotoacloud.top/gtlktntbjv.html

Py:   resp.json()
来源：http://hz.redwolf501.top/gtyuskyiga.html

PHP:  json_decode($body, true);
来源：http://hz.zhengqikj.top/gtmikoyqaf.html

JS:   await resp.json()
来源：http://hz.gaohongyu789.top/gttxykegil.html

TS:   await resp.json()
来源：http://hz.jianghu66.top/gtenogphkl.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.mhx1999.top/gtlkkhcian.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.yangfankeji.com/gtlemjhuqg.html

Ruby: JSON.parse(resp.body)
来源：http://hz.yj20258.top/gtmaqhdztk.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.jiagoushi.top/gtpojmysxg.html

[L07] 处理 HTTP 状态码
来源：http://hz.hnxiangtu.top/gtwaugizla.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.yonumen.top/gtabauxuau.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.nwbrower.top/gtscushezk.html

JS:   resp.ok;  resp.status
来源：http://hz.quarkkingdee.top/gtedafxbaa.html

TS:   resp.ok;  resp.status
来源：http://hz.cheryme.top/gtvpsntmgc.html

Java: resp.statusCode()
来源：http://hz.ybcxt.top/gtumarboep.html

Go:   resp.StatusCode
来源：http://hz.jlsjyb.cn/gtkknpimrm.html

Ruby: resp.code.to_i
来源：http://hz.jqgfzy.top/gtyaupydcq.html

C#:   (int)resp.StatusCode
来源：http://hz.jlsjyb.cn/gtzzmawcjf.html

[L08] 并发请求多个地址
来源：http://hz.hysaishi.cn/gtjsnvvakw.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.redwolf501.top/gttzyxtoog.html

PHP:  curl_multi_init() 系列
来源：http://hz.jiagoushi.top/gtyqrqxtkb.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.gaohongyu789.top/gtamcjqwjl.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.chenzaomai.com/gttqruohqu.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.yongpay.top/gtkwswcgsc.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.yj202588.top/gtbcgaiohb.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.birdmap.top/gtplfhabeq.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.haohaochexian.top/gtbudbvjgb.html

================================================================================
来源：http://hz.hywenlv.cn/gtngkmwmqw.html

M. 命令行 / 进程 / 环境
来源：http://hz.andypj.xyz/gtazlsnhdq.html

================================================================================
来源：http://hz.c1oappe.top/gtmisxfjsw.html

[M01] 读取命令行参数
来源：http://hz.gogol.net.cn/gtoffztuoz.html

Py:   sys.argv[1:]
来源：http://hz.jinghuilouyu.cn/gtkazcmvfa.html

PHP:  $argv;  $argc;
来源：http://hz.zycfv.cn/gtpsadktes.html

JS:   process.argv.slice(2)
来源：http://hz.c1oappe.top/gtyoooxxjq.html

TS:   process.argv.slice(2)
来源：http://hz.yongpay.top/gtluzuliic.html

Java: args 数组（main 方法参数）
来源：http://hz.hongshengwenyu.top/gtxlauehok.html

Go:   os.Args[1:]
来源：http://hz.jianghu66.top/gtsdarhepd.html

Ruby: ARGV
来源：http://hz.shzxlz.cn/gtuekhhvjo.html

C#:   args 数组（Main 方法参数）
来源：http://hz.yangfankeji.com/gtpichvgri.html

[M02] 读取环境变量
来源：http://hz.fzhhl.top/gtuufsikdy.html

Py:   os.environ.get("HOME")
来源：http://hz.cheryme.top/gtffxxhson.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.xziqi.cn/gtwcidvxnw.html

JS:   process.env.HOME
来源：http://hz.nwbrower.top/gtomnkcoir.html

TS:   process.env.HOME
来源：http://hz.kuanghao11.cn/gtywlfaupb.html

Java: System.getenv("HOME")
来源：http://hz.quarkkingdee.top/gtkzedwfij.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.jiagoushi.top/gtslcgwtre.html

Ruby: ENV["HOME"]
来源：http://hz.gzhubu.top/gtzoelfbdq.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.yj202588.top/gtdesgmvgv.html

[M03] 执行外部命令
来源：http://hz.zhijiandao.cn/gtyqnnkkes.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.ehwqpu.com/gtxoitkcco.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.shanyushiyangtech.top/gtclgtnetx.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.feifeiyinyue.top/gtqfxsyssa.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.yangfankeji.com/gtyggggvuh.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.nanxinkj.top/gtetzvitbv.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.yj202588.top/gtibjpeidd.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.pengpengdd.cyou/gtgnprjppm.html

C#:   Process.Start("ls", "-l");
来源：http://hz.xylfe.cn/gtawcxmynv.html

[M04] 获取当前工作目录
来源：http://hz.zdqjudy.top/gtpocnnfeb.html

Py:   os.getcwd()
来源：http://hz.hywenlv.cn/gtmjwegtqr.html

PHP:  getcwd();
来源：http://hz.jlsjyb.cn/gtfigwnogm.html

JS:   process.cwd()
来源：http://hz.zdqjudy.top/gtlujxldlc.html

TS:   process.cwd()
来源：http://hz.bjfxy.top/gthbxsyezy.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.redwolf501.top/gtyjnsxgec.html

Go:   os.Getwd()
来源：http://hz.yuxming.cn/gttivqpkuv.html

Ruby: Dir.pwd
来源：http://hz.wangdashe.top/gtltjbsctt.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.chenjidiqi.icu/gtejxaeuns.html

[M05] 设置退出码
来源：http://hz.xylfe.cn/gtynkxfboz.html

Py:   sys.exit(1)
来源：http://hz.cucudq.cn/gtdnyzyvto.html

PHP:  exit(1);
来源：http://hz.chenjidiqi.icu/gtvpvrxcqq.html

JS:   process.exit(1)
来源：http://hz.jinqigfzy.top/gtydsuycex.html

TS:   process.exit(1)
来源：http://hz.316326.xyz/gtwpxchlai.html

Java: System.exit(1)
来源：http://hz.yj20258.top/gttwilbtnz.html

Go:   os.Exit(1)
来源：http://hz.yanxiufei.cn/gtkxrtuzyb.html

Ruby: exit 1
来源：http://hz.nanxuanxn.top/gtgyyxnsgv.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.xziqi.cn/gtiybrdyly.html

[M06] 向标准错误输出
来源：http://hz.ydzc1.top/gtbjljopuj.html

Py:   print("err", file=sys.stderr)
来源：http://hz.9152youxi.cn/gtlxqbotek.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.jiagoushi.top/gthywpalce.html

JS:   console.error("err")
来源：http://hz.xinyue.icu/gtwxrviaqc.html

TS:   console.error("err")
来源：http://hz.smart0.xyz/gtlfbuteqj.html

Java: System.err.println("err")
来源：http://hz.yongpay.top/gtqtgbnpdk.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.andypj.xyz/gtsnnqgnzs.html

Ruby: warn "err"
来源：http://hz.zycfv.cn/gtrmjfrkqf.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.quarkkingdee.top/gtqvjcfrvs.html

[M07] 判断是否为主入口
来源：http://hz.sysykeji.top/gtfbputwzx.html

Py:   if __name__ == "__main__":
来源：http://hz.hammf.cn/gtyjbwxuvj.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.fzhhl.top/gtjszgoogf.html

JS:   require.main === module
来源：http://hz.hongshengwenyu.top/gttfjyfrfr.html

TS:   require.main === module
来源：http://hz.jqgfzy.top/gthwsrquea.html

Java: public static void main(String[] args)
来源：http://hz.zhijiandao.cn/gtpzpbkvwx.html

Go:   func main()
来源：http://hz.zhaomingkeji.xyz/gtfcntsjdr.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.snrcjt.cn/gteogwhlbc.html

C#:   static void Main(string[] args)
来源：http://hz.gotoacloud.top/gtkdfsvuws.html

[M08] 获取系统与运行时信息
来源：http://hz.ywan-chungtsiang.top/gtyigkudfa.html

Py:   platform.system();  platform.python_version()
来源：http://hz.shangyingyoupin.top/gtgwlgqqll.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.jianghu66.top/gtfrrurkmh.html

JS:   process.platform;  process.version
来源：http://hz.shangyingyoupin.top/gthkfouacb.html

TS:   process.platform;  process.version
来源：http://hz.yuanzhike.top/gtlpqciyzj.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.nanxuanxn.top/gtnpatomoz.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.ywan-chungtsiang.top/gtbsjcfsze.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.zhijiandao.cn/gtlziuldkn.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.shanyushiyangtech.top/gtztkjdjqi.html

================================================================================
来源：http://hz.zycfv.cn/gtebcvzoso.html

N. 数据结构与算法
来源：http://hz.cheryme.top/gtpbpmkaag.html

================================================================================
来源：http://hz.yonumen.top/gtqydcatxf.html

[N01] 二分查找（有序数组）
来源：http://hz.snrcjt.cn/gtffckegfn.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.hammf.cn/gtjvsluafl.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.xingfuxueyuan.xyz/gtsukbwxgd.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.hammf.cn/gtvapfmatr.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.hywenlv.cn/gtpsoauzxr.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.hammf.cn/gtugzgbsvp.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.yangfankeji.com/gtvcyvesrp.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.pycfn.com/gtwfjwtfln.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.nanxinkj.top/gtvzpzurgv.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.zhongyouzk.top/gtbpwljeig.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.ydjk.org.cn/gtwpybbtmu.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.svipenyu.cn/gtqhalffcn.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jinghuilouyu.cn/gtyuktsaov.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.daxiang520.top/gtohwtphxq.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.pengpengdd.cyou/gtpjpclndy.html

Go:   slices.Sort(arr)
来源：http://hz.aizwys.cn/gtvgoeunvp.html

Ruby: arr.sort
来源：http://hz.dashuyun.cn/gtlzerrsod.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.chenjidiqi.icu/gtunwlgcvt.html

[N03] 快速排序（分治示例）
来源：http://hz.jianghu66.top/gtzcoycuvt.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.pycfn.com/gtkxpsqmdb.html

PHP:  // 递归实现，或用 usort
来源：http://hz.hammf.cn/gtrnciikiv.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yangfankeji.com/gtmogsgrim.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.52xcode.cn/gtemxavfib.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.gzhubu.top/gtjebjrsjz.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.pycfn.com/gtignoiypp.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.nwbrower.top/gthgoyoqtp.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.tianlin.xyz/gtzwnxtcaq.html

[N04] 斐波那契数列
来源：http://hz.jianghu66.top/gtdskcmbrl.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.tian-w.cn/gtvlmyvtrw.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.jlsjyb.cn/gtjzoeenny.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.cashguo.top/gtjngqysxd.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.sxryk.cn/gtabelggrz.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.cucudq.cn/gtcxjokjlz.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.sweek.top/gtmgejtpzu.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.gotoacloud.top/gtkqhilbpe.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.yanxiufei.cn/gtgmofcgmc.html

[N05] 最大公约数
来源：http://hz.andypj.xyz/gtafvgumur.html

Py:   math.gcd(a, b)
来源：http://hz.ivvv.top/gtzqladoor.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.smart0.xyz/gtjllsbjwj.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yj202588.top/gtneptyecq.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.ybcxt.top/gtxrhdcnli.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.daxiang520.top/gtepmtrvpf.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.kuanghao11.cn/gtepiapwfn.html

Ruby: a.gcd(b)
来源：http://hz.andypj.xyz/gtakncjjuk.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.gaohongyu789.top/gtbmkaxjcw.html

[N06] 判断回文字符串
来源：http://hz.bjfxy.top/gtcgyorngt.html

Py:   s == s[::-1]
来源：http://hz.xziqi.cn/gtarxibenf.html

PHP:  $s === strrev($s);
来源：http://hz.zhengqikj.top/gtfwdviwdg.html

JS:   s === [...s].reverse().join("")
来源：http://hz.aibaodan.cn/gtxasakctf.html

TS:   s === [...s].reverse().join("")
来源：http://hz.yj20258.top/gtanxefzyh.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.zhoulong.xyz/gtwekykmwf.html

Go:   // 双指针从两端比较
来源：http://hz.jlsjyb.cn/gtacvcpcbj.html

Ruby: s == s.reverse
来源：http://hz.wangdashe.top/gtcanjeobt.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.zhoulong.xyz/gtybshswnw.html

[N07] 两数之和（返回下标）
来源：http://hz.chenlongwang.top/gttjtxdnsx.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.iojbl.cn/gtoorpwfjw.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.fzhhl.top/gtskvkefyy.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.nwbrower.top/gtqeihkcdm.html

TS:   // 手写 Map<string, number>
来源：http://hz.hongshengwenyu.top/gtunmmrint.html

Java: // 手写 HashMap
来源：http://hz.chenlongwang.top/gtprtlpdjt.html

Go:   // 手写 map[int]int
来源：http://hz.316326.xyz/gtrpxgavmm.html

Ruby: // 手写 Hash
来源：http://hz.yvedp.cn/gtaneiehab.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.hywenlv.cn/gtqzjvpyrc.html

[N08] 生成全排列
来源：http://hz.ydjk.org.cn/gtbhrkfpwt.html

Py:   itertools.permutations(arr)
来源：http://hz.chenlongwang.top/gtyzlndmwo.html

PHP:  // 手写递归交换
来源：http://hz.nanxinkj.top/gtlnnpmdbq.html

JS:   // 手写回溯递归
来源：http://hz.jiagoushi.top/gtpzlxbefi.html

TS:   // 手写回溯递归
来源：http://hz.jianghu66.top/gtmhsmanbn.html

Java: // 手写回溯递归
来源：http://hz.xinyue.icu/gtdmzolcxo.html

Go:   // 手写回溯递归
来源：http://hz.haohaochexian.top/gtxxaagwff.html

Ruby: arr.permutation.to_a
来源：http://hz.kuanghao11.cn/gtgglglrnd.html

C#:   // 手写回溯递归
来源：http://hz.wangdashe.top/gtawjivqwh.html

[N09] 栈与队列
来源：http://hz.ehwqpu.com/gteulybmqi.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.nanxuanxn.top/gtjrhevqhi.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.fengsongda.top/gtyupcfjei.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.hammf.cn/gtesknkzzq.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.wangdashe.top/gtojqlrmaa.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.wangdashe.top/gtrqfmoymo.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.dashuyun.cn/gtotmzrnpg.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.yj20258888.top/gtxtubbfdm.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.jinghuilouyu.cn/gtwsmcpisu.html

[N10] 链表节点定义
来源：http://hz.yuxming.cn/gtlfrbnedr.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.sysykeji.top/gtvlraxpta.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.ppjwa.cn/gtjdihmslf.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.ivvv.top/gtiytigfqu.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.zhengqikj.top/gtlflkmzbb.html

Java: class Node { int v; Node next; }
来源：http://hz.52xcode.cn/gtfcenaaza.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.hysaishi.cn/gtbquzwshs.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.cqqwz.cn/gtuiyumeti.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.mhx1999.top/gtnerxjgxj.html

[N11] 二叉树中序遍历
来源：http://hz.gotoacloud.top/gtlfbohkdd.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.hywenlv.cn/gtdgcdtapv.html

PHP:  // 手写递归函数
来源：http://hz.cdnleiting.top/gtymndalnn.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.dianchejie.cn/gtbikngqts.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.birdmap.top/gtwcifazqr.html

Java: // 手写递归
来源：http://hz.yuxming.cn/gtgnloagia.html

Go:   // 手写递归
来源：http://hz.tanke756.top/gtyclbdlte.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.xziqi.cn/gtceawacia.html

C#:   // 手写递归
来源：http://hz.nanxinkj.top/gtttfasigc.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.yuanzhike.top/gtnisvhnel.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.zhiwuduotai.top/gtmakhfpch.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.yanxiufei.cn/gtmqojnkbt.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.sxryk.cn/gthnngcchp.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.zdqjudy.top/gtboxhjrox.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.xylfe.cn/gtzunervds.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.pycfn.com/gtdvyeuvny.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.andypj.xyz/gttbrhwopv.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yj20258888.top/gtvzyvjqqc.html

================================================================================
来源：http://hz.redwolf501.top/gthnhdluwe.html

O. 并发与异步
来源：http://hz.zdqjudy.top/gtwrzkblaw.html

================================================================================
来源：http://hz.yvedp.cn/gtbrmnxvzo.html

[O01] 启动一个线程
来源：http://hz.snrcjt.cn/gtiufmynrt.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.hnxiangtu.top/gtvmzpozbv.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.jyoumei.cn/gtdojebugc.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.zhiwuduotai.top/gtrqfxhqbt.html

TS:   // 同 JS
来源：http://hz.cucudq.cn/gtctiipqfd.html

Java: new Thread(() -> f()).start()
来源：http://hz.xingfuxueyuan.xyz/gtounafmlm.html

Go:   go f()
来源：http://hz.redwolf501.top/gtyjrhlwwp.html

Ruby: Thread.new { f }
来源：http://hz.gaohongyu789.top/gtyfrehobq.html

C#:   Task.Run(() => F());
来源：http://hz.chenjidiqi.icu/gtpdyfnaif.html

[O02] 使用线程池
来源：http://hz.redwolf501.top/gtfsxyytxj.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.c1oappe.top/gtxxsxxqcn.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.xylfe.cn/gtxyerptaf.html

JS:   // worker_threads 线程池
来源：http://hz.bjfxy.top/gtrdmltvyh.html

TS:   // worker_threads 线程池
来源：http://hz.sysykeji.top/gtzilhmjrg.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.fengsongda.top/gtipwhhsxt.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.zhijiandao.cn/gtmzcsfkej.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.svipenyu.cn/gtkystqjsw.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.jinyuanbaomall.cn/gtclkjpkxe.html

[O03] 加锁保护共享数据
来源：http://hz.yonumen.top/gtihiwegax.html

Py:   with lock: shared += 1
来源：http://hz.xinyue.icu/gtkvebesqh.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.aibaodan.cn/gtpfykzhgc.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.zycfv.cn/gtwwrlhzzs.html

TS:   // 同 JS
来源：http://hz.zhongyouzk.top/gtiiankfyz.html

Java: synchronized (this) { shared++; }
来源：http://hz.guannengcc.top/gtuijzwglz.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.sweek.top/gteagwgtbt.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.hfpthk.cn/gtobkxbxal.html

C#:   lock (gate) { shared++; }
来源：http://hz.aibaodan.cn/gtnemuhdqc.html

[O04] 定义异步函数并等待
来源：http://hz.0kj1m.cn/gtgqxjetcp.html

Py:   async def f():⏎    await g()
来源：http://hz.feifeiyinyue.top/gtkpvxtjyo.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.cucudq.cn/gtztjxwwlg.html

JS:   async function f() { await g(); }
来源：http://hz.zhaomingkeji.xyz/gtfhkxkokr.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.svipenyu.cn/gtvzmbtqhl.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.fzhhl.top/gtnefnjywm.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.vqdsnc.cn/gtttgwvffk.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.jqgfzy.top/gtfkkczwfs.html

C#:   async Task F() { await G(); }
来源：http://hz.hfpthk.cn/gttosyphzu.html

[O05] 并发执行并等待全部完成
来源：http://hz.nwbrower.top/gthukkboqv.html

Py:   asyncio.gather(*tasks)
来源：http://hz.svipenyu.cn/gtmkcvsffk.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.andypj.xyz/gtfzfeixzj.html

JS:   await Promise.all(tasks)
来源：http://hz.hfpthk.cn/gtqxulvlsr.html

TS:   await Promise.all(tasks)
来源：http://hz.yonumen.top/gtevhuuutj.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.ydzc1.top/gtotevwbwr.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.ydjk.org.cn/gtwkifrxbm.html

Ruby: threads.map(&:join)
来源：http://hz.guannengcc.top/gtqavzegqm.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.guannengcc.top/gthetcmmlg.html

[O06] 使用进程池
来源：http://hz.kuanghao11.cn/gteeqxeezq.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.jqgufenzy.top/gtojbdmvnk.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.hnqzz.top/gtfcijusmh.html

JS:   // child_process / cluster 模块
来源：http://hz.hnqzz.top/gtwkjrhjvd.html

TS:   // child_process / cluster 模块
来源：http://hz.zhaomingkeji.xyz/gtmcdzghnm.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.cashguo.top/gtgsirnidy.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.redwolf501.top/gtqliisjke.html

Ruby: // fork 块
来源：http://hz.nwbrower.top/gtfhjwqeza.html

C#:   Parallel.For
来源：http://hz.xingfuxueyuan.xyz/gthgalofhf.html

================================================================================
来源：http://hz.hfpthk.cn/gtugswuuix.html

P. 常用工具函数
来源：http://hz.xinyue.icu/gttqkxkrgw.html

================================================================================
来源：http://hz.316326.xyz/gtbmmzckpr.html

[P01] 生成 UUID
来源：http://hz.hywenlv.cn/gthvguqlkb.html

Py:   str(uuid.uuid4())
来源：http://hz.jiagoushi.top/gtqhdioeyo.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.pycfn.com/gtqjrfcksw.html

JS:   crypto.randomUUID()
来源：http://hz.yj20258.top/gthkehfnrm.html

TS:   crypto.randomUUID()
来源：http://hz.haohaochexian.top/gtliqznvxc.html

Java: UUID.randomUUID().toString()
来源：http://hz.yvedp.cn/gtchcezjzw.html

Go:   // 用 github.com/google/uuid
来源：http://hz.aibaodan.cn/gtoymwntqk.html

Ruby: SecureRandom.uuid
来源：http://hz.0kj1m.cn/gtjdprybjp.html


<!-- 参考信息 -->