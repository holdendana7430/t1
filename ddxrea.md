代发 wailian999

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.xylfe.cn/gtjkypcopq.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.zycfv.cn/gtpinzykva.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.hnxiangtu.top/gtmrkzqiyf.html

[L06] 解析响应为 JSON
来源：http://hz.zhiwuduotai.top/gthrjdligq.html

Py:   resp.json()
来源：http://hz.gotoacloud.top/gthprfmjup.html

PHP:  json_decode($body, true);
来源：http://hz.sufxvd.cn/gtovxmjxkj.html

JS:   await resp.json()
来源：http://hz.svipenyu.cn/gtuduttlsb.html

TS:   await resp.json()
来源：http://hz.dashuyun.cn/gtbgmaurcd.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.bjfxy.top/gtexrjbslr.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.andypj.xyz/gtjrhfvmkr.html

Ruby: JSON.parse(resp.body)
来源：http://hz.yonumen.top/gtzakrhuqj.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.jlsjyb.cn/gtqeagtsqm.html

[L07] 处理 HTTP 状态码
来源：http://hz.nanxuanxn.top/gtkibfhilu.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.hfpthk.cn/gtkyqityds.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.xingfuxueyuan.xyz/gtkuelphsi.html

JS:   resp.ok;  resp.status
来源：http://hz.daria6918.cn/gtkaetkfeu.html

TS:   resp.ok;  resp.status
来源：http://hz.ywan-chungtsiang.top/gtppmkbcap.html

Java: resp.statusCode()
来源：http://hz.jinqigufen.top/gtnfiqovnk.html

Go:   resp.StatusCode
来源：http://hz.aizwys.cn/gtzszbuidd.html

Ruby: resp.code.to_i
来源：http://hz.nanxuanxn.top/gtzfqgeljq.html

C#:   (int)resp.StatusCode
来源：http://hz.ywan-chungtsiang.top/gtgwwgdirk.html

[L08] 并发请求多个地址
来源：http://hz.yuanzhike.top/gtzvfyznxo.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.aizwys.cn/gtckgmhzzq.html

PHP:  curl_multi_init() 系列
来源：http://hz.zhengqikj.top/gtxxvnxdxx.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.vqdsnc.cn/gtxnknixvt.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.fengsongda.top/gtpppqmgus.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.hysaishi.cn/gtugmldbhb.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.shangyingyoupin.top/gtegamcchx.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.jqgufenzy.top/gtzpowibjw.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.wangshuangyany.cn/gtnztqklcy.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtbescdzmg.html

M. 命令行 / 进程 / 环境
来源：http://hz.gogol.net.cn/gtjwgjtaqk.html

================================================================================
来源：http://hz.snrcjt.cn/gtzelwmuxn.html

[M01] 读取命令行参数
来源：http://hz.xuanzx.com/gtbhvfqmep.html

Py:   sys.argv[1:]
来源：http://hz.zhaomingkeji.xyz/gtkhybwaqf.html

PHP:  $argv;  $argc;
来源：http://hz.aizwys.cn/gtcqzgdcps.html

JS:   process.argv.slice(2)
来源：http://hz.jinghuilouyu.cn/gtrxhrdwej.html

TS:   process.argv.slice(2)
来源：http://hz.c1oappe.top/gtbsbbuvvf.html

Java: args 数组（main 方法参数）
来源：http://hz.hfpthk.cn/gtrizqvbxp.html

Go:   os.Args[1:]
来源：http://hz.hnqzz.top/gthzsmejjc.html

Ruby: ARGV
来源：http://hz.zdqjudy.top/gtinnokfoz.html

C#:   args 数组（Main 方法参数）
来源：http://hz.pengpengdd.cyou/gtbkcbqjwn.html

[M02] 读取环境变量
来源：http://hz.cucudq.cn/gtcppmixqf.html

Py:   os.environ.get("HOME")
来源：http://hz.daria6918.cn/gtaaqarpao.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.fengsongda.top/gtcbnmgxsh.html

JS:   process.env.HOME
来源：http://hz.yueranfly.top/gtcomogepz.html

TS:   process.env.HOME
来源：http://hz.svipenyu.cn/gtwbuamcpg.html

Java: System.getenv("HOME")
来源：http://hz.aizwys.cn/gtpygtfdkb.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.52xcode.cn/gtkackouew.html

Ruby: ENV["HOME"]
来源：http://hz.jyoumei.cn/gtjdwhbmle.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.yuxming.cn/gtwuwrripw.html

[M03] 执行外部命令
来源：http://hz.zycfv.cn/gtpdjfkbgl.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.wangdashe.top/gtykizdqru.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.haohaochexian.top/gtegwicajx.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.c1oappe.top/gtteqdfdjh.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.zhoulong.xyz/gtzxasjjtk.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.ehwqpu.com/gtwmhmkttp.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.sxryk.cn/gtrcjzhjpr.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.dashuyun.cn/gtwcnlvhbu.html

C#:   Process.Start("ls", "-l");
来源：http://hz.c1oappe.top/gttzkkbbhc.html

[M04] 获取当前工作目录
来源：http://hz.jyoumei.cn/gtbkndicdg.html

Py:   os.getcwd()
来源：http://hz.aibaodan.cn/gtkarhjmgp.html

PHP:  getcwd();
来源：http://hz.hnqzz.top/gtboluaswa.html

JS:   process.cwd()
来源：http://hz.52xcode.cn/gtpghhsdik.html

TS:   process.cwd()
来源：http://hz.ydjk.org.cn/gtyjyyazfj.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.hongshengwenyu.top/gtnaucckdx.html

Go:   os.Getwd()
来源：http://hz.tianlin.xyz/gtxxcthzsz.html

Ruby: Dir.pwd
来源：http://hz.meibo888.top/gtynumqpdx.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.nanxuanxn.top/gtuhphmtnd.html

[M05] 设置退出码
来源：http://hz.nanxinkj.top/gtpgapwtgx.html

Py:   sys.exit(1)
来源：http://hz.sufxvd.cn/gtnkpilsao.html

PHP:  exit(1);
来源：http://hz.zycfv.cn/gtaqwxlsjg.html

JS:   process.exit(1)
来源：http://hz.zhoulong.xyz/gtcvncygjl.html

TS:   process.exit(1)
来源：http://hz.pycfn.com/gtdxzogpwp.html

Java: System.exit(1)
来源：http://hz.dianchejie.cn/gtvxpwcede.html

Go:   os.Exit(1)
来源：http://hz.yonumen.top/gtzuzanzgg.html

Ruby: exit 1
来源：http://hz.gzhubu.top/gtrcublisn.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.guannengcc.top/gtemjxdcef.html

[M06] 向标准错误输出
来源：http://hz.birdmap.top/gtnjetvxlw.html

Py:   print("err", file=sys.stderr)
来源：http://hz.xziqi.cn/gtmbinfzvl.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.redwolf501.top/gtihgeaskk.html

JS:   console.error("err")
来源：http://hz.yuanzhike.top/gtdplmlhfl.html

TS:   console.error("err")
来源：http://hz.dashuyun.cn/gtsfakddym.html

Java: System.err.println("err")
来源：http://hz.cucudq.cn/gtsuddtgjp.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.ydjk.org.cn/gtvdekpwfw.html

Ruby: warn "err"
来源：http://hz.jinqigfzy.top/gtwrpfqotl.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.fengsongda.top/gtdedbitnd.html

[M07] 判断是否为主入口
来源：http://hz.ppjwa.cn/gtjulthjnu.html

Py:   if __name__ == "__main__":
来源：http://hz.guannengcc.top/gtddbeabgt.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.wangshuangyany.cn/gtuvbzgchz.html

JS:   require.main === module
来源：http://hz.chenlongwang.top/gtrafeultr.html

TS:   require.main === module
来源：http://hz.sysykeji.top/gtqvzwrteq.html

Java: public static void main(String[] args)
来源：http://hz.ybcxt.top/gtxfneyupi.html

Go:   func main()
来源：http://hz.nwbrower.top/gtsgqrximi.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.zhijiandao.cn/gtmipgbdis.html

C#:   static void Main(string[] args)
来源：http://hz.ydzc1.top/gtmxqcgraw.html

[M08] 获取系统与运行时信息
来源：http://hz.316326.xyz/gtzplmbpef.html

Py:   platform.system();  platform.python_version()
来源：http://hz.sufxvd.cn/gtobgbadfy.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.smart0.xyz/gtkmwundxj.html

JS:   process.platform;  process.version
来源：http://hz.jinqigufen.top/gtdnabigxs.html

TS:   process.platform;  process.version
来源：http://hz.yj202588.top/gthvzxwrah.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.fzhhl.top/gtmfvvqigz.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.aizwys.cn/gtjhowsuoz.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.svipenyu.cn/gtyuyjoyay.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.xuanzx.com/gtbyklesmk.html

================================================================================
来源：http://hz.jlsjyb.cn/gtggkzarhl.html

N. 数据结构与算法
来源：http://hz.52xcode.cn/gtkzklovsq.html

================================================================================
来源：http://hz.zhengqikj.top/gtshxqasss.html

[N01] 二分查找（有序数组）
来源：http://hz.yvedp.cn/gtfwgvoznf.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.gotoacloud.top/gtkwqqdbxm.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.snrcjt.cn/gtnfoxgwmh.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.hammf.cn/gttrxinldt.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.redwolf501.top/gtodoqrrsc.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.hongshengwenyu.top/gtlyemdxxl.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.c1oappe.top/gtklxpunzm.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.chenlongwang.top/gtnrlvoiuz.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.shzxlz.cn/gtvmnwwiwm.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.zhoulong.xyz/gthwvpgnkw.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jlsjyb.cn/gthhohuuoa.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.tanke756.top/gthiwhkqrz.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.nanxuanxn.top/gtiigpyjmd.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.xuanzx.com/gtkndikosa.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.hysaishi.cn/gtpclqayza.html

Go:   slices.Sort(arr)
来源：http://hz.kuanghao11.cn/gtnjwujpvz.html

Ruby: arr.sort
来源：http://hz.jqgfzy.top/gtvpdhquet.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.gaohongyu789.top/gtptghjnuh.html

[N03] 快速排序（分治示例）
来源：http://hz.jqgfzy.top/gtcdtefjsa.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.sweek.top/gtelpudczu.html

PHP:  // 递归实现，或用 usort
来源：http://hz.yvedp.cn/gttyzbltgp.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jinyuanbaomall.cn/gthdcqckki.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.ywan-chungtsiang.top/gtqiigaehn.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.chenjidiqi.icu/gttdtwpsmg.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.snrcjt.cn/gtzylfpukg.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.xuanzx.com/gtwsgwtytz.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.sysykeji.top/gtrguciqwc.html

[N04] 斐波那契数列
来源：http://hz.nwbrower.top/gttdmovqac.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.snrcjt.cn/gtrpocpvcv.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.52xcode.cn/gtnguqmjfq.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.meibo888.top/gtizfkpehx.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.iojbl.cn/gtrqpgejqf.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.ehwqpu.com/gttjyvuhjy.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.haohaochexian.top/gtwondwlyf.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.birdmap.top/gtvuifobch.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.xingfuxueyuan.xyz/gtoivhvvol.html

[N05] 最大公约数
来源：http://hz.9152youxi.cn/gtjfewlhvu.html

Py:   math.gcd(a, b)
来源：http://hz.ivvv.top/gtpcvzfslo.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.gogol.net.cn/gtdnkdkuvg.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.zhixingplan.top/gtuzlaujhi.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.ppjwa.cn/gtffqihlxv.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.zhiwuduotai.top/gtuuizvawn.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.iojbl.cn/gtgvmvbnot.html

Ruby: a.gcd(b)
来源：http://hz.jinqigfzy.top/gtzpdxscge.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.yj202588.top/gthgumqfag.html

[N06] 判断回文字符串
来源：http://hz.xylfe.cn/gtvqgdamil.html

Py:   s == s[::-1]
来源：http://hz.wangdashe.top/gtodfaklwf.html

PHP:  $s === strrev($s);
来源：http://hz.jinqigfzy.top/gtdszmxjin.html

JS:   s === [...s].reverse().join("")
来源：http://hz.bjfxy.top/gtyltindva.html

TS:   s === [...s].reverse().join("")
来源：http://hz.meibo888.top/gtjacvjbvs.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.zdqjudy.top/gtwnruezcs.html

Go:   // 双指针从两端比较
来源：http://hz.zhaomingkeji.xyz/gthfyhufsg.html

Ruby: s == s.reverse
来源：http://hz.pycfn.com/gtxrdzhnuw.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.ybcxt.top/gtbzyoeqbf.html

[N07] 两数之和（返回下标）
来源：http://hz.ppjwa.cn/gtpfurxttz.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.pengpengdd.cyou/gtazobtoup.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.quarkkingdee.top/gtqkjeaakh.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.birdmap.top/gtfphntcrd.html

TS:   // 手写 Map<string, number>
来源：http://hz.zycfv.cn/gtouabuwti.html

Java: // 手写 HashMap
来源：http://hz.xingfuxueyuan.xyz/gtxesvhtac.html

Go:   // 手写 map[int]int
来源：http://hz.sxryk.cn/gtfymopfqg.html

Ruby: // 手写 Hash
来源：http://hz.yuxming.cn/gtdujgjwvw.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.yvedp.cn/gtmudjdamt.html

[N08] 生成全排列
来源：http://hz.birdmap.top/gtwuxbsvzj.html

Py:   itertools.permutations(arr)
来源：http://hz.gotoacloud.top/gtkecjacfh.html

PHP:  // 手写递归交换
来源：http://hz.zhijiandao.cn/gtrjdiqyjz.html

JS:   // 手写回溯递归
来源：http://hz.wangdashe.top/gtfarnqnrx.html

TS:   // 手写回溯递归
来源：http://hz.shanyushiyangkeji.top/gtxwfptkll.html

Java: // 手写回溯递归
来源：http://hz.xuanzx.com/gtsokhwzeo.html

Go:   // 手写回溯递归
来源：http://hz.ywan-chungtsiang.top/gtlgvckoxj.html

Ruby: arr.permutation.to_a
来源：http://hz.dashuyun.cn/gtbgpbkjof.html

C#:   // 手写回溯递归
来源：http://hz.yuxming.cn/gtrultcjoj.html

[N09] 栈与队列
来源：http://hz.jinghuilouyu.cn/gthwcpecdx.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.jlsjyb.cn/gtnkeuwsoo.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.shanyushiyangkeji.top/gtbnstsrxx.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.52xcode.cn/gtaitnivrg.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.jqgufenzy.top/gtdfdkslyk.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.xinyue.icu/gtcbenxchi.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.wangshuangyany.cn/gtilgijwrk.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.vqdsnc.cn/gtxjyoxwml.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.zhongyouzk.top/gtfwfhzwgl.html

[N10] 链表节点定义
来源：http://hz.nanxuanxn.top/gtypoxrlzl.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.jqgfzy.top/gtsntaiopy.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.xinyue.icu/gtvmzjbvkr.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.nanxuanxn.top/gtskwtfsad.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.daxiang520.top/gtfehsnlbc.html

Java: class Node { int v; Node next; }
来源：http://hz.zhengqikj.top/gtcrlqkdvt.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.yonumen.top/gtroidawtw.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.birdmap.top/gtmndopeig.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.cheryme.top/gtdqxlxrrm.html

[N11] 二叉树中序遍历
来源：http://hz.yuxming.cn/gtcqcjxlvq.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.fzhhl.top/gthgdivlvd.html

PHP:  // 手写递归函数
来源：http://hz.aizwys.cn/gtkklzkqfb.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.dianchejie.cn/gtjfygjqhk.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.shangyingyoupin.top/gtqsrvrfdp.html

Java: // 手写递归
来源：http://hz.aizwys.cn/gtzhwazskd.html

Go:   // 手写递归
来源：http://hz.cashguo.top/gtykyrcgdp.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.jinqigfzy.top/gtriltpblt.html

C#:   // 手写递归
来源：http://hz.iojbl.cn/gtrytkxqov.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.svipenyu.cn/gtzdwtrtfm.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.dashuyun.cn/gtkzefksig.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.0kj1m.cn/gtdunnvcuf.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.cucudq.cn/gthjoplwbz.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.tanke756.top/gtqzziesyb.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.chenlongwang.top/gtxgsmocct.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.guowangkeji.top/gtarktljsy.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.yj20258888.top/gttruvmrni.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.jinghuilouyu.cn/gtpmwjubmo.html

================================================================================
来源：http://hz.c1oappe.top/gthwdgpglm.html

O. 并发与异步
来源：http://hz.zhijiandao.cn/gtrhwtsitt.html

================================================================================
来源：http://hz.yj20258888.top/gthauwuszd.html

[O01] 启动一个线程
来源：http://hz.quarkkingdee.top/gttwedqnec.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.yongpay.top/gtktpxbppe.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.ybcxt.top/gtvxqrhwdk.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.yuanzhike.top/gtifsluxaa.html

TS:   // 同 JS
来源：http://hz.tanke756.top/gtxkknwfny.html

Java: new Thread(() -> f()).start()
来源：http://hz.hywenlv.cn/gtqbacojlu.html

Go:   go f()
来源：http://hz.c1oappe.top/gtlkpkczcx.html

Ruby: Thread.new { f }
来源：http://hz.quarkkingdee.top/gthgddrzmo.html

C#:   Task.Run(() => F());
来源：http://hz.chenlongwang.top/gtfqpqjoge.html

[O02] 使用线程池
来源：http://hz.sysykeji.top/gtltcoyhot.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.hammf.cn/gtqnyvmgbx.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.smart0.xyz/gtfxozrbac.html

JS:   // worker_threads 线程池
来源：http://hz.yj202588.top/gtejonkzql.html

TS:   // worker_threads 线程池
来源：http://hz.gotoacloud.top/gtkljpbltj.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.nanxuanxn.top/gtfdjdvdfi.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.c1oappe.top/gtaehouktj.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.zhijiandao.cn/gtvcztrsrr.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.yanxiufei.cn/gtwkpwjczr.html

[O03] 加锁保护共享数据
来源：http://hz.aizwys.cn/gtngxypbei.html

Py:   with lock: shared += 1
来源：http://hz.52xcode.cn/gtkbkmehyb.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.feifeiyinyue.top/gtjzltpmsu.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.xinyue.icu/gtqeukgnvv.html

TS:   // 同 JS
来源：http://hz.yj202588.top/gtccpoyxir.html

Java: synchronized (this) { shared++; }
来源：http://hz.havefunace.top/gtqmbouhdd.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.cheryme.top/gtmyfqzytm.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.tian-w.cn/gtdndxtdwy.html

C#:   lock (gate) { shared++; }
来源：http://hz.mhx1999.top/gtoacwsrhq.html

[O04] 定义异步函数并等待
来源：http://hz.hnxiangtu.top/gtctvlcyzs.html

Py:   async def f():⏎    await g()
来源：http://hz.wangdashe.top/gtzslymzcs.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.hysaishi.cn/gtrclvlvbh.html

JS:   async function f() { await g(); }
来源：http://hz.shzxlz.cn/gtvoeycffs.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.daria6918.cn/gtsmalfbgl.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.chenjidiqi.icu/gtuxyvfmxu.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.xziqi.cn/gtzrfwmhrb.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.jinqigfzy.top/gtnimcofvt.html

C#:   async Task F() { await G(); }
来源：http://hz.dashuyun.cn/gtjutiduqj.html

[O05] 并发执行并等待全部完成
来源：http://hz.jinqigufen.top/gtdgviehga.html

Py:   asyncio.gather(*tasks)
来源：http://hz.zhongyouzk.top/gtnkgygxwg.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.hywenlv.cn/gtscawkfjh.html

JS:   await Promise.all(tasks)
来源：http://hz.sysykeji.top/gtybrgtakn.html

TS:   await Promise.all(tasks)
来源：http://hz.meibo888.top/gtskxcwoir.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.xuetiantiany.cn/gttzzwgqlf.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.shangyingyoupin.top/gtlbuiuhoo.html

Ruby: threads.map(&:join)
来源：http://hz.shangyingyoupin.top/gtjglerrqz.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.yanxiufei.cn/gtozusuljv.html

[O06] 使用进程池
来源：http://hz.gotoacloud.top/gthmwsimwb.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.jyoumei.cn/gtzudegrsz.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.feifeiyinyue.top/gtbjxgscqg.html

JS:   // child_process / cluster 模块
来源：http://hz.xuanzx.com/gtqtdzulav.html

TS:   // child_process / cluster 模块
来源：http://hz.0kj1m.cn/gtsvcmxumg.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.birdmap.top/gtinkwotoq.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.nwbrower.top/gttrcnxvcc.html

Ruby: // fork 块
来源：http://hz.quarkkingdee.top/gtdpmzhxlz.html

C#:   Parallel.For
来源：http://hz.shanyushiyangtech.top/gtqrfefnuy.html

================================================================================
来源：http://hz.jianghu66.top/gtbqdjavdc.html

P. 常用工具函数
来源：http://hz.hywenlv.cn/gtvoczvtxk.html

================================================================================
来源：http://hz.daxiang520.top/gtjokhroay.html

[P01] 生成 UUID
来源：http://hz.daria6918.cn/gtojadumgn.html

Py:   str(uuid.uuid4())
来源：http://hz.sweek.top/gtnzizqnha.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.jqgufenzy.top/gtpvxvrimf.html

JS:   crypto.randomUUID()
来源：http://hz.jinyuanbaomall.cn/gtefwaotyw.html

TS:   crypto.randomUUID()
来源：http://hz.dashuyun.cn/gtpwtyuagf.html

Java: UUID.randomUUID().toString()
来源：http://hz.ybcxt.top/gtyrsslazg.html

Go:   // 用 github.com/google/uuid
来源：http://hz.zhijiandao.cn/gtnjbheqbd.html

Ruby: SecureRandom.uuid
来源：http://hz.hnxiangtu.top/gttaoyzyir.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.yj20258.top/gtfmromqlg.html

[P02] MD5 / SHA256 摘要
来源：http://hz.ywan-chungtsiang.top/gtdawhambh.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.wangdashe.top/gtekgetdvd.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.chenjidiqi.icu/gtnzqbocqx.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.jinghuilouyu.cn/gthvssufgf.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.guannengcc.top/gtnfhbphbu.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.daria6918.cn/gtibqupxbz.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.guannengcc.top/gtkgebdeiv.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.yj202588.top/gtukrsiill.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.yvedp.cn/gtvpmhoxgf.html

[P03] 生成短随机字符串
来源：http://hz.svipenyu.cn/gtzzwmqnqt.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.feifeiyinyue.top/gttnqdywfd.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hz.aibaodan.cn/gtkuujrywj.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.hywenlv.cn/gtlgjpcmrg.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hz.yj202588.top/gtgygkgece.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hz.sysykeji.top/gtbrdzhldh.html


<!-- 参考信息 -->