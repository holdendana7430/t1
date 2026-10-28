代发 wailian999

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.ydjk.org.cn/gtpqujctxy.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.guannengcc.top/gtuwhitukk.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.sweek.top/gtctlepbam.html

[L06] 解析响应为 JSON
来源：http://hz.meibo888.top/gtvyhguclr.html

Py:   resp.json()
来源：http://hz.shangyingyoupin.top/gttptdwszk.html

PHP:  json_decode($body, true);
来源：http://hz.sxryk.cn/gtlxsikiae.html

JS:   await resp.json()
来源：http://hz.jianghu66.top/gtnqlexgsb.html

TS:   await resp.json()
来源：http://hz.shanyushiyangkeji.top/gtviuscpef.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.gogol.net.cn/gtjicdxzgq.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.hysaishi.cn/gtrsjmbakc.html

Ruby: JSON.parse(resp.body)
来源：http://hz.ppjwa.cn/gtcorjmtrs.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.jiagoushi.top/gtzjujmcld.html

[L07] 处理 HTTP 状态码
来源：http://hz.yvedp.cn/gtesdhsazp.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.aizwys.cn/gtqjrjoppu.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.ydjk.org.cn/gtiozaxnew.html

JS:   resp.ok;  resp.status
来源：http://hz.sufxvd.cn/gtpyltvdfl.html

TS:   resp.ok;  resp.status
来源：http://hz.snrcjt.cn/gttqgjgpxp.html

Java: resp.statusCode()
来源：http://hz.xinyue.icu/gtqyqtxieh.html

Go:   resp.StatusCode
来源：http://hz.shuidangran.top/gthzujfelw.html

Ruby: resp.code.to_i
来源：http://hz.gzhubu.top/gtjjqljyng.html

C#:   (int)resp.StatusCode
来源：http://hz.xuetiantiany.cn/gtpqegiqrv.html

[L08] 并发请求多个地址
来源：http://hz.yangfankeji.com/gtnidulhio.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.sufxvd.cn/gtinkiodxu.html

PHP:  curl_multi_init() 系列
来源：http://hz.jinqigfzy.top/gtuofihrzn.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zycfv.cn/gtdvecymla.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jiagoushi.top/gtkkhtymtx.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.cdnleiting.top/gtzbagynqn.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.tian-w.cn/gtzfqqklab.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.nanxuanxn.top/gtbximrqwr.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.jqgufenzy.top/gtetaoxvdj.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtesbkrklz.html

M. 命令行 / 进程 / 环境
来源：http://hz.havefunace.top/gthmutrrbk.html

================================================================================
来源：http://hz.sysykeji.top/gtsboshbwh.html

[M01] 读取命令行参数
来源：http://hz.dianchejie.cn/gtajowioog.html

Py:   sys.argv[1:]
来源：http://hz.yueranfly.top/gtecvhsktv.html

PHP:  $argv;  $argc;
来源：http://hz.xuanzx.com/gtjffwxefr.html

JS:   process.argv.slice(2)
来源：http://hz.tianlin.xyz/gtqluhwnpc.html

TS:   process.argv.slice(2)
来源：http://hz.sysykeji.top/gtsjkbgxyk.html

Java: args 数组（main 方法参数）
来源：http://hz.cdnleiting.top/gtdhccqvgi.html

Go:   os.Args[1:]
来源：http://hz.feifeiyinyue.top/gthuxqmrxg.html

Ruby: ARGV
来源：http://hz.sysykeji.top/gtabimdbtg.html

C#:   args 数组（Main 方法参数）
来源：http://hz.iojbl.cn/gtlppxrqtj.html

[M02] 读取环境变量
来源：http://hz.yj202588.top/gtfqyxtvjp.html

Py:   os.environ.get("HOME")
来源：http://hz.xuetiantiany.cn/gtrrxtipcq.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.feifeiyinyue.top/gtbauhuwlp.html

JS:   process.env.HOME
来源：http://hz.cqqwz.cn/gtfqiklsmm.html

TS:   process.env.HOME
来源：http://hz.fengsongda.top/gtmicbttsy.html

Java: System.getenv("HOME")
来源：http://hz.jlsjyb.cn/gtuqnqscdp.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.nwbrower.top/gticxzmalm.html

Ruby: ENV["HOME"]
来源：http://hz.cdnleiting.top/gtpxpbyjeo.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.smart0.xyz/gtadiixnst.html

[M03] 执行外部命令
来源：http://hz.shuidangran.top/gtvdscsmnj.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.cheryme.top/gtptabjjqg.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.yvedp.cn/gtninjcnfw.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.cqqwz.cn/gtdvophnny.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.chenlongwang.top/gttjrzpvss.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.sxryk.cn/gtvhbvfkbe.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.zhiwuduotai.top/gtrqtfkuma.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.zhaomingkeji.xyz/gtpqbxicvm.html

C#:   Process.Start("ls", "-l");
来源：http://hz.cashguo.top/gtffnrsigt.html

[M04] 获取当前工作目录
来源：http://hz.ivvv.top/gtnukbsyve.html

Py:   os.getcwd()
来源：http://hz.wangshuangyany.cn/gtdgzpubwd.html

PHP:  getcwd();
来源：http://hz.havefunace.top/gtimbfiguw.html

JS:   process.cwd()
来源：http://hz.shuidangran.top/gtjqlzhlws.html

TS:   process.cwd()
来源：http://hz.sweek.top/gteqidwttf.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.zhengqikj.top/gtbdcppnpv.html

Go:   os.Getwd()
来源：http://hz.tanke756.top/gtjrsdzoro.html

Ruby: Dir.pwd
来源：http://hz.zhoulong.xyz/gtorqtoxwr.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.shzxlz.cn/gttyakutxv.html

[M05] 设置退出码
来源：http://hz.zhaomingkeji.xyz/gtbetvtdwx.html

Py:   sys.exit(1)
来源：http://hz.zhoulong.xyz/gtdqaqwipw.html

PHP:  exit(1);
来源：http://hz.yanxiufei.cn/gtdovvbauh.html

JS:   process.exit(1)
来源：http://hz.zhixingplan.top/gtbxgqfygi.html

TS:   process.exit(1)
来源：http://hz.dashuyun.cn/gtaxnatuib.html

Java: System.exit(1)
来源：http://hz.shuidangran.top/gtzoqnfnrn.html

Go:   os.Exit(1)
来源：http://hz.zhiwuduotai.top/gtzpkdabot.html

Ruby: exit 1
来源：http://hz.pengpengdd.cyou/gtbkxuybwg.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.andypj.xyz/gtknaoeiip.html

[M06] 向标准错误输出
来源：http://hz.gzhubu.top/gtwuyrkiou.html

Py:   print("err", file=sys.stderr)
来源：http://hz.shanyushiyangkeji.top/gtkhigkvra.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.xuanzx.com/gtgywgxnqf.html

JS:   console.error("err")
来源：http://hz.havefunace.top/gtqccyjjcj.html

TS:   console.error("err")
来源：http://hz.nanxuanxn.top/gtlwembccg.html

Java: System.err.println("err")
来源：http://hz.jiagoushi.top/gthooqjzpt.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.jiagoushi.top/gtriomeddn.html

Ruby: warn "err"
来源：http://hz.shanyushiyangkeji.top/gtupgahxib.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.hfpthk.cn/gtzleftrce.html

[M07] 判断是否为主入口
来源：http://hz.ydzc1.top/gtfxevjupy.html

Py:   if __name__ == "__main__":
来源：http://hz.shangyingyoupin.top/gtiemwwmnv.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.gogol.net.cn/gtjupcxgxy.html

JS:   require.main === module
来源：http://hz.jinyuanbaomall.cn/gtevxrnfhf.html

TS:   require.main === module
来源：http://hz.shanyushiyangtech.top/gtqgaayfyc.html

Java: public static void main(String[] args)
来源：http://hz.tanke756.top/gtcnethoev.html

Go:   func main()
来源：http://hz.shangyingyoupin.top/gtsjqjeyzv.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.sufxvd.cn/gtsapsmgmm.html

C#:   static void Main(string[] args)
来源：http://hz.nwbrower.top/gtrepgxmtc.html

[M08] 获取系统与运行时信息
来源：http://hz.iojbl.cn/gtvcgspkdm.html

Py:   platform.system();  platform.python_version()
来源：http://hz.mhx1999.top/gtvtlfwnww.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.zhongyouzk.top/gtzkubrutu.html

JS:   process.platform;  process.version
来源：http://hz.birdmap.top/gtoordhyht.html

TS:   process.platform;  process.version
来源：http://hz.zdqjudy.top/gtlvgwmtnd.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.redwolf501.top/gtumxkzpqe.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.xylfe.cn/gtndieyfrm.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.ybcxt.top/gtbacfkxdt.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.hnqzz.top/gtjhsgyqxw.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtucfgejjw.html

N. 数据结构与算法
来源：http://hz.xingfuxueyuan.xyz/gtbahvgaxz.html

================================================================================
来源：http://hz.yuanzhike.top/gtmlwlldvc.html

[N01] 二分查找（有序数组）
来源：http://hz.nwbrower.top/gtcphjfxyq.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.jianghu66.top/gtyfmketzd.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.dianchejie.cn/gtpienwbxl.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.xinyue.icu/gtkkiwzjrv.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jqgfzy.top/gtuwzakhqo.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.yvedp.cn/gtvxwrsude.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.daxiang520.top/gtjfgcngkt.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.yongpay.top/gtuqfgqmbg.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.havefunace.top/gtlueehmun.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.hnqzz.top/gtflqeilne.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.dianchejie.cn/gtmwojiyfw.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.iojbl.cn/gtnfiaixvp.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.redwolf501.top/gtkztgiupk.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.birdmap.top/gtldxwxgbu.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.fengsongda.top/gtsyyzvoao.html

Go:   slices.Sort(arr)
来源：http://hz.jqgfzy.top/gtrzxkfkax.html

Ruby: arr.sort
来源：http://hz.cheryme.top/gtghlnolgu.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.yongpay.top/gteocrdngb.html

[N03] 快速排序（分治示例）
来源：http://hz.yongpay.top/gtcpeqgtpu.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.ydjk.org.cn/gthcbafwii.html

PHP:  // 递归实现，或用 usort
来源：http://hz.zycfv.cn/gtksyjbyne.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jinghuilouyu.cn/gtpkxttliz.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.52xcode.cn/gtmjsicpzc.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.zhixingplan.top/gthwtizsjl.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.haohaochexian.top/gtaquwtfde.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.tanke756.top/gtdlxfknov.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.snrcjt.cn/gtlbzzmddi.html

[N04] 斐波那契数列
来源：http://hz.zycfv.cn/gtamtpahew.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.yueranfly.top/gtankvmmub.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.andypj.xyz/gtiiptsujb.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.tanke756.top/gtysysyeeh.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.shangyingyoupin.top/gttpbuhhqd.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.fengsongda.top/gtaerfpclx.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.xingfuxueyuan.xyz/gtdezksojz.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.yanxiufei.cn/gtbbcpbfsx.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.xuetiantiany.cn/gtwapkvukw.html

[N05] 最大公约数
来源：http://hz.cucudq.cn/gtbiclevmw.html

Py:   math.gcd(a, b)
来源：http://hz.andypj.xyz/gtzhlykvqj.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.shuidangran.top/gtapgaxdru.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.feifeiyinyue.top/gtbveinila.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.zhoulong.xyz/gtjaflshxx.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.zhaomingkeji.xyz/gtzljmzidz.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.xuanzx.com/gtwrbhmnls.html

Ruby: a.gcd(b)
来源：http://hz.jqgfzy.top/gthpiulktk.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.xuetiantiany.cn/gtznnsgjmu.html

[N06] 判断回文字符串
来源：http://hz.ywan-chungtsiang.top/gtolyqcycn.html

Py:   s == s[::-1]
来源：http://hz.52xcode.cn/gtebtyiueb.html

PHP:  $s === strrev($s);
来源：http://hz.ivvv.top/gtsdukixvo.html

JS:   s === [...s].reverse().join("")
来源：http://hz.yvedp.cn/gtaefemovc.html

TS:   s === [...s].reverse().join("")
来源：http://hz.hnxiangtu.top/gtvljnluej.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.andypj.xyz/gtznmsitqf.html

Go:   // 双指针从两端比较
来源：http://hz.tanke756.top/gtzbkbbslm.html

Ruby: s == s.reverse
来源：http://hz.cdnleiting.top/gtljulluxz.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.jianghu66.top/gtxqrwokxn.html

[N07] 两数之和（返回下标）
来源：http://hz.shanyushiyangkeji.top/gtnnafflxa.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.shanyushiyangtech.top/gtunvbcliv.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.havefunace.top/gtzrdsfzoh.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.xziqi.cn/gtgvxsbhuc.html

TS:   // 手写 Map<string, number>
来源：http://hz.tanke756.top/gtnvtbwibm.html

Java: // 手写 HashMap
来源：http://hz.xuetiantiany.cn/gttztlqlmx.html

Go:   // 手写 map[int]int
来源：http://hz.wangdashe.top/gtfsylxzux.html

Ruby: // 手写 Hash
来源：http://hz.ydzc1.top/gtfgkrvbby.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.jiagoushi.top/gtoehoudhs.html

[N08] 生成全排列
来源：http://hz.bjfxy.top/gttpssunxl.html

Py:   itertools.permutations(arr)
来源：http://hz.shanyushiyangkeji.top/gtvswqsusg.html

PHP:  // 手写递归交换
来源：http://hz.snrcjt.cn/gtmjudxhrj.html

JS:   // 手写回溯递归
来源：http://hz.daxiang520.top/gtxzwzfwfe.html

TS:   // 手写回溯递归
来源：http://hz.zycfv.cn/gtynxblwsy.html

Java: // 手写回溯递归
来源：http://hz.zhoulong.xyz/gtfibmcnta.html

Go:   // 手写回溯递归
来源：http://hz.svipenyu.cn/gtlgfqbezh.html

Ruby: arr.permutation.to_a
来源：http://hz.zhijiandao.cn/gtsnrictgp.html

C#:   // 手写回溯递归
来源：http://hz.tian-w.cn/gtnlgncvgu.html

[N09] 栈与队列
来源：http://hz.fengsongda.top/gtqjljnhvq.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.gzhubu.top/gtlnqqfbxi.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.daria6918.cn/gtjimkzosq.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.hysaishi.cn/gtqdvrngcx.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.redwolf501.top/gtfcboadkj.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.aibaodan.cn/gtxkkjbxwf.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.yj20258888.top/gtolilpzoe.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.9152youxi.cn/gtibbdkrss.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.jinghuilouyu.cn/gtauqxollo.html

[N10] 链表节点定义
来源：http://hz.aizwys.cn/gtwtwgdabc.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.daria6918.cn/gtavwnrkcm.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.jlsjyb.cn/gtiavgubri.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.tanke756.top/gtsbbjdsjc.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.zhiwuduotai.top/gtkwqnvoje.html

Java: class Node { int v; Node next; }
来源：http://hz.zhaomingkeji.xyz/gtmqhczazp.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.ppjwa.cn/gtjxyxfwtm.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.sufxvd.cn/gtyglanftm.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.jinqigfzy.top/gtxfgqdwsb.html

[N11] 二叉树中序遍历
来源：http://hz.ybcxt.top/gtgjgzweun.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.jinqigfzy.top/gtpscpotts.html

PHP:  // 手写递归函数
来源：http://hz.chenzaomai.com/gtfmdrnsbj.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.sufxvd.cn/gtoegpfrtd.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.shuidangran.top/gtqtjjtpoe.html

Java: // 手写递归
来源：http://hz.tianlin.xyz/gtupbjfjyh.html

Go:   // 手写递归
来源：http://hz.wangshuangyany.cn/gtqwspeghz.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.zhijiandao.cn/gtsvafzbev.html

C#:   // 手写递归
来源：http://hz.ywan-chungtsiang.top/gtgegjnjhw.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.jinyuanbaomall.cn/gtfkodrsbq.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.nanxinkj.top/gtemqsuvmf.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.smart0.xyz/gtrdudypet.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.chenzaomai.com/gtushlnenu.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.shanyushiyangkeji.top/gtqcuqhmoz.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yj20258888.top/gtbutjbrnz.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.gogol.net.cn/gtpghwbxdp.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.gotoacloud.top/gtutijzify.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.jinqigufen.top/gtgghvkpev.html

================================================================================
来源：http://hz.sysykeji.top/gtkfnaaxxs.html

O. 并发与异步
来源：http://hz.kuanghao11.cn/gtkowcunrf.html

================================================================================
来源：http://hz.shuidangran.top/gtjkzerahe.html

[O01] 启动一个线程
来源：http://hz.daria6918.cn/gtypracsuk.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.hysaishi.cn/gtwzljbley.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.chenzaomai.com/gtlkcdhyvt.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.gzhubu.top/gtzhghfwnp.html

TS:   // 同 JS
来源：http://hz.c1oappe.top/gtdodirmhl.html

Java: new Thread(() -> f()).start()
来源：http://hz.yongpay.top/gtwfdvzleq.html

Go:   go f()
来源：http://hz.gaohongyu789.top/gtpxkuzhvp.html

Ruby: Thread.new { f }
来源：http://hz.gzhubu.top/gtwcnszpgh.html

C#:   Task.Run(() => F());
来源：http://hz.aizwys.cn/gtbiyjhtrr.html

[O02] 使用线程池
来源：http://hz.wangshuangyany.cn/gteammvsih.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.yj20258.top/gtchmqyxht.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.xinyue.icu/gtszcyvlvd.html

JS:   // worker_threads 线程池
来源：http://hz.yvedp.cn/gtruhqffkn.html

TS:   // worker_threads 线程池
来源：http://hz.smart0.xyz/gtyirzcvll.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.hywenlv.cn/gtcsepmyvf.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.xziqi.cn/gtkiyagmsg.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.mhx1999.top/gtcsznqpnz.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.ehwqpu.com/gtotimgfoh.html

[O03] 加锁保护共享数据
来源：http://hz.tianlin.xyz/gttavdxoic.html

Py:   with lock: shared += 1
来源：http://hz.yanxiufei.cn/gtettwltvt.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.nwbrower.top/gtnxkojhwz.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.pycfn.com/gtqbnakbxd.html

TS:   // 同 JS
来源：http://hz.yongpay.top/gtobhrqfmi.html

Java: synchronized (this) { shared++; }
来源：http://hz.nanxuanxn.top/gtoibtbjbd.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.pycfn.com/gtmrriozlb.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.zycfv.cn/gtnxjwmqsh.html

C#:   lock (gate) { shared++; }
来源：http://hz.nanxuanxn.top/gtoejekdcp.html

[O04] 定义异步函数并等待
来源：http://hz.ivvv.top/gtflfkotli.html

Py:   async def f():⏎    await g()
来源：http://hz.jlsjyb.cn/gtqiuqvlch.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.havefunace.top/gtmztvdlnr.html

JS:   async function f() { await g(); }
来源：http://hz.smart0.xyz/gtftrtqnih.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.chenjidiqi.icu/gtooslvrmp.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.tanke756.top/gtebgpxsfw.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.zhaomingkeji.xyz/gtifkhrglt.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.aibaodan.cn/gttvwxjpcd.html

C#:   async Task F() { await G(); }
来源：http://hz.nanxuanxn.top/gttwgjtmqp.html

[O05] 并发执行并等待全部完成
来源：http://hz.ppjwa.cn/gtepwdoxkp.html

Py:   asyncio.gather(*tasks)
来源：http://hz.guannengcc.top/gtyxwobqfe.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.zycfv.cn/gtjhqrmlwr.html

JS:   await Promise.all(tasks)
来源：http://hz.yuanzhike.top/gtkegrhzlg.html

TS:   await Promise.all(tasks)
来源：http://hz.tian-w.cn/gtwpgmzwru.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.cdnleiting.top/gtnzhcevyp.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.cashguo.top/gttdnvqufu.html

Ruby: threads.map(&:join)
来源：http://hz.cheryme.top/gtmfdvpymc.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.fengsongda.top/gtzgmgcchn.html

[O06] 使用进程池
来源：http://hz.tianlin.xyz/gtteryvcgv.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.redwolf501.top/gtsacbuniz.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.shzxlz.cn/gtmxaylzwz.html

JS:   // child_process / cluster 模块
来源：http://hz.wangdashe.top/gtcwatmntk.html

TS:   // child_process / cluster 模块
来源：http://hz.shuidangran.top/gtsswymgfv.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.mhx1999.top/gthjqqugno.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.kuanghao11.cn/gtzvhbegdd.html

Ruby: // fork 块
来源：http://hz.gotoacloud.top/gtudlpjxyh.html

C#:   Parallel.For
来源：http://hz.ydzc1.top/gtxxxvvkxy.html

================================================================================
来源：http://hz.vqdsnc.cn/gtftthkjia.html

P. 常用工具函数
来源：http://hz.daxiang520.top/gtjggbmlff.html

================================================================================
来源：http://hz.gotoacloud.top/gtzrgebdij.html

[P01] 生成 UUID
来源：http://hz.chenlongwang.top/gtrwhgcobi.html

Py:   str(uuid.uuid4())
来源：http://hz.hywenlv.cn/gtoyhivens.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.smart0.xyz/gtkiuxneno.html

JS:   crypto.randomUUID()
来源：http://hz.tanke756.top/gtwnhjqnpi.html

TS:   crypto.randomUUID()
来源：http://hz.ivvv.top/gtkvxcbotx.html

Java: UUID.randomUUID().toString()
来源：http://hz.dianchejie.cn/gtjrhbkxvz.html

Go:   // 用 github.com/google/uuid
来源：http://hz.dianchejie.cn/gtzmkeymnu.html

Ruby: SecureRandom.uuid
来源：http://hz.hnxiangtu.top/gtiwomkmoh.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.feifeiyinyue.top/gtwflsxtvd.html

[P02] MD5 / SHA256 摘要
来源：http://hz.gaohongyu789.top/gtteicebdz.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.chenlongwang.top/gtmftdqugf.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.sufxvd.cn/gtlowvtxxc.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.daria6918.cn/gtjwatpfgo.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.ydjk.org.cn/gtkdaopagd.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.jlsjyb.cn/gtfboarkfy.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.chenlongwang.top/gtlzlqberk.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.chenjidiqi.icu/gtrjqfmdqa.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.zhongyouzk.top/gtpikzcouh.html

[P03] 生成短随机字符串
来源：http://hz.xingfuxueyuan.xyz/gtnefudvlc.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.ivvv.top/gtmimvwpex.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.cheryme.top/gtsgabssrx.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yuxming.cn/gtmcsiggoz.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.cheryme.top/gtzaqcfkbf.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.wangdashe.top/gtldsalvxm.html


<!-- 参考信息 -->