代发 wailian999

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.xziqi.cn/gtjkskqldn.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.zhijiandao.cn/gtlosgpeku.html

Ruby: JSON.parse(resp.body)
来源：http://hz.xuetiantiany.cn/gtsmnxbpxa.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.chenjidiqi.icu/gtvztuidrc.html

[L07] 处理 HTTP 状态码
来源：http://hz.smart0.xyz/gtyufmdely.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.shangyingyoupin.top/gtfxxxudkb.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.nanxinkj.top/gtoziiexya.html

JS:   resp.ok;  resp.status
来源：http://hz.wangdashe.top/gtodgizrli.html

TS:   resp.ok;  resp.status
来源：http://hz.zhiwuduotai.top/gtmtaewtad.html

Java: resp.statusCode()
来源：http://hz.bjfxy.top/gtqpkilfue.html

Go:   resp.StatusCode
来源：http://hz.zhengqikj.top/gtahmksssd.html

Ruby: resp.code.to_i
来源：http://hz.daxiang520.top/gtaygrwtdb.html

C#:   (int)resp.StatusCode
来源：http://hz.nanxinkj.top/gtnvsuxnea.html

[L08] 并发请求多个地址
来源：http://hz.pycfn.com/gtzxzgnhfo.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.dianchejie.cn/gtsjrraahs.html

PHP:  curl_multi_init() 系列
来源：http://hz.iojbl.cn/gtneudhbbn.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yueranfly.top/gtkbanhkxd.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhongyouzk.top/gteinzmart.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.redwolf501.top/gthkzspxdk.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.chenjidiqi.icu/gtyaovyipw.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.zhixingplan.top/gtpcbrjrhe.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.yangfankeji.com/gtfwmsdpds.html

================================================================================
来源：http://hz.tianlin.xyz/gtifqifkxa.html

M. 命令行 / 进程 / 环境
来源：http://hz.birdmap.top/gtxnuhvqyz.html

================================================================================
来源：http://hz.yonumen.top/gtaxtegvui.html

[M01] 读取命令行参数
来源：http://hz.dashuyun.cn/gtslvrfbgf.html

Py:   sys.argv[1:]
来源：http://hz.jqgufenzy.top/gtxjppplbk.html

PHP:  $argv;  $argc;
来源：http://hz.cqqwz.cn/gtvwkxfrjd.html

JS:   process.argv.slice(2)
来源：http://hz.dianchejie.cn/gtfylvsidd.html

TS:   process.argv.slice(2)
来源：http://hz.hywenlv.cn/gtuklglemy.html

Java: args 数组（main 方法参数）
来源：http://hz.ywan-chungtsiang.top/gtvcezumcx.html

Go:   os.Args[1:]
来源：http://hz.sweek.top/gtcirvonfr.html

Ruby: ARGV
来源：http://hz.shangyingyoupin.top/gtkcszkuyx.html

C#:   args 数组（Main 方法参数）
来源：http://hz.shanyushiyangkeji.top/gtppobaihl.html

[M02] 读取环境变量
来源：http://hz.vqdsnc.cn/gtigenufaq.html

Py:   os.environ.get("HOME")
来源：http://hz.xuanzx.com/gtzxdglxwg.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.xziqi.cn/gtknohlqyo.html

JS:   process.env.HOME
来源：http://hz.dianchejie.cn/gtquwbwfbh.html

TS:   process.env.HOME
来源：http://hz.zhoulong.xyz/gtyddcdotu.html

Java: System.getenv("HOME")
来源：http://hz.daria6918.cn/gtidkauchu.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.gogol.net.cn/gtgvxrkhit.html

Ruby: ENV["HOME"]
来源：http://hz.shuidangran.top/gtwuofdxop.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.shuidangran.top/gteuruiusa.html

[M03] 执行外部命令
来源：http://hz.zhoulong.xyz/gtpcvntnem.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.kuanghao11.cn/gtwalybxxm.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.fengsongda.top/gtpayzhaka.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.tian-w.cn/gtrbilwvln.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.yonumen.top/gtpybqrokw.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.dianchejie.cn/gtbjyiidwt.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.kuanghao11.cn/gtnlnkdnnr.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.hnxiangtu.top/gtnzbidmai.html

C#:   Process.Start("ls", "-l");
来源：http://hz.yongpay.top/gtmiueccfi.html

[M04] 获取当前工作目录
来源：http://hz.birdmap.top/gtujctbhxq.html

Py:   os.getcwd()
来源：http://hz.dianchejie.cn/gtkmmbbfmj.html

PHP:  getcwd();
来源：http://hz.yuanzhike.top/gtfgajjfql.html

JS:   process.cwd()
来源：http://hz.yvedp.cn/gtrbhxreak.html

TS:   process.cwd()
来源：http://hz.yangfankeji.com/gtitomhhia.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.dashuyun.cn/gtrefxoiox.html

Go:   os.Getwd()
来源：http://hz.jqgfzy.top/gtxzklqamm.html

Ruby: Dir.pwd
来源：http://hz.cashguo.top/gtpzpoawrl.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.daxiang520.top/gtfichkjnn.html

[M05] 设置退出码
来源：http://hz.jinghuilouyu.cn/gtkbaspjzh.html

Py:   sys.exit(1)
来源：http://hz.zhongyouzk.top/gtfjnyojdj.html

PHP:  exit(1);
来源：http://hz.snrcjt.cn/gtllwzqnyj.html

JS:   process.exit(1)
来源：http://hz.jinghuilouyu.cn/gtzkpafrkl.html

TS:   process.exit(1)
来源：http://hz.hnxiangtu.top/gtmezfbnoq.html

Java: System.exit(1)
来源：http://hz.yongpay.top/gtmmdazibv.html

Go:   os.Exit(1)
来源：http://hz.xinyue.icu/gtwogsggqe.html

Ruby: exit 1
来源：http://hz.jqgfzy.top/gtifwrffxv.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.jyoumei.cn/gthbbzcftp.html

[M06] 向标准错误输出
来源：http://hz.jyoumei.cn/gtlzfjetlo.html

Py:   print("err", file=sys.stderr)
来源：http://hz.jqgufenzy.top/gtuqgaqbvk.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.hywenlv.cn/gtqhxtjuxi.html

JS:   console.error("err")
来源：http://hz.cqqwz.cn/gtlikosums.html

TS:   console.error("err")
来源：http://hz.wangshuangyany.cn/gtbuewegyj.html

Java: System.err.println("err")
来源：http://hz.fzhhl.top/gttllgzeja.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.zhoulong.xyz/gtjtaesivi.html

Ruby: warn "err"
来源：http://hz.aibaodan.cn/gtszwbvshh.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.9152youxi.cn/gtusagmnwb.html

[M07] 判断是否为主入口
来源：http://hz.pengpengdd.cyou/gtdiiwjqct.html

Py:   if __name__ == "__main__":
来源：http://hz.daxiang520.top/gtryiqnbpl.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.jinghuilouyu.cn/gtikfjmpzp.html

JS:   require.main === module
来源：http://hz.daria6918.cn/gttkzxuwxr.html

TS:   require.main === module
来源：http://hz.ydzc1.top/gtbvwukvlf.html

Java: public static void main(String[] args)
来源：http://hz.shuidangran.top/gtfptxmesj.html

Go:   func main()
来源：http://hz.0kj1m.cn/gtwmooslwz.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.jinqigfzy.top/gtcarwilpj.html

C#:   static void Main(string[] args)
来源：http://hz.meibo888.top/gtzgqlptqn.html

[M08] 获取系统与运行时信息
来源：http://hz.jlsjyb.cn/gtdgwvzcuz.html

Py:   platform.system();  platform.python_version()
来源：http://hz.zhoulong.xyz/gtrtpobqam.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.vqdsnc.cn/gtfowkvgoc.html

JS:   process.platform;  process.version
来源：http://hz.ivvv.top/gthwjpzgwo.html

TS:   process.platform;  process.version
来源：http://hz.jinyuanbaomall.cn/gtevmpabru.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.hammf.cn/gtuehcfloo.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.jinghuilouyu.cn/gthyfhpgon.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.fengsongda.top/gttubcgjjz.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.cqqwz.cn/gtmnevyxfx.html

================================================================================
来源：http://hz.svipenyu.cn/gtxxlqldnq.html

N. 数据结构与算法
来源：http://hz.xziqi.cn/gtioljiobk.html

================================================================================
来源：http://hz.cheryme.top/gtdcrugoyp.html

[N01] 二分查找（有序数组）
来源：http://hz.ywan-chungtsiang.top/gtlcqdabhg.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.ppjwa.cn/gtplsityxf.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.jyoumei.cn/gtumnrsnps.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yuanzhike.top/gtvalpasgg.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zhengqikj.top/gtdfrkugii.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.birdmap.top/gtosyhnkwf.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.jinyuanbaomall.cn/gteuancgti.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.yuxming.cn/gtacppqljf.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.xuanzx.com/gtoffsccct.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.aibaodan.cn/gtbzifyyxq.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.yj202588.top/gtrvlgxyeq.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.meibo888.top/gtpxnlcnwb.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.c1oappe.top/gtgusyhrrl.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jqgufenzy.top/gtfpypeqqa.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.c1oappe.top/gtdynwfuqf.html

Go:   slices.Sort(arr)
来源：http://hz.ehwqpu.com/gtdbyngzsz.html

Ruby: arr.sort
来源：http://hz.ywan-chungtsiang.top/gthcrudtuj.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.tian-w.cn/gtnapolbqc.html

[N03] 快速排序（分治示例）
来源：http://hz.shanyushiyangtech.top/gtvmaudxkk.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.yanxiufei.cn/gtpbkaroju.html

PHP:  // 递归实现，或用 usort
来源：http://hz.chenjidiqi.icu/gtpmgephvm.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.dashuyun.cn/gtaxhnnbnl.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.cucudq.cn/gtolewojnx.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.fengsongda.top/gtkuhikfgq.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.xuetiantiany.cn/gtvlthroxd.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.wangdashe.top/gtalsootff.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.fzhhl.top/gtcbcnqhqk.html

[N04] 斐波那契数列
来源：http://hz.jinqigfzy.top/gtaeslczbm.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.aibaodan.cn/gtnfpsvkwl.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.gotoacloud.top/gtirxsbysz.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.zhoulong.xyz/gtlfnobbyi.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.birdmap.top/gtjgggonaj.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.zycfv.cn/gtbqmszpif.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.cqqwz.cn/gtgvjivfed.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.daria6918.cn/gtirsgbzpd.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.haohaochexian.top/gtiwqwibag.html

[N05] 最大公约数
来源：http://hz.yonumen.top/gtosffnflq.html

Py:   math.gcd(a, b)
来源：http://hz.iojbl.cn/gtaolanuif.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.pengpengdd.cyou/gtmpkfmjwj.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.redwolf501.top/gttfuagjjc.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.aizwys.cn/gtgsahpqsb.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.nwbrower.top/gtoucujzjs.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.yangfankeji.com/gthrsvfigo.html

Ruby: a.gcd(b)
来源：http://hz.ydzc1.top/gtnonfocma.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.shuidangran.top/gtcfttfbuz.html

[N06] 判断回文字符串
来源：http://hz.tanke756.top/gtzghqmftd.html

Py:   s == s[::-1]
来源：http://hz.yangfankeji.com/gtzfidguog.html

PHP:  $s === strrev($s);
来源：http://hz.cucudq.cn/gtyuslruml.html

JS:   s === [...s].reverse().join("")
来源：http://hz.yvedp.cn/gtfyaswwdm.html

TS:   s === [...s].reverse().join("")
来源：http://hz.zhaomingkeji.xyz/gtijsqppys.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.jinqigufen.top/gteohadwxg.html

Go:   // 双指针从两端比较
来源：http://hz.aizwys.cn/gtdvqwindd.html

Ruby: s == s.reverse
来源：http://hz.yuxming.cn/gtwcchbbpu.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.sufxvd.cn/gtjkralxws.html

[N07] 两数之和（返回下标）
来源：http://hz.aibaodan.cn/gtscewiycm.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.9152youxi.cn/gtmfxklhnh.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.jianghu66.top/gtzoqhutue.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.mhx1999.top/gtcqyhbcgn.html

TS:   // 手写 Map<string, number>
来源：http://hz.ywan-chungtsiang.top/gtnczdeszb.html

Java: // 手写 HashMap
来源：http://hz.daria6918.cn/gtappbbuut.html

Go:   // 手写 map[int]int
来源：http://hz.chenjidiqi.icu/gtbgipheln.html

Ruby: // 手写 Hash
来源：http://hz.kuanghao11.cn/gtptoijbpx.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.gotoacloud.top/gttouiwddk.html

[N08] 生成全排列
来源：http://hz.haohaochexian.top/gtbkmkxvof.html

Py:   itertools.permutations(arr)
来源：http://hz.0kj1m.cn/gtelzpagzn.html

PHP:  // 手写递归交换
来源：http://hz.gaohongyu789.top/gtpgievzot.html

JS:   // 手写回溯递归
来源：http://hz.zhiwuduotai.top/gtzkdbtaym.html

TS:   // 手写回溯递归
来源：http://hz.zhijiandao.cn/gtvboqsjvy.html

Java: // 手写回溯递归
来源：http://hz.52xcode.cn/gtddhqjlkh.html

Go:   // 手写回溯递归
来源：http://hz.xziqi.cn/gtxbhiuucg.html

Ruby: arr.permutation.to_a
来源：http://hz.jyoumei.cn/gtyufzowbk.html

C#:   // 手写回溯递归
来源：http://hz.hywenlv.cn/gtxxistnqs.html

[N09] 栈与队列
来源：http://hz.daxiang520.top/gtyvmlpwet.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.ivvv.top/gtmikgumwq.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.jinqigfzy.top/gtgxdyumyt.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.redwolf501.top/gtjkyujbfa.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.zycfv.cn/gtjtnuxbbn.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.ydjk.org.cn/gthhpndybd.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.gogol.net.cn/gtocdrgrtp.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.xuanzx.com/gttvpxztjo.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.shzxlz.cn/gtfdelxwxb.html

[N10] 链表节点定义
来源：http://hz.ehwqpu.com/gthriujcjd.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.zhengqikj.top/gtxrwgukqh.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.chenlongwang.top/gtypctbpsa.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.ppjwa.cn/gtnunwpgcs.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.cashguo.top/gttfjdxczp.html

Java: class Node { int v; Node next; }
来源：http://hz.jianghu66.top/gtvsxznjii.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.9152youxi.cn/gthinpuwnj.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.cheryme.top/gtgayqvwiv.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.jinyuanbaomall.cn/gtorsypuoc.html

[N11] 二叉树中序遍历
来源：http://hz.c1oappe.top/gtjkyepuyb.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.ywan-chungtsiang.top/gtqvxdllxx.html

PHP:  // 手写递归函数
来源：http://hz.yuxming.cn/gtdmvgqaql.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.ppjwa.cn/gtdgwtqkwt.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.cdnleiting.top/gtpvnleaki.html

Java: // 手写递归
来源：http://hz.daria6918.cn/gtdzfzbtuq.html

Go:   // 手写递归
来源：http://hz.hnxiangtu.top/gtrjohdjst.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.zhoulong.xyz/gtnklrkwiy.html

C#:   // 手写递归
来源：http://hz.jinyuanbaomall.cn/gtdigbtaeq.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.shzxlz.cn/gtaiqbwqln.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.gotoacloud.top/gtjnldhruc.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.yangfankeji.com/gtydeenrvu.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.cdnleiting.top/gtyupojjtf.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jqgufenzy.top/gtwfiwllrj.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.xziqi.cn/gtetnmdlam.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.nanxuanxn.top/gtlvbwwnmp.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.xuetiantiany.cn/gtketwpllu.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.sweek.top/gtpzukbddj.html

================================================================================
来源：http://hz.mhx1999.top/gtmsivtjma.html

O. 并发与异步
来源：http://hz.gotoacloud.top/gtliiukkxa.html

================================================================================
来源：http://hz.redwolf501.top/gtctdvnyhc.html

[O01] 启动一个线程
来源：http://hz.mhx1999.top/gtrfgsdpvd.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.yvedp.cn/gtrrvwwfaf.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.ydzc1.top/gtchxwocxf.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.hongshengwenyu.top/gtloftczmz.html

TS:   // 同 JS
来源：http://hz.redwolf501.top/gtsyurfuky.html

Java: new Thread(() -> f()).start()
来源：http://hz.nanxinkj.top/gtqlrgzwsw.html

Go:   go f()
来源：http://hz.andypj.xyz/gtflfsglpv.html

Ruby: Thread.new { f }
来源：http://hz.yanxiufei.cn/gtxrxncptv.html

C#:   Task.Run(() => F());
来源：http://hz.hywenlv.cn/gtupacmqut.html

[O02] 使用线程池
来源：http://hz.9152youxi.cn/gtluwsiudu.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.sxryk.cn/gtcxcqhtwe.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.zhoulong.xyz/gtrblkulzh.html

JS:   // worker_threads 线程池
来源：http://hz.xinyue.icu/gtropnmcdi.html

TS:   // worker_threads 线程池
来源：http://hz.ppjwa.cn/gttdzyxowg.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.ydjk.org.cn/gtrxlstiyr.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.jyoumei.cn/gtiptmtkif.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.zhijiandao.cn/gtgbmwbfvk.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.guowangkeji.top/gtgdagfquw.html

[O03] 加锁保护共享数据
来源：http://hz.shuidangran.top/gtotolrbka.html

Py:   with lock: shared += 1
来源：http://hz.ydzc1.top/gteovsxfvl.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.xuanzx.com/gtgxtfsadg.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.meibo888.top/gtcmzwroeq.html

TS:   // 同 JS
来源：http://hz.cucudq.cn/gtgedvvxoz.html

Java: synchronized (this) { shared++; }
来源：http://hz.hnxiangtu.top/gtaqakbyii.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.ivvv.top/gtnasgeakq.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.tianlin.xyz/gtluwqhyws.html

C#:   lock (gate) { shared++; }
来源：http://hz.jqgufenzy.top/gtdxpllsbg.html

[O04] 定义异步函数并等待
来源：http://hz.hongshengwenyu.top/gtwdocsnvr.html

Py:   async def f():⏎    await g()
来源：http://hz.gaohongyu789.top/gthkkzcgbp.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.hywenlv.cn/gtaagiitui.html

JS:   async function f() { await g(); }
来源：http://hz.guannengcc.top/gtlxkqmrua.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.zycfv.cn/gtbnipebkd.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.birdmap.top/gthdjltdcr.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.fzhhl.top/gtpeeossms.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.shanyushiyangkeji.top/gtmkbgptjp.html

C#:   async Task F() { await G(); }
来源：http://hz.svipenyu.cn/gtadfjzlqr.html

[O05] 并发执行并等待全部完成
来源：http://hz.smart0.xyz/gtkytkgmse.html

Py:   asyncio.gather(*tasks)
来源：http://hz.haohaochexian.top/gtmddcnszm.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.xziqi.cn/gtziutxadj.html

JS:   await Promise.all(tasks)
来源：http://hz.jinghuilouyu.cn/gtqaattsmc.html

TS:   await Promise.all(tasks)
来源：http://hz.shanyushiyangtech.top/gtfpvggxci.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.hysaishi.cn/gtlwmfvutp.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.fengsongda.top/gtkdlenqer.html

Ruby: threads.map(&:join)
来源：http://hz.yj20258.top/gtbrayigxm.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.redwolf501.top/gtcnezbhdp.html

[O06] 使用进程池
来源：http://hz.zycfv.cn/gttqdccemu.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.bjfxy.top/gthvmxluso.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.chenzaomai.com/gtgaicwrht.html

JS:   // child_process / cluster 模块
来源：http://hz.zhijiandao.cn/gtyekpoocs.html

TS:   // child_process / cluster 模块
来源：http://hz.zycfv.cn/gtcyomulqm.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.cashguo.top/gtodckkffk.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.redwolf501.top/gtzcxulagn.html

Ruby: // fork 块
来源：http://hz.svipenyu.cn/gtxcggdykw.html

C#:   Parallel.For
来源：http://hz.pycfn.com/gtzsirzbfj.html

================================================================================
来源：http://hz.yvedp.cn/gtjxplwbbd.html

P. 常用工具函数
来源：http://hz.jiagoushi.top/gtaijfbbzb.html

================================================================================
来源：http://hz.yuxming.cn/gtfzwpyarp.html

[P01] 生成 UUID
来源：http://hz.hywenlv.cn/gtyirtgvug.html

Py:   str(uuid.uuid4())
来源：http://hz.shangyingyoupin.top/gtglnznhcd.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.c1oappe.top/gthgdratqm.html

JS:   crypto.randomUUID()
来源：http://hz.yueranfly.top/gtigggsrma.html

TS:   crypto.randomUUID()
来源：http://hz.zhiwuduotai.top/gtgokyqumi.html

Java: UUID.randomUUID().toString()
来源：http://hz.jqgufenzy.top/gtroabnaol.html

Go:   // 用 github.com/google/uuid
来源：http://hz.guowangkeji.top/gtbrgmzwfi.html

Ruby: SecureRandom.uuid
来源：http://hz.xinyue.icu/gtpufeorih.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.ydzc1.top/gtvrslaztb.html

[P02] MD5 / SHA256 摘要
来源：http://hz.yongpay.top/gtuldldjjr.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.tianlin.xyz/gtiayuvpqb.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.nanxinkj.top/gtpqbcuwfd.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.yonumen.top/gtwfinexsm.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.yongpay.top/gtjxfmiekq.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.havefunace.top/gtseywdwyz.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.daria6918.cn/gtcijyeyjp.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.52xcode.cn/gtiartjogj.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.smart0.xyz/gtxdbnxlnl.html

[P03] 生成短随机字符串
来源：http://hz.pycfn.com/gtsvdzdjpr.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.ybcxt.top/gtfhwrhvzl.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.yongpay.top/gtxdsxsvaf.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.shuidangran.top/gtulmvmphg.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.xuetiantiany.cn/gtylauvsad.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.jianghu66.top/gtukwhomrv.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.jlsjyb.cn/gtcchzozkv.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.ehwqpu.com/gtumynyraw.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.yanxiufei.cn/gtzlyronbc.html

[P04] 求长度
来源：http://hz.hnqzz.top/gttdrdwctj.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.zycfv.cn/gtnxmegtci.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.shanyushiyangkeji.top/gtdocrsbed.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.ehwqpu.com/gtdonmmecv.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.xuetiantiany.cn/gtevrvqmxo.html


<!-- 参考信息 -->