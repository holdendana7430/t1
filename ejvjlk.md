代发 wailian999

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.nanxinkj.top/gtvrpdjhsp.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yueranfly.top/gtwbcfnkte.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.meibo888.top/gtlkmaqvms.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.hywenlv.cn/gtprmxltet.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.wangshuangyany.cn/gtcxyxmioi.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.cashguo.top/gtbmpiloqb.html

[L05] 上传文件（multipart）
来源：http://hz.chenzaomai.com/gtjiqnpatu.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.yvedp.cn/gtivmkwyna.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.shzxlz.cn/gtbhgophdg.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.hnxiangtu.top/gtewrihufy.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.chenzaomai.com/gtrmdywbix.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.quarkkingdee.top/gtaruikdrt.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.zhoulong.xyz/gtksfdbito.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.zhongyouzk.top/gtekdratax.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.bjfxy.top/gtbbvhxhcp.html

[L06] 解析响应为 JSON
来源：http://hz.c1oappe.top/gtibkyfkdw.html

Py:   resp.json()
来源：http://hz.yuxming.cn/gtsepvpbnd.html

PHP:  json_decode($body, true);
来源：http://hz.wangshuangyany.cn/gtdbgssasp.html

JS:   await resp.json()
来源：http://hz.c1oappe.top/gtgzgcmbyr.html

TS:   await resp.json()
来源：http://hz.xuetiantiany.cn/gtjrccntsu.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.redwolf501.top/gtiexrmwmn.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.cashguo.top/gtwvmywsec.html

Ruby: JSON.parse(resp.body)
来源：http://hz.zhengqikj.top/gtgnkcexsc.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.zhijiandao.cn/gtqknenmev.html

[L07] 处理 HTTP 状态码
来源：http://hz.cheryme.top/gtiqavhynk.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.gaohongyu789.top/gttqilvijd.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.jqgufenzy.top/gtfrvblyhn.html

JS:   resp.ok;  resp.status
来源：http://hz.dianchejie.cn/gtmkhftzoh.html

TS:   resp.ok;  resp.status
来源：http://hz.zycfv.cn/gtzrtxgypg.html

Java: resp.statusCode()
来源：http://hz.ppjwa.cn/gtyoqjeavx.html

Go:   resp.StatusCode
来源：http://hz.haohaochexian.top/gtrxbnohns.html

Ruby: resp.code.to_i
来源：http://hz.haohaochexian.top/gtrjnxpyvl.html

C#:   (int)resp.StatusCode
来源：http://hz.guowangkeji.top/gtcgcraymk.html

[L08] 并发请求多个地址
来源：http://hz.yangfankeji.com/gtidmkgtoo.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.yj20258888.top/gtkhxtgjyi.html

PHP:  curl_multi_init() 系列
来源：http://hz.wangshuangyany.cn/gtnnzaftub.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhengqikj.top/gttgfdnbvi.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.xziqi.cn/gtwopfygnf.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.daxiang520.top/gtrtwvjvjd.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.jinyuanbaomall.cn/gtjtiqbzpo.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.yonumen.top/gtetnardao.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.bjfxy.top/gtwkcbiije.html

================================================================================
来源：http://hz.jyoumei.cn/gtlscwuqxh.html

M. 命令行 / 进程 / 环境
来源：http://hz.yvedp.cn/gtxrsyfhpc.html

================================================================================
来源：http://hz.ydzc1.top/gtjruxdvct.html

[M01] 读取命令行参数
来源：http://hz.cashguo.top/gtctdtokwa.html

Py:   sys.argv[1:]
来源：http://hz.xuanzx.com/gttqrzgdvc.html

PHP:  $argv;  $argc;
来源：http://hz.aibaodan.cn/gtxbxdxvkl.html

JS:   process.argv.slice(2)
来源：http://hz.sufxvd.cn/gtvagajgiw.html

TS:   process.argv.slice(2)
来源：http://hz.jiagoushi.top/gttgxsvcqw.html

Java: args 数组（main 方法参数）
来源：http://hz.ywan-chungtsiang.top/gtkxyywcig.html

Go:   os.Args[1:]
来源：http://hz.snrcjt.cn/gtipecsyxd.html

Ruby: ARGV
来源：http://hz.hfpthk.cn/gtffberlak.html

C#:   args 数组（Main 方法参数）
来源：http://hz.kuanghao11.cn/gtddlnenjz.html

[M02] 读取环境变量
来源：http://hz.chenzaomai.com/gtcfdowesb.html

Py:   os.environ.get("HOME")
来源：http://hz.vqdsnc.cn/gtxaphekwz.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.316326.xyz/gtqlvawnbh.html

JS:   process.env.HOME
来源：http://hz.aizwys.cn/gtuinkmbxt.html

TS:   process.env.HOME
来源：http://hz.jqgufenzy.top/gthdbqaapf.html

Java: System.getenv("HOME")
来源：http://hz.feifeiyinyue.top/gtxkvwxekp.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.zdqjudy.top/gtsgqulkma.html

Ruby: ENV["HOME"]
来源：http://hz.9152youxi.cn/gtvjsggfja.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.xziqi.cn/gtwdpnqqhw.html

[M03] 执行外部命令
来源：http://hz.xuanzx.com/gtwjcebddv.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.ydjk.org.cn/gtmdsgoaud.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.jqgufenzy.top/gtcmqiudvo.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.pycfn.com/gttaujryfh.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.zhiwuduotai.top/gtntbikzsa.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.ydzc1.top/gtnbavknkh.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.jianghu66.top/gtytmnsnyd.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.guannengcc.top/gtoaggvahy.html

C#:   Process.Start("ls", "-l");
来源：http://hz.andypj.xyz/gtwcjrjbjx.html

[M04] 获取当前工作目录
来源：http://hz.xuetiantiany.cn/gtogpnwixj.html

Py:   os.getcwd()
来源：http://hz.cdnleiting.top/gtnnxshlpm.html

PHP:  getcwd();
来源：http://hz.chenjidiqi.icu/gtxnxtqvwe.html

JS:   process.cwd()
来源：http://hz.jyoumei.cn/gtvftmculx.html

TS:   process.cwd()
来源：http://hz.ydzc1.top/gtanjbnfxn.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.svipenyu.cn/gtlestiofb.html

Go:   os.Getwd()
来源：http://hz.xziqi.cn/gtprcqbany.html

Ruby: Dir.pwd
来源：http://hz.sweek.top/gtgxyzmpof.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.gzhubu.top/gtsysqfbed.html

[M05] 设置退出码
来源：http://hz.nanxuanxn.top/gtmjcxoldm.html

Py:   sys.exit(1)
来源：http://hz.shanyushiyangtech.top/gtoqsljkky.html

PHP:  exit(1);
来源：http://hz.redwolf501.top/gtnziyzqhg.html

JS:   process.exit(1)
来源：http://hz.hammf.cn/gtbgdmulnv.html

TS:   process.exit(1)
来源：http://hz.zhongyouzk.top/gtknomtequ.html

Java: System.exit(1)
来源：http://hz.quarkkingdee.top/gttxrngujj.html

Go:   os.Exit(1)
来源：http://hz.ywan-chungtsiang.top/gtzmtbxrjn.html

Ruby: exit 1
来源：http://hz.chenlongwang.top/gtypbwxqad.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.xingfuxueyuan.xyz/gtvgkddjnm.html

[M06] 向标准错误输出
来源：http://hz.andypj.xyz/gtnefdnsnx.html

Py:   print("err", file=sys.stderr)
来源：http://hz.sysykeji.top/gtxhnboahf.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.zhoulong.xyz/gtzaxnygit.html

JS:   console.error("err")
来源：http://hz.ybcxt.top/gtzaieooas.html

TS:   console.error("err")
来源：http://hz.jiagoushi.top/gtvycgebvs.html

Java: System.err.println("err")
来源：http://hz.yonumen.top/gtbctmqimb.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.sysykeji.top/gtqgtasnjn.html

Ruby: warn "err"
来源：http://hz.xingfuxueyuan.xyz/gtvncrjbab.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.ivvv.top/gtcfatqgqo.html

[M07] 判断是否为主入口
来源：http://hz.fzhhl.top/gtsvqqjpqx.html

Py:   if __name__ == "__main__":
来源：http://hz.sysykeji.top/gtdttrmsps.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.guowangkeji.top/gtmmemnkri.html

JS:   require.main === module
来源：http://hz.zhongyouzk.top/gtmyjooekh.html

TS:   require.main === module
来源：http://hz.cashguo.top/gtfialefah.html

Java: public static void main(String[] args)
来源：http://hz.yonumen.top/gtdxssqvst.html

Go:   func main()
来源：http://hz.pengpengdd.cyou/gtaamajzmr.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.ppjwa.cn/gturitatin.html

C#:   static void Main(string[] args)
来源：http://hz.hongshengwenyu.top/gtawfmvvhz.html

[M08] 获取系统与运行时信息
来源：http://hz.zhaomingkeji.xyz/gtqgtqekhp.html

Py:   platform.system();  platform.python_version()
来源：http://hz.ydjk.org.cn/gtisdplvef.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.jinqigfzy.top/gthdjzojsj.html

JS:   process.platform;  process.version
来源：http://hz.dashuyun.cn/gtnhkyknlt.html

TS:   process.platform;  process.version
来源：http://hz.feifeiyinyue.top/gtkxjreczs.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.iojbl.cn/gtdogaggff.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.jinqigufen.top/gtgixewsqp.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.redwolf501.top/gthmcjjnaq.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.yj202588.top/gtyckclcte.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtpndbndes.html

N. 数据结构与算法
来源：http://hz.hnxiangtu.top/gtvzowptne.html

================================================================================
来源：http://hz.daria6918.cn/gtgdaqukus.html

[N01] 二分查找（有序数组）
来源：http://hz.sysykeji.top/gtpydomvqd.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.jinghuilouyu.cn/gtzvebmzls.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.cashguo.top/gtkxvogkzi.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.smart0.xyz/gtjjfcqmkh.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.pengpengdd.cyou/gtxvaxdppy.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.cheryme.top/gtisvohkoh.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.shangyingyoupin.top/gtvmlzuyaz.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.shangyingyoupin.top/gtptnonctn.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.yanxiufei.cn/gtnmkmvqap.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.316326.xyz/gtghpxnqxh.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.yanxiufei.cn/gtmuzebopx.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.birdmap.top/gtcgfljbws.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.gzhubu.top/gtgelsbzew.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.hysaishi.cn/gtcryorczf.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.ivvv.top/gtawygpugg.html

Go:   slices.Sort(arr)
来源：http://hz.xingfuxueyuan.xyz/gttwdgfwli.html

Ruby: arr.sort
来源：http://hz.c1oappe.top/gtxrmxlnyc.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.zhongyouzk.top/gtrzgrcepj.html

[N03] 快速排序（分治示例）
来源：http://hz.tian-w.cn/gtjzujmood.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.yj202588.top/gtedontujk.html

PHP:  // 递归实现，或用 usort
来源：http://hz.tanke756.top/gtwzmvesgv.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zhaomingkeji.xyz/gtbinikfvb.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.9152youxi.cn/gtqxxeawrp.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.zycfv.cn/gtqpjoodhp.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.fengsongda.top/gtmburzcbs.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.jinghuilouyu.cn/gtcaumrmqr.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.ppjwa.cn/gturewfoly.html

[N04] 斐波那契数列
来源：http://hz.cheryme.top/gtizsuluew.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.zhijiandao.cn/gtpocaubhx.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.hnxiangtu.top/gtlybkkjbq.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.cqqwz.cn/gtyutzwmtk.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.chenlongwang.top/gtkzwdgasf.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.yj20258.top/gtznxkgfxv.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.xuanzx.com/gtrolekueg.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.zhaomingkeji.xyz/gtjhvazcss.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.jinqigfzy.top/gtyimkrebp.html

[N05] 最大公约数
来源：http://hz.zdqjudy.top/gtqecixafo.html

Py:   math.gcd(a, b)
来源：http://hz.bjfxy.top/gtbovjtlmb.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.shanyushiyangtech.top/gtuaasnnic.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.daxiang520.top/gthwlzgyxn.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jqgfzy.top/gtvhawvzhv.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.cdnleiting.top/gtdfudytxd.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.316326.xyz/gtqrcfjmtg.html

Ruby: a.gcd(b)
来源：http://hz.hongshengwenyu.top/gtuzvxkxtk.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.hnqzz.top/gtvshvicjo.html

[N06] 判断回文字符串
来源：http://hz.hysaishi.cn/gtwgxuzcyq.html

Py:   s == s[::-1]
来源：http://hz.xylfe.cn/gtcrnghyqw.html

PHP:  $s === strrev($s);
来源：http://hz.tianlin.xyz/gtnwsqnuww.html

JS:   s === [...s].reverse().join("")
来源：http://hz.chenlongwang.top/gteiaxllet.html

TS:   s === [...s].reverse().join("")
来源：http://hz.pengpengdd.cyou/gtiwgmogal.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.chenlongwang.top/gtgogpdalq.html

Go:   // 双指针从两端比较
来源：http://hz.chenlongwang.top/gtfbslxade.html

Ruby: s == s.reverse
来源：http://hz.yj202588.top/gtmyoiolsb.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.haohaochexian.top/gtvpljabqe.html

[N07] 两数之和（返回下标）
来源：http://hz.nanxinkj.top/gthpoqmuqd.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.sweek.top/gtrcaaayqe.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.ehwqpu.com/gthdnybeme.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.havefunace.top/gtscdkiluy.html

TS:   // 手写 Map<string, number>
来源：http://hz.daria6918.cn/gtgsjbcnmw.html

Java: // 手写 HashMap
来源：http://hz.shuidangran.top/gtxslqpmrl.html

Go:   // 手写 map[int]int
来源：http://hz.pengpengdd.cyou/gtidcanyxa.html

Ruby: // 手写 Hash
来源：http://hz.cdnleiting.top/gtndvscmih.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.jqgfzy.top/gtonfghbyq.html

[N08] 生成全排列
来源：http://hz.haohaochexian.top/gtnffcxvjd.html

Py:   itertools.permutations(arr)
来源：http://hz.zhongyouzk.top/gththzhurw.html

PHP:  // 手写递归交换
来源：http://hz.hnxiangtu.top/gtosqmcorh.html

JS:   // 手写回溯递归
来源：http://hz.dianchejie.cn/gtirnfovlx.html

TS:   // 手写回溯递归
来源：http://hz.hongshengwenyu.top/gtboqbgftn.html

Java: // 手写回溯递归
来源：http://hz.chenlongwang.top/gtekufypcl.html

Go:   // 手写回溯递归
来源：http://hz.yanxiufei.cn/gtfghqygqy.html

Ruby: arr.permutation.to_a
来源：http://hz.xylfe.cn/gtnsegeiwq.html

C#:   // 手写回溯递归
来源：http://hz.9152youxi.cn/gtfhmukgjs.html

[N09] 栈与队列
来源：http://hz.316326.xyz/gtiwqgsjio.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.xinyue.icu/gtcmowjqfp.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.sufxvd.cn/gthjxhhafj.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.daxiang520.top/gtaedhdltz.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.chenlongwang.top/gtyquevytc.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.hongshengwenyu.top/gtjjfcnmdo.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.9152youxi.cn/gtdlqdyidz.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.zycfv.cn/gtgvllxotz.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.xuetiantiany.cn/gtlfanurbp.html

[N10] 链表节点定义
来源：http://hz.ppjwa.cn/gtqwmweqpr.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.snrcjt.cn/gtstslkzbe.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.jyoumei.cn/gtdicladyp.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.chenjidiqi.icu/gtrgreonvk.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.pengpengdd.cyou/gtfgjwdsfl.html

Java: class Node { int v; Node next; }
来源：http://hz.aibaodan.cn/gtxwhpfcaa.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.guannengcc.top/gtuztboxvf.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.jinqigufen.top/gtizrytvjq.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.hongshengwenyu.top/gtpleboxsw.html

[N11] 二叉树中序遍历
来源：http://hz.nwbrower.top/gtvwzkggci.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.xinyue.icu/gtuiizskop.html

PHP:  // 手写递归函数
来源：http://hz.hnqzz.top/gtgundcrub.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yonumen.top/gtspqueiiq.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.xuanzx.com/gtpyonrczd.html

Java: // 手写递归
来源：http://hz.zhijiandao.cn/gtjbqbbtyd.html

Go:   // 手写递归
来源：http://hz.yonumen.top/gtbclmqztw.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.tian-w.cn/gtjhepdrwe.html

C#:   // 手写递归
来源：http://hz.jqgufenzy.top/gtwcrkjfkq.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.zycfv.cn/gtzbzfxocx.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.jyoumei.cn/gtjtbhmhbj.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.cashguo.top/gtwicqkwvi.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.shuidangran.top/gtksnbjeof.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jinghuilouyu.cn/gtzbmggkdx.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.jinqigufen.top/gthtrdicgr.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.jianghu66.top/gtcztjgjlz.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.birdmap.top/gtaulbydlm.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.birdmap.top/gtfpwmhyrp.html

================================================================================
来源：http://hz.ybcxt.top/gtsgkhvbaq.html

O. 并发与异步
来源：http://hz.hysaishi.cn/gtubxycvdr.html

================================================================================
来源：http://hz.zhoulong.xyz/gtkhkggwss.html

[O01] 启动一个线程
来源：http://hz.jianghu66.top/gtimkafznz.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.yongpay.top/gtfflzvamu.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.jinqigufen.top/gtvfzwvvxx.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.cdnleiting.top/gtaykeqvgp.html

TS:   // 同 JS
来源：http://hz.xylfe.cn/gtcgwsirzq.html

Java: new Thread(() -> f()).start()
来源：http://hz.haohaochexian.top/gtrbvmzlic.html

Go:   go f()
来源：http://hz.daxiang520.top/gtvugmmeno.html

Ruby: Thread.new { f }
来源：http://hz.shanyushiyangtech.top/gthumokxvy.html

C#:   Task.Run(() => F());
来源：http://hz.ivvv.top/gtlxfwjksq.html

[O02] 使用线程池
来源：http://hz.yanxiufei.cn/gtmgjyzegb.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.wangshuangyany.cn/gtnviuhsde.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.chenjidiqi.icu/gtfwafbskm.html

JS:   // worker_threads 线程池
来源：http://hz.xingfuxueyuan.xyz/gtgfdoaqaj.html

TS:   // worker_threads 线程池
来源：http://hz.yj20258.top/gtwdfvogbv.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.zhixingplan.top/gtmukawabi.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.hongshengwenyu.top/gtshxbzfua.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.shzxlz.cn/gtahlfqubn.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.chenjidiqi.icu/gtzkmvgarn.html

[O03] 加锁保护共享数据
来源：http://hz.tanke756.top/gthuubwdpj.html

Py:   with lock: shared += 1
来源：http://hz.jianghu66.top/gtfcyedkbs.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.redwolf501.top/gtdiqyctzk.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.cheryme.top/gtdpexcjtd.html

TS:   // 同 JS
来源：http://hz.dianchejie.cn/gtgjnyafoy.html

Java: synchronized (this) { shared++; }
来源：http://hz.jianghu66.top/gttcatotsk.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.birdmap.top/gtneydcbsg.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.52xcode.cn/gtvbsiamuv.html

C#:   lock (gate) { shared++; }
来源：http://hz.zhaomingkeji.xyz/gtabdhxgud.html

[O04] 定义异步函数并等待
来源：http://hz.ydzc1.top/gtgzgshfyt.html

Py:   async def f():⏎    await g()
来源：http://hz.zhengqikj.top/gtvgfjnrcy.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.hfpthk.cn/gtsdmnrbbf.html

JS:   async function f() { await g(); }
来源：http://hz.svipenyu.cn/gttvorkhlb.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.ydzc1.top/gtkotdwhie.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.quarkkingdee.top/gtkibxtapb.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.yuxming.cn/gtyspgecsx.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.cucudq.cn/gtdlmzatal.html

C#:   async Task F() { await G(); }
来源：http://hz.zhongyouzk.top/gtlmnsobtv.html

[O05] 并发执行并等待全部完成
来源：http://hz.aizwys.cn/gtaafsoppw.html

Py:   asyncio.gather(*tasks)
来源：http://hz.bjfxy.top/gtilhomayt.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.gogol.net.cn/gtflcpzobw.html

JS:   await Promise.all(tasks)
来源：http://hz.ybcxt.top/gtopovxzhl.html

TS:   await Promise.all(tasks)
来源：http://hz.zhijiandao.cn/gtugfxvncc.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.cucudq.cn/gtqcwsygsl.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.hnqzz.top/gtmwfsdsrk.html

Ruby: threads.map(&:join)
来源：http://hz.yueranfly.top/gtosbwpxia.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.ivvv.top/gtwpmuskay.html

[O06] 使用进程池
来源：http://hz.zhixingplan.top/gtkixsvebo.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.haohaochexian.top/gthhyzlifv.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.nanxuanxn.top/gtouwztpbu.html

JS:   // child_process / cluster 模块
来源：http://hz.zhijiandao.cn/gtpfdzjauv.html

TS:   // child_process / cluster 模块
来源：http://hz.meibo888.top/gtownsaslc.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.redwolf501.top/gtbifhxewb.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.gaohongyu789.top/gtfhmvqtjz.html

Ruby: // fork 块
来源：http://hz.feifeiyinyue.top/gtshftuiih.html

C#:   Parallel.For
来源：http://hz.cqqwz.cn/gtwgbhzegv.html

================================================================================
来源：http://hz.cqqwz.cn/gtxwwiqofp.html

P. 常用工具函数
来源：http://hz.c1oappe.top/gtbkypfwyu.html

================================================================================
来源：http://hz.316326.xyz/gteoboeurq.html

[P01] 生成 UUID
来源：http://hz.zhaomingkeji.xyz/gtpjusjjgv.html

Py:   str(uuid.uuid4())
来源：http://hz.svipenyu.cn/gtxhfyjbfp.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.yanxiufei.cn/gthsuaieik.html

JS:   crypto.randomUUID()
来源：http://hz.yj202588.top/gtthcwrojj.html

TS:   crypto.randomUUID()
来源：http://hz.aibaodan.cn/gtfnfjxlxp.html

Java: UUID.randomUUID().toString()
来源：http://hz.zhengqikj.top/gtaorucqlm.html

Go:   // 用 github.com/google/uuid
来源：http://hz.snrcjt.cn/gtsvnefxzw.html

Ruby: SecureRandom.uuid
来源：http://hz.jyoumei.cn/gtplrtxait.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.iojbl.cn/gtswspxbcf.html

[P02] MD5 / SHA256 摘要
来源：http://hz.zdqjudy.top/gtrtgypzim.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.yj20258888.top/gtcxvedusd.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.zhongyouzk.top/gtderkppzb.html


<!-- 参考信息 -->