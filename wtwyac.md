代发 wailian999

Py:   resp.json()
来源：http://hz.andypj.xyz/gtfubwppnz.html

PHP:  json_decode($body, true);
来源：http://hz.cdnleiting.top/gtysulkhpi.html

JS:   await resp.json()
来源：http://hz.316326.xyz/gtodlayeeb.html

TS:   await resp.json()
来源：http://hz.hammf.cn/gtfygfyseb.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.chenjidiqi.icu/gtzjzlduvk.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.jqgufenzy.top/gtwtynqcss.html

Ruby: JSON.parse(resp.body)
来源：http://hz.gotoacloud.top/gtlcdnirxo.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.9152youxi.cn/gtqvyjklpj.html

[L07] 处理 HTTP 状态码
来源：http://hz.hnxiangtu.top/gtugpndalx.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.zhengqikj.top/gtpeoyvoca.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.aibaodan.cn/gthelbnbil.html

JS:   resp.ok;  resp.status
来源：http://hz.wangshuangyany.cn/gtwdrndwok.html

TS:   resp.ok;  resp.status
来源：http://hz.ydzc1.top/gtmilqcstx.html

Java: resp.statusCode()
来源：http://hz.ydzc1.top/gtwbulrtqh.html

Go:   resp.StatusCode
来源：http://hz.andypj.xyz/gtkoayzpjq.html

Ruby: resp.code.to_i
来源：http://hz.svipenyu.cn/gtsdsdfnqw.html

C#:   (int)resp.StatusCode
来源：http://hz.svipenyu.cn/gtylcfuqgz.html

[L08] 并发请求多个地址
来源：http://hz.zhongyouzk.top/gtuiwrisgo.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.aibaodan.cn/gtcpjkrjts.html

PHP:  curl_multi_init() 系列
来源：http://hz.havefunace.top/gtigpxpbyr.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.havefunace.top/gtsivtabnm.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jlsjyb.cn/gtyktuliud.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.haohaochexian.top/gtaphseeui.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.jqgufenzy.top/gtccrmkdcn.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.shanyushiyangtech.top/gttmsuzoyb.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.hnxiangtu.top/gtwihqessk.html

================================================================================
来源：http://hz.xziqi.cn/gtkdwhixdf.html

M. 命令行 / 进程 / 环境
来源：http://hz.hysaishi.cn/gtputuwjer.html

================================================================================
来源：http://hz.cdnleiting.top/gtweckgnem.html

[M01] 读取命令行参数
来源：http://hz.hnqzz.top/gtwrhekjem.html

Py:   sys.argv[1:]
来源：http://hz.zycfv.cn/gtrvbadtfg.html

PHP:  $argv;  $argc;
来源：http://hz.9152youxi.cn/gthmxmglbb.html

JS:   process.argv.slice(2)
来源：http://hz.ivvv.top/gtflllhvjx.html

TS:   process.argv.slice(2)
来源：http://hz.yuanzhike.top/gtrpwypaiy.html

Java: args 数组（main 方法参数）
来源：http://hz.jianghu66.top/gthhlsnxop.html

Go:   os.Args[1:]
来源：http://hz.andypj.xyz/gtwxzbdyeu.html

Ruby: ARGV
来源：http://hz.daria6918.cn/gtrulorcnl.html

C#:   args 数组（Main 方法参数）
来源：http://hz.yj20258.top/gtouthtlwp.html

[M02] 读取环境变量
来源：http://hz.feifeiyinyue.top/gtipyitcln.html

Py:   os.environ.get("HOME")
来源：http://hz.gotoacloud.top/gtgndpixzl.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.zhoulong.xyz/gtzrxkpmnk.html

JS:   process.env.HOME
来源：http://hz.yanxiufei.cn/gtwdysbxpk.html

TS:   process.env.HOME
来源：http://hz.gotoacloud.top/gtcyramcew.html

Java: System.getenv("HOME")
来源：http://hz.zhiwuduotai.top/gtmrdcwlsv.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.gzhubu.top/gtbleaezre.html

Ruby: ENV["HOME"]
来源：http://hz.dianchejie.cn/gtazdehdkk.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.havefunace.top/gtuwaegecl.html

[M03] 执行外部命令
来源：http://hz.haohaochexian.top/gtllwdtaoa.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.mhx1999.top/gtapnlpfcy.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.0kj1m.cn/gtgcgpxdbu.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.9152youxi.cn/gtsvovfnuj.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.jinyuanbaomall.cn/gtzsrumqcn.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.jlsjyb.cn/gtbmsfrbrl.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.pengpengdd.cyou/gtijnpdkel.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.zhijiandao.cn/gtqxwjrurv.html

C#:   Process.Start("ls", "-l");
来源：http://hz.daria6918.cn/gtvjzqkjjg.html

[M04] 获取当前工作目录
来源：http://hz.yuanzhike.top/gtgpfodhwo.html

Py:   os.getcwd()
来源：http://hz.havefunace.top/gtnpbhuygm.html

PHP:  getcwd();
来源：http://hz.gogol.net.cn/gthjhonutt.html

JS:   process.cwd()
来源：http://hz.tianlin.xyz/gtjdmqoemj.html

TS:   process.cwd()
来源：http://hz.jlsjyb.cn/gtqawupfbh.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.sweek.top/gtxjsuxnoc.html

Go:   os.Getwd()
来源：http://hz.pycfn.com/gtiuhavxwd.html

Ruby: Dir.pwd
来源：http://hz.wangshuangyany.cn/gtluhvplnc.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.xingfuxueyuan.xyz/gtenzsekuq.html

[M05] 设置退出码
来源：http://hz.nwbrower.top/gtkcqlsrhg.html

Py:   sys.exit(1)
来源：http://hz.tanke756.top/gtrduuzawx.html

PHP:  exit(1);
来源：http://hz.yongpay.top/gthmjxbypj.html

JS:   process.exit(1)
来源：http://hz.jqgfzy.top/gttuvqoeqr.html

TS:   process.exit(1)
来源：http://hz.havefunace.top/gtqbmxgnbj.html

Java: System.exit(1)
来源：http://hz.svipenyu.cn/gtktqhwzml.html

Go:   os.Exit(1)
来源：http://hz.fengsongda.top/gtnvjqejyi.html

Ruby: exit 1
来源：http://hz.xziqi.cn/gtxztnoxtc.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.ybcxt.top/gtaqnizzxw.html

[M06] 向标准错误输出
来源：http://hz.iojbl.cn/gtnsjtivxh.html

Py:   print("err", file=sys.stderr)
来源：http://hz.pengpengdd.cyou/gtpnovpyov.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.hywenlv.cn/gtoojglhok.html

JS:   console.error("err")
来源：http://hz.ivvv.top/gtypkwgvha.html

TS:   console.error("err")
来源：http://hz.bjfxy.top/gtvpungiks.html

Java: System.err.println("err")
来源：http://hz.fzhhl.top/gtavngtwex.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.yvedp.cn/gtswdgffuk.html

Ruby: warn "err"
来源：http://hz.bjfxy.top/gthkjdtqhx.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.xuetiantiany.cn/gtrvbrqoao.html

[M07] 判断是否为主入口
来源：http://hz.hysaishi.cn/gtkgolyyru.html

Py:   if __name__ == "__main__":
来源：http://hz.hysaishi.cn/gtjveccztp.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.vqdsnc.cn/gtmxrencid.html

JS:   require.main === module
来源：http://hz.hfpthk.cn/gtxkvjefyr.html

TS:   require.main === module
来源：http://hz.nwbrower.top/gtpktalske.html

Java: public static void main(String[] args)
来源：http://hz.jianghu66.top/gtmxpzflaq.html

Go:   func main()
来源：http://hz.andypj.xyz/gtafoxlguo.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.guowangkeji.top/gtqehpstfb.html

C#:   static void Main(string[] args)
来源：http://hz.gogol.net.cn/gtrmfnqxnc.html

[M08] 获取系统与运行时信息
来源：http://hz.pycfn.com/gtumvmkaye.html

Py:   platform.system();  platform.python_version()
来源：http://hz.guowangkeji.top/gtquyhjcrz.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.yangfankeji.com/gtcliuovmf.html

JS:   process.platform;  process.version
来源：http://hz.52xcode.cn/gtpipvgrbd.html

TS:   process.platform;  process.version
来源：http://hz.hysaishi.cn/gtigbjniuj.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.jinqigfzy.top/gtnphgtyeo.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.quarkkingdee.top/gtwsoaonat.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.zhongyouzk.top/gtnkxvllvu.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.zhijiandao.cn/gtvawprjew.html

================================================================================
来源：http://hz.yueranfly.top/gtsxcgrdfh.html

N. 数据结构与算法
来源：http://hz.yanxiufei.cn/gtgjfzeuxw.html

================================================================================
来源：http://hz.fengsongda.top/gtczqdjppx.html

[N01] 二分查找（有序数组）
来源：http://hz.tianlin.xyz/gtpwwfsfei.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.snrcjt.cn/gtboqzpvln.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.ppjwa.cn/gtdoehpcgl.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.quarkkingdee.top/gtnsmocohe.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.meibo888.top/gtjqsbuttv.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.smart0.xyz/gthjflxyam.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.hnqzz.top/gtemvgmbsa.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.hnqzz.top/gttavgvfje.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.shuidangran.top/gtqftdmoeu.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.nanxinkj.top/gtovelvhzz.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.chenjidiqi.icu/gtuoeaclez.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.tanke756.top/gtjzoykyrd.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.haohaochexian.top/gtvdttljio.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jlsjyb.cn/gtrcazosbr.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.guannengcc.top/gtqenveaec.html

Go:   slices.Sort(arr)
来源：http://hz.xziqi.cn/gtmcibkmgu.html

Ruby: arr.sort
来源：http://hz.ivvv.top/gtzqbevibv.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.andypj.xyz/gtdssdmwjp.html

[N03] 快速排序（分治示例）
来源：http://hz.dianchejie.cn/gtljqmvzsj.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.smart0.xyz/gtcilrhgwg.html

PHP:  // 递归实现，或用 usort
来源：http://hz.yangfankeji.com/gtoehlarab.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.gogol.net.cn/gtsalfltwo.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.xylfe.cn/gtpljodiif.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.shanyushiyangkeji.top/gticynqqze.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.316326.xyz/gtzkejbeza.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.sxryk.cn/gtennlxeta.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.shzxlz.cn/gtjtfwvewc.html

[N04] 斐波那契数列
来源：http://hz.chenlongwang.top/gteldacfdc.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.jinyuanbaomall.cn/gtgbufgamf.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.jinyuanbaomall.cn/gtwfkyqdbj.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yangfankeji.com/gtuxriqrgn.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jianghu66.top/gtiogppsep.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.9152youxi.cn/gtyfbnmhki.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.nanxinkj.top/gtavzwejfm.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.iojbl.cn/gtrrooopjk.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.xinyue.icu/gtetbhtdpz.html

[N05] 最大公约数
来源：http://hz.9152youxi.cn/gtaeaoimex.html

Py:   math.gcd(a, b)
来源：http://hz.xuanzx.com/gtjuldbdvm.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.snrcjt.cn/gtxprnbslr.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.guannengcc.top/gtetplmlxu.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.haohaochexian.top/gtvfdghxke.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.shanyushiyangkeji.top/gtrufwcxyj.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.daxiang520.top/gtbzhaepoz.html

Ruby: a.gcd(b)
来源：http://hz.316326.xyz/gtwrvirwya.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.ydzc1.top/gtxoytxnoo.html

[N06] 判断回文字符串
来源：http://hz.chenlongwang.top/gtpatzvbtw.html

Py:   s == s[::-1]
来源：http://hz.yongpay.top/gttbtfqqkb.html

PHP:  $s === strrev($s);
来源：http://hz.quarkkingdee.top/gtembhxvst.html

JS:   s === [...s].reverse().join("")
来源：http://hz.nanxuanxn.top/gtnoopzgem.html

TS:   s === [...s].reverse().join("")
来源：http://hz.zdqjudy.top/gtcjleuvir.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.yvedp.cn/gtewghqsgn.html

Go:   // 双指针从两端比较
来源：http://hz.xziqi.cn/gtygyhhrve.html

Ruby: s == s.reverse
来源：http://hz.nanxuanxn.top/gtfoaetqxi.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.tian-w.cn/gtktruopat.html

[N07] 两数之和（返回下标）
来源：http://hz.fengsongda.top/gtbqkihnbr.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.jinghuilouyu.cn/gtygjglheg.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.sweek.top/gtdamrtdrr.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.gaohongyu789.top/gtkspzoepj.html

TS:   // 手写 Map<string, number>
来源：http://hz.pycfn.com/gtdirvrhrz.html

Java: // 手写 HashMap
来源：http://hz.shanyushiyangtech.top/gttnadlveb.html

Go:   // 手写 map[int]int
来源：http://hz.zhengqikj.top/gtcffggihh.html

Ruby: // 手写 Hash
来源：http://hz.jqgfzy.top/gtfoqyymog.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.yvedp.cn/gtbhpqxotz.html

[N08] 生成全排列
来源：http://hz.cashguo.top/gtybtsfoia.html

Py:   itertools.permutations(arr)
来源：http://hz.shzxlz.cn/gtcoyybrpn.html

PHP:  // 手写递归交换
来源：http://hz.tian-w.cn/gtaxaauwee.html

JS:   // 手写回溯递归
来源：http://hz.hnqzz.top/gtlvvtidco.html

TS:   // 手写回溯递归
来源：http://hz.chenlongwang.top/gttqfhlkkr.html

Java: // 手写回溯递归
来源：http://hz.fzhhl.top/gtjblnbmfj.html

Go:   // 手写回溯递归
来源：http://hz.tian-w.cn/gtqaqpvbte.html

Ruby: arr.permutation.to_a
来源：http://hz.shanyushiyangtech.top/gtixxvlumh.html

C#:   // 手写回溯递归
来源：http://hz.yanxiufei.cn/gtnoqnusgd.html

[N09] 栈与队列
来源：http://hz.ppjwa.cn/gtifijejsa.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.hongshengwenyu.top/gtgmekbqdy.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.guowangkeji.top/gtpeimstwy.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.bjfxy.top/gtkkbmrwlf.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.guowangkeji.top/gtgerovwwe.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.gotoacloud.top/gtsibkmswo.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.birdmap.top/gtsimbjdgz.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.bjfxy.top/gtnrppyuip.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.hysaishi.cn/gtugghwnzs.html

[N10] 链表节点定义
来源：http://hz.hammf.cn/gtdpkjqrul.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.ppjwa.cn/gtukzotdop.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.yuxming.cn/gtwfbkpzvk.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.yueranfly.top/gttjzeelwe.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.tian-w.cn/gtctmbslnw.html

Java: class Node { int v; Node next; }
来源：http://hz.aibaodan.cn/gtemcknsmw.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.dashuyun.cn/gtcupqdmff.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.jyoumei.cn/gtdqhzwtbf.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.xylfe.cn/gtntwaufsm.html

[N11] 二叉树中序遍历
来源：http://hz.chenjidiqi.icu/gtibqjwzyg.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.xingfuxueyuan.xyz/gtehasuusd.html

PHP:  // 手写递归函数
来源：http://hz.ppjwa.cn/gtteachrru.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.guannengcc.top/gtmlcvxyxw.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.ywan-chungtsiang.top/gtpbzzyghh.html

Java: // 手写递归
来源：http://hz.zdqjudy.top/gtivgsblgj.html

Go:   // 手写递归
来源：http://hz.iojbl.cn/gtwfjklcqy.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.wangshuangyany.cn/gtoodsioxa.html

C#:   // 手写递归
来源：http://hz.chenjidiqi.icu/gtllavaeeb.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.dashuyun.cn/gtgldvpmbx.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.guannengcc.top/gtjaiwocgr.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.jinqigufen.top/gtgnvxtyeg.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.chenzaomai.com/gtyksvwvjd.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jyoumei.cn/gtpfijqbkm.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.cdnleiting.top/gtpkkvytzd.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.jianghu66.top/gtjwatplfh.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.hywenlv.cn/gtvlbyhupi.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.fengsongda.top/gtiaxxrtdt.html

================================================================================
来源：http://hz.wangdashe.top/gtfkdeoojj.html

O. 并发与异步
来源：http://hz.birdmap.top/gtukgvauec.html

================================================================================
来源：http://hz.jinqigufen.top/gttavnsksl.html

[O01] 启动一个线程
来源：http://hz.hnxiangtu.top/gtlirztzjl.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.yongpay.top/gtzwfdqgvi.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.zdqjudy.top/gtobswpzfs.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.zhixingplan.top/gtftpfeaac.html

TS:   // 同 JS
来源：http://hz.sysykeji.top/gtppqmhxxd.html

Java: new Thread(() -> f()).start()
来源：http://hz.birdmap.top/gtofbbdfqy.html

Go:   go f()
来源：http://hz.mhx1999.top/gtmxxvrdis.html

Ruby: Thread.new { f }
来源：http://hz.haohaochexian.top/gtyvdidedf.html

C#:   Task.Run(() => F());
来源：http://hz.jinqigfzy.top/gteepxfruz.html

[O02] 使用线程池
来源：http://hz.shzxlz.cn/gtcyksegld.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.c1oappe.top/gtzvbdqcsz.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.feifeiyinyue.top/gtdccjkuht.html

JS:   // worker_threads 线程池
来源：http://hz.ppjwa.cn/gtdgoepeoc.html

TS:   // worker_threads 线程池
来源：http://hz.yonumen.top/gtlftdgxin.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.hammf.cn/gtlykefvxl.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.yj202588.top/gtnhlccqre.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.redwolf501.top/gtfqpitlxj.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.jinqigfzy.top/gtamvskgox.html

[O03] 加锁保护共享数据
来源：http://hz.yj202588.top/gtzvbanjbn.html

Py:   with lock: shared += 1
来源：http://hz.guannengcc.top/gtdhpzhenp.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.gogol.net.cn/gtdjpyebdn.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.vqdsnc.cn/gtmsrwgnmz.html

TS:   // 同 JS
来源：http://hz.yuxming.cn/gtfthkloxy.html

Java: synchronized (this) { shared++; }
来源：http://hz.kuanghao11.cn/gtrdfzdbjx.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.yueranfly.top/gtfybzhjjw.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.c1oappe.top/gtdtuhzsxb.html

C#:   lock (gate) { shared++; }
来源：http://hz.zhongyouzk.top/gtmctupoop.html

[O04] 定义异步函数并等待
来源：http://hz.hammf.cn/gtptlsdznq.html

Py:   async def f():⏎    await g()
来源：http://hz.tian-w.cn/gtksaaduul.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.wangdashe.top/gtydhlukzp.html

JS:   async function f() { await g(); }
来源：http://hz.sufxvd.cn/gthjpksteh.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.shangyingyoupin.top/gtdecftwlx.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.aizwys.cn/gtbfnlujkr.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.hongshengwenyu.top/gtyksrmggm.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.chenjidiqi.icu/gtwlcrmecj.html

C#:   async Task F() { await G(); }
来源：http://hz.shangyingyoupin.top/gtljyozrim.html

[O05] 并发执行并等待全部完成
来源：http://hz.pengpengdd.cyou/gtcraycwni.html

Py:   asyncio.gather(*tasks)
来源：http://hz.jqgfzy.top/gtlpcajovw.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.c1oappe.top/gtyqmectvr.html

JS:   await Promise.all(tasks)
来源：http://hz.daria6918.cn/gtxzmxzing.html

TS:   await Promise.all(tasks)
来源：http://hz.chenjidiqi.icu/gtvbxlypkc.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.andypj.xyz/gtrxwfesmk.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.meibo888.top/gtodvzidhu.html

Ruby: threads.map(&:join)
来源：http://hz.pycfn.com/gtiegtnstj.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.jyoumei.cn/gtqbrgedvf.html

[O06] 使用进程池
来源：http://hz.zycfv.cn/gtavxvvlxp.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.tian-w.cn/gtnhbzavwy.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.zycfv.cn/gtudrwgajg.html

JS:   // child_process / cluster 模块
来源：http://hz.fzhhl.top/gtxnernfix.html

TS:   // child_process / cluster 模块
来源：http://hz.cashguo.top/gtrxqfvssz.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.xingfuxueyuan.xyz/gtbfczhojc.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.feifeiyinyue.top/gttivpmkjs.html

Ruby: // fork 块
来源：http://hz.jlsjyb.cn/gtrmclmmfq.html

C#:   Parallel.For
来源：http://hz.yanxiufei.cn/gtnqgzzpmm.html

================================================================================
来源：http://hz.hnqzz.top/gtzliracaw.html

P. 常用工具函数
来源：http://hz.52xcode.cn/gtxrxkxqpy.html

================================================================================
来源：http://hz.9152youxi.cn/gtgmionbyq.html

[P01] 生成 UUID
来源：http://hz.tanke756.top/gtqzfbwsso.html

Py:   str(uuid.uuid4())
来源：http://hz.birdmap.top/gtdzlxbbin.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.jinyuanbaomall.cn/gtsrxxvkld.html

JS:   crypto.randomUUID()
来源：http://hz.shuidangran.top/gtvfmytejq.html

TS:   crypto.randomUUID()
来源：http://hz.dianchejie.cn/gtnewxgspl.html

Java: UUID.randomUUID().toString()
来源：http://hz.9152youxi.cn/gtxeernhbp.html

Go:   // 用 github.com/google/uuid
来源：http://hz.hongshengwenyu.top/gtphzigkya.html

Ruby: SecureRandom.uuid
来源：http://hz.yj20258.top/gtmveoezic.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.ybcxt.top/gtkqcxulrv.html

[P02] MD5 / SHA256 摘要
来源：http://hz.hywenlv.cn/gtrbkhwyma.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.c1oappe.top/gtbjggfuuz.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.dianchejie.cn/gtjfaukesy.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.tanke756.top/gtulqqydgu.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.quarkkingdee.top/gtfjqieygi.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.cucudq.cn/gttuxsesxc.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.yj20258888.top/gtsmrsxawy.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.c1oappe.top/gtshootgxw.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.shanyushiyangtech.top/gtbhiorjjn.html

[P03] 生成短随机字符串
来源：http://hz.sysykeji.top/gtpmmpyqeg.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.ydzc1.top/gtfhfciomt.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.wangshuangyany.cn/gtosyroxjm.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.ivvv.top/gtojllozhw.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.ppjwa.cn/gtibblidqo.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.ydzc1.top/gtzjqgftrt.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hz.shanyushiyangkeji.top/gtcyfdumnk.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://hz.ybcxt.top/gthwdamucd.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hz.xylfe.cn/gttbbrsvml.html

[P04] 求长度
来源：http://hz.hysaishi.cn/gtoycpktii.html


<!-- 参考信息 -->