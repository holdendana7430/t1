代发 wailian999

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.hammf.cn/gtmdrflxfc.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.hfpthk.cn/gtwokagwfa.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.sysykeji.top/gtkecifccp.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.pengpengdd.cyou/gtnxbjwomi.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.gotoacloud.top/gtqrajwivz.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.yj20258888.top/gtwiqhxsrs.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.zycfv.cn/gtwntlrmka.html

[L06] 解析响应为 JSON
来源：http://hz.shuidangran.top/gtgauthrdh.html

Py:   resp.json()
来源：http://hz.cashguo.top/gtfriqycfp.html

PHP:  json_decode($body, true);
来源：http://hz.hysaishi.cn/gtreososxd.html

JS:   await resp.json()
来源：http://hz.zhoulong.xyz/gtrdvevrsh.html

TS:   await resp.json()
来源：http://hz.yonumen.top/gtrarzzrke.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.jiagoushi.top/gtmbnnvwmd.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.gzhubu.top/gtmtqvwrpp.html

Ruby: JSON.parse(resp.body)
来源：http://hz.yuxming.cn/gtqjuydzry.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.hfpthk.cn/gtwpcyahrq.html

[L07] 处理 HTTP 状态码
来源：http://hz.xuanzx.com/gtzayeqdki.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.bjfxy.top/gtlarvajzq.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.gotoacloud.top/gtnugszrin.html

JS:   resp.ok;  resp.status
来源：http://hz.dianchejie.cn/gtibvriweo.html

TS:   resp.ok;  resp.status
来源：http://hz.meibo888.top/gtoejzvcwk.html

Java: resp.statusCode()
来源：http://hz.yj20258888.top/gtqkdfbtml.html

Go:   resp.StatusCode
来源：http://hz.gogol.net.cn/gtopeoamyc.html

Ruby: resp.code.to_i
来源：http://hz.guannengcc.top/gtstusopvf.html

C#:   (int)resp.StatusCode
来源：http://hz.ydzc1.top/gtvcprkxeq.html

[L08] 并发请求多个地址
来源：http://hz.feifeiyinyue.top/gtpgtyxzle.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.hysaishi.cn/gtavtxbxbl.html

PHP:  curl_multi_init() 系列
来源：http://hz.kuanghao11.cn/gtmzizlnpd.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.havefunace.top/gtbjabufbs.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.haohaochexian.top/gtiqhdzhab.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.daria6918.cn/gtpkkdxizl.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.chenlongwang.top/gtbhtnktmj.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.ivvv.top/gtwnvhyawj.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.zhaomingkeji.xyz/gtmbllifku.html

================================================================================
来源：http://hz.jlsjyb.cn/gtajedaelt.html

M. 命令行 / 进程 / 环境
来源：http://hz.guannengcc.top/gtpurakrju.html

================================================================================
来源：http://hz.jiagoushi.top/gtzupkifed.html

[M01] 读取命令行参数
来源：http://hz.sufxvd.cn/gtqygnfcpr.html

Py:   sys.argv[1:]
来源：http://hz.wangdashe.top/gtpbdewxri.html

PHP:  $argv;  $argc;
来源：http://hz.jinyuanbaomall.cn/gtksbtwpjg.html

JS:   process.argv.slice(2)
来源：http://hz.yangfankeji.com/gtmqfqllwc.html

TS:   process.argv.slice(2)
来源：http://hz.ywan-chungtsiang.top/gtqdwpvzsk.html

Java: args 数组（main 方法参数）
来源：http://hz.zhongyouzk.top/gtmykmivlr.html

Go:   os.Args[1:]
来源：http://hz.cashguo.top/gtlxoqjwnj.html

Ruby: ARGV
来源：http://hz.meibo888.top/gtjbwfujrr.html

C#:   args 数组（Main 方法参数）
来源：http://hz.bjfxy.top/gtbgwfxdrb.html

[M02] 读取环境变量
来源：http://hz.ppjwa.cn/gtyrcnhltk.html

Py:   os.environ.get("HOME")
来源：http://hz.dianchejie.cn/gtusgyemdc.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.shanyushiyangtech.top/gtonjacmpw.html

JS:   process.env.HOME
来源：http://hz.shangyingyoupin.top/gthwvicyfs.html

TS:   process.env.HOME
来源：http://hz.yvedp.cn/gthrahxypo.html

Java: System.getenv("HOME")
来源：http://hz.jqgfzy.top/gtfalratfe.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.haohaochexian.top/gtavgbwuhy.html

Ruby: ENV["HOME"]
来源：http://hz.nwbrower.top/gtejvwqvdk.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.dianchejie.cn/gtniocptfy.html

[M03] 执行外部命令
来源：http://hz.aizwys.cn/gtxnhhltim.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.9152youxi.cn/gtidmgrusk.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.andypj.xyz/gtegiylpem.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.gogol.net.cn/gtavdtankm.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.ydjk.org.cn/gtjvfqacim.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.jinyuanbaomall.cn/gtjrvzwizy.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.jlsjyb.cn/gtnojmapte.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.mhx1999.top/gtdkbirmbl.html

C#:   Process.Start("ls", "-l");
来源：http://hz.jianghu66.top/gtmxjvxoyh.html

[M04] 获取当前工作目录
来源：http://hz.gzhubu.top/gttoywnlnp.html

Py:   os.getcwd()
来源：http://hz.52xcode.cn/gtukndmlne.html

PHP:  getcwd();
来源：http://hz.9152youxi.cn/gtfpjtldzs.html

JS:   process.cwd()
来源：http://hz.ehwqpu.com/gtzrujdjjv.html

TS:   process.cwd()
来源：http://hz.xuanzx.com/gtccyubqzr.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.kuanghao11.cn/gtbtdymsfa.html

Go:   os.Getwd()
来源：http://hz.yongpay.top/gtqwoiydab.html

Ruby: Dir.pwd
来源：http://hz.hywenlv.cn/gtzmajtyyt.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.cqqwz.cn/gtrheptlfi.html

[M05] 设置退出码
来源：http://hz.hammf.cn/gtvieytvdk.html

Py:   sys.exit(1)
来源：http://hz.yangfankeji.com/gtbnpwqmep.html

PHP:  exit(1);
来源：http://hz.chenjidiqi.icu/gtxxegrufz.html

JS:   process.exit(1)
来源：http://hz.gaohongyu789.top/gtyxxrmscu.html

TS:   process.exit(1)
来源：http://hz.snrcjt.cn/gttkybtxjc.html

Java: System.exit(1)
来源：http://hz.cashguo.top/gtyhfvyppe.html

Go:   os.Exit(1)
来源：http://hz.tian-w.cn/gtlettfymk.html

Ruby: exit 1
来源：http://hz.jyoumei.cn/gtqukffxwh.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.pengpengdd.cyou/gtmmdndncs.html

[M06] 向标准错误输出
来源：http://hz.shanyushiyangkeji.top/gtmoryuciz.html

Py:   print("err", file=sys.stderr)
来源：http://hz.dashuyun.cn/gtuufkjpvy.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.meibo888.top/gtrrlgnddn.html

JS:   console.error("err")
来源：http://hz.hnqzz.top/gttrqvcsda.html

TS:   console.error("err")
来源：http://hz.daria6918.cn/gtjmfnuaqn.html

Java: System.err.println("err")
来源：http://hz.tianlin.xyz/gtvfkvkywz.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.yonumen.top/gtbwdejelp.html

Ruby: warn "err"
来源：http://hz.nanxinkj.top/gtqdwkonmz.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.jinyuanbaomall.cn/gtocspbrkh.html

[M07] 判断是否为主入口
来源：http://hz.zhengqikj.top/gtjdfarvna.html

Py:   if __name__ == "__main__":
来源：http://hz.shzxlz.cn/gtyhatnrqw.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.hysaishi.cn/gtpuxndgsv.html

JS:   require.main === module
来源：http://hz.chenzaomai.com/gtniyivinw.html

TS:   require.main === module
来源：http://hz.9152youxi.cn/gtlzhxtnne.html

Java: public static void main(String[] args)
来源：http://hz.yongpay.top/gtfjygvbjk.html

Go:   func main()
来源：http://hz.snrcjt.cn/gtxcuxkzdx.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.ydjk.org.cn/gtxgdhpbwn.html

C#:   static void Main(string[] args)
来源：http://hz.jiagoushi.top/gthvynihbd.html

[M08] 获取系统与运行时信息
来源：http://hz.yongpay.top/gthjrvsmnw.html

Py:   platform.system();  platform.python_version()
来源：http://hz.meibo888.top/gtxbttksjh.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.hysaishi.cn/gtdiuezpha.html

JS:   process.platform;  process.version
来源：http://hz.shanyushiyangtech.top/gttiqajubx.html

TS:   process.platform;  process.version
来源：http://hz.hfpthk.cn/gtqzqjokpy.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.xylfe.cn/gtcwaskksb.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.jianghu66.top/gtdxhwswoy.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.zycfv.cn/gtbxzigdxk.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.yueranfly.top/gtvnncuwoc.html

================================================================================
来源：http://hz.zycfv.cn/gtbuekilpg.html

N. 数据结构与算法
来源：http://hz.gaohongyu789.top/gtdqbavszi.html

================================================================================
来源：http://hz.tian-w.cn/gtahbtxxkg.html

[N01] 二分查找（有序数组）
来源：http://hz.guannengcc.top/gtjeosymgw.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.ppjwa.cn/gtdenmfhni.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.wangshuangyany.cn/gtxdqyccyb.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zhiwuduotai.top/gtseytntzf.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yanxiufei.cn/gtyhacqkft.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.guowangkeji.top/gttviaciai.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.jinyuanbaomall.cn/gtxgxvewmz.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.jqgufenzy.top/gtfqmpvxyf.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.fzhhl.top/gtztpdudjg.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.chenjidiqi.icu/gttgfxooyl.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.yj20258888.top/gtcbpblkdq.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.xingfuxueyuan.xyz/gtjfhdqdsd.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.fzhhl.top/gtbrblryyn.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.ivvv.top/gteflkpzjx.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.meibo888.top/gtluafsyhd.html

Go:   slices.Sort(arr)
来源：http://hz.cucudq.cn/gtynvhsozc.html

Ruby: arr.sort
来源：http://hz.meibo888.top/gtdofqbhll.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.zhaomingkeji.xyz/gthhmxbphu.html

[N03] 快速排序（分治示例）
来源：http://hz.yvedp.cn/gtlmqgoewu.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.fengsongda.top/gtknhqgxry.html

PHP:  // 递归实现，或用 usort
来源：http://hz.jiagoushi.top/gthcsjigzw.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.tanke756.top/gtpbmwrhit.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.birdmap.top/gtbgnybxee.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.ppjwa.cn/gtfqcrbzvy.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.haohaochexian.top/gtuqcrrzdn.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.xuanzx.com/gthbfuvhth.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.cucudq.cn/gtjpbyhuaw.html

[N04] 斐波那契数列
来源：http://hz.zhixingplan.top/gtkasfabsd.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.yonumen.top/gtjwtgqhfp.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.cucudq.cn/gtpmhxixlq.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.birdmap.top/gtbgjbawly.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yvedp.cn/gtvghixoeu.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.yanxiufei.cn/gtywumdcgd.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.havefunace.top/gtkeowjnkr.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.yuxming.cn/gtwlyqmfrh.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.chenzaomai.com/gtzdkvfkul.html

[N05] 最大公约数
来源：http://hz.zhiwuduotai.top/gtyazruawm.html

Py:   math.gcd(a, b)
来源：http://hz.gotoacloud.top/gtriabrztr.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.cheryme.top/gthgfbphwi.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jinghuilouyu.cn/gtkxjksgky.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.andypj.xyz/gtfjtgmvje.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.mhx1999.top/gtdgngatgd.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.jinyuanbaomall.cn/gtadjkxbrz.html

Ruby: a.gcd(b)
来源：http://hz.yuanzhike.top/gtduypxmov.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.iojbl.cn/gtozzhdtus.html

[N06] 判断回文字符串
来源：http://hz.yueranfly.top/gtvsqwajry.html

Py:   s == s[::-1]
来源：http://hz.yangfankeji.com/gtnegptogr.html

PHP:  $s === strrev($s);
来源：http://hz.jinqigufen.top/gtozhxisek.html

JS:   s === [...s].reverse().join("")
来源：http://hz.redwolf501.top/gtlcznpkly.html

TS:   s === [...s].reverse().join("")
来源：http://hz.yj20258888.top/gteycbthiq.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.tanke756.top/gtpelshsvb.html

Go:   // 双指针从两端比较
来源：http://hz.andypj.xyz/gtkrzhejry.html

Ruby: s == s.reverse
来源：http://hz.yuxming.cn/gtqenopstz.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.jinyuanbaomall.cn/gtzuvuktnl.html

[N07] 两数之和（返回下标）
来源：http://hz.feifeiyinyue.top/gtkqicyqzg.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.yanxiufei.cn/gtorplqddc.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.hysaishi.cn/gtefvuyqzz.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.smart0.xyz/gtswpxpsss.html

TS:   // 手写 Map<string, number>
来源：http://hz.chenzaomai.com/gtvdfdiawa.html

Java: // 手写 HashMap
来源：http://hz.shuidangran.top/gtqrntzcct.html

Go:   // 手写 map[int]int
来源：http://hz.jinyuanbaomall.cn/gtjhdilkia.html

Ruby: // 手写 Hash
来源：http://hz.tian-w.cn/gtqxwgeued.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.yj20258.top/gtmawigarg.html

[N08] 生成全排列
来源：http://hz.zhaomingkeji.xyz/gtlbdwemuf.html

Py:   itertools.permutations(arr)
来源：http://hz.xuanzx.com/gtrbxjrjlq.html

PHP:  // 手写递归交换
来源：http://hz.wangshuangyany.cn/gtkbfbynqx.html

JS:   // 手写回溯递归
来源：http://hz.jyoumei.cn/gtfejzpimt.html

TS:   // 手写回溯递归
来源：http://hz.havefunace.top/gtluknsjtj.html

Java: // 手写回溯递归
来源：http://hz.gzhubu.top/gtmuhbjiej.html

Go:   // 手写回溯递归
来源：http://hz.pengpengdd.cyou/gtmirrgcqf.html

Ruby: arr.permutation.to_a
来源：http://hz.cucudq.cn/gtqoxmyzhl.html

C#:   // 手写回溯递归
来源：http://hz.gaohongyu789.top/gtqbrqkbqf.html

[N09] 栈与队列
来源：http://hz.dashuyun.cn/gtvvgcaoer.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.tianlin.xyz/gtjukpgafa.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.cqqwz.cn/gtcesbsvvt.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.feifeiyinyue.top/gtfhzsrnwx.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.cqqwz.cn/gtjhixrvan.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.feifeiyinyue.top/gttxabywzp.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.birdmap.top/gtzcekjogp.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.daria6918.cn/gtwkxibyed.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.hfpthk.cn/gtgszvyfex.html

[N10] 链表节点定义
来源：http://hz.hywenlv.cn/gtuurnqfnb.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.shangyingyoupin.top/gtalrcvkuf.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.andypj.xyz/gtgjfdcpcg.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.ybcxt.top/gtessgtqkz.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.hammf.cn/gtiaobflpe.html

Java: class Node { int v; Node next; }
来源：http://hz.ywan-chungtsiang.top/gtjafvvaoh.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.52xcode.cn/gtqjehkyvv.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.cdnleiting.top/gtdwrswvxc.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.gotoacloud.top/gtnhbzpmhj.html

[N11] 二叉树中序遍历
来源：http://hz.hammf.cn/gtuigmfjtm.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.xuetiantiany.cn/gtojcjezaj.html

PHP:  // 手写递归函数
来源：http://hz.yj20258.top/gtfrxnsnbp.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.xziqi.cn/gtopzxnnkx.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yj20258.top/gthsazdzhg.html

Java: // 手写递归
来源：http://hz.tanke756.top/gtqrcplcql.html

Go:   // 手写递归
来源：http://hz.shanyushiyangtech.top/gtqlgvhxwl.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.jlsjyb.cn/gtiqscwpce.html

C#:   // 手写递归
来源：http://hz.pycfn.com/gtatjvvsyj.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.hfpthk.cn/gtfbqkjthv.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.jyoumei.cn/gtkjjorbwz.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.jinqigfzy.top/gtqjyoqlcq.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.daria6918.cn/gtsezvluhl.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.dianchejie.cn/gtxwxhewsg.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.zhoulong.xyz/gtuuonirqv.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.zhongyouzk.top/gtntminurw.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.iojbl.cn/gtdshvwsow.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yj20258888.top/gtdqjdzbzm.html

================================================================================
来源：http://hz.xylfe.cn/gtcpwqdpdc.html

O. 并发与异步
来源：http://hz.cqqwz.cn/gtwtfpoudh.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtbxuskosg.html

[O01] 启动一个线程
来源：http://hz.cqqwz.cn/gtysthdjlw.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.jinyuanbaomall.cn/gturxgwssg.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.yj20258888.top/gtisxksjab.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.fzhhl.top/gtlbkxymnt.html

TS:   // 同 JS
来源：http://hz.nanxinkj.top/gtpvfnpipj.html

Java: new Thread(() -> f()).start()
来源：http://hz.yj20258.top/gtnabblzzo.html

Go:   go f()
来源：http://hz.zhengqikj.top/gtlnajyrfn.html

Ruby: Thread.new { f }
来源：http://hz.havefunace.top/gtqfrntqmp.html

C#:   Task.Run(() => F());
来源：http://hz.0kj1m.cn/gtuxdciucm.html

[O02] 使用线程池
来源：http://hz.shuidangran.top/gtszsxworu.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.yonumen.top/gteysmroyz.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.vqdsnc.cn/gtewitfxaf.html

JS:   // worker_threads 线程池
来源：http://hz.nwbrower.top/gtcscxchjn.html

TS:   // worker_threads 线程池
来源：http://hz.jiagoushi.top/gtovarlovh.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.jinqigufen.top/gttpqoeqow.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.mhx1999.top/gtsbqhmyuq.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.ybcxt.top/gtnjotfbqa.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.zhixingplan.top/gtwnffzkzc.html

[O03] 加锁保护共享数据
来源：http://hz.gogol.net.cn/gtofrgsywt.html

Py:   with lock: shared += 1
来源：http://hz.aibaodan.cn/gtbpdyykun.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.bjfxy.top/gtdldjxtdf.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.sxryk.cn/gttpwjldgn.html

TS:   // 同 JS
来源：http://hz.andypj.xyz/gtuimwphlh.html

Java: synchronized (this) { shared++; }
来源：http://hz.tanke756.top/gtjocceobk.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.iojbl.cn/gtpyhrvevq.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.zhoulong.xyz/gtgoiruazg.html

C#:   lock (gate) { shared++; }
来源：http://hz.quarkkingdee.top/gtcygiingz.html

[O04] 定义异步函数并等待
来源：http://hz.jinqigfzy.top/gtqvgqhvta.html

Py:   async def f():⏎    await g()
来源：http://hz.shuidangran.top/gtokwzbcxd.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.zhixingplan.top/gtibxdnuru.html

JS:   async function f() { await g(); }
来源：http://hz.aizwys.cn/gtyvpvngqd.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.aibaodan.cn/gtvwswrvia.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.shangyingyoupin.top/gtnekxysae.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.sxryk.cn/gtvtawdzmo.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.vqdsnc.cn/gtdsdjsflf.html

C#:   async Task F() { await G(); }
来源：http://hz.daxiang520.top/gtxldeglhm.html

[O05] 并发执行并等待全部完成
来源：http://hz.meibo888.top/gteoryrhyw.html

Py:   asyncio.gather(*tasks)
来源：http://hz.gogol.net.cn/gtmctymoth.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.feifeiyinyue.top/gtefstzswh.html

JS:   await Promise.all(tasks)
来源：http://hz.jiagoushi.top/gtfappqhpa.html

TS:   await Promise.all(tasks)
来源：http://hz.xziqi.cn/gttefemjyp.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.zhiwuduotai.top/gtsdbzwypa.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.ydzc1.top/gtnankwvcs.html

Ruby: threads.map(&:join)
来源：http://hz.316326.xyz/gtevovbcma.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.nwbrower.top/gtgvvbycti.html

[O06] 使用进程池
来源：http://hz.haohaochexian.top/gtjkdwushv.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.nanxuanxn.top/gtehdhzhqn.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.ywan-chungtsiang.top/gtdvgieqwv.html

JS:   // child_process / cluster 模块
来源：http://hz.feifeiyinyue.top/gtpidlnkux.html

TS:   // child_process / cluster 模块
来源：http://hz.meibo888.top/gtwgthveef.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.chenlongwang.top/gtlkmycksc.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.dashuyun.cn/gtaxujniax.html

Ruby: // fork 块
来源：http://hz.havefunace.top/gtdybsrmco.html

C#:   Parallel.For
来源：http://hz.nanxinkj.top/gtgwpasvry.html

================================================================================
来源：http://hz.aibaodan.cn/gtpaxtezzo.html

P. 常用工具函数
来源：http://hz.xziqi.cn/gtsvpjtlqo.html

================================================================================
来源：http://hz.jqgufenzy.top/gtshyklprf.html

[P01] 生成 UUID
来源：http://hz.wangdashe.top/gttijfhyvc.html

Py:   str(uuid.uuid4())
来源：http://hz.hfpthk.cn/gtxcvrfltn.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.sufxvd.cn/gtynpzivda.html

JS:   crypto.randomUUID()
来源：http://hz.tianlin.xyz/gthmcszmmb.html

TS:   crypto.randomUUID()
来源：http://hz.52xcode.cn/gtcfrlmcos.html

Java: UUID.randomUUID().toString()
来源：http://hz.snrcjt.cn/gtxwenkbro.html

Go:   // 用 github.com/google/uuid
来源：http://hz.bjfxy.top/gtnqifzckq.html

Ruby: SecureRandom.uuid
来源：http://hz.iojbl.cn/gtwinagpjk.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.jinyuanbaomall.cn/gtccphteiw.html

[P02] MD5 / SHA256 摘要
来源：http://hz.kuanghao11.cn/gtxmvulpzc.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.ydzc1.top/gtljfwbrng.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.mhx1999.top/gthoobjpsi.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.cheryme.top/gtbyckgrhw.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.chenjidiqi.icu/gtwpvlhhfi.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.kuanghao11.cn/gtfavcsije.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.tian-w.cn/gtgvplojzq.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.sufxvd.cn/gtoitzlutx.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.ydzc1.top/gtoyksuyym.html

[P03] 生成短随机字符串
来源：http://hz.hnqzz.top/gtievftynt.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.yangfankeji.com/gtseofjgco.html


<!-- 参考信息 -->