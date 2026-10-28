代发 wailian999

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.zycfv.cn/gttgjwiixf.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.chenjidiqi.icu/gtbpicnsvi.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.svipenyu.cn/gtnxfwhuve.html

[L06] 解析响应为 JSON
来源：http://hz.andypj.xyz/gtztwnekcz.html

Py:   resp.json()
来源：http://hz.ppjwa.cn/gthcklwsdd.html

PHP:  json_decode($body, true);
来源：http://hz.jinghuilouyu.cn/gthbniftjh.html

JS:   await resp.json()
来源：http://hz.yj20258.top/gttejtzexq.html

TS:   await resp.json()
来源：http://hz.jinqigufen.top/gtugyfscat.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.nanxinkj.top/gtwqknrwiv.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.zhiwuduotai.top/gtgkattdzp.html

Ruby: JSON.parse(resp.body)
来源：http://hz.yueranfly.top/gtvrbllmai.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.ehwqpu.com/gtytcmddqm.html

[L07] 处理 HTTP 状态码
来源：http://hz.zhixingplan.top/gtamldifka.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.cheryme.top/gtysrnmazu.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.zhaomingkeji.xyz/gtmxsrjkcr.html

JS:   resp.ok;  resp.status
来源：http://hz.aibaodan.cn/gtfmpdrocp.html

TS:   resp.ok;  resp.status
来源：http://hz.bjfxy.top/gteovhrfwc.html

Java: resp.statusCode()
来源：http://hz.daria6918.cn/gttmyjyrvd.html

Go:   resp.StatusCode
来源：http://hz.xziqi.cn/gtoerjwntu.html

Ruby: resp.code.to_i
来源：http://hz.52xcode.cn/gtgwmsyesp.html

C#:   (int)resp.StatusCode
来源：http://hz.redwolf501.top/gtusueskif.html

[L08] 并发请求多个地址
来源：http://hz.9152youxi.cn/gtvgxqoogg.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.nanxinkj.top/gtpnswtcea.html

PHP:  curl_multi_init() 系列
来源：http://hz.yuanzhike.top/gtxvbofoqt.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jinyuanbaomall.cn/gtdizjrotv.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.cashguo.top/gtlcuxtgle.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.dashuyun.cn/gtkbidizoy.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.vqdsnc.cn/gtyachidgl.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.hnqzz.top/gtvzjgmmnb.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.andypj.xyz/gtgnqjelrj.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtmscjnucr.html

M. 命令行 / 进程 / 环境
来源：http://hz.zhiwuduotai.top/gtjymfvphx.html

================================================================================
来源：http://hz.bjfxy.top/gthavtextf.html

[M01] 读取命令行参数
来源：http://hz.hysaishi.cn/gtagcaexmn.html

Py:   sys.argv[1:]
来源：http://hz.yueranfly.top/gtatcfcwrn.html

PHP:  $argv;  $argc;
来源：http://hz.nanxuanxn.top/gtngzkutnm.html

JS:   process.argv.slice(2)
来源：http://hz.birdmap.top/gtxiobcqtx.html

TS:   process.argv.slice(2)
来源：http://hz.havefunace.top/gtsmthpwnx.html

Java: args 数组（main 方法参数）
来源：http://hz.jqgufenzy.top/gtugvsdjps.html

Go:   os.Args[1:]
来源：http://hz.jinqigufen.top/gtyyruweui.html

Ruby: ARGV
来源：http://hz.0kj1m.cn/gtgjihjwgp.html

C#:   args 数组（Main 方法参数）
来源：http://hz.zycfv.cn/gtsgckxlhx.html

[M02] 读取环境变量
来源：http://hz.chenzaomai.com/gtxmxpdexz.html

Py:   os.environ.get("HOME")
来源：http://hz.ppjwa.cn/gtokgixpid.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.xinyue.icu/gtaczgvrho.html

JS:   process.env.HOME
来源：http://hz.wangshuangyany.cn/gtcgoycruy.html

TS:   process.env.HOME
来源：http://hz.sxryk.cn/gtnmhuqyoi.html

Java: System.getenv("HOME")
来源：http://hz.jqgufenzy.top/gtxwwijcjz.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.tian-w.cn/gtuviqzlms.html

Ruby: ENV["HOME"]
来源：http://hz.smart0.xyz/gtqfmywkxb.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.mhx1999.top/gtcsjpkcrw.html

[M03] 执行外部命令
来源：http://hz.yj202588.top/gtzefhluuy.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.wangshuangyany.cn/gtvyfxqmey.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.xylfe.cn/gtlnlgtojy.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.jqgufenzy.top/gtkprlfren.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.hnqzz.top/gtrfbpjhhl.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.gaohongyu789.top/gtxbfvzajy.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.pycfn.com/gtpgvdigcr.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.yuanzhike.top/gtojrhillq.html

C#:   Process.Start("ls", "-l");
来源：http://hz.gzhubu.top/gtisybylmr.html

[M04] 获取当前工作目录
来源：http://hz.tian-w.cn/gtpmpxahkx.html

Py:   os.getcwd()
来源：http://hz.xuetiantiany.cn/gtgzmneach.html

PHP:  getcwd();
来源：http://hz.shzxlz.cn/gtdjlqjheo.html

JS:   process.cwd()
来源：http://hz.gaohongyu789.top/gtvfplrkzl.html

TS:   process.cwd()
来源：http://hz.birdmap.top/gtyjonkfho.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.jiagoushi.top/gtbktvymdc.html

Go:   os.Getwd()
来源：http://hz.kuanghao11.cn/gtrvitibpo.html

Ruby: Dir.pwd
来源：http://hz.hammf.cn/gtoxcjzpxg.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.jqgufenzy.top/gtdeqxfyzj.html

[M05] 设置退出码
来源：http://hz.guannengcc.top/gtcencduhx.html

Py:   sys.exit(1)
来源：http://hz.sxryk.cn/gttgcmjcqs.html

PHP:  exit(1);
来源：http://hz.iojbl.cn/gtoozlfdtx.html

JS:   process.exit(1)
来源：http://hz.jyoumei.cn/gtumguqgdj.html

TS:   process.exit(1)
来源：http://hz.xylfe.cn/gtmsrbxarx.html

Java: System.exit(1)
来源：http://hz.ydjk.org.cn/gtntnliibd.html

Go:   os.Exit(1)
来源：http://hz.havefunace.top/gtmusgtmmn.html

Ruby: exit 1
来源：http://hz.iojbl.cn/gtlyzuzaiv.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.sxryk.cn/gthtvanquk.html

[M06] 向标准错误输出
来源：http://hz.hnxiangtu.top/gtawlpxfxp.html

Py:   print("err", file=sys.stderr)
来源：http://hz.ppjwa.cn/gtuitcmpcs.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.zhoulong.xyz/gtxlwcncuo.html

JS:   console.error("err")
来源：http://hz.316326.xyz/gtnhuzlwvo.html

TS:   console.error("err")
来源：http://hz.daxiang520.top/gtcknmevtq.html

Java: System.err.println("err")
来源：http://hz.cheryme.top/gtoivuicwo.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.c1oappe.top/gtstvpcfua.html

Ruby: warn "err"
来源：http://hz.ivvv.top/gtxlvfvboa.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.zycfv.cn/gtayoodneu.html

[M07] 判断是否为主入口
来源：http://hz.316326.xyz/gtqonearnl.html

Py:   if __name__ == "__main__":
来源：http://hz.pengpengdd.cyou/gtummwaaxa.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.kuanghao11.cn/gtesavvsgl.html

JS:   require.main === module
来源：http://hz.yj202588.top/gtjegctpfo.html

TS:   require.main === module
来源：http://hz.jinqigfzy.top/gtpkcpkzaj.html

Java: public static void main(String[] args)
来源：http://hz.tanke756.top/gtqmtsufni.html

Go:   func main()
来源：http://hz.316326.xyz/gtvqxgthdc.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.bjfxy.top/gtwthlmmjt.html

C#:   static void Main(string[] args)
来源：http://hz.zhengqikj.top/gtkqcmmoop.html

[M08] 获取系统与运行时信息
来源：http://hz.ybcxt.top/gtjlaocgeo.html

Py:   platform.system();  platform.python_version()
来源：http://hz.zhoulong.xyz/gtngbikynq.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.hywenlv.cn/gtvpmidivh.html

JS:   process.platform;  process.version
来源：http://hz.ybcxt.top/gtujrxcvob.html

TS:   process.platform;  process.version
来源：http://hz.aibaodan.cn/gtdyhrnnpk.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.nwbrower.top/gtmvsdzmrw.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.gaohongyu789.top/gtbfqasrtu.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.zhongyouzk.top/gtdcabsweh.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.zhoulong.xyz/gttyfjgfja.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtlgwhjixf.html

N. 数据结构与算法
来源：http://hz.wangshuangyany.cn/gteojclcgk.html

================================================================================
来源：http://hz.shzxlz.cn/gtojkalltq.html

[N01] 二分查找（有序数组）
来源：http://hz.zdqjudy.top/gtepmqhhkh.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.haohaochexian.top/gtaopytazx.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.ehwqpu.com/gtubgzjasr.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zhengqikj.top/gtuvockiqn.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.hywenlv.cn/gtwxkovglv.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.52xcode.cn/gtyvmgphhl.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.jiagoushi.top/gtvqdweeza.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.ydjk.org.cn/gtivdtasvq.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.mhx1999.top/gtdzzrgcgr.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.chenlongwang.top/gtshcicpwx.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.tian-w.cn/gtlthrzwnk.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.smart0.xyz/gtvvazwuxs.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.cqqwz.cn/gtkwdhgvrq.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.xuanzx.com/gtotprapql.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.0kj1m.cn/gtrnvenqxl.html

Go:   slices.Sort(arr)
来源：http://hz.ybcxt.top/gtzvbtizwn.html

Ruby: arr.sort
来源：http://hz.redwolf501.top/gtrdkwawhz.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.ehwqpu.com/gtpmzcdyzk.html

[N03] 快速排序（分治示例）
来源：http://hz.shuidangran.top/gtdowxznkf.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.cdnleiting.top/gthebxmmie.html

PHP:  // 递归实现，或用 usort
来源：http://hz.cheryme.top/gtsmfrctgc.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jiagoushi.top/gtcgaaqphv.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.316326.xyz/gtwcgjjlrd.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.yj202588.top/gtohtsuyqt.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.jianghu66.top/gtkzfxpnus.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.pengpengdd.cyou/gtjnexvknj.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.jinqigfzy.top/gtaxwgkewp.html

[N04] 斐波那契数列
来源：http://hz.dianchejie.cn/gtvoflrzxt.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.fengsongda.top/gthdghhcbn.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.tianlin.xyz/gteifremwf.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.hysaishi.cn/gtcdbigzqa.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.chenlongwang.top/gtodpdqsfd.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.jinghuilouyu.cn/gtgijiphmb.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.daxiang520.top/gtznyxtmfl.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.zdqjudy.top/gtroeiajpf.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.havefunace.top/gtxinlswqu.html

[N05] 最大公约数
来源：http://hz.xziqi.cn/gtdubagolb.html

Py:   math.gcd(a, b)
来源：http://hz.shanyushiyangtech.top/gtbmdwsdre.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.ppjwa.cn/gtquqwvunh.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.hnxiangtu.top/gtwtfrkirn.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.52xcode.cn/gtgarxekal.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.yangfankeji.com/gttripvrmu.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.yongpay.top/gtfpagrlpi.html

Ruby: a.gcd(b)
来源：http://hz.yanxiufei.cn/gtsptwyhjr.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.9152youxi.cn/gthzuvsmcx.html

[N06] 判断回文字符串
来源：http://hz.316326.xyz/gtjuwtrceh.html

Py:   s == s[::-1]
来源：http://hz.yueranfly.top/gtjncskhae.html

PHP:  $s === strrev($s);
来源：http://hz.52xcode.cn/gtiraagtdx.html

JS:   s === [...s].reverse().join("")
来源：http://hz.316326.xyz/gtroxshmuv.html

TS:   s === [...s].reverse().join("")
来源：http://hz.316326.xyz/gtuhpohvst.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.shangyingyoupin.top/gtlydpsdeq.html

Go:   // 双指针从两端比较
来源：http://hz.ydjk.org.cn/gtajwxlnja.html

Ruby: s == s.reverse
来源：http://hz.yongpay.top/gtymdsrcmf.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.zhoulong.xyz/gtsgaqbqdi.html

[N07] 两数之和（返回下标）
来源：http://hz.daria6918.cn/gtssppkayn.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.andypj.xyz/gtjqqfkylp.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.hnxiangtu.top/gtubdqtamk.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.jinyuanbaomall.cn/gtcncqdzns.html

TS:   // 手写 Map<string, number>
来源：http://hz.xziqi.cn/gtejlqsaqv.html

Java: // 手写 HashMap
来源：http://hz.fengsongda.top/gtqvzupelz.html

Go:   // 手写 map[int]int
来源：http://hz.shzxlz.cn/gtoxlumsxs.html

Ruby: // 手写 Hash
来源：http://hz.cqqwz.cn/gtslcpkbxc.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.hongshengwenyu.top/gtlpkkdcyg.html

[N08] 生成全排列
来源：http://hz.yvedp.cn/gtjkpvvash.html

Py:   itertools.permutations(arr)
来源：http://hz.nanxinkj.top/gtkxagcmfn.html

PHP:  // 手写递归交换
来源：http://hz.mhx1999.top/gtotxevfin.html

JS:   // 手写回溯递归
来源：http://hz.jinqigfzy.top/gttafjuifk.html

TS:   // 手写回溯递归
来源：http://hz.sxryk.cn/gtbebgsxcb.html

Java: // 手写回溯递归
来源：http://hz.hongshengwenyu.top/gtckwjdgvy.html

Go:   // 手写回溯递归
来源：http://hz.fengsongda.top/gtxdrclvkw.html

Ruby: arr.permutation.to_a
来源：http://hz.hammf.cn/gtwgxnunat.html

C#:   // 手写回溯递归
来源：http://hz.gogol.net.cn/gtzeegwuki.html

[N09] 栈与队列
来源：http://hz.xinyue.icu/gtjffnigou.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.sufxvd.cn/gtyxupcwzx.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.wangshuangyany.cn/gtzlqzcnrw.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.chenzaomai.com/gtwlgalvnb.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.hfpthk.cn/gtlzehkvkm.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.guowangkeji.top/gtkbdyewen.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.daxiang520.top/gtheyxmwqa.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.c1oappe.top/gtgajkikyj.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.wangshuangyany.cn/gtlqkajuhn.html

[N10] 链表节点定义
来源：http://hz.zhijiandao.cn/gtlnwtdqky.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.xuanzx.com/gtwfbnizww.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.jianghu66.top/gtjmjzkgep.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.hammf.cn/gtsrjrbnyb.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.bjfxy.top/gtemjjfgwp.html

Java: class Node { int v; Node next; }
来源：http://hz.cashguo.top/gtaatfomrx.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.yuanzhike.top/gtrrsddjdq.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.yj20258.top/gtgegtzdpk.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.nanxinkj.top/gtekzhyznc.html

[N11] 二叉树中序遍历
来源：http://hz.sysykeji.top/gtzczvwzec.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.vqdsnc.cn/gtqxoctwlx.html

PHP:  // 手写递归函数
来源：http://hz.xziqi.cn/gttdybxhqw.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.ydjk.org.cn/gtmywjevvx.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.ehwqpu.com/gtrsgguzjs.html

Java: // 手写递归
来源：http://hz.redwolf501.top/gtptrwtpiv.html

Go:   // 手写递归
来源：http://hz.cqqwz.cn/gtcaromlxd.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.nanxuanxn.top/gtccvitlsb.html

C#:   // 手写递归
来源：http://hz.daxiang520.top/gthvzjnone.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.daria6918.cn/gtcjnxcfct.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.yj20258.top/gtxvfjrpvf.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.yangfankeji.com/gtosfiiurc.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.0kj1m.cn/gtjumwwwcw.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.ivvv.top/gtdomsqpbe.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.bjfxy.top/gtidxrtyun.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.yvedp.cn/gtmphofojt.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.sweek.top/gtftuaxhcp.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yuxming.cn/gtjjxdpidz.html

================================================================================
来源：http://hz.xziqi.cn/gtrhgceauy.html

O. 并发与异步
来源：http://hz.iojbl.cn/gtmznknegu.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gthazejzyx.html

[O01] 启动一个线程
来源：http://hz.gogol.net.cn/gtneuurcec.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.xziqi.cn/gtpaepfyhm.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.nanxuanxn.top/gtcrnbefwm.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.zhongyouzk.top/gtiuwmaqrc.html

TS:   // 同 JS
来源：http://hz.jqgfzy.top/gtpircboqq.html

Java: new Thread(() -> f()).start()
来源：http://hz.aizwys.cn/gtbkjwpwjd.html

Go:   go f()
来源：http://hz.zhaomingkeji.xyz/gtvkuphhve.html

Ruby: Thread.new { f }
来源：http://hz.sxryk.cn/gtbxwbrocr.html

C#:   Task.Run(() => F());
来源：http://hz.jinqigufen.top/gtxgmrrjcl.html

[O02] 使用线程池
来源：http://hz.jqgfzy.top/gtavcckaaw.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.jinyuanbaomall.cn/gtaxcgosuz.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.yongpay.top/gtbpyvywao.html

JS:   // worker_threads 线程池
来源：http://hz.52xcode.cn/gtwleelcys.html

TS:   // worker_threads 线程池
来源：http://hz.hysaishi.cn/gtrcymzoex.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.meibo888.top/gtmtasgpyf.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.svipenyu.cn/gtnnuvvgbt.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.mhx1999.top/gtqlkykyit.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.52xcode.cn/gtmqniblys.html

[O03] 加锁保护共享数据
来源：http://hz.iojbl.cn/gtqotqrtpf.html

Py:   with lock: shared += 1
来源：http://hz.yvedp.cn/gtyclnpgtu.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.quarkkingdee.top/gtdvdzuuph.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.jinqigufen.top/gthrainpbq.html

TS:   // 同 JS
来源：http://hz.gzhubu.top/gtsuvqflnr.html

Java: synchronized (this) { shared++; }
来源：http://hz.yongpay.top/gtuwbzbndp.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.feifeiyinyue.top/gtjunxpcka.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.zhixingplan.top/gtuutnythg.html

C#:   lock (gate) { shared++; }
来源：http://hz.xinyue.icu/gtghzqrzdo.html

[O04] 定义异步函数并等待
来源：http://hz.cucudq.cn/gtbwubhwqn.html

Py:   async def f():⏎    await g()
来源：http://hz.shanyushiyangkeji.top/gtiephdfcb.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.yonumen.top/gtvwtbxhrj.html

JS:   async function f() { await g(); }
来源：http://hz.tanke756.top/gtzvkouegl.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.havefunace.top/gtkuimfpis.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.mhx1999.top/gtildmltia.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.316326.xyz/gtdstvjkeg.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.ppjwa.cn/gtducfhexh.html

C#:   async Task F() { await G(); }
来源：http://hz.xuetiantiany.cn/gtimhihzms.html

[O05] 并发执行并等待全部完成
来源：http://hz.nwbrower.top/gtmfcacsqq.html

Py:   asyncio.gather(*tasks)
来源：http://hz.316326.xyz/gtirkaemiy.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.gaohongyu789.top/gtdpvrxowm.html

JS:   await Promise.all(tasks)
来源：http://hz.zhaomingkeji.xyz/gtppucigcm.html

TS:   await Promise.all(tasks)
来源：http://hz.hysaishi.cn/gtnbmvvzwr.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.ehwqpu.com/gtpjazbrbw.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.jiagoushi.top/gtdpmrqker.html

Ruby: threads.map(&:join)
来源：http://hz.guannengcc.top/gtkvqvbnft.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.nanxinkj.top/gtnpycimkg.html

[O06] 使用进程池
来源：http://hz.hongshengwenyu.top/gtzpzwglxx.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.vqdsnc.cn/gtejlrgyub.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.xuanzx.com/gtcpehgwsf.html

JS:   // child_process / cluster 模块
来源：http://hz.cheryme.top/gtlgwsmvgg.html

TS:   // child_process / cluster 模块
来源：http://hz.xinyue.icu/gtpkorkfgb.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.hfpthk.cn/gtackgcjts.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.chenjidiqi.icu/gtkyouvuhw.html

Ruby: // fork 块
来源：http://hz.haohaochexian.top/gtwlbyifef.html

C#:   Parallel.For
来源：http://hz.tianlin.xyz/gtrlmgjdhf.html

================================================================================
来源：http://hz.cqqwz.cn/gtiwhftmyi.html

P. 常用工具函数
来源：http://hz.xingfuxueyuan.xyz/gtvfydetjg.html

================================================================================
来源：http://hz.vqdsnc.cn/gtuudxzizx.html

[P01] 生成 UUID
来源：http://hz.shanyushiyangtech.top/gtoyzhskij.html

Py:   str(uuid.uuid4())
来源：http://hz.tanke756.top/gtdqjtngss.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.yvedp.cn/gthmiarong.html

JS:   crypto.randomUUID()
来源：http://hz.gaohongyu789.top/gtpyquglht.html

TS:   crypto.randomUUID()
来源：http://hz.zycfv.cn/gtnykjomwv.html

Java: UUID.randomUUID().toString()
来源：http://hz.gogol.net.cn/gtgmyzmrxp.html

Go:   // 用 github.com/google/uuid
来源：http://hz.nanxinkj.top/gtiabizuyw.html

Ruby: SecureRandom.uuid
来源：http://hz.yuxming.cn/gttcyaguij.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.xuanzx.com/gtqqxbpdwt.html

[P02] MD5 / SHA256 摘要
来源：http://hz.hammf.cn/gtgloaxryo.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.hfpthk.cn/gtcvtnlhvt.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.52xcode.cn/gtvxhkpwms.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.tian-w.cn/gtymiqbiph.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.zhaomingkeji.xyz/gtuenhyadf.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.sysykeji.top/gtmnpgagwd.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.gotoacloud.top/gtpptcwnkm.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.yvedp.cn/gtrdfcrzmu.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.ehwqpu.com/gtlygwgjio.html

[P03] 生成短随机字符串
来源：http://hz.ybcxt.top/gtbitkamjr.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.bjfxy.top/gtzkdtasdd.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.vqdsnc.cn/gtpwfjctro.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.xuetiantiany.cn/gtksarctqw.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yangfankeji.com/gtbbeeibkg.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.jinqigufen.top/gtqccosfhy.html


<!-- 参考信息 -->