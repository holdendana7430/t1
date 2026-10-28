代发 wailian999

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.jinqigfzy.top/gtiuzmqdrm.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.chenjidiqi.icu/gtrlxlsbht.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.aizwys.cn/gtjqbokktx.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.hnqzz.top/gthicvshdr.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.0kj1m.cn/gtnozjrgjc.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.jinqigufen.top/gtxmbobsvd.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.nanxinkj.top/gtvusrdhgg.html

[L06] 解析响应为 JSON
来源：http://hz.yuxming.cn/gthfqdslwu.html

Py:   resp.json()
来源：http://hz.dashuyun.cn/gtweuozser.html

PHP:  json_decode($body, true);
来源：http://hz.cucudq.cn/gtwyhfvflm.html

JS:   await resp.json()
来源：http://hz.zycfv.cn/gtvycvsqhg.html

TS:   await resp.json()
来源：http://hz.hnqzz.top/gtlilffnsm.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.gaohongyu789.top/gtfifunuds.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.yvedp.cn/gthdviccrt.html

Ruby: JSON.parse(resp.body)
来源：http://hz.zhaomingkeji.xyz/gtiqcjysoy.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.dianchejie.cn/gthsbrjrmu.html

[L07] 处理 HTTP 状态码
来源：http://hz.cashguo.top/gtboltucof.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.cashguo.top/gtimjnkedj.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.wangshuangyany.cn/gtemwbsduk.html

JS:   resp.ok;  resp.status
来源：http://hz.bjfxy.top/gtrpiudvmo.html

TS:   resp.ok;  resp.status
来源：http://hz.jqgfzy.top/gteyusyhpj.html

Java: resp.statusCode()
来源：http://hz.nwbrower.top/gtylvklwge.html

Go:   resp.StatusCode
来源：http://hz.zhaomingkeji.xyz/gtdpxwgjlq.html

Ruby: resp.code.to_i
来源：http://hz.redwolf501.top/gtqhihivdp.html

C#:   (int)resp.StatusCode
来源：http://hz.jlsjyb.cn/gtkjtjaraa.html

[L08] 并发请求多个地址
来源：http://hz.feifeiyinyue.top/gtpxnllunm.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.dashuyun.cn/gtolhbwlbt.html

PHP:  curl_multi_init() 系列
来源：http://hz.zycfv.cn/gtbbkshbys.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.sufxvd.cn/gtmcgstvsx.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.tianlin.xyz/gtgkqmglek.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.kuanghao11.cn/gtffouivbh.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.shzxlz.cn/gtadqzuhhf.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.gzhubu.top/gtjyxdwsci.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.hysaishi.cn/gtusbtwmrb.html

================================================================================
来源：http://hz.hysaishi.cn/gtivwtxeti.html

M. 命令行 / 进程 / 环境
来源：http://hz.iojbl.cn/gtrclvbxkx.html

================================================================================
来源：http://hz.xuanzx.com/gtblkiuetg.html

[M01] 读取命令行参数
来源：http://hz.316326.xyz/gtpyfomjpq.html

Py:   sys.argv[1:]
来源：http://hz.jinghuilouyu.cn/gtnntcmcjv.html

PHP:  $argv;  $argc;
来源：http://hz.bjfxy.top/gtvkwusxdh.html

JS:   process.argv.slice(2)
来源：http://hz.zhengqikj.top/gtpqsrhnsz.html

TS:   process.argv.slice(2)
来源：http://hz.shuidangran.top/gtuyfvstvp.html

Java: args 数组（main 方法参数）
来源：http://hz.nwbrower.top/gtudgtzqyf.html

Go:   os.Args[1:]
来源：http://hz.zhixingplan.top/gtbyxmaslw.html

Ruby: ARGV
来源：http://hz.jlsjyb.cn/gtrotsvjpa.html

C#:   args 数组（Main 方法参数）
来源：http://hz.zhiwuduotai.top/gtnxkhynjd.html

[M02] 读取环境变量
来源：http://hz.fzhhl.top/gtuukguoaq.html

Py:   os.environ.get("HOME")
来源：http://hz.xuanzx.com/gtdnrqzefp.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.hfpthk.cn/gtqcoibngr.html

JS:   process.env.HOME
来源：http://hz.yj20258888.top/gtrrfnecgl.html

TS:   process.env.HOME
来源：http://hz.shanyushiyangtech.top/gtfspwkjoj.html

Java: System.getenv("HOME")
来源：http://hz.sxryk.cn/gtlbikrwxs.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.xuetiantiany.cn/gtymooxvvd.html

Ruby: ENV["HOME"]
来源：http://hz.yonumen.top/gtbrazcfqx.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.jinyuanbaomall.cn/gtlwtchcxr.html

[M03] 执行外部命令
来源：http://hz.xingfuxueyuan.xyz/gterozpxlu.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.iojbl.cn/gtyuizkvli.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.yangfankeji.com/gtehyrqnkf.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.gotoacloud.top/gtotyboudn.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.jlsjyb.cn/gtghedsops.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.jqgfzy.top/gtwxibjxft.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.yuanzhike.top/gteigqwbpg.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.zhongyouzk.top/gtaaplswuo.html

C#:   Process.Start("ls", "-l");
来源：http://hz.xuanzx.com/gtlfxzqrbt.html

[M04] 获取当前工作目录
来源：http://hz.aizwys.cn/gttnsxzmnu.html

Py:   os.getcwd()
来源：http://hz.sufxvd.cn/gtajtprtkx.html

PHP:  getcwd();
来源：http://hz.jqgfzy.top/gtlopyqmsl.html

JS:   process.cwd()
来源：http://hz.jinqigufen.top/gtdfehsqih.html

TS:   process.cwd()
来源：http://hz.hywenlv.cn/gtgeuwatgm.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.9152youxi.cn/gtjgzfavlw.html

Go:   os.Getwd()
来源：http://hz.svipenyu.cn/gtqlxagfyi.html

Ruby: Dir.pwd
来源：http://hz.jiagoushi.top/gtbuimtbyx.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.zhiwuduotai.top/gtvefldgak.html

[M05] 设置退出码
来源：http://hz.birdmap.top/gtsfthztni.html

Py:   sys.exit(1)
来源：http://hz.hysaishi.cn/gtvjveeaey.html

PHP:  exit(1);
来源：http://hz.ydzc1.top/gtewrgvsbg.html

JS:   process.exit(1)
来源：http://hz.shzxlz.cn/gtsjuupaqr.html

TS:   process.exit(1)
来源：http://hz.shzxlz.cn/gtxmygiglm.html

Java: System.exit(1)
来源：http://hz.yj202588.top/gtkvodxvsg.html

Go:   os.Exit(1)
来源：http://hz.bjfxy.top/gtdtnszeuf.html

Ruby: exit 1
来源：http://hz.iojbl.cn/gttdntgjhs.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.sysykeji.top/gtesyuzxvh.html

[M06] 向标准错误输出
来源：http://hz.jianghu66.top/gtiegsxmeu.html

Py:   print("err", file=sys.stderr)
来源：http://hz.xingfuxueyuan.xyz/gtkwtdesih.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.kuanghao11.cn/gtynfqyoba.html

JS:   console.error("err")
来源：http://hz.haohaochexian.top/gtzihesbxt.html

TS:   console.error("err")
来源：http://hz.zhengqikj.top/gttjznkyxr.html

Java: System.err.println("err")
来源：http://hz.daxiang520.top/gteazytnyk.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.zhengqikj.top/gttfvrrzdr.html

Ruby: warn "err"
来源：http://hz.chenlongwang.top/gtmonoqjkz.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.ppjwa.cn/gtuubcjxaa.html

[M07] 判断是否为主入口
来源：http://hz.zhiwuduotai.top/gtqahnygal.html

Py:   if __name__ == "__main__":
来源：http://hz.nanxinkj.top/gtrhbugxux.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.sweek.top/gtrybgjewn.html

JS:   require.main === module
来源：http://hz.havefunace.top/gttyplswxg.html

TS:   require.main === module
来源：http://hz.smart0.xyz/gtmvvfgwsl.html

Java: public static void main(String[] args)
来源：http://hz.gaohongyu789.top/gtikzdtthj.html

Go:   func main()
来源：http://hz.wangshuangyany.cn/gtaivaldvp.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.snrcjt.cn/gtydjwemrw.html

C#:   static void Main(string[] args)
来源：http://hz.xuetiantiany.cn/gtesflhpbi.html

[M08] 获取系统与运行时信息
来源：http://hz.cashguo.top/gtqqcjyxym.html

Py:   platform.system();  platform.python_version()
来源：http://hz.meibo888.top/gteibunnxa.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.zhixingplan.top/gtwyzpdfui.html

JS:   process.platform;  process.version
来源：http://hz.jinqigufen.top/gtpbhcxybd.html

TS:   process.platform;  process.version
来源：http://hz.iojbl.cn/gtsrfqxjth.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.meibo888.top/gtutxkhlps.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.jinqigfzy.top/gthojnjhlw.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.zhixingplan.top/gtcjcxxqdr.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.shanyushiyangkeji.top/gtsfljvqsg.html

================================================================================
来源：http://hz.zhijiandao.cn/gthezfmeca.html

N. 数据结构与算法
来源：http://hz.havefunace.top/gtnyxbnmbj.html

================================================================================
来源：http://hz.fengsongda.top/gtbolsghqs.html

[N01] 二分查找（有序数组）
来源：http://hz.cqqwz.cn/gtwkqpknqk.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.hywenlv.cn/gtxddnsnio.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.ydzc1.top/gtzqfczxro.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yueranfly.top/gtooxegada.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.chenzaomai.com/gtyywlgkzo.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.guannengcc.top/gtyzngsstp.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.cheryme.top/gtadxbzxhp.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.zhengqikj.top/gtuepejnzr.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.52xcode.cn/gtkqkmrmeu.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.chenlongwang.top/gthagiczff.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.sysykeji.top/gtdftclsva.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.hammf.cn/gtgihwzuof.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.guannengcc.top/gttqtywmwp.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.hysaishi.cn/gtewihjowg.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.svipenyu.cn/gtlxbjaqlz.html

Go:   slices.Sort(arr)
来源：http://hz.zhongyouzk.top/gtozzrqmyv.html

Ruby: arr.sort
来源：http://hz.hammf.cn/gtvumeanmv.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.redwolf501.top/gtucycckya.html

[N03] 快速排序（分治示例）
来源：http://hz.hysaishi.cn/gtvposjquy.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.hammf.cn/gtbuxyujpu.html

PHP:  // 递归实现，或用 usort
来源：http://hz.tianlin.xyz/gtelnsarpd.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.sufxvd.cn/gtchgrbwrp.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.ehwqpu.com/gtxonbcbhw.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.yuxming.cn/gtenpwjrax.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.smart0.xyz/gtfuauixbw.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.yangfankeji.com/gthjoldqme.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.zhongyouzk.top/gtadxrmdwy.html

[N04] 斐波那契数列
来源：http://hz.yuanzhike.top/gtnagcxwlm.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.zycfv.cn/gtkjxdaifz.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.vqdsnc.cn/gtzbktzjuw.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.haohaochexian.top/gtcciukwbf.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.hfpthk.cn/gtybbxikga.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.tianlin.xyz/gtjlgcaqvr.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.wangshuangyany.cn/gtmsbtcdyn.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.zhaomingkeji.xyz/gtziddvxml.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.gogol.net.cn/gtmksdufaq.html

[N05] 最大公约数
来源：http://hz.andypj.xyz/gtbuxoroxz.html

Py:   math.gcd(a, b)
来源：http://hz.jinqigfzy.top/gtolhrnysf.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.daria6918.cn/gtqowlngjb.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.zhiwuduotai.top/gtzeofbtbd.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.hammf.cn/gtyrqjrqpo.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.jqgfzy.top/gtwsfjykzj.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.hywenlv.cn/gtgchkakby.html

Ruby: a.gcd(b)
来源：http://hz.jianghu66.top/gtyntttjjz.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.yongpay.top/gttmuxpqjq.html

[N06] 判断回文字符串
来源：http://hz.fzhhl.top/gtwxemlgnd.html

Py:   s == s[::-1]
来源：http://hz.tianlin.xyz/gtimejekub.html

PHP:  $s === strrev($s);
来源：http://hz.zhengqikj.top/gtrbkrkioq.html

JS:   s === [...s].reverse().join("")
来源：http://hz.jqgfzy.top/gtrdlqlvtj.html

TS:   s === [...s].reverse().join("")
来源：http://hz.andypj.xyz/gtaffrclvk.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.yuanzhike.top/gtfzomamzp.html

Go:   // 双指针从两端比较
来源：http://hz.yj20258888.top/gthmubrcyu.html

Ruby: s == s.reverse
来源：http://hz.tian-w.cn/gtwjrceszh.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.shangyingyoupin.top/gtsdwwnfbe.html

[N07] 两数之和（返回下标）
来源：http://hz.andypj.xyz/gtdtikheic.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.hysaishi.cn/gtbhnyfdqi.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.xuetiantiany.cn/gtoxckpzwi.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.c1oappe.top/gtzpsyyrjv.html

TS:   // 手写 Map<string, number>
来源：http://hz.andypj.xyz/gtdflxugys.html

Java: // 手写 HashMap
来源：http://hz.yvedp.cn/gtooxodkjk.html

Go:   // 手写 map[int]int
来源：http://hz.zycfv.cn/gtiaaeatbk.html

Ruby: // 手写 Hash
来源：http://hz.andypj.xyz/gtgtzxhzce.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.xinyue.icu/gtakbteqmm.html

[N08] 生成全排列
来源：http://hz.ydjk.org.cn/gthmbqadqj.html

Py:   itertools.permutations(arr)
来源：http://hz.jlsjyb.cn/gtynicfzok.html

PHP:  // 手写递归交换
来源：http://hz.haohaochexian.top/gtjacrvoyo.html

JS:   // 手写回溯递归
来源：http://hz.birdmap.top/gtwcuupzys.html

TS:   // 手写回溯递归
来源：http://hz.gaohongyu789.top/gttkclorvp.html

Java: // 手写回溯递归
来源：http://hz.yangfankeji.com/gtcgizfcdj.html

Go:   // 手写回溯递归
来源：http://hz.aizwys.cn/gtjfegnwke.html

Ruby: arr.permutation.to_a
来源：http://hz.yueranfly.top/gtfuvtaltx.html

C#:   // 手写回溯递归
来源：http://hz.gaohongyu789.top/gtvrhunzrn.html

[N09] 栈与队列
来源：http://hz.yj20258.top/gtnmcderbv.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.sxryk.cn/gtoibfilta.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.hywenlv.cn/gtfnukvceq.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.hammf.cn/gtrzsycjqj.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.cashguo.top/gtrvbjvwks.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.zhijiandao.cn/gtddmcwtda.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.nwbrower.top/gtwvlvxkpo.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.fengsongda.top/gtmmegaael.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.xuanzx.com/gtgrmbwsmd.html

[N10] 链表节点定义
来源：http://hz.shanyushiyangkeji.top/gtzqorluto.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.meibo888.top/gtumebnesi.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.chenjidiqi.icu/gtcjlvedzn.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.daxiang520.top/gtfcrhkbrb.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.xinyue.icu/gtgkrmwjen.html

Java: class Node { int v; Node next; }
来源：http://hz.wangshuangyany.cn/gtstonlrtv.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.jiagoushi.top/gtyfozzfgd.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.xylfe.cn/gtuvktxugf.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.dianchejie.cn/gtimdtfsox.html

[N11] 二叉树中序遍历
来源：http://hz.jqgufenzy.top/gtlcaqjclu.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.jiagoushi.top/gtodmftlij.html

PHP:  // 手写递归函数
来源：http://hz.jianghu66.top/gtqyuvwjkr.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.redwolf501.top/gtzzbgbcks.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.tian-w.cn/gtonncbwgk.html

Java: // 手写递归
来源：http://hz.jlsjyb.cn/gtmqwshsbz.html

Go:   // 手写递归
来源：http://hz.xingfuxueyuan.xyz/gtfurkzttt.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.zhixingplan.top/gtabbepnpz.html

C#:   // 手写递归
来源：http://hz.xziqi.cn/gtilifcrym.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.gogol.net.cn/gtfkaurbbp.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.ehwqpu.com/gtuptmdfjt.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.ydzc1.top/gtnmzujjms.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.kuanghao11.cn/gtoazgumem.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yanxiufei.cn/gtsguwvtqe.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yonumen.top/gtyjdhglvg.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.zhijiandao.cn/gtksqcedmu.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.zhoulong.xyz/gtbkgrnspn.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.cucudq.cn/gtpofvaxwk.html

================================================================================
来源：http://hz.jqgufenzy.top/gtgfirkiwk.html

O. 并发与异步
来源：http://hz.aibaodan.cn/gtgoneflca.html

================================================================================
来源：http://hz.zhongyouzk.top/gtprsfmheg.html

[O01] 启动一个线程
来源：http://hz.guowangkeji.top/gtonneewlw.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.meibo888.top/gtcjfmwmpz.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.gotoacloud.top/gthopjmopq.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.zycfv.cn/gtawpalyps.html

TS:   // 同 JS
来源：http://hz.cashguo.top/gtdvtacyat.html

Java: new Thread(() -> f()).start()
来源：http://hz.c1oappe.top/gtfdqeejcb.html

Go:   go f()
来源：http://hz.aibaodan.cn/gtnkfduhcj.html

Ruby: Thread.new { f }
来源：http://hz.birdmap.top/gtftaowtsm.html

C#:   Task.Run(() => F());
来源：http://hz.daxiang520.top/gtuxqdrwuh.html

[O02] 使用线程池
来源：http://hz.sxryk.cn/gtctgkyhlr.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.hnxiangtu.top/gtinoynuvq.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.ydjk.org.cn/gtwdkafxfk.html

JS:   // worker_threads 线程池
来源：http://hz.ybcxt.top/gtomtxdckx.html

TS:   // worker_threads 线程池
来源：http://hz.shanyushiyangtech.top/gtzqhyxvea.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.ivvv.top/gtehdjmipp.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.chenjidiqi.icu/gthavcoavq.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.xylfe.cn/gtwoowhbhi.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.yj20258.top/gtfhifkhxa.html

[O03] 加锁保护共享数据
来源：http://hz.sxryk.cn/gtereojadn.html

Py:   with lock: shared += 1
来源：http://hz.gzhubu.top/gtuogbgxoe.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.jyoumei.cn/gtglowjihj.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.daxiang520.top/gtkfwxmpsp.html

TS:   // 同 JS
来源：http://hz.nanxuanxn.top/gtfvegbeoe.html

Java: synchronized (this) { shared++; }
来源：http://hz.shuidangran.top/gtlwhvczib.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.kuanghao11.cn/gtjwuzqpxt.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.yj202588.top/gtqdbungwh.html

C#:   lock (gate) { shared++; }
来源：http://hz.kuanghao11.cn/gtjmbcucxx.html

[O04] 定义异步函数并等待
来源：http://hz.shanyushiyangkeji.top/gtkbeoobvm.html

Py:   async def f():⏎    await g()
来源：http://hz.dianchejie.cn/gtihchcnoc.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.cashguo.top/gthmeoaobc.html

JS:   async function f() { await g(); }
来源：http://hz.sweek.top/gtuvmntuaq.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.yj20258.top/gtlttdedzs.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.tian-w.cn/gtlimrfzgc.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.fzhhl.top/gtbmhbhatl.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.yueranfly.top/gtoxkgmpef.html

C#:   async Task F() { await G(); }
来源：http://hz.shzxlz.cn/gtodcbhfma.html

[O05] 并发执行并等待全部完成
来源：http://hz.feifeiyinyue.top/gtrpjjrzxf.html

Py:   asyncio.gather(*tasks)
来源：http://hz.ydzc1.top/gtolpxpwts.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.aizwys.cn/gtydxftdhe.html

JS:   await Promise.all(tasks)
来源：http://hz.kuanghao11.cn/gtynwtiyjv.html

TS:   await Promise.all(tasks)
来源：http://hz.shuidangran.top/gtoxmwwagi.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.snrcjt.cn/gtjfrvfvsz.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.jianghu66.top/gtzsjmdoun.html

Ruby: threads.map(&:join)
来源：http://hz.meibo888.top/gtjujrfeun.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.shzxlz.cn/gtogrbgufa.html

[O06] 使用进程池
来源：http://hz.shuidangran.top/gtoxgasctf.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.nwbrower.top/gtxnhpiduw.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.zhaomingkeji.xyz/gtfwuzithy.html

JS:   // child_process / cluster 模块
来源：http://hz.fengsongda.top/gtrtpwxatt.html

TS:   // child_process / cluster 模块
来源：http://hz.hnqzz.top/gtcaheslex.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.shangyingyoupin.top/gtvkclsicz.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.yj202588.top/gtueofvdvi.html

Ruby: // fork 块
来源：http://hz.sweek.top/gtudxgmjgy.html

C#:   Parallel.For
来源：http://hz.9152youxi.cn/gtbyzlpvws.html

================================================================================
来源：http://hz.smart0.xyz/gtpaginnkp.html

P. 常用工具函数
来源：http://hz.havefunace.top/gtjgaxuonj.html

================================================================================
来源：http://hz.316326.xyz/gtjfxutuyv.html

[P01] 生成 UUID
来源：http://hz.aibaodan.cn/gtsemyaosr.html

Py:   str(uuid.uuid4())
来源：http://hz.zhixingplan.top/gtrfuhbuox.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.zhoulong.xyz/gtuqshkznl.html

JS:   crypto.randomUUID()
来源：http://hz.kuanghao11.cn/gtrpyckuhc.html

TS:   crypto.randomUUID()
来源：http://hz.ydjk.org.cn/gtudrvjxmg.html

Java: UUID.randomUUID().toString()
来源：http://hz.havefunace.top/gtofqilsjl.html

Go:   // 用 github.com/google/uuid
来源：http://hz.ydjk.org.cn/gtggozrwbt.html

Ruby: SecureRandom.uuid
来源：http://hz.jqgufenzy.top/gtveglsvqg.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.jiagoushi.top/gtytyzbxsx.html

[P02] MD5 / SHA256 摘要
来源：http://hz.ywan-chungtsiang.top/gtrzmsfimf.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.chenlongwang.top/gtkjzmznck.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.jyoumei.cn/gterdrwgjn.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.ehwqpu.com/gttcvcjruy.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.tian-w.cn/gtztjidbxt.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.zhoulong.xyz/gtcfddmjmq.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.mhx1999.top/gtomxfczjm.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.chenjidiqi.icu/gtgitehjaz.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.cdnleiting.top/gtntspxjau.html

[P03] 生成短随机字符串
来源：http://hz.xingfuxueyuan.xyz/gtisxhrwpk.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.jyoumei.cn/gtgkxzmpmg.html


<!-- 参考信息 -->