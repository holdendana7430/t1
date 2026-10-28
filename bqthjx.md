代发 wailian999

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.havefunace.top/gtbspffwio.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.ivvv.top/gtzrnalbdp.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.nwbrower.top/gtsoykrikf.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.xuetiantiany.cn/gtzjwriqsd.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.yangfankeji.com/gtsdmjipto.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.gotoacloud.top/gtbccuqwmz.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.nanxuanxn.top/gttrrrqmdx.html

[L06] 解析响应为 JSON
来源：http://hz.jiagoushi.top/gtfqfusivp.html

Py:   resp.json()
来源：http://hz.gogol.net.cn/gtumqrqhkx.html

PHP:  json_decode($body, true);
来源：http://hz.xylfe.cn/gtmqdkkjjf.html

JS:   await resp.json()
来源：http://hz.jqgufenzy.top/gtbcnliupz.html

TS:   await resp.json()
来源：http://hz.cdnleiting.top/gteoqqmzxy.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.hywenlv.cn/gtqruugvby.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.aibaodan.cn/gtcawrfnzf.html

Ruby: JSON.parse(resp.body)
来源：http://hz.zhongyouzk.top/gtutqahvpl.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.chenzaomai.com/gtlgqfrzfo.html

[L07] 处理 HTTP 状态码
来源：http://hz.ehwqpu.com/gtwdsoynth.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.jinyuanbaomall.cn/gthjvlwtpv.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.chenlongwang.top/gtpbtlbyxg.html

JS:   resp.ok;  resp.status
来源：http://hz.sxryk.cn/gtdottgjdu.html

TS:   resp.ok;  resp.status
来源：http://hz.tian-w.cn/gtgzhekmpy.html

Java: resp.statusCode()
来源：http://hz.ydzc1.top/gtnlsuorfp.html

Go:   resp.StatusCode
来源：http://hz.jyoumei.cn/gtvvlwxgdr.html

Ruby: resp.code.to_i
来源：http://hz.yanxiufei.cn/gtygjzczel.html

C#:   (int)resp.StatusCode
来源：http://hz.yangfankeji.com/gtweveeetd.html

[L08] 并发请求多个地址
来源：http://hz.daxiang520.top/gtuirxclti.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.guannengcc.top/gtxngueqzs.html

PHP:  curl_multi_init() 系列
来源：http://hz.gotoacloud.top/gtqndnbbqb.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.ppjwa.cn/gtaizifsnu.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.wangdashe.top/gtmxgayrfr.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.c1oappe.top/gtfcbwkmvo.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.tianlin.xyz/gtyvbwpkce.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.xuanzx.com/gtliovysfd.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.jianghu66.top/gtsbaceahh.html

================================================================================
来源：http://hz.vqdsnc.cn/gtdpewgbow.html

M. 命令行 / 进程 / 环境
来源：http://hz.feifeiyinyue.top/gtpqtsvkbq.html

================================================================================
来源：http://hz.xuanzx.com/gtmzcmgijr.html

[M01] 读取命令行参数
来源：http://hz.zycfv.cn/gtgntgqmql.html

Py:   sys.argv[1:]
来源：http://hz.jinqigufen.top/gtbdpsqfrt.html

PHP:  $argv;  $argc;
来源：http://hz.dianchejie.cn/gtmrewdnrv.html

JS:   process.argv.slice(2)
来源：http://hz.hysaishi.cn/gtfpdwhruh.html

TS:   process.argv.slice(2)
来源：http://hz.dianchejie.cn/gtgskzsyhn.html

Java: args 数组（main 方法参数）
来源：http://hz.meibo888.top/gtdpdokvav.html

Go:   os.Args[1:]
来源：http://hz.tian-w.cn/gtkytizafy.html

Ruby: ARGV
来源：http://hz.meibo888.top/gtoakzjmze.html

C#:   args 数组（Main 方法参数）
来源：http://hz.mhx1999.top/gtvravdpff.html

[M02] 读取环境变量
来源：http://hz.hnqzz.top/gtdrfhtdnw.html

Py:   os.environ.get("HOME")
来源：http://hz.yonumen.top/gtxvsrhorh.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.hongshengwenyu.top/gtosnyuihn.html

JS:   process.env.HOME
来源：http://hz.havefunace.top/gtunoinkgd.html

TS:   process.env.HOME
来源：http://hz.c1oappe.top/gthgdssxox.html

Java: System.getenv("HOME")
来源：http://hz.dashuyun.cn/gtuxartoyu.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.52xcode.cn/gtpdeoxerf.html

Ruby: ENV["HOME"]
来源：http://hz.sufxvd.cn/gtyxasrbfg.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.guowangkeji.top/gtbaqdqhol.html

[M03] 执行外部命令
来源：http://hz.yj20258888.top/gtdapghvdl.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.xuanzx.com/gtfusrbwlm.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.zycfv.cn/gtdlewtncv.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.guannengcc.top/gtvzvnrojg.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.chenzaomai.com/gtxmycvykk.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.shanyushiyangtech.top/gtxejtnlaf.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.havefunace.top/gtuilxpixg.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.jinqigfzy.top/gtddsqhaln.html

C#:   Process.Start("ls", "-l");
来源：http://hz.sufxvd.cn/gtetthufxh.html

[M04] 获取当前工作目录
来源：http://hz.yj202588.top/gtviktvibx.html

Py:   os.getcwd()
来源：http://hz.9152youxi.cn/gttfiyvvci.html

PHP:  getcwd();
来源：http://hz.wangshuangyany.cn/gtviplmokx.html

JS:   process.cwd()
来源：http://hz.kuanghao11.cn/gtsssmwmjd.html

TS:   process.cwd()
来源：http://hz.gzhubu.top/gtbwfuizal.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.yueranfly.top/gtceukoqws.html

Go:   os.Getwd()
来源：http://hz.svipenyu.cn/gtmjwaeelj.html

Ruby: Dir.pwd
来源：http://hz.iojbl.cn/gtwamrbugw.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.yonumen.top/gtdunghdni.html

[M05] 设置退出码
来源：http://hz.birdmap.top/gtqtttzdek.html

Py:   sys.exit(1)
来源：http://hz.jinqigufen.top/gtpjehspod.html

PHP:  exit(1);
来源：http://hz.tianlin.xyz/gttzmqcwmp.html

JS:   process.exit(1)
来源：http://hz.xylfe.cn/gthihokyzg.html

TS:   process.exit(1)
来源：http://hz.gotoacloud.top/gtdyrvrtkc.html

Java: System.exit(1)
来源：http://hz.zycfv.cn/gtkvtnztot.html

Go:   os.Exit(1)
来源：http://hz.shangyingyoupin.top/gtapquccaw.html

Ruby: exit 1
来源：http://hz.c1oappe.top/gtsconqjks.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.nwbrower.top/gtcgfqmqwm.html

[M06] 向标准错误输出
来源：http://hz.hfpthk.cn/gtjcfewlkd.html

Py:   print("err", file=sys.stderr)
来源：http://hz.cdnleiting.top/gthvjejvol.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.xylfe.cn/gtxugawqib.html

JS:   console.error("err")
来源：http://hz.redwolf501.top/gtgyzpnykg.html

TS:   console.error("err")
来源：http://hz.tianlin.xyz/gtosrgiehq.html

Java: System.err.println("err")
来源：http://hz.daria6918.cn/gtsfnkgbmn.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.jianghu66.top/gtfbezcrse.html

Ruby: warn "err"
来源：http://hz.zhengqikj.top/gtrscpotxt.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.shuidangran.top/gtkwsfvovk.html

[M07] 判断是否为主入口
来源：http://hz.guannengcc.top/gthofydxvl.html

Py:   if __name__ == "__main__":
来源：http://hz.tanke756.top/gtjfvwnbvj.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.hongshengwenyu.top/gtmdfppskc.html

JS:   require.main === module
来源：http://hz.ehwqpu.com/gtzccplgio.html

TS:   require.main === module
来源：http://hz.yonumen.top/gtavntcshx.html

Java: public static void main(String[] args)
来源：http://hz.fzhhl.top/gtubxwdyqi.html

Go:   func main()
来源：http://hz.kuanghao11.cn/gtqqgnxuus.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.dianchejie.cn/gtynceuenp.html

C#:   static void Main(string[] args)
来源：http://hz.jlsjyb.cn/gtalfwkyot.html

[M08] 获取系统与运行时信息
来源：http://hz.hongshengwenyu.top/gtcplmwmnf.html

Py:   platform.system();  platform.python_version()
来源：http://hz.daxiang520.top/gtrrrczbby.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.shangyingyoupin.top/gtxrrvldxb.html

JS:   process.platform;  process.version
来源：http://hz.yuanzhike.top/gtxihhjdwh.html

TS:   process.platform;  process.version
来源：http://hz.tianlin.xyz/gtmdsneore.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.snrcjt.cn/gtchjxpymt.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.chenzaomai.com/gtoemfjwtc.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.yj20258.top/gtsnckcjet.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.cashguo.top/gticmkzyfi.html

================================================================================
来源：http://hz.hongshengwenyu.top/gthfigkpsx.html

N. 数据结构与算法
来源：http://hz.jinqigufen.top/gtkxrjzmic.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtexlmfenz.html

[N01] 二分查找（有序数组）
来源：http://hz.wangdashe.top/gtgmdjvfjm.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.daxiang520.top/gtjdjgndrv.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.fengsongda.top/gtfgshncsw.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.svipenyu.cn/gtbajiqdho.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.ywan-chungtsiang.top/gtgjevbzpp.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.snrcjt.cn/gtqolsnizh.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.aibaodan.cn/gtlxcyceiu.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.c1oappe.top/gtxidzgtnj.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.meibo888.top/gtocopspcn.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.jianghu66.top/gtbvphllnw.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.tianlin.xyz/gttqqnbvug.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.zhengqikj.top/gtqfklmilb.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.zhengqikj.top/gtvmvhbvld.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yonumen.top/gthvsgvkgz.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.chenjidiqi.icu/gtqtnghrpv.html

Go:   slices.Sort(arr)
来源：http://hz.yongpay.top/gtcptfvqpr.html

Ruby: arr.sort
来源：http://hz.xuanzx.com/gtghzkhsau.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.jqgufenzy.top/gtohbiudlf.html

[N03] 快速排序（分治示例）
来源：http://hz.gzhubu.top/gtoawfrixt.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.52xcode.cn/gtanuhsnjz.html

PHP:  // 递归实现，或用 usort
来源：http://hz.andypj.xyz/gtcyswipku.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.chenzaomai.com/gtqwhlyjcr.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.dianchejie.cn/gtlidytesv.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.svipenyu.cn/gtkkbmcxqm.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.tianlin.xyz/gtauyrbezm.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.zhixingplan.top/gtymmohnca.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.jqgufenzy.top/gtxmhftcsk.html

[N04] 斐波那契数列
来源：http://hz.jqgfzy.top/gtrheltbyq.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.wangshuangyany.cn/gtewhpgsxk.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.tanke756.top/gtrggzieej.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.bjfxy.top/gtaautjqnu.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.fengsongda.top/gtjqeutzso.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.wangshuangyany.cn/gtfpszoszv.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.ppjwa.cn/gtaaoxxsvg.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.jinyuanbaomall.cn/gtpacwevlk.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.zdqjudy.top/gtwmwmrldo.html

[N05] 最大公约数
来源：http://hz.xylfe.cn/gtwtyrntcs.html

Py:   math.gcd(a, b)
来源：http://hz.chenjidiqi.icu/gtvkbayyfk.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.0kj1m.cn/gtkdftfgat.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.vqdsnc.cn/gtpsablcua.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.xuetiantiany.cn/gttsuzdnvs.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.chenlongwang.top/gtpjrhxivd.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.shangyingyoupin.top/gtnvxnqzgl.html

Ruby: a.gcd(b)
来源：http://hz.wangdashe.top/gtpowubuxb.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.yvedp.cn/gtmjttieph.html

[N06] 判断回文字符串
来源：http://hz.zycfv.cn/gtrbcgzvbd.html

Py:   s == s[::-1]
来源：http://hz.ivvv.top/gtbsqakunz.html

PHP:  $s === strrev($s);
来源：http://hz.zhiwuduotai.top/gtpxkwhmmd.html

JS:   s === [...s].reverse().join("")
来源：http://hz.chenzaomai.com/gthxmmuvzr.html

TS:   s === [...s].reverse().join("")
来源：http://hz.xziqi.cn/gtpqwaipgf.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.hnxiangtu.top/gtieagwslv.html

Go:   // 双指针从两端比较
来源：http://hz.xuanzx.com/gtibyzfzgn.html

Ruby: s == s.reverse
来源：http://hz.jinqigufen.top/gtkcddjrrj.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.nwbrower.top/gtgqlfjpek.html

[N07] 两数之和（返回下标）
来源：http://hz.zhijiandao.cn/gtzxgywsdz.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.cheryme.top/gtpjtqhzdj.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.jlsjyb.cn/gtbkzzatnf.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.ydjk.org.cn/gthmbdqeco.html

TS:   // 手写 Map<string, number>
来源：http://hz.daria6918.cn/gtqbzpnotn.html

Java: // 手写 HashMap
来源：http://hz.dianchejie.cn/gtpyavcraq.html

Go:   // 手写 map[int]int
来源：http://hz.ppjwa.cn/gtfzpvvxdi.html

Ruby: // 手写 Hash
来源：http://hz.sxryk.cn/gtkemldvxe.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.gotoacloud.top/gtkbwzhofa.html

[N08] 生成全排列
来源：http://hz.jyoumei.cn/gtxvvkeogx.html

Py:   itertools.permutations(arr)
来源：http://hz.yj20258888.top/gtenhctgtc.html

PHP:  // 手写递归交换
来源：http://hz.meibo888.top/gtaplcegxi.html

JS:   // 手写回溯递归
来源：http://hz.shanyushiyangtech.top/gtxnqcgqko.html

TS:   // 手写回溯递归
来源：http://hz.yvedp.cn/gtocewwsjp.html

Java: // 手写回溯递归
来源：http://hz.shuidangran.top/gtxfikvfnp.html

Go:   // 手写回溯递归
来源：http://hz.svipenyu.cn/gtcpppmqam.html

Ruby: arr.permutation.to_a
来源：http://hz.gotoacloud.top/gtvspkrcbd.html

C#:   // 手写回溯递归
来源：http://hz.yangfankeji.com/gtrmftrjob.html

[N09] 栈与队列
来源：http://hz.nanxinkj.top/gtmrsxxzwt.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.yj20258.top/gtpommzktt.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.smart0.xyz/gtipxedokp.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.yuxming.cn/gtgyckllrt.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.zycfv.cn/gtszbrtjoy.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.jiagoushi.top/gtpnnngrdl.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.shanyushiyangtech.top/gtfcawycdo.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.guannengcc.top/gtwvgkwyzh.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.xylfe.cn/gtbrcacxjx.html

[N10] 链表节点定义
来源：http://hz.xuanzx.com/gtidehpdng.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.zhijiandao.cn/gtvqvyredy.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.zhongyouzk.top/gtftrhaqzp.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.zycfv.cn/gtxpentseu.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.sufxvd.cn/gtszhesvwc.html

Java: class Node { int v; Node next; }
来源：http://hz.xingfuxueyuan.xyz/gtdpcplyfu.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.yongpay.top/gtxbdnrich.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.chenjidiqi.icu/gttbfjldkj.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.fzhhl.top/gtqnqiabqq.html

[N11] 二叉树中序遍历
来源：http://hz.316326.xyz/gtejvrdghs.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.xylfe.cn/gtdoztfefi.html

PHP:  // 手写递归函数
来源：http://hz.ppjwa.cn/gtbxhgmgiw.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yuanzhike.top/gtwtspatsx.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.hongshengwenyu.top/gtiwksrldy.html

Java: // 手写递归
来源：http://hz.guannengcc.top/gtgtrhghko.html

Go:   // 手写递归
来源：http://hz.xylfe.cn/gtxcmeklui.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.quarkkingdee.top/gtcgknuxbk.html

C#:   // 手写递归
来源：http://hz.guowangkeji.top/gtblyestex.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.svipenyu.cn/gtjmctbntv.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.316326.xyz/gtigewuvcm.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.yj202588.top/gthkcfplbg.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.shanyushiyangkeji.top/gtytivmnir.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.0kj1m.cn/gthobfutxe.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.jiagoushi.top/gtvprcxump.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.havefunace.top/gtqbbwgyfu.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.guannengcc.top/gtfiphhqen.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.shuidangran.top/gtjlgtehyp.html

================================================================================
来源：http://hz.iojbl.cn/gtvdwwlkzh.html

O. 并发与异步
来源：http://hz.shangyingyoupin.top/gtcqqljvap.html

================================================================================
来源：http://hz.zdqjudy.top/gteujtkvbm.html

[O01] 启动一个线程
来源：http://hz.52xcode.cn/gtdsonormw.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.zhengqikj.top/gtigqtxopt.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.mhx1999.top/gtnqzqzpxi.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.316326.xyz/gtrmorqvbs.html

TS:   // 同 JS
来源：http://hz.zhixingplan.top/gtvxpkzssc.html

Java: new Thread(() -> f()).start()
来源：http://hz.jlsjyb.cn/gtzxuawjti.html

Go:   go f()
来源：http://hz.nwbrower.top/gtkhelfeie.html

Ruby: Thread.new { f }
来源：http://hz.jqgufenzy.top/gtuswqbywa.html

C#:   Task.Run(() => F());
来源：http://hz.c1oappe.top/gtnjdhhdao.html

[O02] 使用线程池
来源：http://hz.redwolf501.top/gtcxeueltb.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.jinqigfzy.top/gtpezlaoek.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.yj20258.top/gtcrelabsg.html

JS:   // worker_threads 线程池
来源：http://hz.9152youxi.cn/gtjuayytds.html

TS:   // worker_threads 线程池
来源：http://hz.zhixingplan.top/gtwqmfwqah.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.aibaodan.cn/gtdhnxadqz.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.fengsongda.top/gtxdyplhbf.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.haohaochexian.top/gtibgalwnf.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.zhijiandao.cn/gtdgprvwpw.html

[O03] 加锁保护共享数据
来源：http://hz.gaohongyu789.top/gthukxuarp.html

Py:   with lock: shared += 1
来源：http://hz.quarkkingdee.top/gthkhvkpyz.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.sweek.top/gtxasbneue.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.c1oappe.top/gttxmtxksp.html

TS:   // 同 JS
来源：http://hz.cashguo.top/gtmmjqtzkq.html

Java: synchronized (this) { shared++; }
来源：http://hz.fzhhl.top/gtodmowodi.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.shanyushiyangtech.top/gtqzbvhzzd.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.ppjwa.cn/gtmyukaqzl.html

C#:   lock (gate) { shared++; }
来源：http://hz.yanxiufei.cn/gtoivbszrt.html

[O04] 定义异步函数并等待
来源：http://hz.wangshuangyany.cn/gtukqrctyb.html

Py:   async def f():⏎    await g()
来源：http://hz.yangfankeji.com/gtmaqgjbcc.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.jqgfzy.top/gtfspcpflg.html

JS:   async function f() { await g(); }
来源：http://hz.haohaochexian.top/gtgqsnxqyp.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.jyoumei.cn/gtaitmsdjd.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.yvedp.cn/gtbpoifitb.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.meibo888.top/gtguofvtni.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.daxiang520.top/gtxdibpkom.html

C#:   async Task F() { await G(); }
来源：http://hz.yangfankeji.com/gtuhgzbdgk.html

[O05] 并发执行并等待全部完成
来源：http://hz.xuanzx.com/gtpvzxjacy.html

Py:   asyncio.gather(*tasks)
来源：http://hz.jqgfzy.top/gtujojjnjc.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.xziqi.cn/gtajivwxac.html

JS:   await Promise.all(tasks)
来源：http://hz.ppjwa.cn/gtqollzetf.html

TS:   await Promise.all(tasks)
来源：http://hz.xylfe.cn/gttlnyobfr.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.guowangkeji.top/gtbqfkthjz.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.hfpthk.cn/gtyadmrbke.html

Ruby: threads.map(&:join)
来源：http://hz.zhongyouzk.top/gtokaldwmf.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.gzhubu.top/gtybnvguwx.html

[O06] 使用进程池
来源：http://hz.feifeiyinyue.top/gtvvkwyjff.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.bjfxy.top/gtwsvmamzq.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.tanke756.top/gthckqocuf.html

JS:   // child_process / cluster 模块
来源：http://hz.andypj.xyz/gtitsazule.html

TS:   // child_process / cluster 模块
来源：http://hz.0kj1m.cn/gtejzdesgn.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.yvedp.cn/gtscsazpuv.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.hfpthk.cn/gtyumogqcj.html

Ruby: // fork 块
来源：http://hz.chenlongwang.top/gtvwwkncnu.html

C#:   Parallel.For
来源：http://hz.tianlin.xyz/gthgbfgaex.html

================================================================================
来源：http://hz.sufxvd.cn/gttqxxaaqe.html

P. 常用工具函数
来源：http://hz.c1oappe.top/gtnvkcwuew.html

================================================================================
来源：http://hz.0kj1m.cn/gtlimeiqqj.html

[P01] 生成 UUID
来源：http://hz.chenzaomai.com/gtbmgrvfew.html

Py:   str(uuid.uuid4())
来源：http://hz.jinghuilouyu.cn/gtjdchqogi.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.xziqi.cn/gttkzzejea.html

JS:   crypto.randomUUID()
来源：http://hz.shanyushiyangtech.top/gtoxaizlpc.html

TS:   crypto.randomUUID()
来源：http://hz.chenlongwang.top/gtggbqabfd.html

Java: UUID.randomUUID().toString()
来源：http://hz.chenzaomai.com/gtcfknausu.html

Go:   // 用 github.com/google/uuid
来源：http://hz.jinqigufen.top/gtytndgtmu.html

Ruby: SecureRandom.uuid
来源：http://hz.redwolf501.top/gtwpyazbrm.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.yuanzhike.top/gtzbsutpsu.html

[P02] MD5 / SHA256 摘要
来源：http://hz.redwolf501.top/gtgjgnifsh.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.feifeiyinyue.top/gtgzsvxzbw.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.dianchejie.cn/gtyufkpqgn.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.gaohongyu789.top/gtzyoeuyla.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.gaohongyu789.top/gtjebrzwoj.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.sxryk.cn/gtwkoopgai.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.zhongyouzk.top/gttaitdfik.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.sysykeji.top/gtexkghbyg.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.yj20258888.top/gthuxzrszn.html

[P03] 生成短随机字符串
来源：http://hz.hywenlv.cn/gtjzdovvze.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.cheryme.top/gtcgeacnbz.html


<!-- 参考信息 -->