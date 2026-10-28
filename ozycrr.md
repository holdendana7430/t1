代发 wailian999

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.kuanghao11.cn/gtavvdeztr.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.shanyushiyangkeji.top/gtwqwmvqsc.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.xziqi.cn/gtnmbbmszp.html

[L06] 解析响应为 JSON
来源：http://hz.yuanzhike.top/gtkluembey.html

Py:   resp.json()
来源：http://hz.xziqi.cn/gtcglumejx.html

PHP:  json_decode($body, true);
来源：http://hz.gotoacloud.top/gtrxvufqcq.html

JS:   await resp.json()
来源：http://hz.ydjk.org.cn/gtykuojsic.html

TS:   await resp.json()
来源：http://hz.shanyushiyangtech.top/gtkbcfjzzu.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.zhijiandao.cn/gtunynuacu.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.zycfv.cn/gtrfyfibrr.html

Ruby: JSON.parse(resp.body)
来源：http://hz.zdqjudy.top/gttmohmche.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.jiagoushi.top/gttldvjexr.html

[L07] 处理 HTTP 状态码
来源：http://hz.sufxvd.cn/gtopntpxak.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.aizwys.cn/gtbuipbijg.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.jinqigufen.top/gtennnfvne.html

JS:   resp.ok;  resp.status
来源：http://hz.316326.xyz/gtvxfvplox.html

TS:   resp.ok;  resp.status
来源：http://hz.0kj1m.cn/gtrlgiubom.html

Java: resp.statusCode()
来源：http://hz.andypj.xyz/gtyinavffa.html

Go:   resp.StatusCode
来源：http://hz.gogol.net.cn/gtrzyvjthf.html

Ruby: resp.code.to_i
来源：http://hz.xylfe.cn/gtjhjepltj.html

C#:   (int)resp.StatusCode
来源：http://hz.c1oappe.top/gtuhdieamp.html

[L08] 并发请求多个地址
来源：http://hz.jinqigufen.top/gtthbyajsg.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.wangshuangyany.cn/gtvxwpghqt.html

PHP:  curl_multi_init() 系列
来源：http://hz.wangshuangyany.cn/gtkgnijmxl.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.ppjwa.cn/gttazshzbk.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.316326.xyz/gtyyyetztc.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.sufxvd.cn/gtvwxnyzpj.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.yj202588.top/gtfctctceh.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.yanxiufei.cn/gtnrukolqt.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.jinqigufen.top/gtylvrqgre.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtjzxixcmf.html

M. 命令行 / 进程 / 环境
来源：http://hz.hongshengwenyu.top/gtzqgpwidb.html

================================================================================
来源：http://hz.ehwqpu.com/gtuyysjotj.html

[M01] 读取命令行参数
来源：http://hz.guannengcc.top/gttgzqtthj.html

Py:   sys.argv[1:]
来源：http://hz.hammf.cn/gttztbfnmi.html

PHP:  $argv;  $argc;
来源：http://hz.dianchejie.cn/gtpcsudbns.html

JS:   process.argv.slice(2)
来源：http://hz.0kj1m.cn/gtoxizxygs.html

TS:   process.argv.slice(2)
来源：http://hz.nanxinkj.top/gtxrgitbwr.html

Java: args 数组（main 方法参数）
来源：http://hz.pengpengdd.cyou/gtwshcrkkq.html

Go:   os.Args[1:]
来源：http://hz.zhongyouzk.top/gtzadlflsm.html

Ruby: ARGV
来源：http://hz.nanxinkj.top/gtlwudmjzy.html

C#:   args 数组（Main 方法参数）
来源：http://hz.cheryme.top/gtiltyhqeq.html

[M02] 读取环境变量
来源：http://hz.bjfxy.top/gtwxsvafjm.html

Py:   os.environ.get("HOME")
来源：http://hz.chenjidiqi.icu/gtrkqpchpa.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.guowangkeji.top/gtpnqmemvf.html

JS:   process.env.HOME
来源：http://hz.shuidangran.top/gtoawneyjt.html

TS:   process.env.HOME
来源：http://hz.fengsongda.top/gtqrqheucm.html

Java: System.getenv("HOME")
来源：http://hz.zhiwuduotai.top/gtwpzsgmwe.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.fzhhl.top/gtasczrdbe.html

Ruby: ENV["HOME"]
来源：http://hz.yj20258.top/gtukettcxt.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.hfpthk.cn/gtfwxocscs.html

[M03] 执行外部命令
来源：http://hz.svipenyu.cn/gtngjxlyjf.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.xylfe.cn/gtkvdzzqrd.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.52xcode.cn/gtbguprhrl.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.redwolf501.top/gtbcydclwm.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.shangyingyoupin.top/gtyvhuauoa.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.hongshengwenyu.top/gtvczvovee.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.hongshengwenyu.top/gtgbfaqxlw.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.sysykeji.top/gtygnchsxm.html

C#:   Process.Start("ls", "-l");
来源：http://hz.xylfe.cn/gtmxbckods.html

[M04] 获取当前工作目录
来源：http://hz.shangyingyoupin.top/gtaybmncjk.html

Py:   os.getcwd()
来源：http://hz.snrcjt.cn/gtbqztjmme.html

PHP:  getcwd();
来源：http://hz.yj20258888.top/gtcbnszxsw.html

JS:   process.cwd()
来源：http://hz.nanxinkj.top/gtpufrfort.html

TS:   process.cwd()
来源：http://hz.nanxuanxn.top/gtgzjqgqqo.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.jqgfzy.top/gtakbpnyfz.html

Go:   os.Getwd()
来源：http://hz.guannengcc.top/gttpuhohaq.html

Ruby: Dir.pwd
来源：http://hz.aizwys.cn/gthantdfqv.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.iojbl.cn/gthkpqfgkm.html

[M05] 设置退出码
来源：http://hz.shangyingyoupin.top/gtonrosqit.html

Py:   sys.exit(1)
来源：http://hz.haohaochexian.top/gtfdxcthug.html

PHP:  exit(1);
来源：http://hz.daria6918.cn/gtxrpixgge.html

JS:   process.exit(1)
来源：http://hz.jqgufenzy.top/gtxuodnljc.html

TS:   process.exit(1)
来源：http://hz.xuetiantiany.cn/gtyypzfoyg.html

Java: System.exit(1)
来源：http://hz.hywenlv.cn/gtwwkyngjl.html

Go:   os.Exit(1)
来源：http://hz.jlsjyb.cn/gtwogxolvb.html

Ruby: exit 1
来源：http://hz.hnqzz.top/gttbgoxrdj.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.ydjk.org.cn/gtmojbqiin.html

[M06] 向标准错误输出
来源：http://hz.guowangkeji.top/gtlajexwxn.html

Py:   print("err", file=sys.stderr)
来源：http://hz.nwbrower.top/gtnutikcfe.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.chenzaomai.com/gtorenfdfk.html

JS:   console.error("err")
来源：http://hz.zhijiandao.cn/gtjvctpwha.html

TS:   console.error("err")
来源：http://hz.yuanzhike.top/gtchtsgkie.html

Java: System.err.println("err")
来源：http://hz.nwbrower.top/gtqoawvsck.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.zhoulong.xyz/gttdtilvul.html

Ruby: warn "err"
来源：http://hz.zdqjudy.top/gtieycztfx.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.haohaochexian.top/gtysafwejb.html

[M07] 判断是否为主入口
来源：http://hz.hammf.cn/gtledkzvdf.html

Py:   if __name__ == "__main__":
来源：http://hz.0kj1m.cn/gthmahwmuy.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.aizwys.cn/gtkqmribou.html

JS:   require.main === module
来源：http://hz.chenlongwang.top/gtmwwconti.html

TS:   require.main === module
来源：http://hz.jinqigfzy.top/gtsprbjkji.html

Java: public static void main(String[] args)
来源：http://hz.tanke756.top/gtbljqsyea.html

Go:   func main()
来源：http://hz.ydzc1.top/gtzfxnmurt.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.shanyushiyangtech.top/gtngettdrk.html

C#:   static void Main(string[] args)
来源：http://hz.52xcode.cn/gtvlruiosu.html

[M08] 获取系统与运行时信息
来源：http://hz.hywenlv.cn/gttfkthtac.html

Py:   platform.system();  platform.python_version()
来源：http://hz.jinyuanbaomall.cn/gtsfjijvka.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.52xcode.cn/gtdjjwprrz.html

JS:   process.platform;  process.version
来源：http://hz.jqgfzy.top/gtshbulczb.html

TS:   process.platform;  process.version
来源：http://hz.shuidangran.top/gtxwqdodxo.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.gogol.net.cn/gthcqgoexj.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.cqqwz.cn/gtacbnlwnz.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.9152youxi.cn/gtzxamhdwb.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.hnqzz.top/gtnnhoguwk.html

================================================================================
来源：http://hz.zhongyouzk.top/gtlfkxqdkx.html

N. 数据结构与算法
来源：http://hz.svipenyu.cn/gtwejbsykq.html

================================================================================
来源：http://hz.ivvv.top/gtqrzyyizw.html

[N01] 二分查找（有序数组）
来源：http://hz.yongpay.top/gtsbkmonui.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.feifeiyinyue.top/gtvaxudxlr.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.hfpthk.cn/gtanpeiwas.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zycfv.cn/gtzgltkwuo.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.kuanghao11.cn/gteebkdewv.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.c1oappe.top/gtzfgcmnnt.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.svipenyu.cn/gtkvreircy.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.daria6918.cn/gtiukiakvp.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.jqgfzy.top/gtjytcgiab.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.gotoacloud.top/gtntarwvlm.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.ywan-chungtsiang.top/gtqqddjuld.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.jyoumei.cn/gthbtisdfn.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.dianchejie.cn/gtihdwcuna.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.gaohongyu789.top/gtdnldkifc.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.shanyushiyangkeji.top/gtlqkrdlgh.html

Go:   slices.Sort(arr)
来源：http://hz.cheryme.top/gtjxcjllwz.html

Ruby: arr.sort
来源：http://hz.zhixingplan.top/gtwpthvcro.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.jianghu66.top/gtqayiwcna.html

[N03] 快速排序（分治示例）
来源：http://hz.yueranfly.top/gtellkuyse.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.fengsongda.top/gtpdwdpjmj.html

PHP:  // 递归实现，或用 usort
来源：http://hz.smart0.xyz/gtaqsjdhzv.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.haohaochexian.top/gtszsyziwi.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.gogol.net.cn/gtepcctphk.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.jianghu66.top/gtjlxutsud.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.snrcjt.cn/gtaxvgrllb.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.havefunace.top/gtpmbiecjm.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.zycfv.cn/gtxdrjowxf.html

[N04] 斐波那契数列
来源：http://hz.fzhhl.top/gtsyfnzjyi.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.pengpengdd.cyou/gtcqrawxii.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.dianchejie.cn/gtuytirpuq.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.haohaochexian.top/gtzbhfqfnf.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.hnxiangtu.top/gtyytcorti.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.gogol.net.cn/gtfhgcbygi.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.birdmap.top/gtkjhkhbtw.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.tanke756.top/gtivybookj.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.andypj.xyz/gtfklwuqyh.html

[N05] 最大公约数
来源：http://hz.guannengcc.top/gtbluabybl.html

Py:   math.gcd(a, b)
来源：http://hz.52xcode.cn/gtqmbzrcbo.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.xuanzx.com/gtrzklvnfd.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.nanxuanxn.top/gtsllxbhin.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.pycfn.com/gtyjafnada.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.dianchejie.cn/gtlvngittl.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.feifeiyinyue.top/gtvfhsrtoi.html

Ruby: a.gcd(b)
来源：http://hz.yuxming.cn/gthtvtzimk.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.yueranfly.top/gtvglxnrev.html

[N06] 判断回文字符串
来源：http://hz.cucudq.cn/gttvvfiwtu.html

Py:   s == s[::-1]
来源：http://hz.ydjk.org.cn/gtmhybofgi.html

PHP:  $s === strrev($s);
来源：http://hz.zhengqikj.top/gtenkqvfub.html

JS:   s === [...s].reverse().join("")
来源：http://hz.cheryme.top/gtggycvbyp.html

TS:   s === [...s].reverse().join("")
来源：http://hz.havefunace.top/gtjcenythm.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.cucudq.cn/gtpxvxiavv.html

Go:   // 双指针从两端比较
来源：http://hz.ydzc1.top/gtpcspxjij.html

Ruby: s == s.reverse
来源：http://hz.tian-w.cn/gtkzsvmema.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.gaohongyu789.top/gtqixtcpog.html

[N07] 两数之和（返回下标）
来源：http://hz.dashuyun.cn/gtxcwldylx.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.tanke756.top/gtgnvfnrvx.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.hywenlv.cn/gtuxnlmnbe.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.xingfuxueyuan.xyz/gtphqafyry.html

TS:   // 手写 Map<string, number>
来源：http://hz.0kj1m.cn/gtqshfhpvk.html

Java: // 手写 HashMap
来源：http://hz.sxryk.cn/gtidqowjjq.html

Go:   // 手写 map[int]int
来源：http://hz.pengpengdd.cyou/gtbswlkybs.html

Ruby: // 手写 Hash
来源：http://hz.iojbl.cn/gtezqmhdmp.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.mhx1999.top/gtcmgyabqs.html

[N08] 生成全排列
来源：http://hz.cdnleiting.top/gtulhunprr.html

Py:   itertools.permutations(arr)
来源：http://hz.svipenyu.cn/gtjpbdvbee.html

PHP:  // 手写递归交换
来源：http://hz.jinghuilouyu.cn/gtmeayymfy.html

JS:   // 手写回溯递归
来源：http://hz.shangyingyoupin.top/gthsudkyjl.html

TS:   // 手写回溯递归
来源：http://hz.sysykeji.top/gtgyxhxxfm.html

Java: // 手写回溯递归
来源：http://hz.shuidangran.top/gtcdsebqtx.html

Go:   // 手写回溯递归
来源：http://hz.iojbl.cn/gtktcivheg.html

Ruby: arr.permutation.to_a
来源：http://hz.tanke756.top/gttmkiimfy.html

C#:   // 手写回溯递归
来源：http://hz.shanyushiyangkeji.top/gtsbgmqeql.html

[N09] 栈与队列
来源：http://hz.nwbrower.top/gtnlmfrdad.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.cqqwz.cn/gtmjpoeiti.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.daria6918.cn/gtflxmhsmx.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.ybcxt.top/gtlfvhmqpe.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.cucudq.cn/gtipynxlha.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.jinghuilouyu.cn/gterszjutu.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.yueranfly.top/gtsztmimut.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.wangdashe.top/gtxfgrbpie.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.yuxming.cn/gtydtxkxqa.html

[N10] 链表节点定义
来源：http://hz.cheryme.top/gtljslowto.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.shzxlz.cn/gtjuomrcdp.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.tian-w.cn/gtveqjnbbz.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.ywan-chungtsiang.top/gtdcmjdpjt.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.bjfxy.top/gtxayzadem.html

Java: class Node { int v; Node next; }
来源：http://hz.jinqigfzy.top/gtndzzwigj.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.yuxming.cn/gtdayzyrax.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.yj20258888.top/gtzjoiffhy.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.gzhubu.top/gtqfgbtzdi.html

[N11] 二叉树中序遍历
来源：http://hz.xuetiantiany.cn/gtwexmqbst.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.hysaishi.cn/gtpojnhcxq.html

PHP:  // 手写递归函数
来源：http://hz.yonumen.top/gtrtqnrzxe.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.52xcode.cn/gtqribahck.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.ppjwa.cn/gtdozayqpz.html

Java: // 手写递归
来源：http://hz.hfpthk.cn/gtrfgachwl.html

Go:   // 手写递归
来源：http://hz.birdmap.top/gtmiwshelv.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.sufxvd.cn/gtbarptsaw.html

C#:   // 手写递归
来源：http://hz.jinqigufen.top/gthhkdrtnh.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.xinyue.icu/gtrlzsosjh.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.zhixingplan.top/gtzydycfbr.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.zhengqikj.top/gtclwdytch.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.cdnleiting.top/gtyvzgcecd.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.svipenyu.cn/gtdrzzjdzb.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.hysaishi.cn/gtqtixqumo.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.bjfxy.top/gtocowytev.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.yj20258.top/gtejsdzfoy.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.ydjk.org.cn/gthtxzhzip.html

================================================================================
来源：http://hz.hysaishi.cn/gtqslxfqbz.html

O. 并发与异步
来源：http://hz.zhoulong.xyz/gtsitcudch.html

================================================================================
来源：http://hz.zhengqikj.top/gtkueakfko.html

[O01] 启动一个线程
来源：http://hz.yuanzhike.top/gtmaygfjgs.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.shanyushiyangkeji.top/gtboxnisnc.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.haohaochexian.top/gtpbgivxmw.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.hfpthk.cn/gtewwsmezh.html

TS:   // 同 JS
来源：http://hz.andypj.xyz/gttzmagtrx.html

Java: new Thread(() -> f()).start()
来源：http://hz.sysykeji.top/gtuakwwowo.html

Go:   go f()
来源：http://hz.sufxvd.cn/gtezxhdxvl.html

Ruby: Thread.new { f }
来源：http://hz.nanxuanxn.top/gtcpbuvsvd.html

C#:   Task.Run(() => F());
来源：http://hz.zhixingplan.top/gtwxcctvtm.html

[O02] 使用线程池
来源：http://hz.gzhubu.top/gtynttpuvp.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.pengpengdd.cyou/gtpptejjzx.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.jiagoushi.top/gtpbdaadyz.html

JS:   // worker_threads 线程池
来源：http://hz.hnqzz.top/gtfjjfukwd.html

TS:   // worker_threads 线程池
来源：http://hz.vqdsnc.cn/gteehockgp.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.jinyuanbaomall.cn/gtcewmzwww.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.gzhubu.top/gtntgaqyyx.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.andypj.xyz/gthhpfubcp.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.zhijiandao.cn/gtyxvhrxxn.html

[O03] 加锁保护共享数据
来源：http://hz.hongshengwenyu.top/gtrloocjpo.html

Py:   with lock: shared += 1
来源：http://hz.xuetiantiany.cn/gttkprfvbs.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.fzhhl.top/gtnargbzyw.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.zycfv.cn/gtoiurcbhr.html

TS:   // 同 JS
来源：http://hz.shanyushiyangkeji.top/gthldnjahq.html

Java: synchronized (this) { shared++; }
来源：http://hz.tianlin.xyz/gtoicbnucq.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.gaohongyu789.top/gterrmsvkj.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.yueranfly.top/gtmsuthdul.html

C#:   lock (gate) { shared++; }
来源：http://hz.yj20258888.top/gtouetmxns.html

[O04] 定义异步函数并等待
来源：http://hz.zhijiandao.cn/gtduesnkvv.html

Py:   async def f():⏎    await g()
来源：http://hz.sxryk.cn/gtxgfxolds.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.sufxvd.cn/gtzmxuqauy.html

JS:   async function f() { await g(); }
来源：http://hz.zycfv.cn/gtxjqiuiar.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.yongpay.top/gtfkfspaza.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.316326.xyz/gtvfnpxpik.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.yj202588.top/gtgtppgklc.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.guannengcc.top/gtkpvhowpn.html

C#:   async Task F() { await G(); }
来源：http://hz.sysykeji.top/gtkyndsetr.html

[O05] 并发执行并等待全部完成
来源：http://hz.ppjwa.cn/gtblqlosbb.html

Py:   asyncio.gather(*tasks)
来源：http://hz.jiagoushi.top/gtxqyhgbje.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.zycfv.cn/gttntdzjgo.html

JS:   await Promise.all(tasks)
来源：http://hz.52xcode.cn/gtplqwmlpr.html

TS:   await Promise.all(tasks)
来源：http://hz.shanyushiyangtech.top/gtkldoppbh.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.shangyingyoupin.top/gtvmgspdcg.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.shangyingyoupin.top/gthlmjimeg.html

Ruby: threads.map(&:join)
来源：http://hz.wangdashe.top/gtshsxmpqu.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.yonumen.top/gtlzunnduw.html

[O06] 使用进程池
来源：http://hz.dianchejie.cn/gtookjdfoh.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.zhijiandao.cn/gtiyfkzyes.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.gogol.net.cn/gtuaxdhwyl.html

JS:   // child_process / cluster 模块
来源：http://hz.gaohongyu789.top/gtavqjqdgw.html

TS:   // child_process / cluster 模块
来源：http://hz.ivvv.top/gtghuzxxlf.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.daria6918.cn/gtwqetnvdv.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.andypj.xyz/gtmmvliqqd.html

Ruby: // fork 块
来源：http://hz.nanxinkj.top/gtxwsjeacs.html

C#:   Parallel.For
来源：http://hz.zhongyouzk.top/gtujmbqpvh.html

================================================================================
来源：http://hz.bjfxy.top/gtiuzhjlun.html

P. 常用工具函数
来源：http://hz.aizwys.cn/gtcmnwoxom.html

================================================================================
来源：http://hz.hysaishi.cn/gtkpyrdyil.html

[P01] 生成 UUID
来源：http://hz.c1oappe.top/gtzkpmczpm.html

Py:   str(uuid.uuid4())
来源：http://hz.ydjk.org.cn/gtoqnvjzhp.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.daria6918.cn/gtcqofcvlm.html

JS:   crypto.randomUUID()
来源：http://hz.shanyushiyangkeji.top/gtndaohfid.html

TS:   crypto.randomUUID()
来源：http://hz.c1oappe.top/gtdeoffxvl.html

Java: UUID.randomUUID().toString()
来源：http://hz.tian-w.cn/gtbgzcffzs.html

Go:   // 用 github.com/google/uuid
来源：http://hz.guannengcc.top/gtnojbfcfs.html

Ruby: SecureRandom.uuid
来源：http://hz.hysaishi.cn/gtyqcprfwo.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.tian-w.cn/gtmuktliad.html

[P02] MD5 / SHA256 摘要
来源：http://hz.haohaochexian.top/gtvufewwac.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.meibo888.top/gtpsvskkkz.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.hongshengwenyu.top/gtwhmwqhdf.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.yj202588.top/gtcigkiuor.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.hnqzz.top/gttuuehkby.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.hammf.cn/gtvcweicmi.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.hnxiangtu.top/gtcgfkiuuz.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.hnqzz.top/gtsfxjikiq.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.hnxiangtu.top/gtgluunkrv.html

[P03] 生成短随机字符串
来源：http://hz.kuanghao11.cn/gtvgaeqfjs.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.chenlongwang.top/gtgjzscmsd.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.xuetiantiany.cn/gtugtzpobw.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.ydzc1.top/gtorbfpstg.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.xuetiantiany.cn/gtmlfoflnr.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.guannengcc.top/gtcrqlutiv.html


<!-- 参考信息 -->