代发 wailian999

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.yueranfly.top/gtfdfwhjce.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.yj202588.top/gtmbzvkmvc.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.shanyushiyangkeji.top/gtkymvpscv.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.daxiang520.top/gtekikayfc.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.daxiang520.top/gtthseihze.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.chenzaomai.com/gtyrmsbxny.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.shanyushiyangkeji.top/gtosflknkd.html

[L06] 解析响应为 JSON
来源：http://hz.svipenyu.cn/gtzavsawmu.html

Py:   resp.json()
来源：http://hz.gzhubu.top/gtjkxjcnua.html

PHP:  json_decode($body, true);
来源：http://hz.cheryme.top/gtjrvhegjm.html

JS:   await resp.json()
来源：http://hz.hnqzz.top/gtceragboy.html

TS:   await resp.json()
来源：http://hz.yonumen.top/gtfjvbwnbv.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.chenjidiqi.icu/gtohjqztmi.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.gogol.net.cn/gtfvyhfjre.html

Ruby: JSON.parse(resp.body)
来源：http://hz.yuxming.cn/gttjwobqkp.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.birdmap.top/gtlfbbfxvd.html

[L07] 处理 HTTP 状态码
来源：http://hz.cdnleiting.top/gtixpbhuav.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.zhijiandao.cn/gtnowlnuds.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.pycfn.com/gtvxbhznhy.html

JS:   resp.ok;  resp.status
来源：http://hz.yongpay.top/gtuhlkkppo.html

TS:   resp.ok;  resp.status
来源：http://hz.birdmap.top/gtjvvpcbms.html

Java: resp.statusCode()
来源：http://hz.dashuyun.cn/gtnkpuvhbg.html

Go:   resp.StatusCode
来源：http://hz.ybcxt.top/gtjoimryxz.html

Ruby: resp.code.to_i
来源：http://hz.gaohongyu789.top/gtuwnwrxxw.html

C#:   (int)resp.StatusCode
来源：http://hz.jlsjyb.cn/gtvgvmhgjx.html

[L08] 并发请求多个地址
来源：http://hz.xziqi.cn/gtgvnbbmij.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.pycfn.com/gtjhlzcqgg.html

PHP:  curl_multi_init() 系列
来源：http://hz.hammf.cn/gteivhugoa.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.ppjwa.cn/gtyktoprvh.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yanxiufei.cn/gtbcexskcz.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.yonumen.top/gtedqhnkgw.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.ybcxt.top/gtqkteyhqf.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.gogol.net.cn/gtpmfrdild.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.ehwqpu.com/gtdyruwoxp.html

================================================================================
来源：http://hz.ybcxt.top/gtzoecoclx.html

M. 命令行 / 进程 / 环境
来源：http://hz.nanxuanxn.top/gttftukyji.html

================================================================================
来源：http://hz.cashguo.top/gtetnfsogm.html

[M01] 读取命令行参数
来源：http://hz.xuanzx.com/gtziklcpxg.html

Py:   sys.argv[1:]
来源：http://hz.c1oappe.top/gtxwvykomt.html

PHP:  $argv;  $argc;
来源：http://hz.yj20258.top/gtzqkrnwsm.html

JS:   process.argv.slice(2)
来源：http://hz.cheryme.top/gtspstffgj.html

TS:   process.argv.slice(2)
来源：http://hz.fzhhl.top/gtotalyodg.html

Java: args 数组（main 方法参数）
来源：http://hz.yueranfly.top/gtksgqhvte.html

Go:   os.Args[1:]
来源：http://hz.zhongyouzk.top/gtfyoxfquh.html

Ruby: ARGV
来源：http://hz.hnxiangtu.top/gthfasorkg.html

C#:   args 数组（Main 方法参数）
来源：http://hz.hammf.cn/gtwwxcguth.html

[M02] 读取环境变量
来源：http://hz.ybcxt.top/gtfwxedpvu.html

Py:   os.environ.get("HOME")
来源：http://hz.mhx1999.top/gtbjoapusq.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.sxryk.cn/gtrgjflzyc.html

JS:   process.env.HOME
来源：http://hz.jinghuilouyu.cn/gthnfnbgqe.html

TS:   process.env.HOME
来源：http://hz.cucudq.cn/gtihqyvkhy.html

Java: System.getenv("HOME")
来源：http://hz.birdmap.top/gtelpelsvt.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.yuanzhike.top/gtyjtvzrgc.html

Ruby: ENV["HOME"]
来源：http://hz.vqdsnc.cn/gtyylkhdaq.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.fengsongda.top/gtfhwstrxq.html

[M03] 执行外部命令
来源：http://hz.guowangkeji.top/gtkdnkvpmf.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.yvedp.cn/gtsrudsetj.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.zhijiandao.cn/gtaqhxcdgm.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.shanyushiyangkeji.top/gtothqsnuc.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.pengpengdd.cyou/gtwcklwxgy.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.havefunace.top/gtlbhubayj.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.jlsjyb.cn/gtjkklvlcn.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.nanxuanxn.top/gtqkawxrrq.html

C#:   Process.Start("ls", "-l");
来源：http://hz.cdnleiting.top/gtmkmalemm.html

[M04] 获取当前工作目录
来源：http://hz.chenlongwang.top/gtaeuqgwrf.html

Py:   os.getcwd()
来源：http://hz.nanxuanxn.top/gtgshyrkhn.html

PHP:  getcwd();
来源：http://hz.ppjwa.cn/gtvskghfvf.html

JS:   process.cwd()
来源：http://hz.cucudq.cn/gtnfaaxjlb.html

TS:   process.cwd()
来源：http://hz.meibo888.top/gtcekdoabk.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.jiagoushi.top/gtnccemsgt.html

Go:   os.Getwd()
来源：http://hz.jlsjyb.cn/gttlpzdrie.html

Ruby: Dir.pwd
来源：http://hz.xinyue.icu/gtmvretqup.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.quarkkingdee.top/gtuoxdvcka.html

[M05] 设置退出码
来源：http://hz.tianlin.xyz/gtyevkjohu.html

Py:   sys.exit(1)
来源：http://hz.shzxlz.cn/gtcrtwiubg.html

PHP:  exit(1);
来源：http://hz.xylfe.cn/gtfojkbcge.html

JS:   process.exit(1)
来源：http://hz.fengsongda.top/gtwhmeojsw.html

TS:   process.exit(1)
来源：http://hz.zhixingplan.top/gtwvxbdbph.html

Java: System.exit(1)
来源：http://hz.zycfv.cn/gtpwuqvkna.html

Go:   os.Exit(1)
来源：http://hz.xuetiantiany.cn/gtwvcjhzcj.html

Ruby: exit 1
来源：http://hz.vqdsnc.cn/gtwvbqizzk.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.yj20258.top/gtmbkzwkjx.html

[M06] 向标准错误输出
来源：http://hz.gotoacloud.top/gtuxpnxxxb.html

Py:   print("err", file=sys.stderr)
来源：http://hz.yuanzhike.top/gtpvwzekhp.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.cucudq.cn/gtqchjtiuk.html

JS:   console.error("err")
来源：http://hz.yongpay.top/gtksguvkby.html

TS:   console.error("err")
来源：http://hz.zycfv.cn/gtmcgbnxkh.html

Java: System.err.println("err")
来源：http://hz.kuanghao11.cn/gtwrqdizci.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.cucudq.cn/gteseowpzh.html

Ruby: warn "err"
来源：http://hz.birdmap.top/gtgyhcmdid.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.guowangkeji.top/gtthzsltje.html

[M07] 判断是否为主入口
来源：http://hz.9152youxi.cn/gtlinnuxvo.html

Py:   if __name__ == "__main__":
来源：http://hz.ehwqpu.com/gtdwfiowjh.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.nanxuanxn.top/gtxejexxkn.html

JS:   require.main === module
来源：http://hz.birdmap.top/gtsmiiqdnl.html

TS:   require.main === module
来源：http://hz.sysykeji.top/gtejnxfaks.html

Java: public static void main(String[] args)
来源：http://hz.zdqjudy.top/gtejlalhrg.html

Go:   func main()
来源：http://hz.jiagoushi.top/gtfeyjlppd.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.yj20258.top/gtiofzoftv.html

C#:   static void Main(string[] args)
来源：http://hz.xingfuxueyuan.xyz/gtdsceqhoh.html

[M08] 获取系统与运行时信息
来源：http://hz.mhx1999.top/gtrzocdiqj.html

Py:   platform.system();  platform.python_version()
来源：http://hz.dianchejie.cn/gtfqvdfkos.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.birdmap.top/gtpwlqzznl.html

JS:   process.platform;  process.version
来源：http://hz.chenzaomai.com/gtcbzbsobc.html

TS:   process.platform;  process.version
来源：http://hz.tianlin.xyz/gtznnrkkgl.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.kuanghao11.cn/gtmopwpqnb.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.sweek.top/gthrhqfpck.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.nanxuanxn.top/gtzuldyvxy.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.fzhhl.top/gtwjmtzyuy.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtkdhccbvn.html

N. 数据结构与算法
来源：http://hz.shanyushiyangtech.top/gtzegawvrd.html

================================================================================
来源：http://hz.aibaodan.cn/gtxuxuessu.html

[N01] 二分查找（有序数组）
来源：http://hz.yj20258888.top/gtohavgvqg.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.nwbrower.top/gttrzsbopo.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.shzxlz.cn/gtqgyujigs.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jinyuanbaomall.cn/gtxcwydejk.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zycfv.cn/gtxoevhpji.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.jlsjyb.cn/gtircmjwgc.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.snrcjt.cn/gtebuujypf.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.guowangkeji.top/gtvxfntthn.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.xziqi.cn/gtjscxubhf.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.zhaomingkeji.xyz/gtoqjvpefo.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.vqdsnc.cn/gtsyvxhync.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.xingfuxueyuan.xyz/gtyfppjzjs.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.zycfv.cn/gtkknqztih.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jlsjyb.cn/gtatfoymdk.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.cheryme.top/gtahkimdek.html

Go:   slices.Sort(arr)
来源：http://hz.zhengqikj.top/gtmlxdjzmz.html

Ruby: arr.sort
来源：http://hz.zhijiandao.cn/gtnsaiqlgj.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.wangdashe.top/gtavlxikhh.html

[N03] 快速排序（分治示例）
来源：http://hz.svipenyu.cn/gtazpstqrg.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.sufxvd.cn/gtiaovutww.html

PHP:  // 递归实现，或用 usort
来源：http://hz.smart0.xyz/gtrtidfzpp.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.ydzc1.top/gtzkhoghfv.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.cdnleiting.top/gtnhqyrdbu.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.svipenyu.cn/gtqeetlqsp.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.iojbl.cn/gtnjcmzual.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.hywenlv.cn/gtnrtzmznx.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.feifeiyinyue.top/gtwojbaoyj.html

[N04] 斐波那契数列
来源：http://hz.smart0.xyz/gtktaedeey.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.gotoacloud.top/gtjdsbeqxy.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.yuanzhike.top/gtcqdalsou.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.shangyingyoupin.top/gtutuigicg.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.gaohongyu789.top/gtbtfpsbav.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.chenlongwang.top/gtedtcnnnf.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.sufxvd.cn/gteojtzizs.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.hywenlv.cn/gtrhqznazg.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.yonumen.top/gtnwvkwulr.html

[N05] 最大公约数
来源：http://hz.0kj1m.cn/gtrmyzdamv.html

Py:   math.gcd(a, b)
来源：http://hz.yonumen.top/gtjjsavfkr.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.guannengcc.top/gtqrbvmsdn.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.shuidangran.top/gtykyrhvxa.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.ywan-chungtsiang.top/gtacnynqbc.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.xylfe.cn/gtvdbynynm.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.andypj.xyz/gtcarztdvu.html

Ruby: a.gcd(b)
来源：http://hz.shanyushiyangtech.top/gtyyjlrcta.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.haohaochexian.top/gtmbcbhrmc.html

[N06] 判断回文字符串
来源：http://hz.shanyushiyangtech.top/gtfdjvpqly.html

Py:   s == s[::-1]
来源：http://hz.chenjidiqi.icu/gtoezubbtg.html

PHP:  $s === strrev($s);
来源：http://hz.svipenyu.cn/gtigbaqvwo.html

JS:   s === [...s].reverse().join("")
来源：http://hz.sysykeji.top/gtrfjjowoj.html

TS:   s === [...s].reverse().join("")
来源：http://hz.cdnleiting.top/gtmownqdyd.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.kuanghao11.cn/gtynlagbcp.html

Go:   // 双指针从两端比较
来源：http://hz.xylfe.cn/gthqeulhfe.html

Ruby: s == s.reverse
来源：http://hz.havefunace.top/gtglcelheg.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.xuetiantiany.cn/gtfpusrqxx.html

[N07] 两数之和（返回下标）
来源：http://hz.xylfe.cn/gtzrcmqmmy.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.aizwys.cn/gtpkhgtfdj.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.shuidangran.top/gtwghsebdy.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.yuxming.cn/gtgtgkobbl.html

TS:   // 手写 Map<string, number>
来源：http://hz.hnxiangtu.top/gtnitzmgop.html

Java: // 手写 HashMap
来源：http://hz.zhijiandao.cn/gtazgeyjus.html

Go:   // 手写 map[int]int
来源：http://hz.andypj.xyz/gtsydqcmna.html

Ruby: // 手写 Hash
来源：http://hz.xylfe.cn/gtqrwqfxfo.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.redwolf501.top/gtcwkznfny.html

[N08] 生成全排列
来源：http://hz.chenzaomai.com/gtivxquwpo.html

Py:   itertools.permutations(arr)
来源：http://hz.zhixingplan.top/gtsqpruwcl.html

PHP:  // 手写递归交换
来源：http://hz.zhijiandao.cn/gtysyahian.html

JS:   // 手写回溯递归
来源：http://hz.xingfuxueyuan.xyz/gtsgdcpvpf.html

TS:   // 手写回溯递归
来源：http://hz.52xcode.cn/gtwthqohcm.html

Java: // 手写回溯递归
来源：http://hz.tanke756.top/gtbcbhzxtt.html

Go:   // 手写回溯递归
来源：http://hz.nanxinkj.top/gtdpgncrca.html

Ruby: arr.permutation.to_a
来源：http://hz.nanxuanxn.top/gtouuygkji.html

C#:   // 手写回溯递归
来源：http://hz.yj202588.top/gtctfxjsqi.html

[N09] 栈与队列
来源：http://hz.hysaishi.cn/gtbszuhrwz.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.yj20258.top/gtheigglxh.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.gotoacloud.top/gtofqegbwk.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.hfpthk.cn/gtpboaoqkk.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.mhx1999.top/gteggowuiy.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.cheryme.top/gtohivygpt.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.bjfxy.top/gtuqbtvrbf.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.tianlin.xyz/gthtfxfcxl.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.gaohongyu789.top/gtjjexkkxq.html

[N10] 链表节点定义
来源：http://hz.birdmap.top/gtbjnwrkcp.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.sufxvd.cn/gtfoffzkqz.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.9152youxi.cn/gtgbvsqkru.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.jlsjyb.cn/gtiuuvyqce.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.chenlongwang.top/gtfvghhakh.html

Java: class Node { int v; Node next; }
来源：http://hz.jyoumei.cn/gtbwqtwuac.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.jinyuanbaomall.cn/gtdtglngxn.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.tian-w.cn/gtwhwgifhz.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.fzhhl.top/gtoqtqtouv.html

[N11] 二叉树中序遍历
来源：http://hz.52xcode.cn/gtkwyegddo.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.pycfn.com/gtafuvrzyt.html

PHP:  // 手写递归函数
来源：http://hz.daxiang520.top/gtzirmilxj.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.9152youxi.cn/gtesyhdifb.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yvedp.cn/gtibminptv.html

Java: // 手写递归
来源：http://hz.ydzc1.top/gthscgcziy.html

Go:   // 手写递归
来源：http://hz.jiagoushi.top/gtyesvatzc.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.daria6918.cn/gtkxlhdvav.html

C#:   // 手写递归
来源：http://hz.nanxuanxn.top/gtzhaohwng.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.haohaochexian.top/gtkhmpxntl.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.sysykeji.top/gtdbocbzdh.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.zdqjudy.top/gtccudsopr.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.shzxlz.cn/gtvbippjge.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.xuetiantiany.cn/gtamoqkkjk.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.xziqi.cn/gtcxanidjo.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.jlsjyb.cn/gtnwgawlhf.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.yvedp.cn/gtwvuggpfl.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.hammf.cn/gtzwgytaqn.html

================================================================================
来源：http://hz.cdnleiting.top/gtsqsyhhsu.html

O. 并发与异步
来源：http://hz.xinyue.icu/gtuyyghlbc.html

================================================================================
来源：http://hz.zdqjudy.top/gtlnheojjc.html

[O01] 启动一个线程
来源：http://hz.yueranfly.top/gtvraxznji.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.chenlongwang.top/gtnfrqrecm.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.cucudq.cn/gtdgokhxmr.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.mhx1999.top/gtjhpcbwph.html

TS:   // 同 JS
来源：http://hz.yueranfly.top/gtzjyymvpg.html

Java: new Thread(() -> f()).start()
来源：http://hz.jiagoushi.top/gtednidhlj.html

Go:   go f()
来源：http://hz.iojbl.cn/gtvteflyin.html

Ruby: Thread.new { f }
来源：http://hz.chenjidiqi.icu/gtfdnccmhv.html

C#:   Task.Run(() => F());
来源：http://hz.yanxiufei.cn/gtuvpoqgfs.html

[O02] 使用线程池
来源：http://hz.snrcjt.cn/gttwtjanqn.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.hnxiangtu.top/gttepwkkrq.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.hywenlv.cn/gtfsqdtbvy.html

JS:   // worker_threads 线程池
来源：http://hz.zdqjudy.top/gtshqugzxg.html

TS:   // worker_threads 线程池
来源：http://hz.xuetiantiany.cn/gtnhoogbtn.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.shanyushiyangkeji.top/gtdglaxjcl.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.cashguo.top/gtvbzddewj.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.gotoacloud.top/gtfcnlcfrl.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.hongshengwenyu.top/gtevsydawd.html

[O03] 加锁保护共享数据
来源：http://hz.gotoacloud.top/gtjetmrwwv.html

Py:   with lock: shared += 1
来源：http://hz.hysaishi.cn/gtulpvosax.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.meibo888.top/gttqkhdhua.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.zhoulong.xyz/gtdwibaoce.html

TS:   // 同 JS
来源：http://hz.xinyue.icu/gtnaagaqzs.html

Java: synchronized (this) { shared++; }
来源：http://hz.tianlin.xyz/gtayzwzqfo.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.zdqjudy.top/gtpjrhivuu.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.dianchejie.cn/gtcooddbwh.html

C#:   lock (gate) { shared++; }
来源：http://hz.0kj1m.cn/gtpwacbxhc.html

[O04] 定义异步函数并等待
来源：http://hz.jianghu66.top/gttqydxvpr.html

Py:   async def f():⏎    await g()
来源：http://hz.nanxinkj.top/gteuvqjpss.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.xingfuxueyuan.xyz/gtsaqdxsmi.html

JS:   async function f() { await g(); }
来源：http://hz.sxryk.cn/gtvfqnxcjj.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.jqgufenzy.top/gtzkepuyad.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.ydjk.org.cn/gtsddbkwav.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.shangyingyoupin.top/gtrdghruax.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.andypj.xyz/gtzpuuwlhp.html

C#:   async Task F() { await G(); }
来源：http://hz.hammf.cn/gtiophbdkp.html

[O05] 并发执行并等待全部完成
来源：http://hz.yuxming.cn/gtzbmxmbuz.html

Py:   asyncio.gather(*tasks)
来源：http://hz.shangyingyoupin.top/gtunxkozpc.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.hongshengwenyu.top/gtngzbbvyp.html

JS:   await Promise.all(tasks)
来源：http://hz.svipenyu.cn/gtgddzuurf.html

TS:   await Promise.all(tasks)
来源：http://hz.jqgufenzy.top/gtjogeewvz.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.zhoulong.xyz/gtvdnlbwqt.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.zhiwuduotai.top/gtjjqrlbav.html

Ruby: threads.map(&:join)
来源：http://hz.cheryme.top/gtsjvxgict.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.jqgufenzy.top/gtxbmgyvtb.html

[O06] 使用进程池
来源：http://hz.hnqzz.top/gtxawdfplj.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.yonumen.top/gtssfebzmf.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.shangyingyoupin.top/gtdkxlhaht.html

JS:   // child_process / cluster 模块
来源：http://hz.nanxinkj.top/gtmzxgdyie.html

TS:   // child_process / cluster 模块
来源：http://hz.nwbrower.top/gtcclkkrdf.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.jqgufenzy.top/gtfbnsodov.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.zhongyouzk.top/gtsqzzrrta.html

Ruby: // fork 块
来源：http://hz.tianlin.xyz/gtefmmufvx.html

C#:   Parallel.For
来源：http://hz.316326.xyz/gtnynoneua.html

================================================================================
来源：http://hz.yueranfly.top/gtgusiezns.html

P. 常用工具函数
来源：http://hz.52xcode.cn/gtuiftpfmp.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtfmjwasdt.html

[P01] 生成 UUID
来源：http://hz.hnxiangtu.top/gtprptzizb.html

Py:   str(uuid.uuid4())
来源：http://hz.pycfn.com/gtnsdhyxca.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.iojbl.cn/gtmatgnlvm.html

JS:   crypto.randomUUID()
来源：http://hz.redwolf501.top/gtfhzzioth.html

TS:   crypto.randomUUID()
来源：http://hz.sweek.top/gtaiilkmbi.html

Java: UUID.randomUUID().toString()
来源：http://hz.hnqzz.top/gtutatobsb.html

Go:   // 用 github.com/google/uuid
来源：http://hz.zhiwuduotai.top/gtqihwaolo.html

Ruby: SecureRandom.uuid
来源：http://hz.hfpthk.cn/gtejpyfomm.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.jinghuilouyu.cn/gtuakxzcbv.html

[P02] MD5 / SHA256 摘要
来源：http://hz.zhixingplan.top/gtlvistobm.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.fzhhl.top/gtobpzzdex.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.sysykeji.top/gtzrfyvtys.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.ywan-chungtsiang.top/gttcqtsrbj.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.yueranfly.top/gtsxlpaebn.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.zycfv.cn/gtecbrdhdp.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.meibo888.top/gtooyyjzah.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.kuanghao11.cn/gtxvtzvgvf.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.yongpay.top/gtnyqasmwd.html

[P03] 生成短随机字符串
来源：http://hz.cheryme.top/gtotscsarn.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.jqgfzy.top/gtyqhomgei.html


<!-- 参考信息 -->