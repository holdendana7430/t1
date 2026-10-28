代发 wailian999

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.hnqzz.top/gtadwfarzq.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.9152youxi.cn/gtpsoeldwj.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.nanxinkj.top/gtgrqkmkqh.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.shzxlz.cn/gtufpapoqy.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.jianghu66.top/gtqabkkfsy.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.yongpay.top/gtfwcuajnk.html

[L05] 上传文件（multipart）
来源：http://hz.gaohongyu789.top/gtoczeydmn.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.xziqi.cn/gtqlqaizzl.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.ivvv.top/gteafnmuiu.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.shanyushiyangkeji.top/gtfxejvqeb.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.jinqigfzy.top/gthtrswfrv.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.52xcode.cn/gtpviennax.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.hnqzz.top/gticrcagkj.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.sysykeji.top/gtcviyjpou.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.cheryme.top/gterkecxkz.html

[L06] 解析响应为 JSON
来源：http://hz.yj202588.top/gtrvecqljj.html

Py:   resp.json()
来源：http://hz.yj202588.top/gtisikuxwl.html

PHP:  json_decode($body, true);
来源：http://hz.yanxiufei.cn/gthnsczjyu.html

JS:   await resp.json()
来源：http://hz.svipenyu.cn/gtevsgxqpw.html

TS:   await resp.json()
来源：http://hz.hnqzz.top/gtzpqhngrj.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.hnqzz.top/gtzoxmnxhx.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.tanke756.top/gtixgydzqz.html

Ruby: JSON.parse(resp.body)
来源：http://hz.hammf.cn/gtsrkymevr.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.ivvv.top/gtpkgjilmu.html

[L07] 处理 HTTP 状态码
来源：http://hz.xylfe.cn/gtyzyuxzrw.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.feifeiyinyue.top/gtgnydcprj.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.hnxiangtu.top/gtcaphsdfc.html

JS:   resp.ok;  resp.status
来源：http://hz.vqdsnc.cn/gtvwbstasc.html

TS:   resp.ok;  resp.status
来源：http://hz.zhaomingkeji.xyz/gtbsezskbw.html

Java: resp.statusCode()
来源：http://hz.birdmap.top/gtbibowaux.html

Go:   resp.StatusCode
来源：http://hz.yj20258.top/gtofjxtntv.html

Ruby: resp.code.to_i
来源：http://hz.jlsjyb.cn/gtbcltfisf.html

C#:   (int)resp.StatusCode
来源：http://hz.yangfankeji.com/gtkmkzsqix.html

[L08] 并发请求多个地址
来源：http://hz.shangyingyoupin.top/gtisfouxgn.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.xylfe.cn/gtnggqeeeq.html

PHP:  curl_multi_init() 系列
来源：http://hz.dashuyun.cn/gttmtnlqxd.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.aibaodan.cn/gtsmucisvp.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zdqjudy.top/gttpcitdao.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.zhongyouzk.top/gtaodhaapu.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.jqgfzy.top/gtduoghhrk.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.ivvv.top/gtdooryyzj.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.yangfankeji.com/gtzxztwdei.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtfjklrqba.html

M. 命令行 / 进程 / 环境
来源：http://hz.jyoumei.cn/gtskdnsojm.html

================================================================================
来源：http://hz.guowangkeji.top/gtplayuapr.html

[M01] 读取命令行参数
来源：http://hz.ybcxt.top/gttcyhepcx.html

Py:   sys.argv[1:]
来源：http://hz.pycfn.com/gtyrgrdumc.html

PHP:  $argv;  $argc;
来源：http://hz.ivvv.top/gtusjuumda.html

JS:   process.argv.slice(2)
来源：http://hz.shzxlz.cn/gtqwmwycrf.html

TS:   process.argv.slice(2)
来源：http://hz.xuetiantiany.cn/gtejvbnavb.html

Java: args 数组（main 方法参数）
来源：http://hz.pengpengdd.cyou/gtrlynkyhp.html

Go:   os.Args[1:]
来源：http://hz.zhiwuduotai.top/gtbrxzzzyl.html

Ruby: ARGV
来源：http://hz.cucudq.cn/gtljbsazzp.html

C#:   args 数组（Main 方法参数）
来源：http://hz.guowangkeji.top/gtzobxkrca.html

[M02] 读取环境变量
来源：http://hz.xuetiantiany.cn/gttoccrmkc.html

Py:   os.environ.get("HOME")
来源：http://hz.kuanghao11.cn/gtpjvrunoy.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.redwolf501.top/gtomkpmjrc.html

JS:   process.env.HOME
来源：http://hz.shzxlz.cn/gtuhhmjftf.html

TS:   process.env.HOME
来源：http://hz.jinghuilouyu.cn/gtkbblreir.html

Java: System.getenv("HOME")
来源：http://hz.zhixingplan.top/gtzaazzkni.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.feifeiyinyue.top/gtexhzfxtc.html

Ruby: ENV["HOME"]
来源：http://hz.zhengqikj.top/gtccxxujrh.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.zhaomingkeji.xyz/gtqrzyxtxc.html

[M03] 执行外部命令
来源：http://hz.yangfankeji.com/gthjqjiojj.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.guannengcc.top/gtcquxzrjp.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.dashuyun.cn/gtcfaorckn.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.hfpthk.cn/gtjlylgwhn.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.yj20258.top/gtgsqlmvdk.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.nanxinkj.top/gtmsveoiks.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.zhongyouzk.top/gtinjaprcq.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.xylfe.cn/gtpqdgltpu.html

C#:   Process.Start("ls", "-l");
来源：http://hz.hammf.cn/gtumnnwwti.html

[M04] 获取当前工作目录
来源：http://hz.ivvv.top/gtbkppzegq.html

Py:   os.getcwd()
来源：http://hz.zycfv.cn/gtkyphntrs.html

PHP:  getcwd();
来源：http://hz.gzhubu.top/gtbmdzypfp.html

JS:   process.cwd()
来源：http://hz.tanke756.top/gtvaqwlufa.html

TS:   process.cwd()
来源：http://hz.cheryme.top/gtksawtcbm.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.jinyuanbaomall.cn/gttudwiabn.html

Go:   os.Getwd()
来源：http://hz.zhiwuduotai.top/gtubhpefii.html

Ruby: Dir.pwd
来源：http://hz.aibaodan.cn/gtsfifvvyz.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.smart0.xyz/gtthfgcvlt.html

[M05] 设置退出码
来源：http://hz.pengpengdd.cyou/gtysupqifh.html

Py:   sys.exit(1)
来源：http://hz.hnqzz.top/gtshknjnku.html

PHP:  exit(1);
来源：http://hz.xingfuxueyuan.xyz/gtabsocqzt.html

JS:   process.exit(1)
来源：http://hz.fzhhl.top/gtyzgwqzxo.html

TS:   process.exit(1)
来源：http://hz.yuanzhike.top/gtmhxjkfym.html

Java: System.exit(1)
来源：http://hz.aibaodan.cn/gtjivsmedj.html

Go:   os.Exit(1)
来源：http://hz.sxryk.cn/gtmuskbodr.html

Ruby: exit 1
来源：http://hz.nanxuanxn.top/gtqkapdvbi.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.gzhubu.top/gtmckvebgk.html

[M06] 向标准错误输出
来源：http://hz.yj202588.top/gtcqaqjjtg.html

Py:   print("err", file=sys.stderr)
来源：http://hz.chenlongwang.top/gtredunwxy.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.yuxming.cn/gtxuvhlxwo.html

JS:   console.error("err")
来源：http://hz.yanxiufei.cn/gtmumlkomn.html

TS:   console.error("err")
来源：http://hz.redwolf501.top/gtmfquwung.html

Java: System.err.println("err")
来源：http://hz.nanxinkj.top/gtdnltiaye.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.zhengqikj.top/gtqqiszbod.html

Ruby: warn "err"
来源：http://hz.52xcode.cn/gtxsohkomk.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.zhixingplan.top/gtrkzippul.html

[M07] 判断是否为主入口
来源：http://hz.xingfuxueyuan.xyz/gtmcxcusuf.html

Py:   if __name__ == "__main__":
来源：http://hz.birdmap.top/gtrhooxlxh.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.chenjidiqi.icu/gtpmrwzavp.html

JS:   require.main === module
来源：http://hz.guannengcc.top/gtmjygzfjv.html

TS:   require.main === module
来源：http://hz.nwbrower.top/gttxkqmwqf.html

Java: public static void main(String[] args)
来源：http://hz.jinghuilouyu.cn/gtfyknxrbt.html

Go:   func main()
来源：http://hz.yueranfly.top/gtqkrgrlbk.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.sweek.top/gtzwtckgwz.html

C#:   static void Main(string[] args)
来源：http://hz.chenzaomai.com/gtiahdidwh.html

[M08] 获取系统与运行时信息
来源：http://hz.ybcxt.top/gtpnblnveb.html

Py:   platform.system();  platform.python_version()
来源：http://hz.yueranfly.top/gtgnbjedwk.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.bjfxy.top/gtxlmcaayn.html

JS:   process.platform;  process.version
来源：http://hz.xziqi.cn/gtsoucbohv.html

TS:   process.platform;  process.version
来源：http://hz.tian-w.cn/gtrjchlzqg.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.ydzc1.top/gtqixayglg.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.jlsjyb.cn/gtwaxkpxgq.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.jianghu66.top/gtncbuuvgd.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.birdmap.top/gtsikgwdql.html

================================================================================
来源：http://hz.yongpay.top/gtvsryzklb.html

N. 数据结构与算法
来源：http://hz.sysykeji.top/gtcpdgeivx.html

================================================================================
来源：http://hz.jyoumei.cn/gtlmhrabvk.html

[N01] 二分查找（有序数组）
来源：http://hz.xinyue.icu/gtpsctmagw.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.hywenlv.cn/gtealdrhsr.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.zhaomingkeji.xyz/gtlpwgiilq.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.svipenyu.cn/gtienvosfp.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.pengpengdd.cyou/gtvuvubdny.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.xuanzx.com/gtfwwjlylt.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.smart0.xyz/gttuslcrqc.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.jianghu66.top/gtbzuovgpk.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.316326.xyz/gtoiurkcuz.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.zhijiandao.cn/gtvmabzzwk.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.aibaodan.cn/gtngdjkgok.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.tanke756.top/gthichlohj.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yj20258.top/gtkdhwhemh.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.shanyushiyangkeji.top/gtucdfcwqd.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.yangfankeji.com/gtpnqwhbkm.html

Go:   slices.Sort(arr)
来源：http://hz.jiagoushi.top/gtbaepaqys.html

Ruby: arr.sort
来源：http://hz.hysaishi.cn/gtxdvwntvj.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.zdqjudy.top/gttijomgfn.html

[N03] 快速排序（分治示例）
来源：http://hz.gogol.net.cn/gtzxvcziqs.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.pycfn.com/gtjnbnyjqk.html

PHP:  // 递归实现，或用 usort
来源：http://hz.zycfv.cn/gtgpdnxpwj.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.9152youxi.cn/gtaavmyudu.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.ydzc1.top/gteoppbanp.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.ybcxt.top/gtsgyabqoz.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.xuanzx.com/gthngkwwuc.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.redwolf501.top/gtkcaevvtg.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.cashguo.top/gtjrpnalsc.html

[N04] 斐波那契数列
来源：http://hz.jqgfzy.top/gtcqwzkiyh.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.chenzaomai.com/gttsebohba.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.sweek.top/gtijtcjcda.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.hfpthk.cn/gtwaytdtcd.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.ydzc1.top/gtrwbruflm.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.gzhubu.top/gthtbczgua.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.jinqigufen.top/gtawuumfcw.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.zhengqikj.top/gtvsclxixk.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.redwolf501.top/gtnglkwtyo.html

[N05] 最大公约数
来源：http://hz.aizwys.cn/gtgdzjofer.html

Py:   math.gcd(a, b)
来源：http://hz.mhx1999.top/gtfvohguld.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.pengpengdd.cyou/gtpnzirxdl.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.andypj.xyz/gtccmfsums.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.chenzaomai.com/gttkwaksbe.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.snrcjt.cn/gtiqxxjvzz.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.chenlongwang.top/gtyhamstjt.html

Ruby: a.gcd(b)
来源：http://hz.sysykeji.top/gtcltxpuaa.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.yueranfly.top/gtaobaynbj.html

[N06] 判断回文字符串
来源：http://hz.chenjidiqi.icu/gtorxqdgpx.html

Py:   s == s[::-1]
来源：http://hz.guowangkeji.top/gtwaywrkef.html

PHP:  $s === strrev($s);
来源：http://hz.zhongyouzk.top/gtveycgobc.html

JS:   s === [...s].reverse().join("")
来源：http://hz.zhiwuduotai.top/gtylibzhzr.html

TS:   s === [...s].reverse().join("")
来源：http://hz.yuanzhike.top/gtnhejjosz.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.yuanzhike.top/gtutgxlvop.html

Go:   // 双指针从两端比较
来源：http://hz.smart0.xyz/gthbyywvhc.html

Ruby: s == s.reverse
来源：http://hz.zycfv.cn/gtrjxcwypk.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.ybcxt.top/gtjtestdkb.html

[N07] 两数之和（返回下标）
来源：http://hz.jqgfzy.top/gtivgpjrfn.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.xinyue.icu/gthhaqqngs.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.iojbl.cn/gtmylajtze.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.xylfe.cn/gtvwcyndbc.html

TS:   // 手写 Map<string, number>
来源：http://hz.quarkkingdee.top/gtfitrxmxo.html

Java: // 手写 HashMap
来源：http://hz.jinyuanbaomall.cn/gtqlpypiii.html

Go:   // 手写 map[int]int
来源：http://hz.mhx1999.top/gtzwvdgjwg.html

Ruby: // 手写 Hash
来源：http://hz.guannengcc.top/gtnacxtkil.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.smart0.xyz/gttbxotydg.html

[N08] 生成全排列
来源：http://hz.hysaishi.cn/gtjglrmbki.html

Py:   itertools.permutations(arr)
来源：http://hz.havefunace.top/gtotkghgik.html

PHP:  // 手写递归交换
来源：http://hz.jinghuilouyu.cn/gtnfbnvgkl.html

JS:   // 手写回溯递归
来源：http://hz.316326.xyz/gtkmhccvbx.html

TS:   // 手写回溯递归
来源：http://hz.tanke756.top/gtrjztwjkh.html

Java: // 手写回溯递归
来源：http://hz.vqdsnc.cn/gttzdbbvml.html

Go:   // 手写回溯递归
来源：http://hz.zhengqikj.top/gtaklnvcky.html

Ruby: arr.permutation.to_a
来源：http://hz.hnxiangtu.top/gtdpqalqrk.html

C#:   // 手写回溯递归
来源：http://hz.gzhubu.top/gtcuncucsd.html

[N09] 栈与队列
来源：http://hz.jinqigfzy.top/gtqpnzucjb.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.bjfxy.top/gthgduhxui.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.dianchejie.cn/gtevdorwvw.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.tian-w.cn/gtkoyhmtcd.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.hnqzz.top/gtrsxkdsre.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.sweek.top/gtpdrbyjfl.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.yangfankeji.com/gtoibbuwmp.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.jqgfzy.top/gttynhkohy.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.shzxlz.cn/gtcvntegdr.html

[N10] 链表节点定义
来源：http://hz.xuetiantiany.cn/gtxmffgqxg.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.9152youxi.cn/gtrlbbgqfk.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.zhixingplan.top/gtfapqchnq.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.guowangkeji.top/gtatrrjhhm.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.nanxuanxn.top/gtukmkdokf.html

Java: class Node { int v; Node next; }
来源：http://hz.gzhubu.top/gtsgqeneor.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.gzhubu.top/gtimgmkdtk.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.hfpthk.cn/gtpghynksm.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.ybcxt.top/gtclbhpxms.html

[N11] 二叉树中序遍历
来源：http://hz.316326.xyz/gtufvmdsyv.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.sufxvd.cn/gtuwmuqfvg.html

PHP:  // 手写递归函数
来源：http://hz.birdmap.top/gtiefualvs.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.ywan-chungtsiang.top/gtxlmomlro.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.vqdsnc.cn/gtodgtefig.html

Java: // 手写递归
来源：http://hz.aizwys.cn/gtagbnhsab.html

Go:   // 手写递归
来源：http://hz.jinqigufen.top/gtwshjdigu.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.xinyue.icu/gtvcnunnvw.html

C#:   // 手写递归
来源：http://hz.cucudq.cn/gtuqbekpij.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.wangdashe.top/gtsgzjwtrk.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.shangyingyoupin.top/gtmgaoicpx.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.hammf.cn/gtjtiuvysb.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.zhengqikj.top/gtllifqivi.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.zycfv.cn/gtxijtdemb.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.chenjidiqi.icu/gtlpssaioi.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.wangdashe.top/gtxnqhfkcq.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.shangyingyoupin.top/gtnkdcueyz.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.xylfe.cn/gtzslwsnou.html

================================================================================
来源：http://hz.andypj.xyz/gtslyzsset.html

O. 并发与异步
来源：http://hz.zhongyouzk.top/gtihfvlmqi.html

================================================================================
来源：http://hz.hongshengwenyu.top/gttogxyptz.html

[O01] 启动一个线程
来源：http://hz.sysykeji.top/gtrftcfrza.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.hywenlv.cn/gtvxmqhxjc.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.yvedp.cn/gtqhhtsizn.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.jinghuilouyu.cn/gtvwweacwh.html

TS:   // 同 JS
来源：http://hz.yuanzhike.top/gtnttaqaxr.html

Java: new Thread(() -> f()).start()
来源：http://hz.vqdsnc.cn/gtzadyemah.html

Go:   go f()
来源：http://hz.kuanghao11.cn/gtrtwnrvif.html

Ruby: Thread.new { f }
来源：http://hz.cucudq.cn/gtmlyvfkxy.html

C#:   Task.Run(() => F());
来源：http://hz.daria6918.cn/gtmgedoypn.html

[O02] 使用线程池
来源：http://hz.feifeiyinyue.top/gtjyttuqqa.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.zhixingplan.top/gtgthrlhrj.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.quarkkingdee.top/gthffatkrm.html

JS:   // worker_threads 线程池
来源：http://hz.xingfuxueyuan.xyz/gtnruoyyrq.html

TS:   // worker_threads 线程池
来源：http://hz.c1oappe.top/gtnrwkizlv.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.smart0.xyz/gtdgjskifr.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.fzhhl.top/gtglkbksiv.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.zhijiandao.cn/gtfxurebys.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.guowangkeji.top/gtdmyxyqto.html

[O03] 加锁保护共享数据
来源：http://hz.haohaochexian.top/gtlchxfpta.html

Py:   with lock: shared += 1
来源：http://hz.hnxiangtu.top/gttwnqfija.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.zhengqikj.top/gtqoeqpqra.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.gotoacloud.top/gtcvmxtweq.html

TS:   // 同 JS
来源：http://hz.guowangkeji.top/gtshsiavcf.html

Java: synchronized (this) { shared++; }
来源：http://hz.ehwqpu.com/gtoaxoeobh.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.gzhubu.top/gtzngvibhj.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.jinqigufen.top/gtxaxafrcm.html

C#:   lock (gate) { shared++; }
来源：http://hz.tanke756.top/gtomuvfrny.html

[O04] 定义异步函数并等待
来源：http://hz.hongshengwenyu.top/gtcbuwqnaw.html

Py:   async def f():⏎    await g()
来源：http://hz.shuidangran.top/gttkrrlpdi.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.xinyue.icu/gtxcoodeuo.html

JS:   async function f() { await g(); }
来源：http://hz.wangdashe.top/gtoiajvdmp.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.shanyushiyangtech.top/gtdldhhxov.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.havefunace.top/gtwzbzwfxk.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.52xcode.cn/gtxazsgdmv.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.shuidangran.top/gtpemgnkkw.html

C#:   async Task F() { await G(); }
来源：http://hz.jyoumei.cn/gtcvjzcqrz.html

[O05] 并发执行并等待全部完成
来源：http://hz.birdmap.top/gtxybbhwlf.html

Py:   asyncio.gather(*tasks)
来源：http://hz.chenlongwang.top/gthhetukay.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.9152youxi.cn/gtrhgulmir.html

JS:   await Promise.all(tasks)
来源：http://hz.haohaochexian.top/gtpnanrfew.html

TS:   await Promise.all(tasks)
来源：http://hz.xziqi.cn/gtyfmkldgr.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.havefunace.top/gtmetkvitu.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.shangyingyoupin.top/gtkoauhtfo.html

Ruby: threads.map(&:join)
来源：http://hz.hnxiangtu.top/gtleirxvyx.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.zdqjudy.top/gtpguwhdcs.html

[O06] 使用进程池
来源：http://hz.shzxlz.cn/gtvnhksglh.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.gzhubu.top/gtfvbwybjk.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.jinghuilouyu.cn/gtllytwfws.html

JS:   // child_process / cluster 模块
来源：http://hz.cucudq.cn/gtslklnhkw.html

TS:   // child_process / cluster 模块
来源：http://hz.shanyushiyangkeji.top/gtlrpwpkea.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.sweek.top/gtvuzcwklh.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.vqdsnc.cn/gtdeqmfwje.html

Ruby: // fork 块
来源：http://hz.fzhhl.top/gtnimtromk.html

C#:   Parallel.For
来源：http://hz.chenlongwang.top/gtgakpshoi.html

================================================================================
来源：http://hz.nwbrower.top/gtoiossssb.html

P. 常用工具函数
来源：http://hz.yueranfly.top/gtqwynuqis.html

================================================================================
来源：http://hz.hammf.cn/gteysejcgq.html

[P01] 生成 UUID
来源：http://hz.xuanzx.com/gtedlhhkwl.html

Py:   str(uuid.uuid4())
来源：http://hz.yongpay.top/gtvagraoxc.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.tian-w.cn/gtuknpvotk.html

JS:   crypto.randomUUID()
来源：http://hz.shuidangran.top/gtclmrumjh.html

TS:   crypto.randomUUID()
来源：http://hz.xingfuxueyuan.xyz/gtgbduoekp.html

Java: UUID.randomUUID().toString()
来源：http://hz.chenjidiqi.icu/gtolrwzxqb.html

Go:   // 用 github.com/google/uuid
来源：http://hz.0kj1m.cn/gtinwnnyau.html

Ruby: SecureRandom.uuid
来源：http://hz.haohaochexian.top/gtvcxcronx.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.fzhhl.top/gtrnkusaxs.html

[P02] MD5 / SHA256 摘要
来源：http://hz.meibo888.top/gtvweliaef.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.jiagoushi.top/gtjiguxgkc.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.xylfe.cn/gtdbwaiuvv.html


<!-- 参考信息 -->