代发 wailian999

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.haohaochexian.top/gthhxzyipv.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.feifeiyinyue.top/gtonwxrfga.html

Ruby: JSON.parse(resp.body)
来源：http://hz.wangdashe.top/gtlntnbgzh.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.tianlin.xyz/gtnomuhfdy.html

[L07] 处理 HTTP 状态码
来源：http://hz.cashguo.top/gtsickbhfg.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.zhixingplan.top/gtlavyaxax.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.jqgfzy.top/gtdtfviqco.html

JS:   resp.ok;  resp.status
来源：http://hz.gaohongyu789.top/gtjfhusuod.html

TS:   resp.ok;  resp.status
来源：http://hz.hysaishi.cn/gtobrpnbzt.html

Java: resp.statusCode()
来源：http://hz.zhoulong.xyz/gtdtnapayx.html

Go:   resp.StatusCode
来源：http://hz.jlsjyb.cn/gtlebdlpof.html

Ruby: resp.code.to_i
来源：http://hz.ppjwa.cn/gtlljwquxc.html

C#:   (int)resp.StatusCode
来源：http://hz.cqqwz.cn/gtlhmphjvj.html

[L08] 并发请求多个地址
来源：http://hz.sysykeji.top/gthylxvbxn.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.xuanzx.com/gtenpzmxec.html

PHP:  curl_multi_init() 系列
来源：http://hz.cheryme.top/gtkmqjzwym.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.cqqwz.cn/gtwslzraxd.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.hysaishi.cn/gtgmvsccgz.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.hfpthk.cn/gtubwisiff.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.yj20258888.top/gtewbdfwil.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.redwolf501.top/gtwivoaqlh.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.zdqjudy.top/gtrzxhpeyv.html

================================================================================
来源：http://hz.jianghu66.top/gtfsojygxn.html

M. 命令行 / 进程 / 环境
来源：http://hz.sxryk.cn/gtrmjzfadn.html

================================================================================
来源：http://hz.yj20258888.top/gtitzomazc.html

[M01] 读取命令行参数
来源：http://hz.yanxiufei.cn/gtklndcyra.html

Py:   sys.argv[1:]
来源：http://hz.birdmap.top/gtkvnedwky.html

PHP:  $argv;  $argc;
来源：http://hz.wangdashe.top/gtaaajlbzg.html

JS:   process.argv.slice(2)
来源：http://hz.0kj1m.cn/gtymucdure.html

TS:   process.argv.slice(2)
来源：http://hz.guannengcc.top/gtzmevhyay.html

Java: args 数组（main 方法参数）
来源：http://hz.chenjidiqi.icu/gtfkhywcyg.html

Go:   os.Args[1:]
来源：http://hz.vqdsnc.cn/gtroiazkea.html

Ruby: ARGV
来源：http://hz.aibaodan.cn/gtrjzounaz.html

C#:   args 数组（Main 方法参数）
来源：http://hz.jyoumei.cn/gtjczvwbcn.html

[M02] 读取环境变量
来源：http://hz.nanxuanxn.top/gtzmvshorr.html

Py:   os.environ.get("HOME")
来源：http://hz.0kj1m.cn/gtspdshamg.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.wangdashe.top/gtxciaksay.html

JS:   process.env.HOME
来源：http://hz.dashuyun.cn/gtfdgpouwv.html

TS:   process.env.HOME
来源：http://hz.vqdsnc.cn/gtcayldjow.html

Java: System.getenv("HOME")
来源：http://hz.yongpay.top/gtvldgkasv.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.gotoacloud.top/gtxefrqngr.html

Ruby: ENV["HOME"]
来源：http://hz.xuanzx.com/gtkosyqgfm.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.pengpengdd.cyou/gtxwfaedbb.html

[M03] 执行外部命令
来源：http://hz.chenjidiqi.icu/gtwuopmdfj.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.kuanghao11.cn/gtjixbowxo.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.jlsjyb.cn/gtckeflhff.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.hysaishi.cn/gtzktkczzh.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.cashguo.top/gtkgtqjigq.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.yueranfly.top/gtadjbwxep.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.haohaochexian.top/gtxzmmyeqr.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.aizwys.cn/gtbsseehze.html

C#:   Process.Start("ls", "-l");
来源：http://hz.sxryk.cn/gtyhbatfgk.html

[M04] 获取当前工作目录
来源：http://hz.xylfe.cn/gtycqhahkt.html

Py:   os.getcwd()
来源：http://hz.chenlongwang.top/gtgtyjwvkd.html

PHP:  getcwd();
来源：http://hz.dashuyun.cn/gtjmhrlxrq.html

JS:   process.cwd()
来源：http://hz.redwolf501.top/gtfkpdaiic.html

TS:   process.cwd()
来源：http://hz.dashuyun.cn/gtmmnflufq.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.dashuyun.cn/gtuuivcubx.html

Go:   os.Getwd()
来源：http://hz.jlsjyb.cn/gtmvvzvowo.html

Ruby: Dir.pwd
来源：http://hz.daxiang520.top/gtdukrkfbg.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.zhijiandao.cn/gtgnuyqxac.html

[M05] 设置退出码
来源：http://hz.shanyushiyangtech.top/gtkfhpazcv.html

Py:   sys.exit(1)
来源：http://hz.zycfv.cn/gtnmlxuyxa.html

PHP:  exit(1);
来源：http://hz.yj20258.top/gtjtxwlnyc.html

JS:   process.exit(1)
来源：http://hz.svipenyu.cn/gtluszapza.html

TS:   process.exit(1)
来源：http://hz.daria6918.cn/gtmuftfahy.html

Java: System.exit(1)
来源：http://hz.ehwqpu.com/gtbgmterce.html

Go:   os.Exit(1)
来源：http://hz.cdnleiting.top/gtmoiyhahh.html

Ruby: exit 1
来源：http://hz.ivvv.top/gtxnmdpypq.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.ehwqpu.com/gtizfyuwjk.html

[M06] 向标准错误输出
来源：http://hz.52xcode.cn/gtykycjiyi.html

Py:   print("err", file=sys.stderr)
来源：http://hz.ybcxt.top/gtyrhmqtly.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.aizwys.cn/gtuouhsaxr.html

JS:   console.error("err")
来源：http://hz.jyoumei.cn/gtphmggxtg.html

TS:   console.error("err")
来源：http://hz.pengpengdd.cyou/gtgayljhyc.html

Java: System.err.println("err")
来源：http://hz.zhoulong.xyz/gtuqcodvty.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.chenlongwang.top/gtkziyvkuv.html

Ruby: warn "err"
来源：http://hz.hysaishi.cn/gtizsawcqb.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.nanxinkj.top/gtlzzjrqaw.html

[M07] 判断是否为主入口
来源：http://hz.nwbrower.top/gtuprwnzdg.html

Py:   if __name__ == "__main__":
来源：http://hz.yueranfly.top/gtdjyodpda.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.yonumen.top/gtyvkgitry.html

JS:   require.main === module
来源：http://hz.hnxiangtu.top/gtugeswcgb.html

TS:   require.main === module
来源：http://hz.aizwys.cn/gtycjdrhfv.html

Java: public static void main(String[] args)
来源：http://hz.yj202588.top/gthxskldfq.html

Go:   func main()
来源：http://hz.zhongyouzk.top/gtqzadobyo.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.daxiang520.top/gtpphgczlm.html

C#:   static void Main(string[] args)
来源：http://hz.vqdsnc.cn/gtxafjdtvq.html

[M08] 获取系统与运行时信息
来源：http://hz.ydzc1.top/gtvhdgxzhy.html

Py:   platform.system();  platform.python_version()
来源：http://hz.xingfuxueyuan.xyz/gtjcrpjwfk.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.gotoacloud.top/gtxicvheiy.html

JS:   process.platform;  process.version
来源：http://hz.mhx1999.top/gtyrdmqqkh.html

TS:   process.platform;  process.version
来源：http://hz.yueranfly.top/gtwbuwnwhp.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.iojbl.cn/gtttzlfpah.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.yanxiufei.cn/gtbpdqgueo.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.aizwys.cn/gthdmsfsua.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.sysykeji.top/gtgbeansle.html

================================================================================
来源：http://hz.ivvv.top/gtstakihge.html

N. 数据结构与算法
来源：http://hz.shanyushiyangkeji.top/gtmmhmzjet.html

================================================================================
来源：http://hz.yuxming.cn/gtrsvlrehk.html

[N01] 二分查找（有序数组）
来源：http://hz.chenzaomai.com/gtpynzimht.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.yuxming.cn/gtxnvlndtj.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.jlsjyb.cn/gtjpwpaxgs.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.xylfe.cn/gtraavrodm.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.xuanzx.com/gtzpzuzedm.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.jinyuanbaomall.cn/gtjndatkwf.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.jinyuanbaomall.cn/gtntpcaovz.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.zhaomingkeji.xyz/gtvkpmpblf.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.cucudq.cn/gtsgjdmbsx.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.ydjk.org.cn/gtvysjbpty.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.ywan-chungtsiang.top/gtphoiiqmk.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.xuanzx.com/gtkdxscdtt.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.c1oappe.top/gtidyqztvi.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.ppjwa.cn/gtsailvvfw.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.jianghu66.top/gtqveecapp.html

Go:   slices.Sort(arr)
来源：http://hz.pycfn.com/gtqbdyxgzf.html

Ruby: arr.sort
来源：http://hz.chenzaomai.com/gtcwmeeelt.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.xziqi.cn/gtcatskjim.html

[N03] 快速排序（分治示例）
来源：http://hz.chenzaomai.com/gtwfpxgxtf.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.svipenyu.cn/gtakgwfpzx.html

PHP:  // 递归实现，或用 usort
来源：http://hz.yonumen.top/gtbgybmrcb.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.nwbrower.top/gtokzhqpzr.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.ydjk.org.cn/gtsmzgjajt.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.zycfv.cn/gtkscmwrtj.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.dashuyun.cn/gtlsddlsnv.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.chenlongwang.top/gtueynmjzj.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.yueranfly.top/gtuejucxxj.html

[N04] 斐波那契数列
来源：http://hz.yanxiufei.cn/gtpqjrdqxm.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.xinyue.icu/gtcbuvanvj.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.hfpthk.cn/gtmprtohrk.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.hywenlv.cn/gtlgfeyjuf.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.snrcjt.cn/gtdkdlycay.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.yuanzhike.top/gtsiofbpyx.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.wangdashe.top/gtvcutqonr.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.xziqi.cn/gttexvniwr.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.xziqi.cn/gtxymmxqxv.html

[N05] 最大公约数
来源：http://hz.chenjidiqi.icu/gtcgqokhpl.html

Py:   math.gcd(a, b)
来源：http://hz.jyoumei.cn/gtkhdfqioh.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.wangdashe.top/gtyrnchltw.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.hongshengwenyu.top/gtjmmpdeqe.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.xinyue.icu/gtlakuhhwq.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.cqqwz.cn/gttrvtxrby.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.hysaishi.cn/gtdufafnac.html

Ruby: a.gcd(b)
来源：http://hz.aibaodan.cn/gtvnedmbrg.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.hysaishi.cn/gtyqsjvbul.html

[N06] 判断回文字符串
来源：http://hz.ydzc1.top/gtpnshayzk.html

Py:   s == s[::-1]
来源：http://hz.yuxming.cn/gtaycktbsb.html

PHP:  $s === strrev($s);
来源：http://hz.aibaodan.cn/gtkhwspark.html

JS:   s === [...s].reverse().join("")
来源：http://hz.snrcjt.cn/gtqyabyyrx.html

TS:   s === [...s].reverse().join("")
来源：http://hz.wangshuangyany.cn/gtptqybuoy.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.daria6918.cn/gtnlwsfbjw.html

Go:   // 双指针从两端比较
来源：http://hz.yvedp.cn/gtkfofipjk.html

Ruby: s == s.reverse
来源：http://hz.jiagoushi.top/gthiegwkep.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.zhengqikj.top/gtugzgthdn.html

[N07] 两数之和（返回下标）
来源：http://hz.jianghu66.top/gtdtucphzx.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.ywan-chungtsiang.top/gtfvhjzcbh.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.dashuyun.cn/gtvwrfkghp.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.zhengqikj.top/gtwytgpyek.html

TS:   // 手写 Map<string, number>
来源：http://hz.zhixingplan.top/gtdjqoyrgq.html

Java: // 手写 HashMap
来源：http://hz.ivvv.top/gtbeugbyeo.html

Go:   // 手写 map[int]int
来源：http://hz.hysaishi.cn/gtrtjevpxr.html

Ruby: // 手写 Hash
来源：http://hz.ydzc1.top/gtyphykdtz.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.chenjidiqi.icu/gtnaimzfrq.html

[N08] 生成全排列
来源：http://hz.wangshuangyany.cn/gthexgpyxl.html

Py:   itertools.permutations(arr)
来源：http://hz.xingfuxueyuan.xyz/gtlitpuxtu.html

PHP:  // 手写递归交换
来源：http://hz.jinyuanbaomall.cn/gtdqwzcylu.html

JS:   // 手写回溯递归
来源：http://hz.hfpthk.cn/gtnwmrhgci.html

TS:   // 手写回溯递归
来源：http://hz.zhengqikj.top/gtcppdcmuz.html

Java: // 手写回溯递归
来源：http://hz.feifeiyinyue.top/gtkwvbhump.html

Go:   // 手写回溯递归
来源：http://hz.zdqjudy.top/gtzhmvaljv.html

Ruby: arr.permutation.to_a
来源：http://hz.yvedp.cn/gtvdzoacsu.html

C#:   // 手写回溯递归
来源：http://hz.52xcode.cn/gtwwzdxclx.html

[N09] 栈与队列
来源：http://hz.meibo888.top/gtzwmgemjk.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.ehwqpu.com/gtiqyxwdan.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.xingfuxueyuan.xyz/gthrwatvce.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.yuanzhike.top/gtxhfngiut.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.iojbl.cn/gthcgsfzik.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.zycfv.cn/gtfvqtxwlb.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.yonumen.top/gtvsqfvdww.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.jiagoushi.top/gtwfdesrmt.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.aizwys.cn/gtljsppnyw.html

[N10] 链表节点定义
来源：http://hz.xylfe.cn/gtlmrmhplk.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.yonumen.top/gtvuekmqrd.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.jianghu66.top/gtrmddxrbx.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.shangyingyoupin.top/gtdgmlttcz.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.yongpay.top/gtxkesztuv.html

Java: class Node { int v; Node next; }
来源：http://hz.jianghu66.top/gtcmtyzyxy.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.bjfxy.top/gtnbjhpcmg.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.gotoacloud.top/gtgrpktwju.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.zycfv.cn/gtbuiachwd.html

[N11] 二叉树中序遍历
来源：http://hz.yj20258.top/gtzfdgsanf.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.tianlin.xyz/gtfopgatgs.html

PHP:  // 手写递归函数
来源：http://hz.andypj.xyz/gtfkwjzilu.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.kuanghao11.cn/gtkdyisjpu.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.redwolf501.top/gtyozubroj.html

Java: // 手写递归
来源：http://hz.zycfv.cn/gtqunuvdbt.html

Go:   // 手写递归
来源：http://hz.birdmap.top/gtpyulowev.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.ydzc1.top/gtxkzndpan.html

C#:   // 手写递归
来源：http://hz.52xcode.cn/gtvkljpzpm.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.ivvv.top/gtqkisdmdz.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.ydjk.org.cn/gtqugtgxxa.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.jqgfzy.top/gtuzoqhnqq.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.gotoacloud.top/gtenwmoxob.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.xinyue.icu/gtcvqqdsum.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.dashuyun.cn/gtghvfsvwj.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.zhixingplan.top/gtgkkshpga.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.sufxvd.cn/gtibvhueby.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.nanxinkj.top/gtgqpcoigr.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtkjdlwnov.html

O. 并发与异步
来源：http://hz.cashguo.top/gtomwvsjxk.html

================================================================================
来源：http://hz.nanxinkj.top/gtwbjkgvug.html

[O01] 启动一个线程
来源：http://hz.snrcjt.cn/gtuongorsw.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.redwolf501.top/gtfkkvbbfb.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.dianchejie.cn/gtrkyydgwo.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.xziqi.cn/gtrislcvvs.html

TS:   // 同 JS
来源：http://hz.iojbl.cn/gtnllujsze.html

Java: new Thread(() -> f()).start()
来源：http://hz.ivvv.top/gtiggurfba.html

Go:   go f()
来源：http://hz.zhijiandao.cn/gtzaoqnopx.html

Ruby: Thread.new { f }
来源：http://hz.haohaochexian.top/gthfvuafzd.html

C#:   Task.Run(() => F());
来源：http://hz.shuidangran.top/gtmvnsattj.html

[O02] 使用线程池
来源：http://hz.zycfv.cn/gtafadmtqv.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.xingfuxueyuan.xyz/gtzgopflhf.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.yuanzhike.top/gtrdwrcokq.html

JS:   // worker_threads 线程池
来源：http://hz.cucudq.cn/gtawhrykug.html

TS:   // worker_threads 线程池
来源：http://hz.yvedp.cn/gtttnukinv.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.cashguo.top/gtrxhjjbpy.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.yvedp.cn/gtiaekernx.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.svipenyu.cn/gtrplyglre.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.cheryme.top/gtespcfvlt.html

[O03] 加锁保护共享数据
来源：http://hz.xuanzx.com/gttkhylqjh.html

Py:   with lock: shared += 1
来源：http://hz.daxiang520.top/gtmuumcyoo.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.fzhhl.top/gtspmugxkc.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.chenjidiqi.icu/gtdnikzbgc.html

TS:   // 同 JS
来源：http://hz.meibo888.top/gtlvuuezdj.html

Java: synchronized (this) { shared++; }
来源：http://hz.hysaishi.cn/gtbabkwmgp.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.jiagoushi.top/gtmkclyekm.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.hfpthk.cn/gtoknrlloe.html

C#:   lock (gate) { shared++; }
来源：http://hz.jinqigufen.top/gtkhxbvfha.html

[O04] 定义异步函数并等待
来源：http://hz.dianchejie.cn/gtiidiwzaa.html

Py:   async def f():⏎    await g()
来源：http://hz.kuanghao11.cn/gtegcivouj.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.yonumen.top/gtqouxaziv.html

JS:   async function f() { await g(); }
来源：http://hz.feifeiyinyue.top/gtgwzbtzkc.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.hnqzz.top/gtqfiemaqx.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.cqqwz.cn/gtppmvewfv.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.zhijiandao.cn/gtdxkbrwyr.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.gogol.net.cn/gtroqreoou.html

C#:   async Task F() { await G(); }
来源：http://hz.andypj.xyz/gtwtbhjpux.html

[O05] 并发执行并等待全部完成
来源：http://hz.aibaodan.cn/gthsvscpmf.html

Py:   asyncio.gather(*tasks)
来源：http://hz.zhaomingkeji.xyz/gttpxrwsup.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.zdqjudy.top/gtzelxjfmw.html

JS:   await Promise.all(tasks)
来源：http://hz.xziqi.cn/gtituabmgf.html

TS:   await Promise.all(tasks)
来源：http://hz.yonumen.top/gtkjttztnu.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.pycfn.com/gtzstgovym.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.shzxlz.cn/gtxnafgdbq.html

Ruby: threads.map(&:join)
来源：http://hz.hongshengwenyu.top/gthbfsxbct.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.xylfe.cn/gteoevzuty.html

[O06] 使用进程池
来源：http://hz.dianchejie.cn/gtfedwrruq.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.gaohongyu789.top/gtabfdwhgf.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.tanke756.top/gtldaopvgt.html

JS:   // child_process / cluster 模块
来源：http://hz.jlsjyb.cn/gtqagqyswn.html

TS:   // child_process / cluster 模块
来源：http://hz.yj20258888.top/gtzlcqzdlx.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.yvedp.cn/gtqtjsuucg.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.yvedp.cn/gtcfevbgfo.html

Ruby: // fork 块
来源：http://hz.feifeiyinyue.top/gtxvmxifqu.html

C#:   Parallel.For
来源：http://hz.jinghuilouyu.cn/gtvpdwdfxd.html

================================================================================
来源：http://hz.xinyue.icu/gthhtxjaed.html

P. 常用工具函数
来源：http://hz.snrcjt.cn/gtfuacgsxv.html

================================================================================
来源：http://hz.yuxming.cn/gtzhqoagwe.html

[P01] 生成 UUID
来源：http://hz.cheryme.top/gtjhwltpcp.html

Py:   str(uuid.uuid4())
来源：http://hz.sxryk.cn/gtarogiieb.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.daria6918.cn/gtdyzfqgde.html

JS:   crypto.randomUUID()
来源：http://hz.yonumen.top/gtwmgyukpm.html

TS:   crypto.randomUUID()
来源：http://hz.sxryk.cn/gtfwckmbwe.html

Java: UUID.randomUUID().toString()
来源：http://hz.tianlin.xyz/gtfnrutedu.html

Go:   // 用 github.com/google/uuid
来源：http://hz.kuanghao11.cn/gtiiqbzmfu.html

Ruby: SecureRandom.uuid
来源：http://hz.cheryme.top/gtzmtxynoc.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.gotoacloud.top/gtiyqrhcmj.html

[P02] MD5 / SHA256 摘要
来源：http://hz.vqdsnc.cn/gtqxcbfidp.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.dashuyun.cn/gtycqhvtfh.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.aizwys.cn/gtmzavhuxn.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.tanke756.top/gtwwoglcjh.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.xziqi.cn/gtbcuiwmjq.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.wangdashe.top/gttidcdyok.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.yj20258.top/gtazjmdszg.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.cqqwz.cn/gtmldclejs.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.cdnleiting.top/gthmaijbnx.html

[P03] 生成短随机字符串
来源：http://hz.bjfxy.top/gtagojifuq.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.birdmap.top/gtuxgbfmln.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.jianghu66.top/gtlnzztyty.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.gotoacloud.top/gtgctxxgqn.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.zhongyouzk.top/gteaeeodwb.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.yangfankeji.com/gtavnxexep.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.daxiang520.top/gtnuxxyxjv.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.wangdashe.top/gtjmriprdc.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.hammf.cn/gtynytnejk.html

[P04] 求长度
来源：http://hz.jinqigufen.top/gtjrqtztjk.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.chenlongwang.top/gtiriptdeh.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.svipenyu.cn/gtqemoxjbe.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.daria6918.cn/gtwlskuggd.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.sxryk.cn/gtystwsibc.html


<!-- 参考信息 -->