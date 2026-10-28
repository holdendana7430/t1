代发 wailian999

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.yueranfly.top/gtmmumlxbm.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.meibo888.top/gtpkewkhvv.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.yj20258.top/gtnnkrliok.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.snrcjt.cn/gtnkbqugdi.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.jianghu66.top/gtinzyrtfr.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.sweek.top/gtifrnjhay.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.feifeiyinyue.top/gtuvxwildu.html

[L06] 解析响应为 JSON
来源：http://hz.sysykeji.top/gtwztmbpvj.html

Py:   resp.json()
来源：http://hz.jlsjyb.cn/gtqmgeycpo.html

PHP:  json_decode($body, true);
来源：http://hz.iojbl.cn/gtqvpflfth.html

JS:   await resp.json()
来源：http://hz.jianghu66.top/gtwvphuljg.html

TS:   await resp.json()
来源：http://hz.ydjk.org.cn/gtzbxidfeb.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.jinqigfzy.top/gtnzhpeejd.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.zhijiandao.cn/gtofmemfdm.html

Ruby: JSON.parse(resp.body)
来源：http://hz.zhiwuduotai.top/gtttunqlxt.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.shangyingyoupin.top/gttplpfitq.html

[L07] 处理 HTTP 状态码
来源：http://hz.zhoulong.xyz/gtlotnykmk.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.chenlongwang.top/gtqljqmudv.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.zhixingplan.top/gtdhlhqveb.html

JS:   resp.ok;  resp.status
来源：http://hz.zycfv.cn/gtlqkfadpm.html

TS:   resp.ok;  resp.status
来源：http://hz.hysaishi.cn/gtifagljex.html

Java: resp.statusCode()
来源：http://hz.yongpay.top/gtfsvokvpr.html

Go:   resp.StatusCode
来源：http://hz.nanxuanxn.top/gtrywuspdg.html

Ruby: resp.code.to_i
来源：http://hz.shzxlz.cn/gtqxahoowq.html

C#:   (int)resp.StatusCode
来源：http://hz.zhoulong.xyz/gteecxepwq.html

[L08] 并发请求多个地址
来源：http://hz.xuetiantiany.cn/gtrnkqqmln.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.tian-w.cn/gteqehxpmc.html

PHP:  curl_multi_init() 系列
来源：http://hz.kuanghao11.cn/gtrptehaay.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.fzhhl.top/gttfjdtzvi.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yueranfly.top/gtehzdsjzc.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.c1oappe.top/gtwdftfaex.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.pycfn.com/gtdutafkqa.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.jyoumei.cn/gtowhwfwlh.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.gzhubu.top/gtldcrtkba.html

================================================================================
来源：http://hz.9152youxi.cn/gtkuwqywgo.html

M. 命令行 / 进程 / 环境
来源：http://hz.zhijiandao.cn/gtiunmyhhk.html

================================================================================
来源：http://hz.yangfankeji.com/gtpczrxmqc.html

[M01] 读取命令行参数
来源：http://hz.shuidangran.top/gtwmiwzegh.html

Py:   sys.argv[1:]
来源：http://hz.ydjk.org.cn/gtxkgiboxt.html

PHP:  $argv;  $argc;
来源：http://hz.sxryk.cn/gtgqluxlou.html

JS:   process.argv.slice(2)
来源：http://hz.shzxlz.cn/gtszmpczlt.html

TS:   process.argv.slice(2)
来源：http://hz.ydzc1.top/gtynfzxlkd.html

Java: args 数组（main 方法参数）
来源：http://hz.shuidangran.top/gthxrmcang.html

Go:   os.Args[1:]
来源：http://hz.fzhhl.top/gtwldxhqja.html

Ruby: ARGV
来源：http://hz.birdmap.top/gtbhndrpnl.html

C#:   args 数组（Main 方法参数）
来源：http://hz.shangyingyoupin.top/gtvvaammvg.html

[M02] 读取环境变量
来源：http://hz.cashguo.top/gtnrdxnovt.html

Py:   os.environ.get("HOME")
来源：http://hz.hfpthk.cn/gtwzxgvvzx.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.fzhhl.top/gtqahvcmmv.html

JS:   process.env.HOME
来源：http://hz.aizwys.cn/gtgwtilcli.html

TS:   process.env.HOME
来源：http://hz.jianghu66.top/gtwcbkvjwa.html

Java: System.getenv("HOME")
来源：http://hz.daria6918.cn/gtzxciamgl.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.zhiwuduotai.top/gtfykhriwu.html

Ruby: ENV["HOME"]
来源：http://hz.hfpthk.cn/gtfgwytmvi.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.jinqigfzy.top/gtkruqvczw.html

[M03] 执行外部命令
来源：http://hz.yj20258888.top/gtlmhpkonb.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.sysykeji.top/gttfrsgwka.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.guowangkeji.top/gtwcfucanc.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.svipenyu.cn/gtcfcdrmed.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.zhoulong.xyz/gtjefsybvi.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.daxiang520.top/gtrziduzxh.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.jianghu66.top/gtatcjluos.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.snrcjt.cn/gthqkwbift.html

C#:   Process.Start("ls", "-l");
来源：http://hz.bjfxy.top/gtfzceoscf.html

[M04] 获取当前工作目录
来源：http://hz.zhijiandao.cn/gtxxjasesy.html

Py:   os.getcwd()
来源：http://hz.fengsongda.top/gtbqvlejry.html

PHP:  getcwd();
来源：http://hz.cqqwz.cn/gtpkcgjbfk.html

JS:   process.cwd()
来源：http://hz.xuanzx.com/gtbadzazak.html

TS:   process.cwd()
来源：http://hz.hnxiangtu.top/gtmszdsdhf.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.52xcode.cn/gtvqzyjbnz.html

Go:   os.Getwd()
来源：http://hz.cucudq.cn/gtyfknmfrn.html

Ruby: Dir.pwd
来源：http://hz.yongpay.top/gtlpbjmslh.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.316326.xyz/gtxgipuhml.html

[M05] 设置退出码
来源：http://hz.zhiwuduotai.top/gtimnnldmi.html

Py:   sys.exit(1)
来源：http://hz.yj202588.top/gtwdkqkxkc.html

PHP:  exit(1);
来源：http://hz.haohaochexian.top/gtlmtircth.html

JS:   process.exit(1)
来源：http://hz.zhixingplan.top/gtaliqjase.html

TS:   process.exit(1)
来源：http://hz.nwbrower.top/gtpvotervb.html

Java: System.exit(1)
来源：http://hz.yangfankeji.com/gtztkoexos.html

Go:   os.Exit(1)
来源：http://hz.xinyue.icu/gtfmyrkgyn.html

Ruby: exit 1
来源：http://hz.zhongyouzk.top/gtpbzdbucm.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.sweek.top/gttlunqoei.html

[M06] 向标准错误输出
来源：http://hz.kuanghao11.cn/gtzaouaptq.html

Py:   print("err", file=sys.stderr)
来源：http://hz.xingfuxueyuan.xyz/gtkpcoerak.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.aibaodan.cn/gtkjiqdkli.html

JS:   console.error("err")
来源：http://hz.zdqjudy.top/gtndnrffkz.html

TS:   console.error("err")
来源：http://hz.tanke756.top/gtzjwtohcb.html

Java: System.err.println("err")
来源：http://hz.smart0.xyz/gtrlmtaomy.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.zhengqikj.top/gtsxiqmxzw.html

Ruby: warn "err"
来源：http://hz.aizwys.cn/gtklxdzaim.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.zhiwuduotai.top/gtekawvpxi.html

[M07] 判断是否为主入口
来源：http://hz.zhixingplan.top/gtsolpjzli.html

Py:   if __name__ == "__main__":
来源：http://hz.c1oappe.top/gtnmdxijfi.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.shuidangran.top/gtvggbydtd.html

JS:   require.main === module
来源：http://hz.gzhubu.top/gtzfmcpsbp.html

TS:   require.main === module
来源：http://hz.tanke756.top/gtvkcvubig.html

Java: public static void main(String[] args)
来源：http://hz.dashuyun.cn/gtqcaacsvd.html

Go:   func main()
来源：http://hz.yanxiufei.cn/gtcaszhdii.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.cucudq.cn/gtnmgsxuce.html

C#:   static void Main(string[] args)
来源：http://hz.nwbrower.top/gtuikdzosk.html

[M08] 获取系统与运行时信息
来源：http://hz.redwolf501.top/gtltjlrqkp.html

Py:   platform.system();  platform.python_version()
来源：http://hz.xuetiantiany.cn/gtnjakxmxt.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.svipenyu.cn/gtbhpbnoxk.html

JS:   process.platform;  process.version
来源：http://hz.shzxlz.cn/gtooesjqsi.html

TS:   process.platform;  process.version
来源：http://hz.nwbrower.top/gtkgnqijnr.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.ppjwa.cn/gtkejcvfna.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.nanxinkj.top/gtaytouscw.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.yj202588.top/gtqyrafoxr.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.yj202588.top/gtmwmaiwvp.html

================================================================================
来源：http://hz.jinqigufen.top/gtszkgsksa.html

N. 数据结构与算法
来源：http://hz.zdqjudy.top/gtihkjxmtr.html

================================================================================
来源：http://hz.ybcxt.top/gtesypdqvc.html

[N01] 二分查找（有序数组）
来源：http://hz.shzxlz.cn/gtchtyqgic.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.xuetiantiany.cn/gtoziegeds.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.tian-w.cn/gttkixjcly.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.cheryme.top/gtpivokzyj.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.fzhhl.top/gtymbuqpmn.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.xingfuxueyuan.xyz/gtrhrlbehp.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.zdqjudy.top/gtsoyczzdh.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.yuxming.cn/gteeujqbnd.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.shuidangran.top/gtpukfuagg.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.chenzaomai.com/gttvhuieib.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.dashuyun.cn/gtqdbrnald.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.svipenyu.cn/gtwwpnbyri.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.c1oappe.top/gtrayziewv.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.tianlin.xyz/gtvhkrzmzg.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.pengpengdd.cyou/gttehabrxb.html

Go:   slices.Sort(arr)
来源：http://hz.sufxvd.cn/gtovcolfll.html

Ruby: arr.sort
来源：http://hz.aizwys.cn/gtkmocwitr.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.zhixingplan.top/gtkpvolcjl.html

[N03] 快速排序（分治示例）
来源：http://hz.daria6918.cn/gtjgusymzh.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.yj20258888.top/gtabvugivl.html

PHP:  // 递归实现，或用 usort
来源：http://hz.hfpthk.cn/gtbafkbpfo.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.0kj1m.cn/gtkbxnmkmq.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.sxryk.cn/gtugfqvojx.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.mhx1999.top/gtrdpwagxn.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.haohaochexian.top/gtojrkrkwl.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.hywenlv.cn/gtvxpyiscr.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.52xcode.cn/gtrvspwjvb.html

[N04] 斐波那契数列
来源：http://hz.mhx1999.top/gtglfqtake.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.shuidangran.top/gtzeyypnev.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.snrcjt.cn/gtzlazmgtj.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.daxiang520.top/gtjbrlqmaq.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.birdmap.top/gttaasvkql.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.52xcode.cn/gtpdpcevgo.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.chenjidiqi.icu/gtgcnmzgdq.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.cucudq.cn/gtcxawodzm.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.ppjwa.cn/gtejmvqypk.html

[N05] 最大公约数
来源：http://hz.cqqwz.cn/gtooxwwxkl.html

Py:   math.gcd(a, b)
来源：http://hz.tanke756.top/gtvcqpaent.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.ppjwa.cn/gttpjsxrcv.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jinghuilouyu.cn/gtkucfxvef.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yuxming.cn/gtkqymrnsl.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.zhongyouzk.top/gtkktzwnbj.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.jinqigfzy.top/gtsvryocct.html

Ruby: a.gcd(b)
来源：http://hz.andypj.xyz/gtqtaizcss.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.jiagoushi.top/gtijlthcws.html

[N06] 判断回文字符串
来源：http://hz.nanxinkj.top/gtxzeatqes.html

Py:   s == s[::-1]
来源：http://hz.chenlongwang.top/gttpgypeyv.html

PHP:  $s === strrev($s);
来源：http://hz.316326.xyz/gtldwzsevq.html

JS:   s === [...s].reverse().join("")
来源：http://hz.yuanzhike.top/gtepsgkbkz.html

TS:   s === [...s].reverse().join("")
来源：http://hz.xinyue.icu/gttlifnzqw.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.zhoulong.xyz/gtjskihnjw.html

Go:   // 双指针从两端比较
来源：http://hz.gaohongyu789.top/gtgphqqckk.html

Ruby: s == s.reverse
来源：http://hz.bjfxy.top/gtzydmrito.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.redwolf501.top/gtrpaqcbgp.html

[N07] 两数之和（返回下标）
来源：http://hz.zhaomingkeji.xyz/gtdyovdcwl.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.hammf.cn/gtvpngdahg.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.nanxinkj.top/gtzxmazwrf.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.zycfv.cn/gtzubhxogu.html

TS:   // 手写 Map<string, number>
来源：http://hz.cucudq.cn/gtzovgknpe.html

Java: // 手写 HashMap
来源：http://hz.tianlin.xyz/gtmwmyulex.html

Go:   // 手写 map[int]int
来源：http://hz.chenzaomai.com/gtbpfzzona.html

Ruby: // 手写 Hash
来源：http://hz.yongpay.top/gtjqvdscnk.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.316326.xyz/gtuosszmxs.html

[N08] 生成全排列
来源：http://hz.yonumen.top/gtehoiagxa.html

Py:   itertools.permutations(arr)
来源：http://hz.wangshuangyany.cn/gtolcrdgfy.html

PHP:  // 手写递归交换
来源：http://hz.yj202588.top/gtjdanjges.html

JS:   // 手写回溯递归
来源：http://hz.feifeiyinyue.top/gtdcvmuclw.html

TS:   // 手写回溯递归
来源：http://hz.daxiang520.top/gtpwtdalbz.html

Java: // 手写回溯递归
来源：http://hz.c1oappe.top/gtxpgovmxf.html

Go:   // 手写回溯递归
来源：http://hz.cashguo.top/gtzgmjzjwb.html

Ruby: arr.permutation.to_a
来源：http://hz.daxiang520.top/gtjuvjrart.html

C#:   // 手写回溯递归
来源：http://hz.feifeiyinyue.top/gthnzzrene.html

[N09] 栈与队列
来源：http://hz.ydjk.org.cn/gtncjpctqp.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.ydzc1.top/gtwabohsjv.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.chenlongwang.top/gtqrfmuwhn.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.yuanzhike.top/gthayyatcf.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.gaohongyu789.top/gtpunqcvyi.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.haohaochexian.top/gttnailyqe.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.chenzaomai.com/gtobfwdfvj.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.pengpengdd.cyou/gtcgsdrltg.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.cheryme.top/gtnxutapma.html

[N10] 链表节点定义
来源：http://hz.hongshengwenyu.top/gtpsbyfftu.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.zhaomingkeji.xyz/gtcvelnzhj.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.aizwys.cn/gtpwozokes.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.feifeiyinyue.top/gtczbldpmg.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.yongpay.top/gtxyoudxli.html

Java: class Node { int v; Node next; }
来源：http://hz.ybcxt.top/gtkwkmqrmd.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.pycfn.com/gtkcljzumq.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.shanyushiyangkeji.top/gtxnmysqsy.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.ydzc1.top/gtsunlnjlw.html

[N11] 二叉树中序遍历
来源：http://hz.zhoulong.xyz/gtopnqwtqg.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.yangfankeji.com/gtscaapheh.html

PHP:  // 手写递归函数
来源：http://hz.gogol.net.cn/gtmgdyajwu.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.haohaochexian.top/gtcmlorotr.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jqgfzy.top/gttsteendg.html

Java: // 手写递归
来源：http://hz.cdnleiting.top/gtrevzvcoe.html

Go:   // 手写递归
来源：http://hz.cucudq.cn/gtrzupgybo.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.ydzc1.top/gtfobpyqdr.html

C#:   // 手写递归
来源：http://hz.ydjk.org.cn/gtcbjcawlv.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.9152youxi.cn/gtwsgxgzni.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.gotoacloud.top/gtrzcdnrjf.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.cucudq.cn/gtfzwtkdwh.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.guannengcc.top/gtwrjcswfx.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.dianchejie.cn/gtwwnjdlet.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.jinyuanbaomall.cn/gtjwnkqkwh.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.52xcode.cn/gthweozciy.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.sufxvd.cn/gtydubvkxo.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.zhaomingkeji.xyz/gtureyfibf.html

================================================================================
来源：http://hz.yvedp.cn/gtjklmwypb.html

O. 并发与异步
来源：http://hz.shuidangran.top/gtqwirseaf.html

================================================================================
来源：http://hz.chenzaomai.com/gtcmskexvt.html

[O01] 启动一个线程
来源：http://hz.shzxlz.cn/gtrfvixant.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.snrcjt.cn/gtuxfayqwj.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.pengpengdd.cyou/gtmwntxkgc.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.yvedp.cn/gtvcmtmnhi.html

TS:   // 同 JS
来源：http://hz.ydzc1.top/gtynqlncpi.html

Java: new Thread(() -> f()).start()
来源：http://hz.nanxuanxn.top/gtptxtqtac.html

Go:   go f()
来源：http://hz.wangshuangyany.cn/gtvfbldrsq.html

Ruby: Thread.new { f }
来源：http://hz.cheryme.top/gtetzwnczk.html

C#:   Task.Run(() => F());
来源：http://hz.quarkkingdee.top/gtwdhrjkhy.html

[O02] 使用线程池
来源：http://hz.wangdashe.top/gtuwnwvgoo.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.yanxiufei.cn/gtlycjjuub.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.yueranfly.top/gtehkbtbzj.html

JS:   // worker_threads 线程池
来源：http://hz.0kj1m.cn/gtntzhsefz.html

TS:   // worker_threads 线程池
来源：http://hz.haohaochexian.top/gtnkhontuj.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.cheryme.top/gtnbzghkah.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.hnqzz.top/gtwdoercai.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.fengsongda.top/gttnqtxsjh.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.guowangkeji.top/gtntmuqrik.html

[O03] 加锁保护共享数据
来源：http://hz.hywenlv.cn/gteodgpszv.html

Py:   with lock: shared += 1
来源：http://hz.jqgufenzy.top/gtnyxsowvl.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.fengsongda.top/gtjqmbdxjt.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.daxiang520.top/gtcbslgtoq.html

TS:   // 同 JS
来源：http://hz.chenjidiqi.icu/gtzwyiihbw.html

Java: synchronized (this) { shared++; }
来源：http://hz.yuanzhike.top/gtdlcxzqma.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.zhoulong.xyz/gtoabxnjnz.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.hysaishi.cn/gtgiilfwxb.html

C#:   lock (gate) { shared++; }
来源：http://hz.jinghuilouyu.cn/gtbloobxnl.html

[O04] 定义异步函数并等待
来源：http://hz.ybcxt.top/gtvidhgavv.html

Py:   async def f():⏎    await g()
来源：http://hz.zhiwuduotai.top/gtwzjltzbb.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.sysykeji.top/gtyxzwsuzq.html

JS:   async function f() { await g(); }
来源：http://hz.0kj1m.cn/gtbgrpmlzh.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.jyoumei.cn/gtdvkzeqso.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.ehwqpu.com/gtzagpiftg.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.cucudq.cn/gtcirjeryd.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.quarkkingdee.top/gtzxocqczt.html

C#:   async Task F() { await G(); }
来源：http://hz.gaohongyu789.top/gtvsqduzrk.html

[O05] 并发执行并等待全部完成
来源：http://hz.jinqigufen.top/gtmvemjbkl.html

Py:   asyncio.gather(*tasks)
来源：http://hz.chenlongwang.top/gtgiudxhag.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.xylfe.cn/gtqquplkgi.html

JS:   await Promise.all(tasks)
来源：http://hz.wangdashe.top/gtpjddwgcy.html

TS:   await Promise.all(tasks)
来源：http://hz.yanxiufei.cn/gtobosqjow.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.shanyushiyangtech.top/gtdtiemlan.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.tianlin.xyz/gtrwimtytj.html

Ruby: threads.map(&:join)
来源：http://hz.shanyushiyangkeji.top/gtnnmmyamm.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.yj202588.top/gtsgtbjjbb.html

[O06] 使用进程池
来源：http://hz.xylfe.cn/gtynlnjmpt.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.sufxvd.cn/gtfxrthryi.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.wangshuangyany.cn/gtgmuujpty.html

JS:   // child_process / cluster 模块
来源：http://hz.yangfankeji.com/gtmsitawrf.html

TS:   // child_process / cluster 模块
来源：http://hz.gogol.net.cn/gtolbsnhkf.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.bjfxy.top/gtiorgwltp.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.cheryme.top/gtqttbbxze.html

Ruby: // fork 块
来源：http://hz.nanxinkj.top/gtgsmocwgw.html

C#:   Parallel.For
来源：http://hz.yj20258888.top/gtfjlxcgdl.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtwwanvgom.html

P. 常用工具函数
来源：http://hz.shanyushiyangkeji.top/gtgremmjqx.html

================================================================================
来源：http://hz.nanxuanxn.top/gtdsbngxba.html

[P01] 生成 UUID
来源：http://hz.jinqigufen.top/gtokasbafo.html

Py:   str(uuid.uuid4())
来源：http://hz.tanke756.top/gtpafnxckn.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.ivvv.top/gtsjtylsdo.html

JS:   crypto.randomUUID()
来源：http://hz.xuanzx.com/gtyslgjxxe.html

TS:   crypto.randomUUID()
来源：http://hz.shzxlz.cn/gtriehltsg.html

Java: UUID.randomUUID().toString()
来源：http://hz.nanxuanxn.top/gtbgvkcrff.html

Go:   // 用 github.com/google/uuid
来源：http://hz.yj20258.top/gtjnzkeaaj.html

Ruby: SecureRandom.uuid
来源：http://hz.smart0.xyz/gtbshwgujk.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.xuanzx.com/gtvlentxxn.html

[P02] MD5 / SHA256 摘要
来源：http://hz.jiagoushi.top/gtehfexuso.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.c1oappe.top/gthoqnxxyc.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.jinqigufen.top/gtfysmcgww.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.andypj.xyz/gtotqspjkc.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.yongpay.top/gtojkthylv.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.hnqzz.top/gtedeajtrs.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.hammf.cn/gtfsqwxzkn.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.jinyuanbaomall.cn/gtmxlzhpko.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.zhixingplan.top/gtggfagsax.html

[P03] 生成短随机字符串
来源：http://hz.yj20258888.top/gtlaktchnq.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.jlsjyb.cn/gtiktqdnsv.html


<!-- 参考信息 -->