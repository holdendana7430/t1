代发 wailian999

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.jqgufenzy.top/gtuuirlfmu.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.zhijiandao.cn/gtmswtdwfu.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.yuanzhike.top/gtevajonag.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.jiagoushi.top/gtdixnhwlx.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.dianchejie.cn/gtyrzrjjxv.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.chenlongwang.top/gtjehatlxx.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.jyoumei.cn/gtabcrbdls.html

[L06] 解析响应为 JSON
来源：http://hz.jianghu66.top/gtidwtzwbk.html

Py:   resp.json()
来源：http://hz.ivvv.top/gtfpwllflm.html

PHP:  json_decode($body, true);
来源：http://hz.xuanzx.com/gtvjpfibzx.html

JS:   await resp.json()
来源：http://hz.dianchejie.cn/gtcusxynjo.html

TS:   await resp.json()
来源：http://hz.ywan-chungtsiang.top/gtzaggzlpa.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.jinqigfzy.top/gtxhmotpmc.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.cqqwz.cn/gtkvllwbhn.html

Ruby: JSON.parse(resp.body)
来源：http://hz.gotoacloud.top/gthnwtdxfp.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.gaohongyu789.top/gtebkmaeoi.html

[L07] 处理 HTTP 状态码
来源：http://hz.yueranfly.top/gtkyhbrdkb.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.zhongyouzk.top/gtmgxqqatz.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.c1oappe.top/gtimyhtaox.html

JS:   resp.ok;  resp.status
来源：http://hz.havefunace.top/gtxhzosjly.html

TS:   resp.ok;  resp.status
来源：http://hz.xylfe.cn/gtxcmwkdrn.html

Java: resp.statusCode()
来源：http://hz.aibaodan.cn/gtcgzfmvxo.html

Go:   resp.StatusCode
来源：http://hz.shuidangran.top/gtbylabiqb.html

Ruby: resp.code.to_i
来源：http://hz.andypj.xyz/gtanrspqcs.html

C#:   (int)resp.StatusCode
来源：http://hz.cashguo.top/gtogzjfbct.html

[L08] 并发请求多个地址
来源：http://hz.jinqigufen.top/gtnjcrqucq.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.mhx1999.top/gtxdwxpdbl.html

PHP:  curl_multi_init() 系列
来源：http://hz.shangyingyoupin.top/gthhhnpgze.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yangfankeji.com/gtmbnrvxze.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.svipenyu.cn/gtzvdevwxq.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.yj202588.top/gtmkjofuvq.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.fengsongda.top/gtajqocnef.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.tianlin.xyz/gtjlpmcqvf.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.snrcjt.cn/gtpkzdfszs.html

================================================================================
来源：http://hz.hfpthk.cn/gtgcvgguyw.html

M. 命令行 / 进程 / 环境
来源：http://hz.zhijiandao.cn/gtdlstmnft.html

================================================================================
来源：http://hz.vqdsnc.cn/gtmqnhfngu.html

[M01] 读取命令行参数
来源：http://hz.yangfankeji.com/gtywrnnkgr.html

Py:   sys.argv[1:]
来源：http://hz.birdmap.top/gtqqeigtya.html

PHP:  $argv;  $argc;
来源：http://hz.zhongyouzk.top/gtnbfisdir.html

JS:   process.argv.slice(2)
来源：http://hz.jqgufenzy.top/gtjohrmdna.html

TS:   process.argv.slice(2)
来源：http://hz.chenjidiqi.icu/gtkxsitzsm.html

Java: args 数组（main 方法参数）
来源：http://hz.316326.xyz/gttpmofrjs.html

Go:   os.Args[1:]
来源：http://hz.meibo888.top/gthfezylla.html

Ruby: ARGV
来源：http://hz.haohaochexian.top/gtakmpybkt.html

C#:   args 数组（Main 方法参数）
来源：http://hz.yongpay.top/gtyfuuonah.html

[M02] 读取环境变量
来源：http://hz.shzxlz.cn/gtpyhczkwy.html

Py:   os.environ.get("HOME")
来源：http://hz.zycfv.cn/gtcxjtdihh.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.vqdsnc.cn/gtxegsqewi.html

JS:   process.env.HOME
来源：http://hz.tianlin.xyz/gtewkcizjr.html

TS:   process.env.HOME
来源：http://hz.chenzaomai.com/gturjqftey.html

Java: System.getenv("HOME")
来源：http://hz.sweek.top/gtdezjzesp.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.mhx1999.top/gtnucdkqhm.html

Ruby: ENV["HOME"]
来源：http://hz.hfpthk.cn/gtwxbtglyn.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.guowangkeji.top/gtgoburwmo.html

[M03] 执行外部命令
来源：http://hz.sufxvd.cn/gtsmuajake.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.aizwys.cn/gtuymulpot.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.jinyuanbaomall.cn/gtwfqbnmlk.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.zhoulong.xyz/gtanerechv.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.svipenyu.cn/gtpzqbtsne.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.pengpengdd.cyou/gtjrpbeial.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.feifeiyinyue.top/gtxeqqlamy.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.yanxiufei.cn/gtdzdpvhhq.html

C#:   Process.Start("ls", "-l");
来源：http://hz.wangshuangyany.cn/gtyugzfmjq.html

[M04] 获取当前工作目录
来源：http://hz.yangfankeji.com/gtgszlzbir.html

Py:   os.getcwd()
来源：http://hz.zdqjudy.top/gtrzybtyef.html

PHP:  getcwd();
来源：http://hz.shuidangran.top/gtwaojkgdx.html

JS:   process.cwd()
来源：http://hz.ydjk.org.cn/gtjkszeamm.html

TS:   process.cwd()
来源：http://hz.fzhhl.top/gtnhlcfbmp.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.chenjidiqi.icu/gtiuzsvemp.html

Go:   os.Getwd()
来源：http://hz.jiagoushi.top/gtwwfhzsck.html

Ruby: Dir.pwd
来源：http://hz.sufxvd.cn/gtfdywnbak.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.guowangkeji.top/gtyfgndkge.html

[M05] 设置退出码
来源：http://hz.gotoacloud.top/gtzqxufiri.html

Py:   sys.exit(1)
来源：http://hz.cqqwz.cn/gtmeyltodp.html

PHP:  exit(1);
来源：http://hz.dianchejie.cn/gtbfmvghzo.html

JS:   process.exit(1)
来源：http://hz.yonumen.top/gtcuffelrs.html

TS:   process.exit(1)
来源：http://hz.chenzaomai.com/gtzuephrpg.html

Java: System.exit(1)
来源：http://hz.gogol.net.cn/gtlpwszbgi.html

Go:   os.Exit(1)
来源：http://hz.yangfankeji.com/gtpvnhzruo.html

Ruby: exit 1
来源：http://hz.nanxuanxn.top/gtulutsxjf.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.ybcxt.top/gtpnxgypja.html

[M06] 向标准错误输出
来源：http://hz.52xcode.cn/gtwfejtwwm.html

Py:   print("err", file=sys.stderr)
来源：http://hz.shangyingyoupin.top/gtdtrxskni.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.dashuyun.cn/gtimxzvbmy.html

JS:   console.error("err")
来源：http://hz.aibaodan.cn/gtvrnfkdli.html

TS:   console.error("err")
来源：http://hz.daria6918.cn/gtnphsqyjw.html

Java: System.err.println("err")
来源：http://hz.yuxming.cn/gtqzpqoaqo.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.fzhhl.top/gtblzpswnx.html

Ruby: warn "err"
来源：http://hz.shzxlz.cn/gtjtpywfyd.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.yj202588.top/gtrvekcqzo.html

[M07] 判断是否为主入口
来源：http://hz.jqgufenzy.top/gticmaatzx.html

Py:   if __name__ == "__main__":
来源：http://hz.yueranfly.top/gturishdnf.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.316326.xyz/gtqopnpvjj.html

JS:   require.main === module
来源：http://hz.kuanghao11.cn/gtowtorbqu.html

TS:   require.main === module
来源：http://hz.52xcode.cn/gtymjupxxm.html

Java: public static void main(String[] args)
来源：http://hz.mhx1999.top/gthkxdwygh.html

Go:   func main()
来源：http://hz.fengsongda.top/gtdoyesyeq.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.quarkkingdee.top/gtgkjafmzm.html

C#:   static void Main(string[] args)
来源：http://hz.fengsongda.top/gtxlwpesmm.html

[M08] 获取系统与运行时信息
来源：http://hz.pycfn.com/gtakaafweg.html

Py:   platform.system();  platform.python_version()
来源：http://hz.shangyingyoupin.top/gtolcgekgn.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.zhiwuduotai.top/gttutdicbn.html

JS:   process.platform;  process.version
来源：http://hz.andypj.xyz/gtlxmzccka.html

TS:   process.platform;  process.version
来源：http://hz.smart0.xyz/gtpmsjufmp.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.cqqwz.cn/gtcytxuzrw.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.svipenyu.cn/gtqhesesov.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.chenzaomai.com/gtmuxmnrbm.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.daxiang520.top/gtysclnpus.html

================================================================================
来源：http://hz.yj202588.top/gtixerebnl.html

N. 数据结构与算法
来源：http://hz.jianghu66.top/gtgqcsiljn.html

================================================================================
来源：http://hz.daxiang520.top/gtevynvurk.html

[N01] 二分查找（有序数组）
来源：http://hz.wangshuangyany.cn/gtufobrzzs.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.sweek.top/gtidomoyuk.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.ywan-chungtsiang.top/gtcsqenqqn.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.xylfe.cn/gtwfsxhbos.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.andypj.xyz/gtkpffprae.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.aibaodan.cn/gtyqlknkvf.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.birdmap.top/gtyeddgplx.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.fengsongda.top/gtvlinpnpj.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.zhiwuduotai.top/gtdtrlkbrt.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.iojbl.cn/gtxmmjwwge.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.ydzc1.top/gtxxslgeyn.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.zhixingplan.top/gtoxbdsaae.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.ppjwa.cn/gtcokgviit.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.aizwys.cn/gtgnnenskd.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.hammf.cn/gtrupmmwbt.html

Go:   slices.Sort(arr)
来源：http://hz.smart0.xyz/gtnyufdivz.html

Ruby: arr.sort
来源：http://hz.jlsjyb.cn/gtgnkhortd.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.fengsongda.top/gtpyqmpurj.html

[N03] 快速排序（分治示例）
来源：http://hz.dianchejie.cn/gtsnvywkeq.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.gogol.net.cn/gtjjvgvbri.html

PHP:  // 递归实现，或用 usort
来源：http://hz.jianghu66.top/gtgqwxaszi.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.mhx1999.top/gtqzjbjukg.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yuanzhike.top/gtushojkyv.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.gotoacloud.top/gtrngeqgcn.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.hnxiangtu.top/gteowatdic.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.aizwys.cn/gtdjlxaexx.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.jinghuilouyu.cn/gtnywghjdo.html

[N04] 斐波那契数列
来源：http://hz.vqdsnc.cn/gtcnbacffr.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.zhengqikj.top/gtcydbjnld.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.zhaomingkeji.xyz/gtghnlrayy.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.pycfn.com/gttcdjyozs.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.smart0.xyz/gtbnmgpqvf.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.xingfuxueyuan.xyz/gtjgbwmcuk.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.kuanghao11.cn/gtjnfmzskn.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.tanke756.top/gtnfzuulvf.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.jinghuilouyu.cn/gtpqagrvnk.html

[N05] 最大公约数
来源：http://hz.aibaodan.cn/gtfzacxrkt.html

Py:   math.gcd(a, b)
来源：http://hz.guowangkeji.top/gtynpbbjiq.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.bjfxy.top/gtarifkokw.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.zhijiandao.cn/gtortqhios.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.wangshuangyany.cn/gttsvplsmn.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.gogol.net.cn/gttmtmpsqn.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.yanxiufei.cn/gtlxhsuimf.html

Ruby: a.gcd(b)
来源：http://hz.chenlongwang.top/gtdhckbxxo.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.zhengqikj.top/gtoynyqpbk.html

[N06] 判断回文字符串
来源：http://hz.cdnleiting.top/gthdjfpbys.html

Py:   s == s[::-1]
来源：http://hz.yangfankeji.com/gtofzdomky.html

PHP:  $s === strrev($s);
来源：http://hz.xuanzx.com/gtzmnegrbi.html

JS:   s === [...s].reverse().join("")
来源：http://hz.jlsjyb.cn/gtaejasfuy.html

TS:   s === [...s].reverse().join("")
来源：http://hz.xziqi.cn/gtfxhbuiey.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.ivvv.top/gtvhuofkij.html

Go:   // 双指针从两端比较
来源：http://hz.zhiwuduotai.top/gtlxcgxvfc.html

Ruby: s == s.reverse
来源：http://hz.ehwqpu.com/gtextixxkj.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.ivvv.top/gtqovmkltk.html

[N07] 两数之和（返回下标）
来源：http://hz.jinqigufen.top/gtmeatpdmh.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.hysaishi.cn/gtwjuadytj.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.hongshengwenyu.top/gtsfgxfehg.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.guowangkeji.top/gtibdgetwo.html

TS:   // 手写 Map<string, number>
来源：http://hz.bjfxy.top/gtmujdmhcb.html

Java: // 手写 HashMap
来源：http://hz.jqgfzy.top/gtenrzqpbr.html

Go:   // 手写 map[int]int
来源：http://hz.ppjwa.cn/gtskfoyuez.html

Ruby: // 手写 Hash
来源：http://hz.yuxming.cn/gtuxjjtqxu.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.sufxvd.cn/gtljawzdao.html

[N08] 生成全排列
来源：http://hz.ybcxt.top/gtmenhwnhn.html

Py:   itertools.permutations(arr)
来源：http://hz.cdnleiting.top/gttelhlqyb.html

PHP:  // 手写递归交换
来源：http://hz.hongshengwenyu.top/gtgsquffuz.html

JS:   // 手写回溯递归
来源：http://hz.redwolf501.top/gtvnireroh.html

TS:   // 手写回溯递归
来源：http://hz.andypj.xyz/gtwybwytri.html

Java: // 手写回溯递归
来源：http://hz.redwolf501.top/gtaljwrrow.html

Go:   // 手写回溯递归
来源：http://hz.c1oappe.top/gthdvuzrkt.html

Ruby: arr.permutation.to_a
来源：http://hz.hnxiangtu.top/gtvxsgwoua.html

C#:   // 手写回溯递归
来源：http://hz.yueranfly.top/gtqkgaeytq.html

[N09] 栈与队列
来源：http://hz.quarkkingdee.top/gttobcaahc.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.cucudq.cn/gtgskzgjtk.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.yueranfly.top/gteqyfhuzq.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.vqdsnc.cn/gtkdsxhthe.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.cucudq.cn/gtmlztgduq.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.yj20258.top/gtutgsvgew.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.jqgufenzy.top/gtzrchjfka.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.vqdsnc.cn/gtghurvsju.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.guowangkeji.top/gtrggkayld.html

[N10] 链表节点定义
来源：http://hz.cashguo.top/gtioispfxt.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.gogol.net.cn/gtjordislz.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.zhiwuduotai.top/gtdpiypqry.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.fzhhl.top/gtfnxmabdn.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.haohaochexian.top/gtlwdqknsu.html

Java: class Node { int v; Node next; }
来源：http://hz.ydzc1.top/gtqfnvnjlz.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.iojbl.cn/gtbhqjecbe.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.jinqigfzy.top/gtehzstozw.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.bjfxy.top/gtifwoxrpl.html

[N11] 二叉树中序遍历
来源：http://hz.ydzc1.top/gtzvurbqlf.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.guannengcc.top/gtwvmzgtfu.html

PHP:  // 手写递归函数
来源：http://hz.kuanghao11.cn/gtjqcvotgw.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.vqdsnc.cn/gtyqefllfs.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.haohaochexian.top/gtfzduxtgy.html

Java: // 手写递归
来源：http://hz.jqgufenzy.top/gtnowfvdkj.html

Go:   // 手写递归
来源：http://hz.ywan-chungtsiang.top/gtueqddaox.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.ybcxt.top/gtavzqyzdj.html

C#:   // 手写递归
来源：http://hz.jinqigufen.top/gtxocgmqyw.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.cdnleiting.top/gtgnjbehtx.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.ivvv.top/gtdfbrxccs.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.xinyue.icu/gtxrbhkgxc.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yangfankeji.com/gtyqwdwacg.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.feifeiyinyue.top/gtsfjqptri.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.zhiwuduotai.top/gtjesxzdzn.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.hammf.cn/gturslqkrp.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.yj20258.top/gtauviwsze.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.smart0.xyz/gtyuiccnov.html

================================================================================
来源：http://hz.ppjwa.cn/gtmcnyjwsg.html

O. 并发与异步
来源：http://hz.shanyushiyangkeji.top/gtpanzalaz.html

================================================================================
来源：http://hz.pycfn.com/gtaqmubwep.html

[O01] 启动一个线程
来源：http://hz.fengsongda.top/gtvczycuww.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.chenlongwang.top/gtfukvkeaj.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.quarkkingdee.top/gtzybiezwf.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.ehwqpu.com/gtxnehcamm.html

TS:   // 同 JS
来源：http://hz.zhixingplan.top/gtzpuhfkyk.html

Java: new Thread(() -> f()).start()
来源：http://hz.andypj.xyz/gttdzzqhyw.html

Go:   go f()
来源：http://hz.xylfe.cn/gtshqzcidu.html

Ruby: Thread.new { f }
来源：http://hz.xingfuxueyuan.xyz/gtraxydqqq.html

C#:   Task.Run(() => F());
来源：http://hz.sxryk.cn/gthisenxns.html

[O02] 使用线程池
来源：http://hz.hysaishi.cn/gtuykbamcc.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.ppjwa.cn/gtzrbxuprw.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.yj20258.top/gtmmlymiym.html

JS:   // worker_threads 线程池
来源：http://hz.feifeiyinyue.top/gtdeukaicn.html

TS:   // worker_threads 线程池
来源：http://hz.birdmap.top/gtpxwhwmca.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.hammf.cn/gtkpgqfgpf.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.jinyuanbaomall.cn/gtlhedragq.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.yj20258.top/gtagfubzox.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.sysykeji.top/gtggyurrqk.html

[O03] 加锁保护共享数据
来源：http://hz.ivvv.top/gtfolttuwf.html

Py:   with lock: shared += 1
来源：http://hz.sysykeji.top/gtcibmiwuy.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.havefunace.top/gtobwhyndv.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.smart0.xyz/gtwexchhlb.html

TS:   // 同 JS
来源：http://hz.quarkkingdee.top/gthaqvnsbp.html

Java: synchronized (this) { shared++; }
来源：http://hz.hywenlv.cn/gtbcxhxdod.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.yj202588.top/gtmvrazihr.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.dianchejie.cn/gtrwpfihmt.html

C#:   lock (gate) { shared++; }
来源：http://hz.meibo888.top/gtgvzwzioz.html

[O04] 定义异步函数并等待
来源：http://hz.yj20258.top/gtkeewcjxa.html

Py:   async def f():⏎    await g()
来源：http://hz.nanxinkj.top/gtaxredtye.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.hysaishi.cn/gtgtrodgwo.html

JS:   async function f() { await g(); }
来源：http://hz.gaohongyu789.top/gtolcwwudq.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.sxryk.cn/gtextzjwyl.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.guowangkeji.top/gtvzrrorae.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.svipenyu.cn/gtakcwwayf.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.yangfankeji.com/gtfjjrlhgo.html

C#:   async Task F() { await G(); }
来源：http://hz.zdqjudy.top/gtqnijdaae.html

[O05] 并发执行并等待全部完成
来源：http://hz.snrcjt.cn/gtlzdhlfwe.html

Py:   asyncio.gather(*tasks)
来源：http://hz.yuanzhike.top/gtbvpzwdqa.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.ydzc1.top/gtsgnglnzr.html

JS:   await Promise.all(tasks)
来源：http://hz.sufxvd.cn/gtqdisxeuz.html

TS:   await Promise.all(tasks)
来源：http://hz.cashguo.top/gtdcvgwgyz.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.zhongyouzk.top/gttlenpjme.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.0kj1m.cn/gtgcjoyspx.html

Ruby: threads.map(&:join)
来源：http://hz.sufxvd.cn/gtbawjkdws.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.jqgufenzy.top/gtxcwgpkbm.html

[O06] 使用进程池
来源：http://hz.xuanzx.com/gtubeydjdi.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.vqdsnc.cn/gttggbsaqk.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.zdqjudy.top/gtzmsfpptg.html

JS:   // child_process / cluster 模块
来源：http://hz.shuidangran.top/gtgifihlgx.html

TS:   // child_process / cluster 模块
来源：http://hz.shanyushiyangkeji.top/gtifyfhnrd.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.sweek.top/gtocwffaox.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.ydzc1.top/gtyytjprgj.html

Ruby: // fork 块
来源：http://hz.nanxuanxn.top/gtwowrmozp.html

C#:   Parallel.For
来源：http://hz.shuidangran.top/gtrdnionya.html

================================================================================
来源：http://hz.ivvv.top/gtbdjypgcy.html

P. 常用工具函数
来源：http://hz.jianghu66.top/gtrpnzhfsd.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtplmyllkx.html

[P01] 生成 UUID
来源：http://hz.jinyuanbaomall.cn/gtdqbozbqu.html

Py:   str(uuid.uuid4())
来源：http://hz.kuanghao11.cn/gtnqegmdbu.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.shanyushiyangtech.top/gtocfypvdf.html

JS:   crypto.randomUUID()
来源：http://hz.hammf.cn/gtlvvvfneg.html

TS:   crypto.randomUUID()
来源：http://hz.yonumen.top/gtnfwuozik.html

Java: UUID.randomUUID().toString()
来源：http://hz.ppjwa.cn/gthixfwgyw.html

Go:   // 用 github.com/google/uuid
来源：http://hz.iojbl.cn/gtmjzpsies.html

Ruby: SecureRandom.uuid
来源：http://hz.tian-w.cn/gtvvhrncfo.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.hfpthk.cn/gtlskcbaai.html

[P02] MD5 / SHA256 摘要
来源：http://hz.jqgfzy.top/gtndyroorg.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.guannengcc.top/gtseduamos.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.wangdashe.top/gtjmfngfqe.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.c1oappe.top/gtqyfilkgo.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.chenjidiqi.icu/gtxthuqero.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.gotoacloud.top/gttsyqsrls.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.chenlongwang.top/gttmmdfhuj.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hz.jianghu66.top/gtiuppnnox.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hz.ydzc1.top/gtnmwhlkkf.html

[P03] 生成短随机字符串
来源：http://hz.dianchejie.cn/gtdinsrfue.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hz.fzhhl.top/gtoemctecy.html


<!-- 参考信息 -->