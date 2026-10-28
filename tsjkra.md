代发 wailian999

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.nanxuanxn.top/gtbpanltsv.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.hammf.cn/gtavqqqxfy.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.fzhhl.top/gtydyjnxys.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.ydjk.org.cn/gtulxuaxzn.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.sxryk.cn/gtprpzpear.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.jinqigfzy.top/gttvcgtthz.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.birdmap.top/gtfkhtfbjv.html

[L06] 解析响应为 JSON
来源：http://hz.xinyue.icu/gtwgiwxseq.html

Py:   resp.json()
来源：http://hz.cheryme.top/gtvrmxyigp.html

PHP:  json_decode($body, true);
来源：http://hz.hnqzz.top/gtotrgplim.html

JS:   await resp.json()
来源：http://hz.shuidangran.top/gtofcjuwbc.html

TS:   await resp.json()
来源：http://hz.gaohongyu789.top/gtvpkoyecw.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.gogol.net.cn/gtebbxnrxe.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.hongshengwenyu.top/gtydznoeie.html

Ruby: JSON.parse(resp.body)
来源：http://hz.shanyushiyangkeji.top/gtwmeszxhh.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.zhixingplan.top/gtdhvuvxwa.html

[L07] 处理 HTTP 状态码
来源：http://hz.nwbrower.top/gtkxsbkaav.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.xziqi.cn/gtaxvbhkfp.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.jinqigfzy.top/gtoexknkwa.html

JS:   resp.ok;  resp.status
来源：http://hz.aibaodan.cn/gtabeorgqq.html

TS:   resp.ok;  resp.status
来源：http://hz.guowangkeji.top/gtbepservz.html

Java: resp.statusCode()
来源：http://hz.shuidangran.top/gtguydfovw.html

Go:   resp.StatusCode
来源：http://hz.jianghu66.top/gtukcthamm.html

Ruby: resp.code.to_i
来源：http://hz.ydjk.org.cn/gtnqsvwagp.html

C#:   (int)resp.StatusCode
来源：http://hz.dianchejie.cn/gtomevcgjo.html

[L08] 并发请求多个地址
来源：http://hz.hongshengwenyu.top/gteslgbwoq.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.yvedp.cn/gtqnwjoxtb.html

PHP:  curl_multi_init() 系列
来源：http://hz.shuidangran.top/gtfhntsnrz.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.52xcode.cn/gtytbdfceb.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.xziqi.cn/gtlzgzonpr.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.ydjk.org.cn/gtdywuroik.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.iojbl.cn/gtfjxowpez.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.feifeiyinyue.top/gtamhtssic.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.guannengcc.top/gtciwstdmw.html

================================================================================
来源：http://hz.hfpthk.cn/gtsaadnfjt.html

M. 命令行 / 进程 / 环境
来源：http://hz.xuetiantiany.cn/gtsneblgxd.html

================================================================================
来源：http://hz.vqdsnc.cn/gtochcrzto.html

[M01] 读取命令行参数
来源：http://hz.haohaochexian.top/gtslummcym.html

Py:   sys.argv[1:]
来源：http://hz.tanke756.top/gtuxmvaxjb.html

PHP:  $argv;  $argc;
来源：http://hz.ehwqpu.com/gtevvvqdbd.html

JS:   process.argv.slice(2)
来源：http://hz.dashuyun.cn/gtgaknczas.html

TS:   process.argv.slice(2)
来源：http://hz.quarkkingdee.top/gtppjvsbvm.html

Java: args 数组（main 方法参数）
来源：http://hz.jinghuilouyu.cn/gthkumvpnx.html

Go:   os.Args[1:]
来源：http://hz.sysykeji.top/gtcdqsqyce.html

Ruby: ARGV
来源：http://hz.tanke756.top/gtsdcnucuc.html

C#:   args 数组（Main 方法参数）
来源：http://hz.sysykeji.top/gtxmyzqxrj.html

[M02] 读取环境变量
来源：http://hz.nanxinkj.top/gtekxzskuf.html

Py:   os.environ.get("HOME")
来源：http://hz.dashuyun.cn/gtwwxrbmej.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.zhijiandao.cn/gtmiozkwwj.html

JS:   process.env.HOME
来源：http://hz.52xcode.cn/gtvvzefkms.html

TS:   process.env.HOME
来源：http://hz.chenzaomai.com/gtgzdvmfxh.html

Java: System.getenv("HOME")
来源：http://hz.yj20258888.top/gtfqnozeki.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.tianlin.xyz/gtjltarzsl.html

Ruby: ENV["HOME"]
来源：http://hz.zhoulong.xyz/gtertwrqpq.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.xingfuxueyuan.xyz/gtlkwhdqlq.html

[M03] 执行外部命令
来源：http://hz.shanyushiyangtech.top/gtslxiyagn.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.52xcode.cn/gtjtooqdjx.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.chenjidiqi.icu/gtrgvgxuxj.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.gotoacloud.top/gtggaxfmzr.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.smart0.xyz/gtzsbgpjrg.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.ywan-chungtsiang.top/gtamthvenr.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.cqqwz.cn/gtzhirjnei.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.nanxuanxn.top/gtrfszxrcy.html

C#:   Process.Start("ls", "-l");
来源：http://hz.zycfv.cn/gtdsfqwvsu.html

[M04] 获取当前工作目录
来源：http://hz.daria6918.cn/gtasetdjgd.html

Py:   os.getcwd()
来源：http://hz.cqqwz.cn/gtepavinxr.html

PHP:  getcwd();
来源：http://hz.xuanzx.com/gtqdsayimt.html

JS:   process.cwd()
来源：http://hz.shzxlz.cn/gthgvhhwft.html

TS:   process.cwd()
来源：http://hz.jiagoushi.top/gtmpfubfci.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.gaohongyu789.top/gtoakjwlqn.html

Go:   os.Getwd()
来源：http://hz.andypj.xyz/gtpnozafjy.html

Ruby: Dir.pwd
来源：http://hz.zhiwuduotai.top/gtiwchpsww.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.mhx1999.top/gtjuobtbfm.html

[M05] 设置退出码
来源：http://hz.yuanzhike.top/gtftowaktr.html

Py:   sys.exit(1)
来源：http://hz.chenzaomai.com/gtrdxejfaq.html

PHP:  exit(1);
来源：http://hz.jlsjyb.cn/gtyfdvcmyz.html

JS:   process.exit(1)
来源：http://hz.shangyingyoupin.top/gtwdzrmavy.html

TS:   process.exit(1)
来源：http://hz.zycfv.cn/gtrfuzqyvm.html

Java: System.exit(1)
来源：http://hz.cucudq.cn/gtoabbksac.html

Go:   os.Exit(1)
来源：http://hz.yj20258.top/gtymuzbint.html

Ruby: exit 1
来源：http://hz.sweek.top/gtmtqfvutp.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.daria6918.cn/gtgysxyeui.html

[M06] 向标准错误输出
来源：http://hz.meibo888.top/gtsxncmcks.html

Py:   print("err", file=sys.stderr)
来源：http://hz.jinqigfzy.top/gtfrhgekzb.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.zdqjudy.top/gtylrwpver.html

JS:   console.error("err")
来源：http://hz.aizwys.cn/gtcumbpryd.html

TS:   console.error("err")
来源：http://hz.hnqzz.top/gtnvnwtfdx.html

Java: System.err.println("err")
来源：http://hz.gogol.net.cn/gtbarslisf.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.jinqigufen.top/gtecgfhyyb.html

Ruby: warn "err"
来源：http://hz.yuxming.cn/gtmexzxwvd.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.52xcode.cn/gtdcvoskgt.html

[M07] 判断是否为主入口
来源：http://hz.mhx1999.top/gtobycberh.html

Py:   if __name__ == "__main__":
来源：http://hz.zhoulong.xyz/gtokglxygz.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.vqdsnc.cn/gtzzqkkbyr.html

JS:   require.main === module
来源：http://hz.smart0.xyz/gtqxylskfv.html

TS:   require.main === module
来源：http://hz.shzxlz.cn/gtuxqezowr.html

Java: public static void main(String[] args)
来源：http://hz.yueranfly.top/gtbiacznxe.html

Go:   func main()
来源：http://hz.ydjk.org.cn/gtiykuslld.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.yonumen.top/gtugpsoswm.html

C#:   static void Main(string[] args)
来源：http://hz.9152youxi.cn/gtraywkmsf.html

[M08] 获取系统与运行时信息
来源：http://hz.9152youxi.cn/gtfvwlhsyd.html

Py:   platform.system();  platform.python_version()
来源：http://hz.chenzaomai.com/gtfhrmfbud.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.yuxming.cn/gtvyllijbr.html

JS:   process.platform;  process.version
来源：http://hz.gogol.net.cn/gtnlowgqeh.html

TS:   process.platform;  process.version
来源：http://hz.shangyingyoupin.top/gtdroyofjx.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.ivvv.top/gtnlzgujpp.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.ehwqpu.com/gtsdtgpedr.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.0kj1m.cn/gtzwyrcvfh.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.iojbl.cn/gtflishnbu.html

================================================================================
来源：http://hz.zhengqikj.top/gtoiabkemb.html

N. 数据结构与算法
来源：http://hz.yanxiufei.cn/gtzjalzqqg.html

================================================================================
来源：http://hz.bjfxy.top/gtumlwuqit.html

[N01] 二分查找（有序数组）
来源：http://hz.tianlin.xyz/gtddnunkwl.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.fzhhl.top/gtidikzsvp.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.c1oappe.top/gththexyct.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jqgufenzy.top/gtlcqetzou.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.tian-w.cn/gtwzupqyrg.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.guowangkeji.top/gtjvrjshju.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.c1oappe.top/gtcphhpcay.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.shzxlz.cn/gtixbsbafq.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.jqgfzy.top/gtbwspugan.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.cashguo.top/gtmbbgimzz.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.yvedp.cn/gthgyximkp.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.hongshengwenyu.top/gtdhwvkniw.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.aibaodan.cn/gtqddmoycl.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.zhoulong.xyz/gtcrfwgabh.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.chenjidiqi.icu/gtvoligkjo.html

Go:   slices.Sort(arr)
来源：http://hz.gogol.net.cn/gtqytzynmn.html

Ruby: arr.sort
来源：http://hz.xuetiantiany.cn/gtkadfcphz.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.dashuyun.cn/gttcpsqoiy.html

[N03] 快速排序（分治示例）
来源：http://hz.chenjidiqi.icu/gtzkmdzqez.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.meibo888.top/gtzchnbewo.html

PHP:  // 递归实现，或用 usort
来源：http://hz.xinyue.icu/gtwqltgtkp.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.shuidangran.top/gtdyicfvpl.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yuxming.cn/gtyccvdqqx.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.smart0.xyz/gtnrsqyeoz.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.yvedp.cn/gtajafyzbh.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.9152youxi.cn/gtbcteaemd.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.yuanzhike.top/gtsgzgkedm.html

[N04] 斐波那契数列
来源：http://hz.ywan-chungtsiang.top/gtvuxvhsfk.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.zhiwuduotai.top/gtdqndykyi.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.yongpay.top/gtufdbaagh.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.xingfuxueyuan.xyz/gtusofgwuh.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yj20258888.top/gteogrisyo.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.snrcjt.cn/gtclfsirgp.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.zhaomingkeji.xyz/gtbibbgkps.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.meibo888.top/gtwtklqhxf.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.ywan-chungtsiang.top/gtowgpxcza.html

[N05] 最大公约数
来源：http://hz.mhx1999.top/gttnsisxsc.html

Py:   math.gcd(a, b)
来源：http://hz.cashguo.top/gthejggtba.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.gogol.net.cn/gtpwzjzmog.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.c1oappe.top/gtcnzlqmrj.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.xylfe.cn/gtvjsfrmor.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.xylfe.cn/gtfkqmhmfq.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.cheryme.top/gtiwkrsehk.html

Ruby: a.gcd(b)
来源：http://hz.jlsjyb.cn/gtmmftyskg.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.c1oappe.top/gtcizwpetn.html

[N06] 判断回文字符串
来源：http://hz.xuetiantiany.cn/gthvksplcw.html

Py:   s == s[::-1]
来源：http://hz.feifeiyinyue.top/gtcinmdfzy.html

PHP:  $s === strrev($s);
来源：http://hz.hfpthk.cn/gtnzeggahk.html

JS:   s === [...s].reverse().join("")
来源：http://hz.shanyushiyangtech.top/gthauoxliq.html

TS:   s === [...s].reverse().join("")
来源：http://hz.iojbl.cn/gtzsvjfhxj.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.ybcxt.top/gtvmqkcpkd.html

Go:   // 双指针从两端比较
来源：http://hz.yvedp.cn/gtujpgakwt.html

Ruby: s == s.reverse
来源：http://hz.zhaomingkeji.xyz/gtjzwklcan.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.hywenlv.cn/gtlbvtkeaf.html

[N07] 两数之和（返回下标）
来源：http://hz.chenjidiqi.icu/gtusojluba.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.jinyuanbaomall.cn/gtjwhaemel.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.cqqwz.cn/gtdvcomewn.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.sweek.top/gtgqkklpdi.html

TS:   // 手写 Map<string, number>
来源：http://hz.kuanghao11.cn/gtcimwznqd.html

Java: // 手写 HashMap
来源：http://hz.kuanghao11.cn/gtpwrwblae.html

Go:   // 手写 map[int]int
来源：http://hz.sysykeji.top/gtmnuzvvqo.html

Ruby: // 手写 Hash
来源：http://hz.yueranfly.top/gtifjqzows.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.jiagoushi.top/gttibitadm.html

[N08] 生成全排列
来源：http://hz.52xcode.cn/gtcgacedyn.html

Py:   itertools.permutations(arr)
来源：http://hz.tian-w.cn/gttgmceirf.html

PHP:  // 手写递归交换
来源：http://hz.gaohongyu789.top/gtybwlrfer.html

JS:   // 手写回溯递归
来源：http://hz.gogol.net.cn/gtiydktloo.html

TS:   // 手写回溯递归
来源：http://hz.xinyue.icu/gtxetgwmiw.html

Java: // 手写回溯递归
来源：http://hz.tianlin.xyz/gtyvfbqmwg.html

Go:   // 手写回溯递归
来源：http://hz.nanxuanxn.top/gtpxotzhaf.html

Ruby: arr.permutation.to_a
来源：http://hz.gogol.net.cn/gtaorbjjld.html

C#:   // 手写回溯递归
来源：http://hz.hongshengwenyu.top/gtakeueldd.html

[N09] 栈与队列
来源：http://hz.sweek.top/gtrigtdtoe.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.jinqigufen.top/gtdsvvqemp.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.ehwqpu.com/gtywyqpapx.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.fzhhl.top/gtvkamzciu.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.xuetiantiany.cn/gtvpugubco.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.gzhubu.top/gtzphijpjx.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.wangdashe.top/gtgusotwub.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.vqdsnc.cn/gtvkbpdzkg.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.316326.xyz/gtiaeopcva.html

[N10] 链表节点定义
来源：http://hz.daria6918.cn/gtidsdimdc.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.jinghuilouyu.cn/gtcpzgmakc.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.xuanzx.com/gtjlugmeyp.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.vqdsnc.cn/gtjxrmnwee.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.hammf.cn/gtwrciyvcw.html

Java: class Node { int v; Node next; }
来源：http://hz.316326.xyz/gtsspsogqg.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.feifeiyinyue.top/gtbcnlmjyc.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.ydzc1.top/gtxalmoggm.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.cheryme.top/gtvcqmknuc.html

[N11] 二叉树中序遍历
来源：http://hz.fengsongda.top/gtpkpnwifg.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.ywan-chungtsiang.top/gtuwnwqclv.html

PHP:  // 手写递归函数
来源：http://hz.shuidangran.top/gtahtvyjdx.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.xingfuxueyuan.xyz/gtmupzmfnw.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.zdqjudy.top/gtyafehmyz.html

Java: // 手写递归
来源：http://hz.mhx1999.top/gtkzbmhqll.html

Go:   // 手写递归
来源：http://hz.jinqigufen.top/gtddlxyyrs.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.hywenlv.cn/gtadkiaxrb.html

C#:   // 手写递归
来源：http://hz.shangyingyoupin.top/gtwuzayhnz.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.jyoumei.cn/gtmaiorcin.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.yangfankeji.com/gtpztrazrj.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.ydzc1.top/gtlggbzhwd.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.chenzaomai.com/gtwnxgtnwk.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jinqigfzy.top/gtmtousljt.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.sweek.top/gteumuoltl.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.havefunace.top/gtlpxtbxnq.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.hongshengwenyu.top/gtqymihiqr.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.xziqi.cn/gtqezmjkfl.html

================================================================================
来源：http://hz.zhoulong.xyz/gtrftzpgmn.html

O. 并发与异步
来源：http://hz.chenzaomai.com/gtfxutklud.html

================================================================================
来源：http://hz.0kj1m.cn/gtnvvidkxe.html

[O01] 启动一个线程
来源：http://hz.dashuyun.cn/gtksnfhewe.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.hammf.cn/gtrxitsnzm.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.shanyushiyangtech.top/gtlpnujnkw.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.yj20258.top/gterimyoip.html

TS:   // 同 JS
来源：http://hz.jqgufenzy.top/gtkzkmzzbo.html

Java: new Thread(() -> f()).start()
来源：http://hz.gaohongyu789.top/gtieytqwjw.html

Go:   go f()
来源：http://hz.tian-w.cn/gtlniqdklw.html

Ruby: Thread.new { f }
来源：http://hz.yuxming.cn/gtevryvcxj.html

C#:   Task.Run(() => F());
来源：http://hz.xinyue.icu/gtceeecrpw.html

[O02] 使用线程池
来源：http://hz.aibaodan.cn/gtkbrglrcc.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.hammf.cn/gtgeyllqys.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.0kj1m.cn/gtcnvlhkxb.html

JS:   // worker_threads 线程池
来源：http://hz.yj202588.top/gthqmgcqzr.html

TS:   // worker_threads 线程池
来源：http://hz.yueranfly.top/gtdqchcvuh.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.sweek.top/gteywosahe.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.xuetiantiany.cn/gtaxwjmhtx.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.hongshengwenyu.top/gtbcnykbfz.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.jinyuanbaomall.cn/gttrtfrnsb.html

[O03] 加锁保护共享数据
来源：http://hz.daxiang520.top/gtbzvuerth.html

Py:   with lock: shared += 1
来源：http://hz.hnqzz.top/gtdbnthfpj.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.zhiwuduotai.top/gtwdwgyiwz.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.xylfe.cn/gtipmbfaqw.html

TS:   // 同 JS
来源：http://hz.hywenlv.cn/gtwkivaqaq.html

Java: synchronized (this) { shared++; }
来源：http://hz.zhaomingkeji.xyz/gtzwkgexaz.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.xylfe.cn/gttedcouzx.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.tianlin.xyz/gtvoeispcb.html

C#:   lock (gate) { shared++; }
来源：http://hz.zycfv.cn/gtmgqzcjns.html

[O04] 定义异步函数并等待
来源：http://hz.zycfv.cn/gtyywbqftz.html

Py:   async def f():⏎    await g()
来源：http://hz.smart0.xyz/gttzqlffph.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.316326.xyz/gteiefyltg.html

JS:   async function f() { await g(); }
来源：http://hz.chenzaomai.com/gtaamyoned.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.cashguo.top/gtzhfxvqsn.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.tanke756.top/gtpldcfmwq.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.jinqigufen.top/gtnzbudyxq.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.sufxvd.cn/gtyfuwuhvv.html

C#:   async Task F() { await G(); }
来源：http://hz.guannengcc.top/gtlogbleog.html

[O05] 并发执行并等待全部完成
来源：http://hz.vqdsnc.cn/gtguqzxsvz.html

Py:   asyncio.gather(*tasks)
来源：http://hz.yonumen.top/gtguxuchzd.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.redwolf501.top/gtqltcihic.html

JS:   await Promise.all(tasks)
来源：http://hz.hongshengwenyu.top/gtaiofjdhh.html

TS:   await Promise.all(tasks)
来源：http://hz.hammf.cn/gtqeejemel.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.chenlongwang.top/gtkkctafex.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.jianghu66.top/gtqipegpsm.html

Ruby: threads.map(&:join)
来源：http://hz.jqgfzy.top/gtjdrthnpe.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.yj202588.top/gtvvrithgz.html

[O06] 使用进程池
来源：http://hz.daxiang520.top/gtupbsrscc.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.nanxinkj.top/gtoeylxbao.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.nanxuanxn.top/gtdbmblvlg.html

JS:   // child_process / cluster 模块
来源：http://hz.andypj.xyz/gtayrieupm.html

TS:   // child_process / cluster 模块
来源：http://hz.9152youxi.cn/gtwcowozwi.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.nwbrower.top/gtzppttdeu.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.cucudq.cn/gtsvrblrqu.html

Ruby: // fork 块
来源：http://hz.meibo888.top/gtawixjrah.html

C#:   Parallel.For
来源：http://hz.chenzaomai.com/gtvtauwbri.html

================================================================================
来源：http://hz.vqdsnc.cn/gtbpkuvtho.html

P. 常用工具函数
来源：http://hz.jiagoushi.top/gtyyndnjbl.html

================================================================================
来源：http://hz.jinqigfzy.top/gtjpdpyrcx.html

[P01] 生成 UUID
来源：http://hz.yanxiufei.cn/gtnjzmmrgj.html

Py:   str(uuid.uuid4())
来源：http://hz.yonumen.top/gtxsdmdshi.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.tian-w.cn/gtkwkgbomd.html

JS:   crypto.randomUUID()
来源：http://hz.shangyingyoupin.top/gtslupgcqb.html

TS:   crypto.randomUUID()
来源：http://hz.ivvv.top/gtcdwzkjge.html

Java: UUID.randomUUID().toString()
来源：http://hz.zhaomingkeji.xyz/gtwcyavwlx.html

Go:   // 用 github.com/google/uuid
来源：http://hz.tanke756.top/gtingiiqfi.html

Ruby: SecureRandom.uuid
来源：http://hz.jinghuilouyu.cn/gtekurgudp.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.tian-w.cn/gtpwmbgkzb.html

[P02] MD5 / SHA256 摘要
来源：http://hz.sweek.top/gtizffewhs.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.aizwys.cn/gtxceoutpq.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.birdmap.top/gtdohgjhiz.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.sweek.top/gtpfpclphd.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.havefunace.top/gtwmxvdhev.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.daxiang520.top/gtetyzmhvf.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.yonumen.top/gtefpbcqvr.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.daria6918.cn/gtjmpuuhtv.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.guowangkeji.top/gtlarsyohq.html

[P03] 生成短随机字符串
来源：http://hz.sufxvd.cn/gtzxmmfhop.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.sysykeji.top/gtundsqygt.html


<!-- 参考信息 -->