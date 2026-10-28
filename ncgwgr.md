代发 wailian999

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.bjfxy.top/gtksknglvy.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.yueranfly.top/gtqenfgtba.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.chenjidiqi.icu/gtfweypmuh.html

[L06] 解析响应为 JSON
来源：http://hz.cdnleiting.top/gterndyjhz.html

Py:   resp.json()
来源：http://hz.jiagoushi.top/gtaswnsxwn.html

PHP:  json_decode($body, true);
来源：http://hz.yj202588.top/gttorfsnux.html

JS:   await resp.json()
来源：http://hz.havefunace.top/gtynnwckzo.html

TS:   await resp.json()
来源：http://hz.wangdashe.top/gtsayqpwjt.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.sufxvd.cn/gtcqbdqknz.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.jlsjyb.cn/gtilqfrfuq.html

Ruby: JSON.parse(resp.body)
来源：http://hz.cheryme.top/gtatcpvbrw.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.dashuyun.cn/gtxfzucggj.html

[L07] 处理 HTTP 状态码
来源：http://hz.tanke756.top/gtmfispifv.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.smart0.xyz/gtxscdrqov.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.yueranfly.top/gtfsxbwdhv.html

JS:   resp.ok;  resp.status
来源：http://hz.gzhubu.top/gtrlmtdjyp.html

TS:   resp.ok;  resp.status
来源：http://hz.iojbl.cn/gthpipujiu.html

Java: resp.statusCode()
来源：http://hz.jianghu66.top/gtyvawygml.html

Go:   resp.StatusCode
来源：http://hz.pengpengdd.cyou/gtzuokcdif.html

Ruby: resp.code.to_i
来源：http://hz.zhijiandao.cn/gtvnoawrxz.html

C#:   (int)resp.StatusCode
来源：http://hz.dashuyun.cn/gtduijrukv.html

[L08] 并发请求多个地址
来源：http://hz.yuanzhike.top/gtgfyzzmta.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.kuanghao11.cn/gtxukczhie.html

PHP:  curl_multi_init() 系列
来源：http://hz.jinghuilouyu.cn/gtcgubgpka.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jinghuilouyu.cn/gtnktacshe.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhongyouzk.top/gthycksnns.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.cheryme.top/gtsprounfm.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.chenjidiqi.icu/gtfmhcgdph.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.xylfe.cn/gtsujkonvc.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.zhoulong.xyz/gtchmkdtvo.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtyclfxipn.html

M. 命令行 / 进程 / 环境
来源：http://hz.nanxuanxn.top/gttbyxnssr.html

================================================================================
来源：http://hz.fengsongda.top/gtriernuuc.html

[M01] 读取命令行参数
来源：http://hz.yonumen.top/gtrwjtgzgz.html

Py:   sys.argv[1:]
来源：http://hz.redwolf501.top/gtewszviua.html

PHP:  $argv;  $argc;
来源：http://hz.shuidangran.top/gtduwfiyoa.html

JS:   process.argv.slice(2)
来源：http://hz.zhongyouzk.top/gtiwdgvbvo.html

TS:   process.argv.slice(2)
来源：http://hz.ivvv.top/gtjyqnqhrf.html

Java: args 数组（main 方法参数）
来源：http://hz.iojbl.cn/gtojdwwvec.html

Go:   os.Args[1:]
来源：http://hz.guowangkeji.top/gtgpgwumuq.html

Ruby: ARGV
来源：http://hz.mhx1999.top/gtlcmdgrxz.html

C#:   args 数组（Main 方法参数）
来源：http://hz.zdqjudy.top/gtotkpieab.html

[M02] 读取环境变量
来源：http://hz.jianghu66.top/gtpjbpfyxe.html

Py:   os.environ.get("HOME")
来源：http://hz.sysykeji.top/gtrzmyhyuy.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.0kj1m.cn/gtqeammfsd.html

JS:   process.env.HOME
来源：http://hz.0kj1m.cn/gthqcvvxlh.html

TS:   process.env.HOME
来源：http://hz.iojbl.cn/gtuqkvrcps.html

Java: System.getenv("HOME")
来源：http://hz.xuetiantiany.cn/gtcyqcctzq.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.tianlin.xyz/gtllqjnaxw.html

Ruby: ENV["HOME"]
来源：http://hz.birdmap.top/gthbypzcql.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.bjfxy.top/gtvrvqaqxb.html

[M03] 执行外部命令
来源：http://hz.dashuyun.cn/gtakprxdjo.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.pengpengdd.cyou/gtobtnozmd.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.nwbrower.top/gtrdpojukk.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.zycfv.cn/gtqahuglhr.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.ywan-chungtsiang.top/gtypqsnrwg.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.ehwqpu.com/gthywgtoan.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.shangyingyoupin.top/gtklynkkhu.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.9152youxi.cn/gtdcowzxal.html

C#:   Process.Start("ls", "-l");
来源：http://hz.sufxvd.cn/gtzuslwwiv.html

[M04] 获取当前工作目录
来源：http://hz.sweek.top/gttnxlfeqa.html

Py:   os.getcwd()
来源：http://hz.jqgfzy.top/gtrzwcgtrm.html

PHP:  getcwd();
来源：http://hz.meibo888.top/gtuxbhqzlj.html

JS:   process.cwd()
来源：http://hz.dianchejie.cn/gtlooctcdo.html

TS:   process.cwd()
来源：http://hz.jinqigfzy.top/gtzdtuwpgb.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.gotoacloud.top/gtcturvspm.html

Go:   os.Getwd()
来源：http://hz.quarkkingdee.top/gtlqmvbvni.html

Ruby: Dir.pwd
来源：http://hz.shanyushiyangtech.top/gtbenhqeaf.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.svipenyu.cn/gtpoulggzq.html

[M05] 设置退出码
来源：http://hz.tianlin.xyz/gtpmshccfs.html

Py:   sys.exit(1)
来源：http://hz.dashuyun.cn/gteolgfsls.html

PHP:  exit(1);
来源：http://hz.haohaochexian.top/gtnwgthzrm.html

JS:   process.exit(1)
来源：http://hz.daria6918.cn/gtyskzlcdu.html

TS:   process.exit(1)
来源：http://hz.snrcjt.cn/gtiviyfxml.html

Java: System.exit(1)
来源：http://hz.jianghu66.top/gtyphausgl.html

Go:   os.Exit(1)
来源：http://hz.shzxlz.cn/gtomhxzyrx.html

Ruby: exit 1
来源：http://hz.ydzc1.top/gtqnhejnvc.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.mhx1999.top/gtyfkntfzk.html

[M06] 向标准错误输出
来源：http://hz.jinyuanbaomall.cn/gtyzcejzas.html

Py:   print("err", file=sys.stderr)
来源：http://hz.ydzc1.top/gtihtyrkrp.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.tianlin.xyz/gtrchokhrl.html

JS:   console.error("err")
来源：http://hz.zhengqikj.top/gtdzuwupdw.html

TS:   console.error("err")
来源：http://hz.tian-w.cn/gtrszvppun.html

Java: System.err.println("err")
来源：http://hz.yj20258888.top/gtjcavowyi.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.52xcode.cn/gtbywjxkwx.html

Ruby: warn "err"
来源：http://hz.shangyingyoupin.top/gtunvllrmh.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.yuanzhike.top/gtgtjgxsay.html

[M07] 判断是否为主入口
来源：http://hz.yj20258.top/gtfwcdzbpe.html

Py:   if __name__ == "__main__":
来源：http://hz.chenlongwang.top/gtucbstlxh.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.cqqwz.cn/gtuttjtbob.html

JS:   require.main === module
来源：http://hz.nanxuanxn.top/gtzehramzs.html

TS:   require.main === module
来源：http://hz.yvedp.cn/gtowhscnex.html

Java: public static void main(String[] args)
来源：http://hz.chenlongwang.top/gtnivwsmuu.html

Go:   func main()
来源：http://hz.zhaomingkeji.xyz/gtrgyglybw.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.sxryk.cn/gtaudyyphn.html

C#:   static void Main(string[] args)
来源：http://hz.yuanzhike.top/gttnueoilk.html

[M08] 获取系统与运行时信息
来源：http://hz.fzhhl.top/gtztidztgv.html

Py:   platform.system();  platform.python_version()
来源：http://hz.jinghuilouyu.cn/gtsodnfhji.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.kuanghao11.cn/gtkccqtlna.html

JS:   process.platform;  process.version
来源：http://hz.zhengqikj.top/gtkxypakvp.html

TS:   process.platform;  process.version
来源：http://hz.ppjwa.cn/gtgffqpesq.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.zhengqikj.top/gthlpgdfku.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.hfpthk.cn/gtczjngrll.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.shuidangran.top/gtdzqelfjb.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.yj20258888.top/gtbichuyvq.html

================================================================================
来源：http://hz.gogol.net.cn/gtlhfzpqvb.html

N. 数据结构与算法
来源：http://hz.daria6918.cn/gtyhjiwxos.html

================================================================================
来源：http://hz.xinyue.icu/gtgfsbzmxl.html

[N01] 二分查找（有序数组）
来源：http://hz.ywan-chungtsiang.top/gtbxsetgyq.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.xinyue.icu/gtisgvmbxn.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.hongshengwenyu.top/gtfvjqkhil.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jqgfzy.top/gtbbzeqewx.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zhixingplan.top/gtnynotzgz.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.dashuyun.cn/gtoacrdfwc.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.havefunace.top/gtshcszspm.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.nwbrower.top/gtsbinocmm.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.yonumen.top/gtcbluurfg.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.jinghuilouyu.cn/gtccsibwcq.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.yonumen.top/gtbffcdijy.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.xuanzx.com/gtkbvkduvv.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.andypj.xyz/gtninwovft.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yanxiufei.cn/gtddkpumnz.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.yongpay.top/gtzmziqthp.html

Go:   slices.Sort(arr)
来源：http://hz.52xcode.cn/gtjwezmfzv.html

Ruby: arr.sort
来源：http://hz.shzxlz.cn/gthzcvdqmv.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.redwolf501.top/gtqtpsmygf.html

[N03] 快速排序（分治示例）
来源：http://hz.havefunace.top/gtlhloqbhu.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.jlsjyb.cn/gttvmcxyig.html

PHP:  // 递归实现，或用 usort
来源：http://hz.wangshuangyany.cn/gtzrdsqleu.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yanxiufei.cn/gtxjakewws.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.wangshuangyany.cn/gtilensvvl.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.ydzc1.top/gtqvbveevi.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.hysaishi.cn/gtnsdlukuc.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.chenjidiqi.icu/gtfqawtjmf.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.quarkkingdee.top/gtgbizlugi.html

[N04] 斐波那契数列
来源：http://hz.xziqi.cn/gtntkcyzic.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.ivvv.top/gtbkrbeqiq.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.redwolf501.top/gtlcsecnjg.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.cucudq.cn/gtzscqbkhx.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jqgfzy.top/gtehdivewv.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.0kj1m.cn/gtzqvnkqee.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.jianghu66.top/gtjppanxcn.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.yuanzhike.top/gtqgxfswgf.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.yuanzhike.top/gtmvlklzvu.html

[N05] 最大公约数
来源：http://hz.bjfxy.top/gtmkqkozgl.html

Py:   math.gcd(a, b)
来源：http://hz.snrcjt.cn/gtrvrnvibo.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.zhoulong.xyz/gtxcgyypai.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.nanxinkj.top/gtigldrwsl.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.zycfv.cn/gtxxlhamqg.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.smart0.xyz/gtwjwjtgri.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.jyoumei.cn/gtkpdweuqe.html

Ruby: a.gcd(b)
来源：http://hz.guannengcc.top/gthoewoavr.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.sysykeji.top/gtnboupvhj.html

[N06] 判断回文字符串
来源：http://hz.shanyushiyangtech.top/gtvnyqfbjb.html

Py:   s == s[::-1]
来源：http://hz.dianchejie.cn/gtbqvgieap.html

PHP:  $s === strrev($s);
来源：http://hz.zhiwuduotai.top/gtkthgqkls.html

JS:   s === [...s].reverse().join("")
来源：http://hz.xuetiantiany.cn/gtqdakmykr.html

TS:   s === [...s].reverse().join("")
来源：http://hz.gaohongyu789.top/gtbkzouwjz.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.birdmap.top/gtmtvqzqrt.html

Go:   // 双指针从两端比较
来源：http://hz.ppjwa.cn/gtptkrscgl.html

Ruby: s == s.reverse
来源：http://hz.jinyuanbaomall.cn/gtjkqhfnoy.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.jinghuilouyu.cn/gtnsrncyeg.html

[N07] 两数之和（返回下标）
来源：http://hz.birdmap.top/gtafrczopb.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.havefunace.top/gtnfpssmwh.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.jinyuanbaomall.cn/gtzlrchesr.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.chenlongwang.top/gtvjhvfabr.html

TS:   // 手写 Map<string, number>
来源：http://hz.sweek.top/gtexolihkh.html

Java: // 手写 HashMap
来源：http://hz.zhixingplan.top/gtngbjkuis.html

Go:   // 手写 map[int]int
来源：http://hz.aizwys.cn/gtknjwhapm.html

Ruby: // 手写 Hash
来源：http://hz.shanyushiyangkeji.top/gtomokavib.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.jyoumei.cn/gttpduowxr.html

[N08] 生成全排列
来源：http://hz.jinqigfzy.top/gtbobncivx.html

Py:   itertools.permutations(arr)
来源：http://hz.meibo888.top/gtxpyzakhj.html

PHP:  // 手写递归交换
来源：http://hz.hywenlv.cn/gtcxecuolc.html

JS:   // 手写回溯递归
来源：http://hz.shuidangran.top/gtiuknzyfe.html

TS:   // 手写回溯递归
来源：http://hz.sweek.top/gtfwdfpaju.html

Java: // 手写回溯递归
来源：http://hz.hnxiangtu.top/gtizvttudq.html

Go:   // 手写回溯递归
来源：http://hz.ydzc1.top/gtglnifqti.html

Ruby: arr.permutation.to_a
来源：http://hz.cheryme.top/gtftteehbv.html

C#:   // 手写回溯递归
来源：http://hz.jinqigufen.top/gtltycfwms.html

[N09] 栈与队列
来源：http://hz.havefunace.top/gtjddmarxq.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.bjfxy.top/gtosccathr.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.52xcode.cn/gtzftqpwfl.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.yangfankeji.com/gtgshkysaj.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.shanyushiyangtech.top/gtstryckhl.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.zhaomingkeji.xyz/gtqgwozpls.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.xziqi.cn/gtqdtgzyqy.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.hongshengwenyu.top/gthopauhzz.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.nanxuanxn.top/gtrrlhbpsl.html

[N10] 链表节点定义
来源：http://hz.pengpengdd.cyou/gtoaypxjos.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.gogol.net.cn/gtuhnqphuf.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.wangshuangyany.cn/gtltdbhait.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.yj20258888.top/gtnjfpetxr.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.c1oappe.top/gtxzplrsoo.html

Java: class Node { int v; Node next; }
来源：http://hz.xziqi.cn/gtdnabaylh.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.gogol.net.cn/gtpofhkxnf.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.jqgfzy.top/gtfgwwpdeq.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.tian-w.cn/gtxorpfxup.html

[N11] 二叉树中序遍历
来源：http://hz.xinyue.icu/gthirottdw.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.guannengcc.top/gtjgixhpwb.html

PHP:  // 手写递归函数
来源：http://hz.fengsongda.top/gtotoocanc.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.xziqi.cn/gtszgawuph.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jiagoushi.top/gtocfdhmit.html

Java: // 手写递归
来源：http://hz.hammf.cn/gtsgiwhqag.html

Go:   // 手写递归
来源：http://hz.yj20258.top/gtahcwvylm.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.fzhhl.top/gtmbecubhx.html

C#:   // 手写递归
来源：http://hz.gogol.net.cn/gtkxpdprjg.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.jinyuanbaomall.cn/gtckwkhyje.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.daxiang520.top/gtrvagmazi.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.cqqwz.cn/gtcokmstsm.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.zhijiandao.cn/gtjkpdrfpa.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.ywan-chungtsiang.top/gtmemebzxm.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.dianchejie.cn/gtlqisehni.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.jinyuanbaomall.cn/gtimqgprzi.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.hywenlv.cn/gtxbgleuqx.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.havefunace.top/gtuyvdwmzb.html

================================================================================
来源：http://hz.gogol.net.cn/gtrcvmchgk.html

O. 并发与异步
来源：http://hz.dianchejie.cn/gtcxzqlmrq.html

================================================================================
来源：http://hz.cqqwz.cn/gtxnxodomv.html

[O01] 启动一个线程
来源：http://hz.birdmap.top/gtkryuuebe.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.sxryk.cn/gtrlwvkota.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.quarkkingdee.top/gtlubehvta.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.hongshengwenyu.top/gthviotkxk.html

TS:   // 同 JS
来源：http://hz.aibaodan.cn/gtxdfynnra.html

Java: new Thread(() -> f()).start()
来源：http://hz.zhiwuduotai.top/gtyjydjwjm.html

Go:   go f()
来源：http://hz.haohaochexian.top/gtdcgmrcqi.html

Ruby: Thread.new { f }
来源：http://hz.shanyushiyangtech.top/gtysticriv.html

C#:   Task.Run(() => F());
来源：http://hz.xylfe.cn/gtkyuisgmn.html

[O02] 使用线程池
来源：http://hz.tian-w.cn/gtgdpsagcf.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.xziqi.cn/gtezyvhaqi.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.pycfn.com/gtgzjgfdcb.html

JS:   // worker_threads 线程池
来源：http://hz.tianlin.xyz/gthsxfogiu.html

TS:   // worker_threads 线程池
来源：http://hz.yangfankeji.com/gtvpgruxoa.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.kuanghao11.cn/gtwhkvmgwr.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.zdqjudy.top/gtneaveolw.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.jiagoushi.top/gtdtnjaubp.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.hfpthk.cn/gtnystpsue.html

[O03] 加锁保护共享数据
来源：http://hz.0kj1m.cn/gtmpjvtfxs.html

Py:   with lock: shared += 1
来源：http://hz.yvedp.cn/gtxvlyswqc.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.ivvv.top/gtvlbijekz.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.cdnleiting.top/gtwnnhtnnd.html

TS:   // 同 JS
来源：http://hz.nwbrower.top/gtxlshseqo.html

Java: synchronized (this) { shared++; }
来源：http://hz.feifeiyinyue.top/gtjfaieyzo.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.shanyushiyangkeji.top/gtdzacsaco.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.tianlin.xyz/gtfohknben.html

C#:   lock (gate) { shared++; }
来源：http://hz.c1oappe.top/gtciesjchm.html

[O04] 定义异步函数并等待
来源：http://hz.zhengqikj.top/gteoobgyuq.html

Py:   async def f():⏎    await g()
来源：http://hz.ivvv.top/gtlitniahz.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.tianlin.xyz/gtirrixnjr.html

JS:   async function f() { await g(); }
来源：http://hz.jinghuilouyu.cn/gtqwxoevkc.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.smart0.xyz/gtudqixhyg.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.cqqwz.cn/gtxjockoqz.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.hongshengwenyu.top/gtuqfecwjf.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.ppjwa.cn/gtkaxywcos.html

C#:   async Task F() { await G(); }
来源：http://hz.yanxiufei.cn/gthauhsxej.html

[O05] 并发执行并等待全部完成
来源：http://hz.dianchejie.cn/gtlctjitxz.html

Py:   asyncio.gather(*tasks)
来源：http://hz.meibo888.top/gtrhmotupb.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.jlsjyb.cn/gtdcwxdswf.html

JS:   await Promise.all(tasks)
来源：http://hz.daria6918.cn/gtomzmprxy.html

TS:   await Promise.all(tasks)
来源：http://hz.dashuyun.cn/gtfkvuxbqr.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.fzhhl.top/gtwgzleqgn.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.aibaodan.cn/gtlndlurjp.html

Ruby: threads.map(&:join)
来源：http://hz.dashuyun.cn/gtfdaamcgx.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.wangshuangyany.cn/gtqnkkxmnv.html

[O06] 使用进程池
来源：http://hz.yj20258888.top/gtdpufqpip.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.c1oappe.top/gtqwvocyyg.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.bjfxy.top/gtqryypdkt.html

JS:   // child_process / cluster 模块
来源：http://hz.jyoumei.cn/gtxxxikniw.html

TS:   // child_process / cluster 模块
来源：http://hz.quarkkingdee.top/gtgzmdtbbm.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.ywan-chungtsiang.top/gtgeufwqaw.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.fengsongda.top/gtljlefkgp.html

Ruby: // fork 块
来源：http://hz.xingfuxueyuan.xyz/gtjnmdeskl.html

C#:   Parallel.For
来源：http://hz.zhengqikj.top/gtvlwiithu.html

================================================================================
来源：http://hz.dianchejie.cn/gtmdonukoj.html

P. 常用工具函数
来源：http://hz.shanyushiyangtech.top/gtpbmrwrgf.html

================================================================================
来源：http://hz.zhixingplan.top/gtmcfmrqse.html

[P01] 生成 UUID
来源：http://hz.andypj.xyz/gtqrmnhwdn.html

Py:   str(uuid.uuid4())
来源：http://hz.quarkkingdee.top/gtifyoijoe.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.ydzc1.top/gtfcrnhdej.html

JS:   crypto.randomUUID()
来源：http://hz.vqdsnc.cn/gtbopzpxuy.html

TS:   crypto.randomUUID()
来源：http://hz.zycfv.cn/gtzbhhvsvg.html

Java: UUID.randomUUID().toString()
来源：http://hz.cashguo.top/gtxdjzkwom.html

Go:   // 用 github.com/google/uuid
来源：http://hz.xingfuxueyuan.xyz/gtohhmlmfz.html

Ruby: SecureRandom.uuid
来源：http://hz.snrcjt.cn/gtwtxvovxn.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.nwbrower.top/gtizytuhzb.html

[P02] MD5 / SHA256 摘要
来源：http://hz.hfpthk.cn/gtmnpsmqeh.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.hfpthk.cn/gtlbcempwl.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.hfpthk.cn/gtrsirdpql.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.yj202588.top/gtscbzowuq.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.hammf.cn/gtbairzjts.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.shuidangran.top/gtruwftjvl.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.xziqi.cn/gtwwberorm.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.jinghuilouyu.cn/gtabnqosba.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.yuxming.cn/gttvqnhgve.html

[P03] 生成短随机字符串
来源：http://hz.yonumen.top/gtblvwbcdv.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.aizwys.cn/gtesaoqpny.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.52xcode.cn/gttwtiovns.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.haohaochexian.top/gtjvjennpa.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.xuetiantiany.cn/gtqjnkmqkx.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.yongpay.top/gtsyhlunxp.html


<!-- 参考信息 -->