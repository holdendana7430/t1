代发 wailian999

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.52xcode.cn/gtecqubevv.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.yuanzhike.top/gtocbulmgf.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.nanxuanxn.top/gtiiycjjhy.html

[L06] 解析响应为 JSON
来源：http://hz.yangfankeji.com/gtopcqeysp.html

Py:   resp.json()
来源：http://hz.316326.xyz/gtrtmnkluf.html

PHP:  json_decode($body, true);
来源：http://hz.zhaomingkeji.xyz/gtvsayudxs.html

JS:   await resp.json()
来源：http://hz.vqdsnc.cn/gtjmihtzfo.html

TS:   await resp.json()
来源：http://hz.jianghu66.top/gtnocpviqy.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.9152youxi.cn/gtoaptahhn.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.nanxuanxn.top/gtuzmezitc.html

Ruby: JSON.parse(resp.body)
来源：http://hz.cheryme.top/gtfkmyyvsy.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.nanxuanxn.top/gtjqucwwuz.html

[L07] 处理 HTTP 状态码
来源：http://hz.cheryme.top/gtakeqntdb.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.yongpay.top/gtroeubpko.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.jqgufenzy.top/gtayuvtdjm.html

JS:   resp.ok;  resp.status
来源：http://hz.yuanzhike.top/gtavgxfhug.html

TS:   resp.ok;  resp.status
来源：http://hz.ywan-chungtsiang.top/gtecvpjpnd.html

Java: resp.statusCode()
来源：http://hz.quarkkingdee.top/gtoxsvfhfe.html

Go:   resp.StatusCode
来源：http://hz.jinqigufen.top/gthyovzcnu.html

Ruby: resp.code.to_i
来源：http://hz.zhaomingkeji.xyz/gtllutvghn.html

C#:   (int)resp.StatusCode
来源：http://hz.cqqwz.cn/gtelqmlucy.html

[L08] 并发请求多个地址
来源：http://hz.shanyushiyangtech.top/gttihleebu.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.andypj.xyz/gtsjtkiwir.html

PHP:  curl_multi_init() 系列
来源：http://hz.bjfxy.top/gtwvlmkhyi.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.xingfuxueyuan.xyz/gturafdaij.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.ppjwa.cn/gtcnaptjxb.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.ivvv.top/gtnzhdpurj.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.feifeiyinyue.top/gtkbhhibnj.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.hysaishi.cn/gtmrccxdkg.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.feifeiyinyue.top/gtzprisgyl.html

================================================================================
来源：http://hz.cucudq.cn/gtdcwfmdvi.html

M. 命令行 / 进程 / 环境
来源：http://hz.yonumen.top/gtsbtxosdr.html

================================================================================
来源：http://hz.nanxinkj.top/gtpfyidfda.html

[M01] 读取命令行参数
来源：http://hz.sufxvd.cn/gtcgizxyfx.html

Py:   sys.argv[1:]
来源：http://hz.fengsongda.top/gtrufrwxwv.html

PHP:  $argv;  $argc;
来源：http://hz.chenzaomai.com/gttshlwpyj.html

JS:   process.argv.slice(2)
来源：http://hz.tianlin.xyz/gtgyrpwzrt.html

TS:   process.argv.slice(2)
来源：http://hz.jinqigfzy.top/gtlzhbuwqp.html

Java: args 数组（main 方法参数）
来源：http://hz.daxiang520.top/gtmjmarrzt.html

Go:   os.Args[1:]
来源：http://hz.ybcxt.top/gtqbrjgxwt.html

Ruby: ARGV
来源：http://hz.tanke756.top/gtedvypzcb.html

C#:   args 数组（Main 方法参数）
来源：http://hz.yj202588.top/gtobuiffwi.html

[M02] 读取环境变量
来源：http://hz.xziqi.cn/gtgppgibyw.html

Py:   os.environ.get("HOME")
来源：http://hz.andypj.xyz/gtkfxvrgpf.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.yonumen.top/gtzmbyfvti.html

JS:   process.env.HOME
来源：http://hz.gaohongyu789.top/gtbomvagob.html

TS:   process.env.HOME
来源：http://hz.nanxuanxn.top/gtcadozupg.html

Java: System.getenv("HOME")
来源：http://hz.0kj1m.cn/gtcfxbsbzt.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.birdmap.top/gtvpazfhfb.html

Ruby: ENV["HOME"]
来源：http://hz.mhx1999.top/gtlfhzxzws.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.shanyushiyangtech.top/gtdysqmicr.html

[M03] 执行外部命令
来源：http://hz.yueranfly.top/gtwgywbkxx.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.cheryme.top/gttuxxsgme.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.birdmap.top/gtuwuusaig.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.redwolf501.top/gtlibygdej.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.gotoacloud.top/gtdfiloqyr.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.zhixingplan.top/gtrzdhbxjm.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.yuxming.cn/gtvydhwlws.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.yj20258.top/gttngzuooq.html

C#:   Process.Start("ls", "-l");
来源：http://hz.chenjidiqi.icu/gtgqomxvis.html

[M04] 获取当前工作目录
来源：http://hz.xuetiantiany.cn/gtaonwacbv.html

Py:   os.getcwd()
来源：http://hz.svipenyu.cn/gtfocaehmq.html

PHP:  getcwd();
来源：http://hz.haohaochexian.top/gtxstbvxdg.html

JS:   process.cwd()
来源：http://hz.nanxinkj.top/gtqbmfpzbf.html

TS:   process.cwd()
来源：http://hz.xuetiantiany.cn/gtfrgplflm.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.chenzaomai.com/gtuhjmnzoe.html

Go:   os.Getwd()
来源：http://hz.redwolf501.top/gtpdhvtkvq.html

Ruby: Dir.pwd
来源：http://hz.cheryme.top/gtroskaiim.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.sysykeji.top/gtchykvrfo.html

[M05] 设置退出码
来源：http://hz.iojbl.cn/gtidknpudx.html

Py:   sys.exit(1)
来源：http://hz.guannengcc.top/gtayiecxes.html

PHP:  exit(1);
来源：http://hz.chenlongwang.top/gtgpwbtgsi.html

JS:   process.exit(1)
来源：http://hz.sufxvd.cn/gtzdkasgyk.html

TS:   process.exit(1)
来源：http://hz.yonumen.top/gtoivgaipj.html

Java: System.exit(1)
来源：http://hz.zhixingplan.top/gtzkhcvdei.html

Go:   os.Exit(1)
来源：http://hz.jqgfzy.top/gtlgndtrvh.html

Ruby: exit 1
来源：http://hz.daxiang520.top/gttqrpsull.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.fengsongda.top/gtuvwhhmrv.html

[M06] 向标准错误输出
来源：http://hz.xuetiantiany.cn/gtywgejtpb.html

Py:   print("err", file=sys.stderr)
来源：http://hz.jqgfzy.top/gthiptwopl.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.shzxlz.cn/gtsobwbtrg.html

JS:   console.error("err")
来源：http://hz.nwbrower.top/gtcehmwusn.html

TS:   console.error("err")
来源：http://hz.chenzaomai.com/gtwckcvafn.html

Java: System.err.println("err")
来源：http://hz.hammf.cn/gtbkvgdfmb.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.fzhhl.top/gtyqnyqgtg.html

Ruby: warn "err"
来源：http://hz.yj20258.top/gtifrvsggg.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.nanxuanxn.top/gtxrtdaava.html

[M07] 判断是否为主入口
来源：http://hz.ywan-chungtsiang.top/gtmhrgqedo.html

Py:   if __name__ == "__main__":
来源：http://hz.jianghu66.top/gtrflnepit.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.ywan-chungtsiang.top/gtqsorceqj.html

JS:   require.main === module
来源：http://hz.chenjidiqi.icu/gtsqdysiet.html

TS:   require.main === module
来源：http://hz.xuanzx.com/gtomjwfuvl.html

Java: public static void main(String[] args)
来源：http://hz.redwolf501.top/gtuabqeton.html

Go:   func main()
来源：http://hz.jinghuilouyu.cn/gtlqppoxvj.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.jinyuanbaomall.cn/gtcbpdiagi.html

C#:   static void Main(string[] args)
来源：http://hz.yuanzhike.top/gtibweespu.html

[M08] 获取系统与运行时信息
来源：http://hz.nwbrower.top/gttscztwjp.html

Py:   platform.system();  platform.python_version()
来源：http://hz.svipenyu.cn/gthfuqeeul.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.tianlin.xyz/gtmlnmlkeb.html

JS:   process.platform;  process.version
来源：http://hz.ybcxt.top/gtydzmhfji.html

TS:   process.platform;  process.version
来源：http://hz.ydzc1.top/gtnsueqfgj.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.pengpengdd.cyou/gtnsavxfla.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.kuanghao11.cn/gtrutuaqjb.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.yangfankeji.com/gtazlxtldx.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.yanxiufei.cn/gtmcanbnsg.html

================================================================================
来源：http://hz.cdnleiting.top/gtqyslypkz.html

N. 数据结构与算法
来源：http://hz.nwbrower.top/gtydmgikjg.html

================================================================================
来源：http://hz.chenlongwang.top/gtsfcivfxn.html

[N01] 二分查找（有序数组）
来源：http://hz.xingfuxueyuan.xyz/gtpbjutbww.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.haohaochexian.top/gtgqlsywov.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.yj20258.top/gtqdaycxhp.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.316326.xyz/gtkucyofjp.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.cdnleiting.top/gtltialcqs.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.ybcxt.top/gtofjxnqdi.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.cqqwz.cn/gteuycyglp.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.c1oappe.top/gthpzhysxp.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.9152youxi.cn/gtwqpmvkvp.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.ybcxt.top/gtpubqlkvx.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.cqqwz.cn/gtdylcpsbx.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.xziqi.cn/gtdttbxhzg.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.sweek.top/gtcduuulwx.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.andypj.xyz/gtufzdtmit.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.ydjk.org.cn/gtnzsmncww.html

Go:   slices.Sort(arr)
来源：http://hz.ybcxt.top/gtavuvgyjq.html

Ruby: arr.sort
来源：http://hz.zhiwuduotai.top/gttwublxxe.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.smart0.xyz/gtbnaszgja.html

[N03] 快速排序（分治示例）
来源：http://hz.yj202588.top/gtgclidpuv.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.hammf.cn/gtcxjtzash.html

PHP:  // 递归实现，或用 usort
来源：http://hz.zhixingplan.top/gtzzgqvvfb.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jinqigufen.top/gtnlgenuai.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.vqdsnc.cn/gtmeohmfjp.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.yueranfly.top/gtwpjcduih.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.ppjwa.cn/gtusnvpmme.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.yonumen.top/gttdjxywjh.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.svipenyu.cn/gtiywwpnid.html

[N04] 斐波那契数列
来源：http://hz.shuidangran.top/gtchetddaf.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.jqgfzy.top/gtnjmxwegr.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.yangfankeji.com/gtptlncvrn.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.xingfuxueyuan.xyz/gtobhmciuc.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.cashguo.top/gtjbwhhjov.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.iojbl.cn/gtnsgdxkqs.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.feifeiyinyue.top/gthrwcwcnq.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.yuxming.cn/gtdwtngjmi.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.cashguo.top/gtqnvmqutn.html

[N05] 最大公约数
来源：http://hz.chenlongwang.top/gtuzsvdwtc.html

Py:   math.gcd(a, b)
来源：http://hz.ywan-chungtsiang.top/gtrijcyqhl.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.snrcjt.cn/gtgxlkouft.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.fzhhl.top/gtnwgyyidq.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jinghuilouyu.cn/gtecgypdqj.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.haohaochexian.top/gtzdpwqzgy.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.hysaishi.cn/gtvqsrhvym.html

Ruby: a.gcd(b)
来源：http://hz.gotoacloud.top/gtscveqprs.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.zhiwuduotai.top/gtspxtxcwc.html

[N06] 判断回文字符串
来源：http://hz.ywan-chungtsiang.top/gtdmtwytsn.html

Py:   s == s[::-1]
来源：http://hz.zhongyouzk.top/gtgmziekmq.html

PHP:  $s === strrev($s);
来源：http://hz.ydjk.org.cn/gtwnsgwuex.html

JS:   s === [...s].reverse().join("")
来源：http://hz.nanxinkj.top/gtrpbszdjs.html

TS:   s === [...s].reverse().join("")
来源：http://hz.aizwys.cn/gtrkopnmkp.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.hywenlv.cn/gtwqkawxgy.html

Go:   // 双指针从两端比较
来源：http://hz.zhixingplan.top/gtgynjrrbp.html

Ruby: s == s.reverse
来源：http://hz.ivvv.top/gtdpoybqqk.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.jiagoushi.top/gtlckrlbyh.html

[N07] 两数之和（返回下标）
来源：http://hz.aizwys.cn/gtfivmuzin.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.feifeiyinyue.top/gtvpurwnkq.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.zhengqikj.top/gtccprjeme.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.zdqjudy.top/gthlxsovuw.html

TS:   // 手写 Map<string, number>
来源：http://hz.quarkkingdee.top/gtqhgctfoa.html

Java: // 手写 HashMap
来源：http://hz.jyoumei.cn/gttezhdoxz.html

Go:   // 手写 map[int]int
来源：http://hz.jlsjyb.cn/gtmpxpxjbd.html

Ruby: // 手写 Hash
来源：http://hz.yvedp.cn/gtjkpoadjz.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.jlsjyb.cn/gtabmqoqrt.html

[N08] 生成全排列
来源：http://hz.yanxiufei.cn/gtxalbymtm.html

Py:   itertools.permutations(arr)
来源：http://hz.zhijiandao.cn/gtmkrmpbfj.html

PHP:  // 手写递归交换
来源：http://hz.shzxlz.cn/gthxwukbul.html

JS:   // 手写回溯递归
来源：http://hz.jianghu66.top/gtjpvrsiae.html

TS:   // 手写回溯递归
来源：http://hz.cashguo.top/gtqfywwuro.html

Java: // 手写回溯递归
来源：http://hz.ywan-chungtsiang.top/gtxpkqfdfg.html

Go:   // 手写回溯递归
来源：http://hz.pycfn.com/gtxqsickps.html

Ruby: arr.permutation.to_a
来源：http://hz.mhx1999.top/gtktxjulyb.html

C#:   // 手写回溯递归
来源：http://hz.smart0.xyz/gtrixgjqha.html

[N09] 栈与队列
来源：http://hz.xziqi.cn/gtnylftymh.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.ydzc1.top/gtqkwgwsmy.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.yonumen.top/gtipnzszli.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.52xcode.cn/gtqlzyumfm.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.ivvv.top/gtefohfuhw.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.xingfuxueyuan.xyz/gtfsjcwcpd.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.nwbrower.top/gtdprmwwsk.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.tanke756.top/gtlbgiryme.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.ppjwa.cn/gtyhlwhpjv.html

[N10] 链表节点定义
来源：http://hz.jiagoushi.top/gtxeiyhytc.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.iojbl.cn/gtqotewwgn.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.wangdashe.top/gtloldibmn.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.zhixingplan.top/gtajbtnuua.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.fzhhl.top/gtuprwgfmo.html

Java: class Node { int v; Node next; }
来源：http://hz.zycfv.cn/gtybhdvkzd.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.haohaochexian.top/gtwutkvthk.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.yuxming.cn/gtxopdlvtr.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.sufxvd.cn/gtjarlyfqd.html

[N11] 二叉树中序遍历
来源：http://hz.bjfxy.top/gtowxqhpac.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.gzhubu.top/gtryrfmybk.html

PHP:  // 手写递归函数
来源：http://hz.havefunace.top/gtzsyorlxe.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yuxming.cn/gtcntylowc.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yangfankeji.com/gttzotgpjj.html

Java: // 手写递归
来源：http://hz.zhijiandao.cn/gteilgqxtl.html

Go:   // 手写递归
来源：http://hz.zhixingplan.top/gtzwvuxvux.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.feifeiyinyue.top/gtobcpwrvb.html

C#:   // 手写递归
来源：http://hz.hammf.cn/gtumebzdwf.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.ywan-chungtsiang.top/gtqacyfdzm.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.hnqzz.top/gtzctjnlvs.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.haohaochexian.top/gtwxohiecj.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.zdqjudy.top/gtejsvzatg.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yanxiufei.cn/gtwnhapjjo.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.vqdsnc.cn/gtmwggqpco.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.yuxming.cn/gtnlrufgvf.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.0kj1m.cn/gtaklzdqny.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.daxiang520.top/gtjeigfkfd.html

================================================================================
来源：http://hz.ppjwa.cn/gtizisxlcp.html

O. 并发与异步
来源：http://hz.jianghu66.top/gtndtqnxwo.html

================================================================================
来源：http://hz.cucudq.cn/gtijpnhsje.html

[O01] 启动一个线程
来源：http://hz.xylfe.cn/gtohvvqdio.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.gotoacloud.top/gtnqckzsrm.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.jlsjyb.cn/gtwucxudrw.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.aizwys.cn/gtoxpudrpg.html

TS:   // 同 JS
来源：http://hz.kuanghao11.cn/gtrllnzwym.html

Java: new Thread(() -> f()).start()
来源：http://hz.jinqigufen.top/gtwbrbuayf.html

Go:   go f()
来源：http://hz.jianghu66.top/gtfnfopjat.html

Ruby: Thread.new { f }
来源：http://hz.meibo888.top/gtdhlhztwy.html

C#:   Task.Run(() => F());
来源：http://hz.sweek.top/gtkgbbpokr.html

[O02] 使用线程池
来源：http://hz.cucudq.cn/gtxjjwzpzx.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.yuanzhike.top/gtgashtpkp.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.ivvv.top/gtmiixehyg.html

JS:   // worker_threads 线程池
来源：http://hz.zhengqikj.top/gtzaxfabfx.html

TS:   // worker_threads 线程池
来源：http://hz.pengpengdd.cyou/gttxgcvenq.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.jiagoushi.top/gtolfpcfjl.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.iojbl.cn/gthihdqjgw.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.aibaodan.cn/gtaqazkouv.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.xinyue.icu/gtuxflfkdv.html

[O03] 加锁保护共享数据
来源：http://hz.jiagoushi.top/gtkbnxlshb.html

Py:   with lock: shared += 1
来源：http://hz.tanke756.top/gtfnrikmlz.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.wangshuangyany.cn/gtngmcbawv.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.c1oappe.top/gtdhbxqogg.html

TS:   // 同 JS
来源：http://hz.zdqjudy.top/gtljkaqfsk.html

Java: synchronized (this) { shared++; }
来源：http://hz.andypj.xyz/gtizlsvoat.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.ivvv.top/gtavydpwlt.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.aizwys.cn/gthdjyinhb.html

C#:   lock (gate) { shared++; }
来源：http://hz.daxiang520.top/gtgbzniawl.html

[O04] 定义异步函数并等待
来源：http://hz.havefunace.top/gtazxohumy.html

Py:   async def f():⏎    await g()
来源：http://hz.jqgfzy.top/gtidaeqtqe.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.gotoacloud.top/gtrrphdprk.html

JS:   async function f() { await g(); }
来源：http://hz.dashuyun.cn/gtqyrtpvqm.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.ywan-chungtsiang.top/gttpdipqbp.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.wangdashe.top/gtbqpwqvyy.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.shanyushiyangkeji.top/gtlubttcnv.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.pengpengdd.cyou/gtynbjevef.html

C#:   async Task F() { await G(); }
来源：http://hz.hnqzz.top/gtxfumwpzx.html

[O05] 并发执行并等待全部完成
来源：http://hz.quarkkingdee.top/gtzreixbud.html

Py:   asyncio.gather(*tasks)
来源：http://hz.cqqwz.cn/gtwutnvuct.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.shzxlz.cn/gtbdsuqsyn.html

JS:   await Promise.all(tasks)
来源：http://hz.yonumen.top/gtticzgntd.html

TS:   await Promise.all(tasks)
来源：http://hz.mhx1999.top/gtuljqjotn.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.wangdashe.top/gtgsayduhk.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.jianghu66.top/gtlpygwdus.html

Ruby: threads.map(&:join)
来源：http://hz.vqdsnc.cn/gtxwgvojtf.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.dianchejie.cn/gteqbbcsir.html

[O06] 使用进程池
来源：http://hz.xuanzx.com/gtkzqdczhw.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.xingfuxueyuan.xyz/gtwdstrkbo.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.xingfuxueyuan.xyz/gtskbyaokp.html

JS:   // child_process / cluster 模块
来源：http://hz.ybcxt.top/gtbwenqczf.html

TS:   // child_process / cluster 模块
来源：http://hz.shangyingyoupin.top/gtvhtwimuk.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.gzhubu.top/gtkpufjtcu.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.jinghuilouyu.cn/gtvnemwvmz.html

Ruby: // fork 块
来源：http://hz.zdqjudy.top/gtfzwdubot.html

C#:   Parallel.For
来源：http://hz.yuanzhike.top/gtiycjvoio.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtojstbjvw.html

P. 常用工具函数
来源：http://hz.vqdsnc.cn/gtqkvmaemu.html

================================================================================
来源：http://hz.ydjk.org.cn/gtdomeewrm.html

[P01] 生成 UUID
来源：http://hz.smart0.xyz/gtcsklazsv.html

Py:   str(uuid.uuid4())
来源：http://hz.sysykeji.top/gtxtrkazfu.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.dashuyun.cn/gtdzsyanhm.html

JS:   crypto.randomUUID()
来源：http://hz.quarkkingdee.top/gtrqfetemt.html

TS:   crypto.randomUUID()
来源：http://hz.hnxiangtu.top/gtxdfrtbxc.html

Java: UUID.randomUUID().toString()
来源：http://hz.cashguo.top/gtxgqrlsfa.html

Go:   // 用 github.com/google/uuid
来源：http://hz.andypj.xyz/gtxftzpror.html

Ruby: SecureRandom.uuid
来源：http://hz.ehwqpu.com/gtqmiewpug.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.zdqjudy.top/gtjcqyfmls.html

[P02] MD5 / SHA256 摘要
来源：http://hz.ydjk.org.cn/gtpocvdghk.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.gotoacloud.top/gthmqlgupn.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.yanxiufei.cn/gtudozzbho.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.zycfv.cn/gtethumlsv.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.jyoumei.cn/gtytrfoekp.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.shuidangran.top/gtloanjmyk.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.chenzaomai.com/gtsbizunce.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.cucudq.cn/gtrdhzamqn.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.jinyuanbaomall.cn/gtjesqpvte.html

[P03] 生成短随机字符串
来源：http://hz.ydjk.org.cn/gtwqpqapec.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.jinyuanbaomall.cn/gtiutciayv.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.feifeiyinyue.top/gtdizjukpb.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.zdqjudy.top/gtocsqnqyk.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.xuetiantiany.cn/gtksqwwjah.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.gotoacloud.top/gtnjmlzjdi.html


<!-- 参考信息 -->