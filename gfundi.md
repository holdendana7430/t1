代发 wailian999

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.316326.xyz/gtuqhzzshk.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.316326.xyz/gtmeshnefl.html

[L05] 上传文件（multipart）
来源：http://hz.yanxiufei.cn/gtkxnunijm.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.ywan-chungtsiang.top/gtmnlenlee.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.chenlongwang.top/gtvcuyfylh.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.daria6918.cn/gtzqtslrif.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.chenjidiqi.icu/gtizgkdvth.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.fzhhl.top/gtoaebleeg.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.nanxuanxn.top/gtnqmawmba.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.cucudq.cn/gtywpjcltf.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.xuetiantiany.cn/gtszfmuroi.html

[L06] 解析响应为 JSON
来源：http://hz.cucudq.cn/gtmejqijed.html

Py:   resp.json()
来源：http://hz.jinghuilouyu.cn/gtnugpphlh.html

PHP:  json_decode($body, true);
来源：http://hz.xinyue.icu/gtwpedxcqy.html

JS:   await resp.json()
来源：http://hz.chenzaomai.com/gtgmjmvaie.html

TS:   await resp.json()
来源：http://hz.xuanzx.com/gtxuabytim.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.9152youxi.cn/gtjjgzzvbx.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.vqdsnc.cn/gtwfbxchua.html

Ruby: JSON.parse(resp.body)
来源：http://hz.hammf.cn/gtbhgiygrw.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.shuidangran.top/gtkfnvqpne.html

[L07] 处理 HTTP 状态码
来源：http://hz.pengpengdd.cyou/gtjuvozmrq.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.dianchejie.cn/gtzgpmjnvb.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.zhiwuduotai.top/gtyoyhdxxt.html

JS:   resp.ok;  resp.status
来源：http://hz.jinyuanbaomall.cn/gtvzqrjgsp.html

TS:   resp.ok;  resp.status
来源：http://hz.sxryk.cn/gtnrlnhbfe.html

Java: resp.statusCode()
来源：http://hz.jqgfzy.top/gtvgrvztxu.html

Go:   resp.StatusCode
来源：http://hz.pengpengdd.cyou/gthsfiebdz.html

Ruby: resp.code.to_i
来源：http://hz.chenzaomai.com/gtegcknllz.html

C#:   (int)resp.StatusCode
来源：http://hz.snrcjt.cn/gtojrqjbwd.html

[L08] 并发请求多个地址
来源：http://hz.yuanzhike.top/gtpgoqkmmh.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.jinqigufen.top/gtntxldlfn.html

PHP:  curl_multi_init() 系列
来源：http://hz.chenlongwang.top/gtasawbser.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.chenjidiqi.icu/gtmpjimduy.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.sxryk.cn/gtrpehqjyg.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.zycfv.cn/gtarcqmtvh.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.xinyue.icu/gtzfpqmeke.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.chenjidiqi.icu/gtcmwzrmag.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.xuanzx.com/gtvltetfvh.html

================================================================================
来源：http://hz.gzhubu.top/gtgnjfgpxe.html

M. 命令行 / 进程 / 环境
来源：http://hz.guannengcc.top/gtvzbzstub.html

================================================================================
来源：http://hz.iojbl.cn/gtutuemqmo.html

[M01] 读取命令行参数
来源：http://hz.shanyushiyangtech.top/gtrpxdjwjn.html

Py:   sys.argv[1:]
来源：http://hz.sweek.top/gtimhzjvsx.html

PHP:  $argv;  $argc;
来源：http://hz.hysaishi.cn/gtdbujjgee.html

JS:   process.argv.slice(2)
来源：http://hz.chenzaomai.com/gtnrnpxgpd.html

TS:   process.argv.slice(2)
来源：http://hz.yueranfly.top/gtebbkyets.html

Java: args 数组（main 方法参数）
来源：http://hz.jiagoushi.top/gtwoypizbv.html

Go:   os.Args[1:]
来源：http://hz.yj20258.top/gtqvfinela.html

Ruby: ARGV
来源：http://hz.xuanzx.com/gtameprwwp.html

C#:   args 数组（Main 方法参数）
来源：http://hz.ybcxt.top/gtsvwdjzbo.html

[M02] 读取环境变量
来源：http://hz.yangfankeji.com/gtxmfdboes.html

Py:   os.environ.get("HOME")
来源：http://hz.birdmap.top/gtihepzxag.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.guannengcc.top/gtcmpepifl.html

JS:   process.env.HOME
来源：http://hz.zhaomingkeji.xyz/gtggjjpnrw.html

TS:   process.env.HOME
来源：http://hz.jianghu66.top/gtnnbwxagp.html

Java: System.getenv("HOME")
来源：http://hz.jqgufenzy.top/gtikgcoqze.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.xylfe.cn/gtoqjgdlja.html

Ruby: ENV["HOME"]
来源：http://hz.nanxuanxn.top/gtbydfomjx.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.chenlongwang.top/gtbznmmaeb.html

[M03] 执行外部命令
来源：http://hz.hysaishi.cn/gtrgvdltlk.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.cdnleiting.top/gtnyliygoj.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.ydzc1.top/gtkxjwexjz.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.zhiwuduotai.top/gtohyzzbvb.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.shanyushiyangkeji.top/gtizxevbzw.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.smart0.xyz/gtnvhmjemj.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.havefunace.top/gtiornndqq.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.fengsongda.top/gtgkrhxtpz.html

C#:   Process.Start("ls", "-l");
来源：http://hz.xingfuxueyuan.xyz/gtocukzyrh.html

[M04] 获取当前工作目录
来源：http://hz.9152youxi.cn/gtbrqjtrcd.html

Py:   os.getcwd()
来源：http://hz.chenzaomai.com/gtxabtrwxa.html

PHP:  getcwd();
来源：http://hz.yonumen.top/gtpivtjlur.html

JS:   process.cwd()
来源：http://hz.ydjk.org.cn/gtthlvlndi.html

TS:   process.cwd()
来源：http://hz.cheryme.top/gtivzqdebj.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.gaohongyu789.top/gtqrqjlzpt.html

Go:   os.Getwd()
来源：http://hz.zycfv.cn/gtbndfgiql.html

Ruby: Dir.pwd
来源：http://hz.gogol.net.cn/gtzfwrxstu.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.guowangkeji.top/gtycntctki.html

[M05] 设置退出码
来源：http://hz.jinqigfzy.top/gtcqjvibxp.html

Py:   sys.exit(1)
来源：http://hz.yuanzhike.top/gtfnivofqk.html

PHP:  exit(1);
来源：http://hz.aibaodan.cn/gtgaggbyqh.html

JS:   process.exit(1)
来源：http://hz.jinqigfzy.top/gtowjivmdv.html

TS:   process.exit(1)
来源：http://hz.chenzaomai.com/gtkzizedff.html

Java: System.exit(1)
来源：http://hz.wangdashe.top/gttvfdytmb.html

Go:   os.Exit(1)
来源：http://hz.jinqigufen.top/gtusgjdiju.html

Ruby: exit 1
来源：http://hz.ehwqpu.com/gtyaomzypb.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.yonumen.top/gtabuiavcn.html

[M06] 向标准错误输出
来源：http://hz.shuidangran.top/gtgwuecmsl.html

Py:   print("err", file=sys.stderr)
来源：http://hz.jinghuilouyu.cn/gtatapepty.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.cashguo.top/gttkusvvgo.html

JS:   console.error("err")
来源：http://hz.xingfuxueyuan.xyz/gtvfnhtnnz.html

TS:   console.error("err")
来源：http://hz.snrcjt.cn/gtxzczsqbn.html

Java: System.err.println("err")
来源：http://hz.chenzaomai.com/gtctojbapc.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.fzhhl.top/gtnhfyzgtm.html

Ruby: warn "err"
来源：http://hz.shanyushiyangkeji.top/gtwezclflo.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.svipenyu.cn/gtlcvckldq.html

[M07] 判断是否为主入口
来源：http://hz.52xcode.cn/gtlpvpcswk.html

Py:   if __name__ == "__main__":
来源：http://hz.iojbl.cn/gtptayxrut.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.jqgfzy.top/gtzehspgyp.html

JS:   require.main === module
来源：http://hz.quarkkingdee.top/gttxrtkoxb.html

TS:   require.main === module
来源：http://hz.shanyushiyangtech.top/gtojynkznx.html

Java: public static void main(String[] args)
来源：http://hz.cqqwz.cn/gtzlcgxmvl.html

Go:   func main()
来源：http://hz.dashuyun.cn/gtqjiivgdm.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.yangfankeji.com/gtvtjtdyte.html

C#:   static void Main(string[] args)
来源：http://hz.hywenlv.cn/gttatgbspn.html

[M08] 获取系统与运行时信息
来源：http://hz.fzhhl.top/gteizgdjab.html

Py:   platform.system();  platform.python_version()
来源：http://hz.daria6918.cn/gtrqgsdtpi.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.yuanzhike.top/gtcfzmmnng.html

JS:   process.platform;  process.version
来源：http://hz.sufxvd.cn/gtysewnoee.html

TS:   process.platform;  process.version
来源：http://hz.haohaochexian.top/gtbysobofa.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.shanyushiyangtech.top/gtnzhlwrbq.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.c1oappe.top/gtlxysetff.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.daxiang520.top/gtbyeaahep.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.yangfankeji.com/gtbfpqkjsk.html

================================================================================
来源：http://hz.yj20258888.top/gtvdrhtpxa.html

N. 数据结构与算法
来源：http://hz.fengsongda.top/gtjfwidhlf.html

================================================================================
来源：http://hz.iojbl.cn/gtfsrosuda.html

[N01] 二分查找（有序数组）
来源：http://hz.feifeiyinyue.top/gttvuktmel.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.gotoacloud.top/gtbdvomkff.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.xylfe.cn/gthwjlcobb.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.hywenlv.cn/gtxrcmohrv.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zycfv.cn/gtdahadksw.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.yuxming.cn/gtpikzqtkn.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.gaohongyu789.top/gtxqiljfvp.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.tanke756.top/gtvqhrfayk.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.daxiang520.top/gtfedbspqk.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.ywan-chungtsiang.top/gteklxuyzg.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.ppjwa.cn/gtrrvfjmcb.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.pengpengdd.cyou/gtnqdbbecb.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.bjfxy.top/gtwjuhsczt.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.c1oappe.top/gtjkjncstu.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.nwbrower.top/gthquyyann.html

Go:   slices.Sort(arr)
来源：http://hz.xingfuxueyuan.xyz/gtgzppdipl.html

Ruby: arr.sort
来源：http://hz.nanxinkj.top/gtsohekjqq.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.birdmap.top/gtnregqyio.html

[N03] 快速排序（分治示例）
来源：http://hz.ivvv.top/gtiybczcfj.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.daria6918.cn/gtrtyuwkkn.html

PHP:  // 递归实现，或用 usort
来源：http://hz.pengpengdd.cyou/gtltdrkkhx.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yuxming.cn/gtfdqrmkyh.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.hongshengwenyu.top/gtyoljtajx.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.chenzaomai.com/gtaptikyfa.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.quarkkingdee.top/gtlruiqjfh.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.jqgufenzy.top/gttflksvtq.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.hfpthk.cn/gtvzvepvdt.html

[N04] 斐波那契数列
来源：http://hz.birdmap.top/gtyojgiklb.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.ehwqpu.com/gtdtnyzyob.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.havefunace.top/gtgviwyduw.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.xinyue.icu/gtihckxenw.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.nwbrower.top/gtbbvjutut.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.shanyushiyangtech.top/gtgmrwqwro.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.jinqigufen.top/gttoswhlof.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.yuanzhike.top/gtikbwhqkf.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.ehwqpu.com/gtjojyzddk.html

[N05] 最大公约数
来源：http://hz.gogol.net.cn/gtyssqrppr.html

Py:   math.gcd(a, b)
来源：http://hz.ivvv.top/gtxmcnogyv.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.hfpthk.cn/gtylytqxxa.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.xuanzx.com/gtsnvneaep.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yvedp.cn/gtuobhyivs.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.bjfxy.top/gtlkygkiwc.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.svipenyu.cn/gtzdstkuxz.html

Ruby: a.gcd(b)
来源：http://hz.zhiwuduotai.top/gtysqjvuvh.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.cdnleiting.top/gthqtiwcxa.html

[N06] 判断回文字符串
来源：http://hz.ppjwa.cn/gtsddvlrmo.html

Py:   s == s[::-1]
来源：http://hz.tianlin.xyz/gtkfsfaubx.html

PHP:  $s === strrev($s);
来源：http://hz.fzhhl.top/gtkasgirvp.html

JS:   s === [...s].reverse().join("")
来源：http://hz.gogol.net.cn/gtjigwksys.html

TS:   s === [...s].reverse().join("")
来源：http://hz.feifeiyinyue.top/gtssduloyb.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.hongshengwenyu.top/gtbeweagpq.html

Go:   // 双指针从两端比较
来源：http://hz.52xcode.cn/gtqjnztizx.html

Ruby: s == s.reverse
来源：http://hz.shanyushiyangtech.top/gtaxxgtjbw.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.hysaishi.cn/gtgcwjirnv.html

[N07] 两数之和（返回下标）
来源：http://hz.svipenyu.cn/gtbhxwhurq.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.cheryme.top/gtzpdzatbg.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.0kj1m.cn/gtcvrnwpkc.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.xingfuxueyuan.xyz/gtchujvqnm.html

TS:   // 手写 Map<string, number>
来源：http://hz.jianghu66.top/gtrbtbucrx.html

Java: // 手写 HashMap
来源：http://hz.xingfuxueyuan.xyz/gtvmtrdhiu.html

Go:   // 手写 map[int]int
来源：http://hz.guannengcc.top/gtemumyruz.html

Ruby: // 手写 Hash
来源：http://hz.guannengcc.top/gtakuuwcbt.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.mhx1999.top/gthhyelbce.html

[N08] 生成全排列
来源：http://hz.zhaomingkeji.xyz/gtmifqagfe.html

Py:   itertools.permutations(arr)
来源：http://hz.chenlongwang.top/gtdgwsnevb.html

PHP:  // 手写递归交换
来源：http://hz.yuanzhike.top/gtgfnjsaag.html

JS:   // 手写回溯递归
来源：http://hz.andypj.xyz/gtmvwoccqo.html

TS:   // 手写回溯递归
来源：http://hz.hywenlv.cn/gthpnxqqoq.html

Java: // 手写回溯递归
来源：http://hz.jinqigfzy.top/gtgxzjnhrr.html

Go:   // 手写回溯递归
来源：http://hz.wangdashe.top/gtznkaiayp.html

Ruby: arr.permutation.to_a
来源：http://hz.kuanghao11.cn/gtvqshqclj.html

C#:   // 手写回溯递归
来源：http://hz.yanxiufei.cn/gtdxfjsoza.html

[N09] 栈与队列
来源：http://hz.wangshuangyany.cn/gtwhtbdlbt.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.jyoumei.cn/gtkthnqurl.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.snrcjt.cn/gtaomymtup.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.bjfxy.top/gtuksmuuqp.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.aizwys.cn/gtcnzevhie.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.tian-w.cn/gtispxxttq.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.meibo888.top/gthnfjajkr.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.shzxlz.cn/gtltglanyc.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.ppjwa.cn/gtbyhcloyj.html

[N10] 链表节点定义
来源：http://hz.hysaishi.cn/gtwrjbjwki.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.gotoacloud.top/gtbvzlazkd.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.fzhhl.top/gtmtdvaqnk.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.chenzaomai.com/gttyljecuu.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.dashuyun.cn/gthyytopwg.html

Java: class Node { int v; Node next; }
来源：http://hz.andypj.xyz/gtdzfhawuu.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.vqdsnc.cn/gtebbapmjd.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.zhiwuduotai.top/gtrdtgeztx.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.fengsongda.top/gtpfuprjgs.html

[N11] 二叉树中序遍历
来源：http://hz.chenlongwang.top/gtezpksyfn.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.aibaodan.cn/gtiopsujyf.html

PHP:  // 手写递归函数
来源：http://hz.xylfe.cn/gtahtlhwjs.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.ybcxt.top/gtiburzscu.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jyoumei.cn/gtgaatukcj.html

Java: // 手写递归
来源：http://hz.jyoumei.cn/gtiyqahwgk.html

Go:   // 手写递归
来源：http://hz.zycfv.cn/gtbfxcaasj.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.xuetiantiany.cn/gttdetddkc.html

C#:   // 手写递归
来源：http://hz.dashuyun.cn/gtmqlbyupw.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.zhixingplan.top/gtdqslnbuv.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.ehwqpu.com/gtjbylkrla.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.shanyushiyangtech.top/gtoaqimnwh.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jinqigufen.top/gtvvgithfb.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.haohaochexian.top/gtpgfwruau.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.ybcxt.top/gthbdsjode.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.haohaochexian.top/gtqchhwimr.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.zhengqikj.top/gtjuvmewdm.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.0kj1m.cn/gtqajsxvob.html

================================================================================
来源：http://hz.yanxiufei.cn/gtuasnmxnq.html

O. 并发与异步
来源：http://hz.wangdashe.top/gtitsxzlqu.html

================================================================================
来源：http://hz.jianghu66.top/gtlgrgmjeb.html

[O01] 启动一个线程
来源：http://hz.ydjk.org.cn/gtvlcviksh.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.yuxming.cn/gtbebcxutm.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.smart0.xyz/gtslvdpmha.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.316326.xyz/gtyldqtqfb.html

TS:   // 同 JS
来源：http://hz.zhengqikj.top/gtoxckwypv.html

Java: new Thread(() -> f()).start()
来源：http://hz.yuxming.cn/gtppdhevxc.html

Go:   go f()
来源：http://hz.xingfuxueyuan.xyz/gtptzxhlxy.html

Ruby: Thread.new { f }
来源：http://hz.xziqi.cn/gteumjytff.html

C#:   Task.Run(() => F());
来源：http://hz.gzhubu.top/gtojaxbhoe.html

[O02] 使用线程池
来源：http://hz.chenlongwang.top/gtyymbuntw.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.daria6918.cn/gtdfxxusav.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.jqgfzy.top/gtaipzqexx.html

JS:   // worker_threads 线程池
来源：http://hz.tanke756.top/gtxfcabtks.html

TS:   // worker_threads 线程池
来源：http://hz.snrcjt.cn/gtfzaubemy.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.andypj.xyz/gtkhfokxfx.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.zhaomingkeji.xyz/gtgnhtewpi.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.gzhubu.top/gtxuwlaauz.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.xingfuxueyuan.xyz/gtjawgtmfb.html

[O03] 加锁保护共享数据
来源：http://hz.ybcxt.top/gtnoeznuxa.html

Py:   with lock: shared += 1
来源：http://hz.jlsjyb.cn/gtwqwbmcee.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.cqqwz.cn/gtcrkbjqmc.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.redwolf501.top/gtufdgudxs.html

TS:   // 同 JS
来源：http://hz.fengsongda.top/gteybnpvuq.html

Java: synchronized (this) { shared++; }
来源：http://hz.yuxming.cn/gtytsyfqdw.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.c1oappe.top/gtgopppfcb.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.shuidangran.top/gtmzbjwbkl.html

C#:   lock (gate) { shared++; }
来源：http://hz.birdmap.top/gtnfhammkw.html

[O04] 定义异步函数并等待
来源：http://hz.daria6918.cn/gtlrrcaqkc.html

Py:   async def f():⏎    await g()
来源：http://hz.pycfn.com/gtutamdcfr.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.jqgufenzy.top/gtkpbzdedz.html

JS:   async function f() { await g(); }
来源：http://hz.hywenlv.cn/gtujivmlsw.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.vqdsnc.cn/gtelspfpcw.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.snrcjt.cn/gtedifurma.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.snrcjt.cn/gtjpsooayp.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.ydzc1.top/gtwjskhjpq.html

C#:   async Task F() { await G(); }
来源：http://hz.tanke756.top/gtqdmgshcb.html

[O05] 并发执行并等待全部完成
来源：http://hz.vqdsnc.cn/gtkzdtqvmz.html

Py:   asyncio.gather(*tasks)
来源：http://hz.zhixingplan.top/gtgwodqxyp.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.yangfankeji.com/gtpdmketkn.html

JS:   await Promise.all(tasks)
来源：http://hz.hfpthk.cn/gtcqoalhgf.html

TS:   await Promise.all(tasks)
来源：http://hz.sysykeji.top/gtyjtpqxwv.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.wangdashe.top/gtfvullueg.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.hongshengwenyu.top/gtlymrjjki.html

Ruby: threads.map(&:join)
来源：http://hz.chenjidiqi.icu/gtamvyuyts.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.zhijiandao.cn/gtwhwbchvf.html

[O06] 使用进程池
来源：http://hz.tianlin.xyz/gtregnifns.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.shuidangran.top/gtgvbxdasc.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.xingfuxueyuan.xyz/gtsmlwxpgs.html

JS:   // child_process / cluster 模块
来源：http://hz.jlsjyb.cn/gthmshojnv.html

TS:   // child_process / cluster 模块
来源：http://hz.hnxiangtu.top/gthfbcvoeu.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.kuanghao11.cn/gtjorqfdhc.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.nanxuanxn.top/gtwuambebz.html

Ruby: // fork 块
来源：http://hz.jiagoushi.top/gtffmssixe.html

C#:   Parallel.For
来源：http://hz.aibaodan.cn/gteibnjyxb.html

================================================================================
来源：http://hz.pycfn.com/gtgjyugqpu.html

P. 常用工具函数
来源：http://hz.aibaodan.cn/gteaabqpvh.html

================================================================================
来源：http://hz.gogol.net.cn/gtkunflvfz.html

[P01] 生成 UUID
来源：http://hz.jinqigufen.top/gtshktxomp.html

Py:   str(uuid.uuid4())
来源：http://hz.xziqi.cn/gtjtewuwut.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.jinqigufen.top/gtyyejnqfz.html

JS:   crypto.randomUUID()
来源：http://hz.xziqi.cn/gtmaxnfaiz.html

TS:   crypto.randomUUID()
来源：http://hz.hysaishi.cn/gtgsntqjmp.html

Java: UUID.randomUUID().toString()
来源：http://hz.zdqjudy.top/gtpcqzhuqg.html

Go:   // 用 github.com/google/uuid
来源：http://hz.yvedp.cn/gtuehuqkuf.html

Ruby: SecureRandom.uuid
来源：http://hz.nwbrower.top/gtjsibkkgx.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.cashguo.top/gtouggidzb.html

[P02] MD5 / SHA256 摘要
来源：http://hz.zhoulong.xyz/gteikkvjpa.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.snrcjt.cn/gtyrcebfpu.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.redwolf501.top/gtbjmulxwl.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.jqgfzy.top/gtsiztyddn.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.yonumen.top/gtiocjpfgc.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.jiagoushi.top/gtlweqhfeq.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.yongpay.top/gtlziprjlc.html


<!-- 参考信息 -->