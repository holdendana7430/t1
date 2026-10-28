代发 wailian999

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yuxming.cn/gttimqqlie.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.bjfxy.top/gtcgidkaqk.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.daria6918.cn/gtwvsalldi.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.kuanghao11.cn/gtfsniilkv.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.yonumen.top/gthzdgdlbu.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.hnqzz.top/gtjzupyhfv.html

[L05] 上传文件（multipart）
来源：http://hz.ydzc1.top/gtizgguoai.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.yj20258888.top/gtlktqmopt.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.yuxming.cn/gtemaxejkm.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.tian-w.cn/gthrdrrzvp.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.hammf.cn/gtehxefnge.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.tanke756.top/gtaudnczwf.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.meibo888.top/gtwmxeduoi.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.zhiwuduotai.top/gtwgpshshm.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.yvedp.cn/gtcljvzpus.html

[L06] 解析响应为 JSON
来源：http://hz.jinyuanbaomall.cn/gtnsrnivgp.html

Py:   resp.json()
来源：http://hz.kuanghao11.cn/gtqkwzflvp.html

PHP:  json_decode($body, true);
来源：http://hz.yuanzhike.top/gtodtzmqvi.html

JS:   await resp.json()
来源：http://hz.xinyue.icu/gtmqvptwnp.html

TS:   await resp.json()
来源：http://hz.gaohongyu789.top/gtvxdgyjep.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.yuxming.cn/gtlcbjqikx.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.xylfe.cn/gtdybautgs.html

Ruby: JSON.parse(resp.body)
来源：http://hz.xuanzx.com/gtgfknuqwg.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.jinqigufen.top/gtudajfbhx.html

[L07] 处理 HTTP 状态码
来源：http://hz.vqdsnc.cn/gtiztmegit.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.snrcjt.cn/gtmmyficcj.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.hammf.cn/gtmivxwpml.html

JS:   resp.ok;  resp.status
来源：http://hz.hongshengwenyu.top/gtiawywfeb.html

TS:   resp.ok;  resp.status
来源：http://hz.jyoumei.cn/gtyaeucxiv.html

Java: resp.statusCode()
来源：http://hz.zhengqikj.top/gtnllpglyr.html

Go:   resp.StatusCode
来源：http://hz.daxiang520.top/gtjkitxwqg.html

Ruby: resp.code.to_i
来源：http://hz.guannengcc.top/gtmobpnksp.html

C#:   (int)resp.StatusCode
来源：http://hz.pycfn.com/gtmgomoceb.html

[L08] 并发请求多个地址
来源：http://hz.yvedp.cn/gtueidkwdd.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.fzhhl.top/gtclgsezlg.html

PHP:  curl_multi_init() 系列
来源：http://hz.shanyushiyangkeji.top/gtevmjsyxl.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yonumen.top/gtdtfluhbn.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.dashuyun.cn/gtycxccgnw.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.feifeiyinyue.top/gtwlzyqsfo.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.zhaomingkeji.xyz/gtjggawllo.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.c1oappe.top/gtondsehel.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.quarkkingdee.top/gtqaxmmher.html

================================================================================
来源：http://hz.wangdashe.top/gtppsohccw.html

M. 命令行 / 进程 / 环境
来源：http://hz.cashguo.top/gtxsojrqjt.html

================================================================================
来源：http://hz.xylfe.cn/gtbzwpaeva.html

[M01] 读取命令行参数
来源：http://hz.dashuyun.cn/gtwukzdujz.html

Py:   sys.argv[1:]
来源：http://hz.jyoumei.cn/gtnwlwwuor.html

PHP:  $argv;  $argc;
来源：http://hz.feifeiyinyue.top/gtbjckzrme.html

JS:   process.argv.slice(2)
来源：http://hz.shzxlz.cn/gtvegroykn.html

TS:   process.argv.slice(2)
来源：http://hz.zdqjudy.top/gtipfanusp.html

Java: args 数组（main 方法参数）
来源：http://hz.sysykeji.top/gtualczulf.html

Go:   os.Args[1:]
来源：http://hz.gogol.net.cn/gtkkiicqka.html

Ruby: ARGV
来源：http://hz.jinqigufen.top/gtwbqqzats.html

C#:   args 数组（Main 方法参数）
来源：http://hz.snrcjt.cn/gtdkikejau.html

[M02] 读取环境变量
来源：http://hz.zhongyouzk.top/gtypoeyazt.html

Py:   os.environ.get("HOME")
来源：http://hz.zhiwuduotai.top/gtujqopsgc.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.guowangkeji.top/gtbzavvvxu.html

JS:   process.env.HOME
来源：http://hz.jinqigfzy.top/gtfvxtfcce.html

TS:   process.env.HOME
来源：http://hz.tian-w.cn/gtzgrrambi.html

Java: System.getenv("HOME")
来源：http://hz.vqdsnc.cn/gtkldrfhpj.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.zycfv.cn/gtyoywlisb.html

Ruby: ENV["HOME"]
来源：http://hz.hongshengwenyu.top/gtgszwagii.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.cheryme.top/gtecpwtgjl.html

[M03] 执行外部命令
来源：http://hz.yangfankeji.com/gtrrrmcqqy.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.guannengcc.top/gtqedxugvh.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.sweek.top/gtvxtpieso.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.daxiang520.top/gtbcivqnhb.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.xuanzx.com/gtlfppmmbz.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.yongpay.top/gtkelfpebm.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.zhixingplan.top/gtfteqakbh.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.aibaodan.cn/gtzhcwoctj.html

C#:   Process.Start("ls", "-l");
来源：http://hz.xuetiantiany.cn/gtxkzzupll.html

[M04] 获取当前工作目录
来源：http://hz.nanxuanxn.top/gtxtfqjgrq.html

Py:   os.getcwd()
来源：http://hz.jinqigufen.top/gtsnxjuzqy.html

PHP:  getcwd();
来源：http://hz.mhx1999.top/gtarjubnzf.html

JS:   process.cwd()
来源：http://hz.jianghu66.top/gtlgqmowuu.html

TS:   process.cwd()
来源：http://hz.yj202588.top/gtomhyfdov.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.dashuyun.cn/gttuucymhv.html

Go:   os.Getwd()
来源：http://hz.yj20258.top/gtgbgcrnox.html

Ruby: Dir.pwd
来源：http://hz.sweek.top/gtempltbno.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.iojbl.cn/gtktnatung.html

[M05] 设置退出码
来源：http://hz.hongshengwenyu.top/gtghonanyt.html

Py:   sys.exit(1)
来源：http://hz.zhijiandao.cn/gtxlotkdmv.html

PHP:  exit(1);
来源：http://hz.nanxuanxn.top/gtmoqwftyz.html

JS:   process.exit(1)
来源：http://hz.andypj.xyz/gtvlanacjk.html

TS:   process.exit(1)
来源：http://hz.havefunace.top/gtoodhddkk.html

Java: System.exit(1)
来源：http://hz.yongpay.top/gtmwdcdkgq.html

Go:   os.Exit(1)
来源：http://hz.chenzaomai.com/gtxuxvvfai.html

Ruby: exit 1
来源：http://hz.jianghu66.top/gtwwleubgk.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.hammf.cn/gtvcztyscu.html

[M06] 向标准错误输出
来源：http://hz.havefunace.top/gtjqemgiwd.html

Py:   print("err", file=sys.stderr)
来源：http://hz.ehwqpu.com/gtwvzhpqrd.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.gzhubu.top/gtxvovweuy.html

JS:   console.error("err")
来源：http://hz.haohaochexian.top/gtzltljwjs.html

TS:   console.error("err")
来源：http://hz.jinqigfzy.top/gtfcuhwiiv.html

Java: System.err.println("err")
来源：http://hz.xylfe.cn/gtwkfvshjf.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.nwbrower.top/gtyemzkado.html

Ruby: warn "err"
来源：http://hz.316326.xyz/gteuwmpvrg.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.chenlongwang.top/gtwfqxdyko.html

[M07] 判断是否为主入口
来源：http://hz.jinqigufen.top/gtjhbfxdyb.html

Py:   if __name__ == "__main__":
来源：http://hz.jinghuilouyu.cn/gtzjbfyxip.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.ivvv.top/gtsxryrgzq.html

JS:   require.main === module
来源：http://hz.gzhubu.top/gtsfgiofpo.html

TS:   require.main === module
来源：http://hz.hysaishi.cn/gtbsxeobpk.html

Java: public static void main(String[] args)
来源：http://hz.jinghuilouyu.cn/gtjchkjtij.html

Go:   func main()
来源：http://hz.shzxlz.cn/gtfpsotmah.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.guowangkeji.top/gtgsaxkbwd.html

C#:   static void Main(string[] args)
来源：http://hz.zhaomingkeji.xyz/gtzeyjuami.html

[M08] 获取系统与运行时信息
来源：http://hz.shanyushiyangtech.top/gthieaewac.html

Py:   platform.system();  platform.python_version()
来源：http://hz.zhongyouzk.top/gthlaiidpo.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.cashguo.top/gtkljczwkd.html

JS:   process.platform;  process.version
来源：http://hz.hysaishi.cn/gtzfypnfnl.html

TS:   process.platform;  process.version
来源：http://hz.c1oappe.top/gtivndifpu.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.9152youxi.cn/gtgzeimrnw.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.ydzc1.top/gtyufsyeyc.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.wangshuangyany.cn/gtcpmdrghs.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.jinghuilouyu.cn/gtjltekzoj.html

================================================================================
来源：http://hz.zhongyouzk.top/gtpcozzpno.html

N. 数据结构与算法
来源：http://hz.xylfe.cn/gtbqaosreh.html

================================================================================
来源：http://hz.hfpthk.cn/gtukgsktps.html

[N01] 二分查找（有序数组）
来源：http://hz.cdnleiting.top/gtjthvkqbu.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.nanxinkj.top/gtmcmdnrwe.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.xylfe.cn/gtvmcfnyuw.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.meibo888.top/gthqgckmau.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jinghuilouyu.cn/gttmqdylej.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.yuxming.cn/gtdoxfgvsx.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.52xcode.cn/gtcigtwcgd.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.gogol.net.cn/gtlntoitek.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.nanxuanxn.top/gtskuocmmq.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.xziqi.cn/gtodixsuuh.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.xylfe.cn/gtvmkjxlvl.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.redwolf501.top/gtmrugfpmd.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yueranfly.top/gtfwfjillz.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.pengpengdd.cyou/gtsmmctqax.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.andypj.xyz/gtjqolrxbu.html

Go:   slices.Sort(arr)
来源：http://hz.andypj.xyz/gtaysovaxm.html

Ruby: arr.sort
来源：http://hz.gaohongyu789.top/gtypdgohaf.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.yanxiufei.cn/gtfxyicdzj.html

[N03] 快速排序（分治示例）
来源：http://hz.haohaochexian.top/gtvidreuyx.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.jqgufenzy.top/gtijowqffs.html

PHP:  // 递归实现，或用 usort
来源：http://hz.iojbl.cn/gtjznryxfs.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.ppjwa.cn/gtugxkotlw.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yuxming.cn/gtcagkrjbz.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.cucudq.cn/gtdhncuxqo.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.yonumen.top/gtdephqknh.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.c1oappe.top/gtkpnzhxpd.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.shzxlz.cn/gtxztuvxqf.html

[N04] 斐波那契数列
来源：http://hz.9152youxi.cn/gtdlafxqoc.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.ywan-chungtsiang.top/gtbcrsizxt.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.zhongyouzk.top/gtujwtxmke.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.smart0.xyz/gtysuzgjjt.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.sufxvd.cn/gtzxayusnk.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.meibo888.top/gtyxifmein.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.jinqigufen.top/gtrbbeyfuy.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.yueranfly.top/gtkgqoxvkk.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.nanxuanxn.top/gtdlisykwp.html

[N05] 最大公约数
来源：http://hz.zhaomingkeji.xyz/gtilpjhndg.html

Py:   math.gcd(a, b)
来源：http://hz.birdmap.top/gthksdcpcm.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.yuanzhike.top/gteiirskph.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.kuanghao11.cn/gtvcyhipgc.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.cheryme.top/gtiqjwldlg.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.daxiang520.top/gtcyxjyesu.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.nanxuanxn.top/gtzesdggtx.html

Ruby: a.gcd(b)
来源：http://hz.ivvv.top/gtauyrpdmu.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.shangyingyoupin.top/gtngzethnp.html

[N06] 判断回文字符串
来源：http://hz.smart0.xyz/gtaahbdbor.html

Py:   s == s[::-1]
来源：http://hz.jianghu66.top/gthaaphpqb.html

PHP:  $s === strrev($s);
来源：http://hz.haohaochexian.top/gtrtifiyyl.html

JS:   s === [...s].reverse().join("")
来源：http://hz.yj20258888.top/gtghxeeegi.html

TS:   s === [...s].reverse().join("")
来源：http://hz.gogol.net.cn/gtzrywxmyb.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.shangyingyoupin.top/gtohewkucs.html

Go:   // 双指针从两端比较
来源：http://hz.zhaomingkeji.xyz/gtyiojpgea.html

Ruby: s == s.reverse
来源：http://hz.gzhubu.top/gtslslscsk.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.yj202588.top/gttjpaoxqg.html

[N07] 两数之和（返回下标）
来源：http://hz.birdmap.top/gtluaxhqlh.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.hnxiangtu.top/gtwsyczroy.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.jinqigufen.top/gtxdbnqgvt.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.ppjwa.cn/gtatikzekq.html

TS:   // 手写 Map<string, number>
来源：http://hz.yj20258888.top/gtzcrhjngr.html

Java: // 手写 HashMap
来源：http://hz.shuidangran.top/gtvsasgttt.html

Go:   // 手写 map[int]int
来源：http://hz.fengsongda.top/gtgxoffjzl.html

Ruby: // 手写 Hash
来源：http://hz.cashguo.top/gtmxtmfbrn.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.tianlin.xyz/gtxftbptgd.html

[N08] 生成全排列
来源：http://hz.yj20258.top/gtffufevsl.html

Py:   itertools.permutations(arr)
来源：http://hz.hongshengwenyu.top/gtxhagjxth.html

PHP:  // 手写递归交换
来源：http://hz.cqqwz.cn/gtxrogcfef.html

JS:   // 手写回溯递归
来源：http://hz.cucudq.cn/gthjmkasar.html

TS:   // 手写回溯递归
来源：http://hz.hfpthk.cn/gtmqbfzcfl.html

Java: // 手写回溯递归
来源：http://hz.yj202588.top/gtjbypxzdw.html

Go:   // 手写回溯递归
来源：http://hz.fengsongda.top/gtkpacppfp.html

Ruby: arr.permutation.to_a
来源：http://hz.feifeiyinyue.top/gtvnvadbwi.html

C#:   // 手写回溯递归
来源：http://hz.ywan-chungtsiang.top/gtesmmocrl.html

[N09] 栈与队列
来源：http://hz.xuetiantiany.cn/gtxtamjspv.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.cheryme.top/gttkajnktr.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.xuanzx.com/gtmbdolnsc.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.nanxuanxn.top/gthmezhiro.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.daria6918.cn/gtjzrjqyjd.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.andypj.xyz/gthyqzfqob.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.fengsongda.top/gtkeladgrd.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.ybcxt.top/gtfdkssfss.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.sxryk.cn/gtqjkjyxnu.html

[N10] 链表节点定义
来源：http://hz.sufxvd.cn/gtivlrybxd.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.cucudq.cn/gtxnujkmep.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.yangfankeji.com/gtfrjnsbvt.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.hysaishi.cn/gtczkjldpw.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.shzxlz.cn/gtbxcpwatc.html

Java: class Node { int v; Node next; }
来源：http://hz.fengsongda.top/gtntfylglb.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.daria6918.cn/gtwhgnlgrc.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.sweek.top/gtiphvzqxo.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.iojbl.cn/gtlgvhnqsp.html

[N11] 二叉树中序遍历
来源：http://hz.iojbl.cn/gtnipdjlvo.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.zhixingplan.top/gtrphjleeg.html

PHP:  // 手写递归函数
来源：http://hz.mhx1999.top/gtsuavckut.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.xylfe.cn/gtmqkjiavc.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.gogol.net.cn/gtirxpsypn.html

Java: // 手写递归
来源：http://hz.tanke756.top/gtteolyvms.html

Go:   // 手写递归
来源：http://hz.hongshengwenyu.top/gtfssrvtfh.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.redwolf501.top/gtebynjvgi.html

C#:   // 手写递归
来源：http://hz.zhixingplan.top/gtjjibmovj.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.nwbrower.top/gtwuljhtus.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.wangshuangyany.cn/gtmgakilil.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.shangyingyoupin.top/gtksudcodz.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.svipenyu.cn/gtrsnrggmh.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.feifeiyinyue.top/gttjvukozd.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.pycfn.com/gtubwutpig.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.haohaochexian.top/gtdrbxnpkq.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.cqqwz.cn/gtmzbypbom.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.gotoacloud.top/gtqdjpgsfj.html

================================================================================
来源：http://hz.quarkkingdee.top/gtkkmslocv.html

O. 并发与异步
来源：http://hz.gzhubu.top/gtdrdxkonx.html

================================================================================
来源：http://hz.gzhubu.top/gtrtfluzsz.html

[O01] 启动一个线程
来源：http://hz.hysaishi.cn/gtyftzjsly.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.jqgfzy.top/gtyupdimoo.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.yvedp.cn/gtfxmzncdl.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.tian-w.cn/gtdztegbhj.html

TS:   // 同 JS
来源：http://hz.zhengqikj.top/gthezoolgf.html

Java: new Thread(() -> f()).start()
来源：http://hz.xuanzx.com/gterhhniin.html

Go:   go f()
来源：http://hz.jinqigfzy.top/gtuhqoqsok.html

Ruby: Thread.new { f }
来源：http://hz.cucudq.cn/gtngfesjgz.html

C#:   Task.Run(() => F());
来源：http://hz.dianchejie.cn/gtrvfqstmw.html

[O02] 使用线程池
来源：http://hz.yuxming.cn/gtxjedimki.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.gotoacloud.top/gtduewlryt.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.mhx1999.top/gtmdyezmmq.html

JS:   // worker_threads 线程池
来源：http://hz.fzhhl.top/gtgddijqzd.html

TS:   // worker_threads 线程池
来源：http://hz.zhiwuduotai.top/gtbzsnpyli.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.cucudq.cn/gtfpzmjxaw.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.c1oappe.top/gtlriowtjv.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.yongpay.top/gtudaxgyty.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.wangdashe.top/gtsgemager.html

[O03] 加锁保护共享数据
来源：http://hz.aizwys.cn/gtfbslzdzo.html

Py:   with lock: shared += 1
来源：http://hz.zhijiandao.cn/gtajnnqkju.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.svipenyu.cn/gtqklngqlx.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.cheryme.top/gtnuwqdtnn.html

TS:   // 同 JS
来源：http://hz.mhx1999.top/gtrvhzmduj.html

Java: synchronized (this) { shared++; }
来源：http://hz.feifeiyinyue.top/gtbdsyxekx.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.yuxming.cn/gtjwbedvcn.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.hammf.cn/gtgysbvlgj.html

C#:   lock (gate) { shared++; }
来源：http://hz.xuetiantiany.cn/gtspxiedac.html

[O04] 定义异步函数并等待
来源：http://hz.birdmap.top/gtmfrtkfpw.html

Py:   async def f():⏎    await g()
来源：http://hz.zhijiandao.cn/gtycfyqzqt.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.shanyushiyangtech.top/gtmupwevvd.html

JS:   async function f() { await g(); }
来源：http://hz.vqdsnc.cn/gtlxydlqnb.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.c1oappe.top/gtopbjhoos.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.sufxvd.cn/gtavoqxdjj.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.fengsongda.top/gtbkqdosai.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.cheryme.top/gtelgoxyii.html

C#:   async Task F() { await G(); }
来源：http://hz.zhiwuduotai.top/gtypmjnlal.html

[O05] 并发执行并等待全部完成
来源：http://hz.yj202588.top/gtfldmrkba.html

Py:   asyncio.gather(*tasks)
来源：http://hz.zhaomingkeji.xyz/gtiynasote.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.ybcxt.top/gttroofvhc.html

JS:   await Promise.all(tasks)
来源：http://hz.sysykeji.top/gtljlpllzd.html

TS:   await Promise.all(tasks)
来源：http://hz.cdnleiting.top/gtnwjmxroj.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.yueranfly.top/gtknrztbfp.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.hongshengwenyu.top/gtkkxdoebg.html

Ruby: threads.map(&:join)
来源：http://hz.smart0.xyz/gtjtwunskg.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.xingfuxueyuan.xyz/gtjeyhixqd.html

[O06] 使用进程池
来源：http://hz.jinghuilouyu.cn/gtrwdaqhsu.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.dashuyun.cn/gtdmzsbvjm.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.cheryme.top/gtiphawtrz.html

JS:   // child_process / cluster 模块
来源：http://hz.xingfuxueyuan.xyz/gtpjdfsyob.html

TS:   // child_process / cluster 模块
来源：http://hz.jqgfzy.top/gtcmvvelww.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.aibaodan.cn/gttfpnifjs.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.shanyushiyangkeji.top/gtdhgwfjlk.html

Ruby: // fork 块
来源：http://hz.hysaishi.cn/gtdpkwqwnx.html

C#:   Parallel.For
来源：http://hz.52xcode.cn/gtsrvauvvm.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtruvvroio.html

P. 常用工具函数
来源：http://hz.shanyushiyangtech.top/gtfobgoorz.html

================================================================================
来源：http://hz.sweek.top/gticdqcfxr.html

[P01] 生成 UUID
来源：http://hz.xylfe.cn/gtbbmsfhde.html

Py:   str(uuid.uuid4())
来源：http://hz.shanyushiyangtech.top/gtmqsqwhdi.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.jlsjyb.cn/gtbmtfgyuq.html

JS:   crypto.randomUUID()
来源：http://hz.zhiwuduotai.top/gtxvcqlfmo.html

TS:   crypto.randomUUID()
来源：http://hz.hnqzz.top/gtwftwgfzs.html

Java: UUID.randomUUID().toString()
来源：http://hz.aizwys.cn/gtgvbmyclw.html

Go:   // 用 github.com/google/uuid
来源：http://hz.aizwys.cn/gtffxxzfcc.html

Ruby: SecureRandom.uuid
来源：http://hz.jqgfzy.top/gtrisyczqy.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.shanyushiyangtech.top/gtvqduoduh.html

[P02] MD5 / SHA256 摘要
来源：http://hz.zycfv.cn/gthvznhycr.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.gaohongyu789.top/gtziktcwuq.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.cucudq.cn/gtqiutpxmo.html


<!-- 参考信息 -->