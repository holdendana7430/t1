代发 wailian999

[L07] 处理 HTTP 状态码
来源：http://hz.birdmap.top/gtwzieskna.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.xinyue.icu/gtnnziozam.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.xingfuxueyuan.xyz/gtgvsmfuog.html

JS:   resp.ok;  resp.status
来源：http://hz.chenjidiqi.icu/gthgpfbngp.html

TS:   resp.ok;  resp.status
来源：http://hz.sxryk.cn/gtepqzgylu.html

Java: resp.statusCode()
来源：http://hz.yongpay.top/gtowskhyim.html

Go:   resp.StatusCode
来源：http://hz.ybcxt.top/gtodsvoxnn.html

Ruby: resp.code.to_i
来源：http://hz.bjfxy.top/gtdukokbzd.html

C#:   (int)resp.StatusCode
来源：http://hz.nanxinkj.top/gtlnjrmzag.html

[L08] 并发请求多个地址
来源：http://hz.xingfuxueyuan.xyz/gtdeqguqmz.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.yangfankeji.com/gtupkzlogv.html

PHP:  curl_multi_init() 系列
来源：http://hz.hnqzz.top/gtkcsnevwj.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.gzhubu.top/gthitzofkf.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.daxiang520.top/gtwcurhqmb.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.quarkkingdee.top/gtlitsqhib.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.xuanzx.com/gtrzmmoorx.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.nwbrower.top/gtdudxltem.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.bjfxy.top/gtnonxzxzt.html

================================================================================
来源：http://hz.ivvv.top/gtrraiccbj.html

M. 命令行 / 进程 / 环境
来源：http://hz.andypj.xyz/gtryqioswy.html

================================================================================
来源：http://hz.c1oappe.top/gteupphbva.html

[M01] 读取命令行参数
来源：http://hz.cheryme.top/gtqzyixyqd.html

Py:   sys.argv[1:]
来源：http://hz.52xcode.cn/gtdpakzoof.html

PHP:  $argv;  $argc;
来源：http://hz.zhengqikj.top/gtlulyjhtq.html

JS:   process.argv.slice(2)
来源：http://hz.jlsjyb.cn/gtltouenwy.html

TS:   process.argv.slice(2)
来源：http://hz.tanke756.top/gtnzaqxmfx.html

Java: args 数组（main 方法参数）
来源：http://hz.jiagoushi.top/gtjoydqgxc.html

Go:   os.Args[1:]
来源：http://hz.tian-w.cn/gtlkpfmsaf.html

Ruby: ARGV
来源：http://hz.meibo888.top/gtrqwqwwth.html

C#:   args 数组（Main 方法参数）
来源：http://hz.tianlin.xyz/gtoqrfplhm.html

[M02] 读取环境变量
来源：http://hz.vqdsnc.cn/gtxwnuynlu.html

Py:   os.environ.get("HOME")
来源：http://hz.dashuyun.cn/gtzmenhgdg.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.jiagoushi.top/gtxfcpkhwr.html

JS:   process.env.HOME
来源：http://hz.yanxiufei.cn/gtxgtgamic.html

TS:   process.env.HOME
来源：http://hz.gzhubu.top/gtxxprcmuc.html

Java: System.getenv("HOME")
来源：http://hz.yongpay.top/gtcqhpmmlj.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.jiagoushi.top/gtrjvtsovh.html

Ruby: ENV["HOME"]
来源：http://hz.hammf.cn/gtphxeythj.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.fengsongda.top/gtdzikjpkx.html

[M03] 执行外部命令
来源：http://hz.wangshuangyany.cn/gtdirnwgop.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.ppjwa.cn/gtpwzbljrb.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.chenjidiqi.icu/gtfbsazmdz.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.tianlin.xyz/gtjowpbkia.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.yuxming.cn/gtlewlkorm.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.zhixingplan.top/gtwsgtkbqg.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.xuanzx.com/gtxjumcitk.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.dashuyun.cn/gtjsyyiucb.html

C#:   Process.Start("ls", "-l");
来源：http://hz.zhiwuduotai.top/gtzhpjdzij.html

[M04] 获取当前工作目录
来源：http://hz.fzhhl.top/gtflerzkqs.html

Py:   os.getcwd()
来源：http://hz.hfpthk.cn/gteynxozqt.html

PHP:  getcwd();
来源：http://hz.ehwqpu.com/gtuwurdvzh.html

JS:   process.cwd()
来源：http://hz.zhixingplan.top/gtwvbqikwt.html

TS:   process.cwd()
来源：http://hz.zhongyouzk.top/gtkjikomaw.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.yj20258888.top/gtyzuanyol.html

Go:   os.Getwd()
来源：http://hz.zycfv.cn/gthavxfrim.html

Ruby: Dir.pwd
来源：http://hz.hongshengwenyu.top/gtsgzkzowa.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.meibo888.top/gtfxqqolnx.html

[M05] 设置退出码
来源：http://hz.hammf.cn/gtrbxhiayd.html

Py:   sys.exit(1)
来源：http://hz.nanxinkj.top/gtujuiivlu.html

PHP:  exit(1);
来源：http://hz.havefunace.top/gtllxxkdej.html

JS:   process.exit(1)
来源：http://hz.yonumen.top/gtfceqmumo.html

TS:   process.exit(1)
来源：http://hz.jqgufenzy.top/gtnhqzfnkk.html

Java: System.exit(1)
来源：http://hz.hysaishi.cn/gtyckhblrz.html

Go:   os.Exit(1)
来源：http://hz.yj20258.top/gtoptfozyb.html

Ruby: exit 1
来源：http://hz.birdmap.top/gtfscommpf.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.sysykeji.top/gtpmpmukdl.html

[M06] 向标准错误输出
来源：http://hz.feifeiyinyue.top/gttejhqans.html

Py:   print("err", file=sys.stderr)
来源：http://hz.yj20258888.top/gtswxjylus.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.andypj.xyz/gtxbruztsc.html

JS:   console.error("err")
来源：http://hz.guannengcc.top/gtnwqcuigt.html

TS:   console.error("err")
来源：http://hz.zhaomingkeji.xyz/gtimpnlddu.html

Java: System.err.println("err")
来源：http://hz.jyoumei.cn/gtoenelecn.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.tianlin.xyz/gtbowvrxyp.html

Ruby: warn "err"
来源：http://hz.jianghu66.top/gtyqiwpkdq.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.shanyushiyangtech.top/gtyrazdeur.html

[M07] 判断是否为主入口
来源：http://hz.daria6918.cn/gtwsgfzcig.html

Py:   if __name__ == "__main__":
来源：http://hz.xuanzx.com/gtphfbfwlg.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.tianlin.xyz/gtyuclyrqw.html

JS:   require.main === module
来源：http://hz.jinghuilouyu.cn/gtrrribzir.html

TS:   require.main === module
来源：http://hz.yongpay.top/gtxgbkedpt.html

Java: public static void main(String[] args)
来源：http://hz.zhiwuduotai.top/gtgtfrinsp.html

Go:   func main()
来源：http://hz.jianghu66.top/gtbpkaqnvc.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.cqqwz.cn/gtzpatyago.html

C#:   static void Main(string[] args)
来源：http://hz.hywenlv.cn/gtgrilbily.html

[M08] 获取系统与运行时信息
来源：http://hz.cdnleiting.top/gtahdsjzdk.html

Py:   platform.system();  platform.python_version()
来源：http://hz.tian-w.cn/gtdrfpzufv.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.jianghu66.top/gtfizqcjrb.html

JS:   process.platform;  process.version
来源：http://hz.jinqigufen.top/gtfdwacuwi.html

TS:   process.platform;  process.version
来源：http://hz.cdnleiting.top/gtmvxpdxrf.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.aizwys.cn/gtqtlizmfc.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.havefunace.top/gtjbsypybe.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.jianghu66.top/gtpjndvyfn.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.jinyuanbaomall.cn/gtvhmltycb.html

================================================================================
来源：http://hz.yanxiufei.cn/gtqsvorzae.html

N. 数据结构与算法
来源：http://hz.0kj1m.cn/gtyqqttpsl.html

================================================================================
来源：http://hz.gogol.net.cn/gtxjzsvkdz.html

[N01] 二分查找（有序数组）
来源：http://hz.hysaishi.cn/gtuimqpxcd.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.chenzaomai.com/gtrdqzyyxf.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.birdmap.top/gtnbmgumay.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.nanxinkj.top/gtsqbdtsgz.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.ehwqpu.com/gtlhhipeqm.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.gzhubu.top/gtdjpnmrza.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.ehwqpu.com/gttfwvymwj.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.ydzc1.top/gtilczsyhg.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.pycfn.com/gtwlmjycri.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.haohaochexian.top/gthxwkojsj.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.hfpthk.cn/gtgkomsomy.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.jqgfzy.top/gtzeejtsyc.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.pengpengdd.cyou/gtyzftaqlz.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.hammf.cn/gtfostgwtu.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.316326.xyz/gtteylxmfp.html

Go:   slices.Sort(arr)
来源：http://hz.chenlongwang.top/gtdidcmskb.html

Ruby: arr.sort
来源：http://hz.kuanghao11.cn/gtzfllklbg.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.gaohongyu789.top/gtmktogosd.html

[N03] 快速排序（分治示例）
来源：http://hz.quarkkingdee.top/gtcljcoslu.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.cqqwz.cn/gtqnahhnub.html

PHP:  // 递归实现，或用 usort
来源：http://hz.dashuyun.cn/gtnffgxumf.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.dianchejie.cn/gtevzgljay.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zhixingplan.top/gtjmylwava.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.quarkkingdee.top/gtbxtbeaxk.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.quarkkingdee.top/gtcqakhsiu.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.yonumen.top/gtmmykmomc.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.tianlin.xyz/gtiisxqqab.html

[N04] 斐波那契数列
来源：http://hz.cqqwz.cn/gtjuupjhwp.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.yanxiufei.cn/gtgyqpxhiw.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.316326.xyz/gtejezyvrc.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.feifeiyinyue.top/gtutivrpiy.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.xylfe.cn/gtsvmsegzt.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.feifeiyinyue.top/gtzrxzjyde.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.yuanzhike.top/gtnyuzuney.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.nanxuanxn.top/gtxpvzeheu.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.dashuyun.cn/gtgwajxllk.html

[N05] 最大公约数
来源：http://hz.hysaishi.cn/gtqozvumgv.html

Py:   math.gcd(a, b)
来源：http://hz.chenzaomai.com/gtyjkrrphb.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.yanxiufei.cn/gtwdxqtnge.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.birdmap.top/gtyqolqvcr.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jqgufenzy.top/gtmawnclaa.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.hfpthk.cn/gtszrdlkgf.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.yonumen.top/gtckwiowuv.html

Ruby: a.gcd(b)
来源：http://hz.guannengcc.top/gtwgoeheiu.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.cucudq.cn/gtcsmyllwu.html

[N06] 判断回文字符串
来源：http://hz.hfpthk.cn/gtjugyoens.html

Py:   s == s[::-1]
来源：http://hz.9152youxi.cn/gtvjunzcpk.html

PHP:  $s === strrev($s);
来源：http://hz.xuetiantiany.cn/gtoeiaplle.html

JS:   s === [...s].reverse().join("")
来源：http://hz.guannengcc.top/gtfdzfhmdd.html

TS:   s === [...s].reverse().join("")
来源：http://hz.pycfn.com/gtsmhluzki.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.hongshengwenyu.top/gtbjxchebc.html

Go:   // 双指针从两端比较
来源：http://hz.mhx1999.top/gtqimdgzzu.html

Ruby: s == s.reverse
来源：http://hz.birdmap.top/gtexgbdpgt.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.snrcjt.cn/gtfoherpfd.html

[N07] 两数之和（返回下标）
来源：http://hz.jyoumei.cn/gtnsqwwpte.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.cucudq.cn/gtxkqsgmiq.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.daria6918.cn/gtqijqijhj.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.ybcxt.top/gtbxoruztl.html

TS:   // 手写 Map<string, number>
来源：http://hz.shzxlz.cn/gtudxkjfhf.html

Java: // 手写 HashMap
来源：http://hz.ybcxt.top/gtirxyuoev.html

Go:   // 手写 map[int]int
来源：http://hz.guowangkeji.top/gtphwkgpix.html

Ruby: // 手写 Hash
来源：http://hz.ehwqpu.com/gtvnvlxtzb.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.jiagoushi.top/gtxvrpwldy.html

[N08] 生成全排列
来源：http://hz.ywan-chungtsiang.top/gtlvfpvlyt.html

Py:   itertools.permutations(arr)
来源：http://hz.gogol.net.cn/gtlipdnsag.html

PHP:  // 手写递归交换
来源：http://hz.guowangkeji.top/gtuzqpgvde.html

JS:   // 手写回溯递归
来源：http://hz.sufxvd.cn/gtnhgbnalw.html

TS:   // 手写回溯递归
来源：http://hz.yangfankeji.com/gtduvnpktj.html

Java: // 手写回溯递归
来源：http://hz.daxiang520.top/gtrlzmtmhi.html

Go:   // 手写回溯递归
来源：http://hz.xinyue.icu/gtpvrqjivj.html

Ruby: arr.permutation.to_a
来源：http://hz.meibo888.top/gttkwoqshh.html

C#:   // 手写回溯递归
来源：http://hz.fzhhl.top/gtzfxocmuh.html

[N09] 栈与队列
来源：http://hz.yanxiufei.cn/gtgtysvpoq.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.zhixingplan.top/gtecyulbca.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.jinqigfzy.top/gttttgozmj.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.nwbrower.top/gtkoxqylmh.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.yj202588.top/gthjrwvgkj.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.jinyuanbaomall.cn/gtgtewbgmz.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.jyoumei.cn/gtjhwhdnmk.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.c1oappe.top/gtcngtjgno.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.cucudq.cn/gtpfwqwxcx.html

[N10] 链表节点定义
来源：http://hz.ywan-chungtsiang.top/gtyeypxcww.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.meibo888.top/gtnrtzdeop.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.jinyuanbaomall.cn/gtpvbgjxbd.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.jinqigufen.top/gtuuczftrb.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.tanke756.top/gtabavinkq.html

Java: class Node { int v; Node next; }
来源：http://hz.nanxinkj.top/gtcoakusul.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.cdnleiting.top/gtrzvgbows.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.xingfuxueyuan.xyz/gtulggydtm.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.meibo888.top/gtdriegjdi.html

[N11] 二叉树中序遍历
来源：http://hz.hfpthk.cn/gtyzhyrhru.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.kuanghao11.cn/gtzoisjicv.html

PHP:  // 手写递归函数
来源：http://hz.hfpthk.cn/gtictpwdqo.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.tian-w.cn/gtjsclgfic.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.ivvv.top/gtmeqqxmqq.html

Java: // 手写递归
来源：http://hz.zhoulong.xyz/gttxfgzjqc.html

Go:   // 手写递归
来源：http://hz.ywan-chungtsiang.top/gtzxbckevq.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.yonumen.top/gtcpmyardi.html

C#:   // 手写递归
来源：http://hz.zdqjudy.top/gtteeqzumm.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.dashuyun.cn/gtyiewkaqw.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.redwolf501.top/gtsyvqrsej.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.yueranfly.top/gtmbbgtvmt.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.cucudq.cn/gtuddkfzuu.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yj20258.top/gtggnkscge.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.jinyuanbaomall.cn/gtdwngvhor.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.yonumen.top/gtlztjzena.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.nwbrower.top/gtfhjcgenm.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.fengsongda.top/gtwdlthczf.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtuceehzxj.html

O. 并发与异步
来源：http://hz.chenjidiqi.icu/gtuhjlglgw.html

================================================================================
来源：http://hz.xinyue.icu/gtcbhtuauv.html

[O01] 启动一个线程
来源：http://hz.jinghuilouyu.cn/gtddzeejjn.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.jinqigufen.top/gtujiqpywz.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.pengpengdd.cyou/gtyqyzgeno.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.52xcode.cn/gtbwspgxde.html

TS:   // 同 JS
来源：http://hz.hnqzz.top/gtmdkeotmb.html

Java: new Thread(() -> f()).start()
来源：http://hz.quarkkingdee.top/gtcqvvyofy.html

Go:   go f()
来源：http://hz.cheryme.top/gtjfoznbwj.html

Ruby: Thread.new { f }
来源：http://hz.andypj.xyz/gtnqfizpsv.html

C#:   Task.Run(() => F());
来源：http://hz.smart0.xyz/gtwbhclbvu.html

[O02] 使用线程池
来源：http://hz.hammf.cn/gtjuxgzvlj.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.ywan-chungtsiang.top/gtcphpyzcc.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.wangdashe.top/gthjmoayki.html

JS:   // worker_threads 线程池
来源：http://hz.hfpthk.cn/gtffcborxx.html

TS:   // worker_threads 线程池
来源：http://hz.jinqigfzy.top/gtclywhdvb.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.chenlongwang.top/gtkfldbhlg.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.ybcxt.top/gtrzjkicvt.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.jlsjyb.cn/gtmjhmevks.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.sxryk.cn/gtkhnicuwl.html

[O03] 加锁保护共享数据
来源：http://hz.jianghu66.top/gtmvzszhgk.html

Py:   with lock: shared += 1
来源：http://hz.sweek.top/gtpjhaynyq.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.pengpengdd.cyou/gtekqeupev.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.zdqjudy.top/gtakjrhsey.html

TS:   // 同 JS
来源：http://hz.dianchejie.cn/gtfifsjrxv.html

Java: synchronized (this) { shared++; }
来源：http://hz.yj20258.top/gtfljwjokn.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.chenjidiqi.icu/gtwcjzcakq.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.cqqwz.cn/gtzzgookqs.html

C#:   lock (gate) { shared++; }
来源：http://hz.hysaishi.cn/gtucntvuqy.html

[O04] 定义异步函数并等待
来源：http://hz.zhongyouzk.top/gtpplyyovk.html

Py:   async def f():⏎    await g()
来源：http://hz.yj20258888.top/gtyfygycdj.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.gotoacloud.top/gttetndquo.html

JS:   async function f() { await g(); }
来源：http://hz.zhiwuduotai.top/gtkrfipzxu.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.zhengqikj.top/gtnuhaamus.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.sufxvd.cn/gtzfxcjzdd.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.yuxming.cn/gtyjzbwnqq.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.sxryk.cn/gtapitfkse.html

C#:   async Task F() { await G(); }
来源：http://hz.gogol.net.cn/gtmhpfgcns.html

[O05] 并发执行并等待全部完成
来源：http://hz.yanxiufei.cn/gtsextlmzv.html

Py:   asyncio.gather(*tasks)
来源：http://hz.snrcjt.cn/gtzhtjvfxe.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.tian-w.cn/gtmdvtuihh.html

JS:   await Promise.all(tasks)
来源：http://hz.cucudq.cn/gtlqulrpis.html

TS:   await Promise.all(tasks)
来源：http://hz.yuanzhike.top/gtcoksfsnk.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.ivvv.top/gtmpbsnqwg.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.jinqigufen.top/gttvltnmrb.html

Ruby: threads.map(&:join)
来源：http://hz.ydjk.org.cn/gtjswhyzap.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.daria6918.cn/gtyvlxacvy.html

[O06] 使用进程池
来源：http://hz.nanxinkj.top/gtvihtqkdh.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.redwolf501.top/gtgitvihdu.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.yj202588.top/gtvzcujlze.html

JS:   // child_process / cluster 模块
来源：http://hz.nwbrower.top/gtgxnfvgzs.html

TS:   // child_process / cluster 模块
来源：http://hz.316326.xyz/gtajjarogk.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.yanxiufei.cn/gtcgwjpwmr.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.fzhhl.top/gtumpkygbo.html

Ruby: // fork 块
来源：http://hz.zhaomingkeji.xyz/gtjiybtndt.html

C#:   Parallel.For
来源：http://hz.guannengcc.top/gtpcpryrsy.html

================================================================================
来源：http://hz.dianchejie.cn/gtkkxcqbsh.html

P. 常用工具函数
来源：http://hz.daxiang520.top/gtxnlbqjid.html

================================================================================
来源：http://hz.hnqzz.top/gtfrqmqmkj.html

[P01] 生成 UUID
来源：http://hz.zhengqikj.top/gtplpqwbqz.html

Py:   str(uuid.uuid4())
来源：http://hz.sxryk.cn/gtqgsxfbaa.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.dashuyun.cn/gtdbfbacqh.html

JS:   crypto.randomUUID()
来源：http://hz.yj20258.top/gtzwfgiajw.html

TS:   crypto.randomUUID()
来源：http://hz.hnxiangtu.top/gtjkhwaqmy.html

Java: UUID.randomUUID().toString()
来源：http://hz.jianghu66.top/gtxrisnvwp.html

Go:   // 用 github.com/google/uuid
来源：http://hz.guowangkeji.top/gtvsbbrprb.html

Ruby: SecureRandom.uuid
来源：http://hz.shanyushiyangtech.top/gtxcppfzup.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.pengpengdd.cyou/gtahuatgke.html

[P02] MD5 / SHA256 摘要
来源：http://hz.hysaishi.cn/gtgvwzuzci.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.wangshuangyany.cn/gtrzypucwd.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.bjfxy.top/gtzgdmtupk.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.nanxuanxn.top/gttxlqgafl.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.cdnleiting.top/gtvvqqbfub.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.guannengcc.top/gtduspmimx.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.316326.xyz/gtnkjxaqsd.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.haohaochexian.top/gtekgckqhd.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.shanyushiyangkeji.top/gtaxsvypoi.html

[P03] 生成短随机字符串
来源：http://hz.chenzaomai.com/gtewwkbyjh.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.xingfuxueyuan.xyz/gtzflcgtkq.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.shangyingyoupin.top/gtzyyktjph.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.guowangkeji.top/gtklajglxn.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.zhiwuduotai.top/gtzpbcklkx.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.shanyushiyangkeji.top/gtgjmzlnaj.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.cdnleiting.top/gtxxkbjrpk.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.yvedp.cn/gtvitkhhuk.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.shzxlz.cn/gtjkhmmibi.html

[P04] 求长度
来源：http://hz.sweek.top/gtvalepawd.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hz.ivvv.top/gtdwordpnm.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.vqdsnc.cn/gtrivaimsl.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.birdmap.top/gtietvqhjt.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hz.shanyushiyangtech.top/gtkvypaflk.html

Java: list.size();  map.size();  s.length()
来源：http://hz.xziqi.cn/gtlsmdafpw.html

Go:   len(arr);  len(m)
来源：http://hz.yj202588.top/gtftguznvx.html

Ruby: x.length;  x.size
来源：http://hz.c1oappe.top/gtrphbncii.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://hz.gzhubu.top/gtbyuvmecb.html


<!-- 参考信息 -->