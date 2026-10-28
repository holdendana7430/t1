代发 wailian999

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.ehwqpu.com/gtzzzssxtn.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.zdqjudy.top/gthpugbelp.html

[L05] 上传文件（multipart）
来源：http://hz.hammf.cn/gtjgguihbg.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.bjfxy.top/gtdzaalfhz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.jyoumei.cn/gtcnhlcoed.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.jinyuanbaomall.cn/gtgoqybubz.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.nanxinkj.top/gtrdoltkyb.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.yangfankeji.com/gtuysctcyn.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.xinyue.icu/gtovjgwinx.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.shuidangran.top/gtlnlddslm.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.hongshengwenyu.top/gtqjewahqw.html

[L06] 解析响应为 JSON
来源：http://hz.jlsjyb.cn/gtsngfqhcq.html

Py:   resp.json()
来源：http://hz.yuanzhike.top/gtikpnmwnu.html

PHP:  json_decode($body, true);
来源：http://hz.pengpengdd.cyou/gtiijskzpf.html

JS:   await resp.json()
来源：http://hz.gzhubu.top/gtewgqzjiy.html

TS:   await resp.json()
来源：http://hz.daria6918.cn/gtqrmtijbo.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.yangfankeji.com/gtdmasdnzf.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.fengsongda.top/gtrezaorsb.html

Ruby: JSON.parse(resp.body)
来源：http://hz.fengsongda.top/gtkfebkith.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.dashuyun.cn/gtblzuvspa.html

[L07] 处理 HTTP 状态码
来源：http://hz.ywan-chungtsiang.top/gtftmxvezy.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.vqdsnc.cn/gtjwsfysyq.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.guowangkeji.top/gtiktrlfrp.html

JS:   resp.ok;  resp.status
来源：http://hz.shanyushiyangkeji.top/gtiexgpyzv.html

TS:   resp.ok;  resp.status
来源：http://hz.yanxiufei.cn/gtszlillbu.html

Java: resp.statusCode()
来源：http://hz.jiagoushi.top/gtrehlokyi.html

Go:   resp.StatusCode
来源：http://hz.xziqi.cn/gtdruuyshz.html

Ruby: resp.code.to_i
来源：http://hz.pengpengdd.cyou/gtzhvjweej.html

C#:   (int)resp.StatusCode
来源：http://hz.sufxvd.cn/gtlujyhvfb.html

[L08] 并发请求多个地址
来源：http://hz.yj20258888.top/gtsczghxzm.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.jinghuilouyu.cn/gtagdlofuq.html

PHP:  curl_multi_init() 系列
来源：http://hz.xuetiantiany.cn/gtqotapomq.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.daria6918.cn/gtozfcfdsw.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.xziqi.cn/gtwwknaqnh.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.mhx1999.top/gtocbjmgtu.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.c1oappe.top/gtzlijlqid.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.quarkkingdee.top/gtenlbbzsa.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.shangyingyoupin.top/gttnltmrpw.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtoullntcc.html

M. 命令行 / 进程 / 环境
来源：http://hz.cashguo.top/gtzhitlahn.html

================================================================================
来源：http://hz.hnqzz.top/gtmzvbkijn.html

[M01] 读取命令行参数
来源：http://hz.jiagoushi.top/gtoswveakh.html

Py:   sys.argv[1:]
来源：http://hz.yvedp.cn/gtysmluqno.html

PHP:  $argv;  $argc;
来源：http://hz.xuetiantiany.cn/gtdzwysokd.html

JS:   process.argv.slice(2)
来源：http://hz.xuanzx.com/gtcmqatjfe.html

TS:   process.argv.slice(2)
来源：http://hz.yueranfly.top/gtphfftifv.html

Java: args 数组（main 方法参数）
来源：http://hz.jinqigfzy.top/gtudfxtfpf.html

Go:   os.Args[1:]
来源：http://hz.c1oappe.top/gthhhihrxa.html

Ruby: ARGV
来源：http://hz.316326.xyz/gtlpkgtmbo.html

C#:   args 数组（Main 方法参数）
来源：http://hz.vqdsnc.cn/gtgzvqprke.html

[M02] 读取环境变量
来源：http://hz.mhx1999.top/gtmkrfuwld.html

Py:   os.environ.get("HOME")
来源：http://hz.zhiwuduotai.top/gtjxwfarll.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.guannengcc.top/gtfkxbuhma.html

JS:   process.env.HOME
来源：http://hz.shangyingyoupin.top/gtvtfodria.html

TS:   process.env.HOME
来源：http://hz.hywenlv.cn/gtoubbhrzr.html

Java: System.getenv("HOME")
来源：http://hz.dashuyun.cn/gtizmnpgft.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.hysaishi.cn/gtkwgeskoa.html

Ruby: ENV["HOME"]
来源：http://hz.fengsongda.top/gtqexttjus.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.iojbl.cn/gtkhuvrgaz.html

[M03] 执行外部命令
来源：http://hz.gaohongyu789.top/gtucboewzx.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.yonumen.top/gtzyrqykpw.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.ydzc1.top/gtmdfrqghd.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.shuidangran.top/gtpgjcuucg.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.shangyingyoupin.top/gtmyiwmnic.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.hfpthk.cn/gtvbrkulrx.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.guannengcc.top/gtouzzkzpv.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.jyoumei.cn/gtfmtmwzbt.html

C#:   Process.Start("ls", "-l");
来源：http://hz.ywan-chungtsiang.top/gtrcwhtfng.html

[M04] 获取当前工作目录
来源：http://hz.jianghu66.top/gttvnhnxtj.html

Py:   os.getcwd()
来源：http://hz.ybcxt.top/gtkzghjafo.html

PHP:  getcwd();
来源：http://hz.svipenyu.cn/gtgprqshbm.html

JS:   process.cwd()
来源：http://hz.sufxvd.cn/gtmizlueod.html

TS:   process.cwd()
来源：http://hz.guannengcc.top/gtpbraydlu.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.iojbl.cn/gtvymptxsy.html

Go:   os.Getwd()
来源：http://hz.zdqjudy.top/gtwmievvrx.html

Ruby: Dir.pwd
来源：http://hz.hfpthk.cn/gttxtrjbtp.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.cashguo.top/gtwtdzwwdr.html

[M05] 设置退出码
来源：http://hz.vqdsnc.cn/gtollygfce.html

Py:   sys.exit(1)
来源：http://hz.yongpay.top/gtqglmwfvw.html

PHP:  exit(1);
来源：http://hz.aizwys.cn/gtmvqujhrr.html

JS:   process.exit(1)
来源：http://hz.guowangkeji.top/gtrmldjtbs.html

TS:   process.exit(1)
来源：http://hz.pengpengdd.cyou/gtehcstjtg.html

Java: System.exit(1)
来源：http://hz.yuanzhike.top/gtcxisfxfz.html

Go:   os.Exit(1)
来源：http://hz.yonumen.top/gtkiuwzfwv.html

Ruby: exit 1
来源：http://hz.cucudq.cn/gttqctnhrd.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.xingfuxueyuan.xyz/gtdczmnhtt.html

[M06] 向标准错误输出
来源：http://hz.hammf.cn/gtgrpfkkgp.html

Py:   print("err", file=sys.stderr)
来源：http://hz.shanyushiyangkeji.top/gthlyvqsbf.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.jqgfzy.top/gtvqffnjtd.html

JS:   console.error("err")
来源：http://hz.andypj.xyz/gtdwjwgrim.html

TS:   console.error("err")
来源：http://hz.cqqwz.cn/gtyafkyhys.html

Java: System.err.println("err")
来源：http://hz.chenjidiqi.icu/gtbdtwqmnc.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.wangdashe.top/gtzpewagks.html

Ruby: warn "err"
来源：http://hz.kuanghao11.cn/gtamqivsgl.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.chenjidiqi.icu/gtlivmkzch.html

[M07] 判断是否为主入口
来源：http://hz.chenjidiqi.icu/gtkdgzyrso.html

Py:   if __name__ == "__main__":
来源：http://hz.jinqigfzy.top/gtcuggiqho.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.zycfv.cn/gtpxfqmmxr.html

JS:   require.main === module
来源：http://hz.aibaodan.cn/gtaknocmbu.html

TS:   require.main === module
来源：http://hz.tanke756.top/gtsaaxzyff.html

Java: public static void main(String[] args)
来源：http://hz.xziqi.cn/gtbcttryih.html

Go:   func main()
来源：http://hz.nwbrower.top/gttsucvjww.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.52xcode.cn/gtlwqzvlgq.html

C#:   static void Main(string[] args)
来源：http://hz.bjfxy.top/gtzoocrxef.html

[M08] 获取系统与运行时信息
来源：http://hz.hnxiangtu.top/gtdtubbxec.html

Py:   platform.system();  platform.python_version()
来源：http://hz.xylfe.cn/gtxktvbfvu.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.aibaodan.cn/gtyuhsgrno.html

JS:   process.platform;  process.version
来源：http://hz.yuxming.cn/gtlsmkqlou.html

TS:   process.platform;  process.version
来源：http://hz.jqgufenzy.top/gttsdvoizs.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.yueranfly.top/gtlkmiqtxb.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.jqgufenzy.top/gtzcwwnzby.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.yanxiufei.cn/gtnenfxzsp.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.wangshuangyany.cn/gtpwentvuo.html

================================================================================
来源：http://hz.sufxvd.cn/gtzgxwbglj.html

N. 数据结构与算法
来源：http://hz.quarkkingdee.top/gtjmmcykpw.html

================================================================================
来源：http://hz.yueranfly.top/gtyjjihgeo.html

[N01] 二分查找（有序数组）
来源：http://hz.xinyue.icu/gtzyzbkipz.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.havefunace.top/gtrbnnepyu.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.daxiang520.top/gtdszvuzqv.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jianghu66.top/gtpywmcrft.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.daxiang520.top/gtqgvxtrfe.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.quarkkingdee.top/gtujmgcjoo.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.yj20258888.top/gtqkebkpyr.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.guannengcc.top/gtuodfgowy.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.dashuyun.cn/gtrtbzijam.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.jlsjyb.cn/gtbzkzbkcm.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.zhijiandao.cn/gtyupglyrt.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.smart0.xyz/gtauiykakc.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.bjfxy.top/gtxvxuwikz.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.ybcxt.top/gtsmyfpjuj.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.gotoacloud.top/gtqdlhgrdr.html

Go:   slices.Sort(arr)
来源：http://hz.hysaishi.cn/gtvryvctzn.html

Ruby: arr.sort
来源：http://hz.yuxming.cn/gtlovzksnb.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.jqgfzy.top/gtiacdarfa.html

[N03] 快速排序（分治示例）
来源：http://hz.zhengqikj.top/gtsvvyyocs.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.9152youxi.cn/gtfukuuruy.html

PHP:  // 递归实现，或用 usort
来源：http://hz.wangshuangyany.cn/gtoqmcxvrx.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jqgufenzy.top/gtetshuoat.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.shuidangran.top/gtwydetbbz.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.yj20258888.top/gtbxehvzer.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.shangyingyoupin.top/gtuimbqomk.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.pengpengdd.cyou/gtsbqrmvpf.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.sweek.top/gtrxztsocw.html

[N04] 斐波那契数列
来源：http://hz.bjfxy.top/gtfluqhcxm.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.jlsjyb.cn/gtlgvjdhkv.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.hysaishi.cn/gtenylxcen.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.hfpthk.cn/gtuibjizqh.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.birdmap.top/gtsezqjvkw.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.yueranfly.top/gtbcevqpab.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.aibaodan.cn/gtbufylcjw.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.shuidangran.top/gtiesgasbz.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.kuanghao11.cn/gtniyuppsu.html

[N05] 最大公约数
来源：http://hz.mhx1999.top/gtjhzixkgv.html

Py:   math.gcd(a, b)
来源：http://hz.zhiwuduotai.top/gtyupotana.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.andypj.xyz/gthiehtvbj.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.xziqi.cn/gteotzbkwh.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.redwolf501.top/gtwffmdbtx.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.fzhhl.top/gtcbtkeicc.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.ybcxt.top/gthtvunlvn.html

Ruby: a.gcd(b)
来源：http://hz.chenlongwang.top/gtsckcnjkm.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.0kj1m.cn/gtfwjhjrsp.html

[N06] 判断回文字符串
来源：http://hz.vqdsnc.cn/gtwyfugeuo.html

Py:   s == s[::-1]
来源：http://hz.nwbrower.top/gtdigrhbuz.html

PHP:  $s === strrev($s);
来源：http://hz.daxiang520.top/gtipdhucwd.html

JS:   s === [...s].reverse().join("")
来源：http://hz.sufxvd.cn/gtxaiafree.html

TS:   s === [...s].reverse().join("")
来源：http://hz.andypj.xyz/gtcmibeatz.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.yj20258.top/gttsmywlzh.html

Go:   // 双指针从两端比较
来源：http://hz.jinqigufen.top/gtoayeuxtb.html

Ruby: s == s.reverse
来源：http://hz.yj20258888.top/gtdflohmgy.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.hywenlv.cn/gtzohwyffr.html

[N07] 两数之和（返回下标）
来源：http://hz.52xcode.cn/gtqfcghiyn.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.sweek.top/gtxlnsntij.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.cheryme.top/gtliscyfxw.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.guowangkeji.top/gtfyycjxtz.html

TS:   // 手写 Map<string, number>
来源：http://hz.jinghuilouyu.cn/gtdtjrfkgi.html

Java: // 手写 HashMap
来源：http://hz.xziqi.cn/gtnmopfoty.html

Go:   // 手写 map[int]int
来源：http://hz.zhaomingkeji.xyz/gttxxhkflg.html

Ruby: // 手写 Hash
来源：http://hz.nanxinkj.top/gttzpjiqfp.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.bjfxy.top/gtxjnhkwzc.html

[N08] 生成全排列
来源：http://hz.bjfxy.top/gtzhdforwx.html

Py:   itertools.permutations(arr)
来源：http://hz.wangshuangyany.cn/gtndtbrlts.html

PHP:  // 手写递归交换
来源：http://hz.fzhhl.top/gtynraovyo.html

JS:   // 手写回溯递归
来源：http://hz.yonumen.top/gtzcuccgpq.html

TS:   // 手写回溯递归
来源：http://hz.chenzaomai.com/gtoixbmswp.html

Java: // 手写回溯递归
来源：http://hz.xinyue.icu/gttjgfimrk.html

Go:   // 手写回溯递归
来源：http://hz.yvedp.cn/gteyrwyqso.html

Ruby: arr.permutation.to_a
来源：http://hz.zhaomingkeji.xyz/gtchvgvyxw.html

C#:   // 手写回溯递归
来源：http://hz.c1oappe.top/gttxwnplrj.html

[N09] 栈与队列
来源：http://hz.ppjwa.cn/gtgbnxakyv.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.ehwqpu.com/gtcubgwfkl.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.sufxvd.cn/gtrccnveph.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.yuanzhike.top/gtczwebfgt.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.dashuyun.cn/gtoujdfsji.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.yongpay.top/gtqxumpqon.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.yj20258.top/gtewvlkiva.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.dashuyun.cn/gtthmjltrt.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.c1oappe.top/gtwoozbonx.html

[N10] 链表节点定义
来源：http://hz.yvedp.cn/gtengaadpe.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.zdqjudy.top/gtgksdsvbc.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.andypj.xyz/gtlonmhqws.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.yonumen.top/gtyvsdaabl.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.jlsjyb.cn/gtccjdradl.html

Java: class Node { int v; Node next; }
来源：http://hz.yanxiufei.cn/gtpzzlkoqj.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.xuanzx.com/gttxboscuc.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.xuanzx.com/gtibbxcgbe.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.aibaodan.cn/gtbgjfclyd.html

[N11] 二叉树中序遍历
来源：http://hz.ppjwa.cn/gtrxbfobfy.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.yonumen.top/gtmanknxsz.html

PHP:  // 手写递归函数
来源：http://hz.yj202588.top/gtemsncyzf.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.fzhhl.top/gtjtkficsw.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.gogol.net.cn/gtanewcymv.html

Java: // 手写递归
来源：http://hz.xinyue.icu/gtamhmsswp.html

Go:   // 手写递归
来源：http://hz.yvedp.cn/gtbtskzumk.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.zycfv.cn/gtjobfsfyx.html

C#:   // 手写递归
来源：http://hz.yanxiufei.cn/gtakxycall.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.zhixingplan.top/gtijmfaydc.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.fengsongda.top/gtbckzpsxn.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.sweek.top/gtkvlkuaxq.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.wangdashe.top/gtgfcqkaqe.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.zycfv.cn/gtyhgemalc.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.jqgufenzy.top/gtwbikezoz.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.zhengqikj.top/gtigsbtxlc.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.ydjk.org.cn/gtmqyiprfr.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.chenzaomai.com/gtmegdemnl.html

================================================================================
来源：http://hz.xylfe.cn/gtbuqofstm.html

O. 并发与异步
来源：http://hz.tianlin.xyz/gtjhnquzsk.html

================================================================================
来源：http://hz.havefunace.top/gtxjywyjqt.html

[O01] 启动一个线程
来源：http://hz.yongpay.top/gtzspkuqec.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.xuetiantiany.cn/gtibtpewqh.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.pengpengdd.cyou/gtqdyskvlw.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.sufxvd.cn/gtosppstac.html

TS:   // 同 JS
来源：http://hz.ivvv.top/gtlirpdvvs.html

Java: new Thread(() -> f()).start()
来源：http://hz.snrcjt.cn/gtpzyddzca.html

Go:   go f()
来源：http://hz.shzxlz.cn/gtrdhkiseg.html

Ruby: Thread.new { f }
来源：http://hz.hongshengwenyu.top/gtjccuozkm.html

C#:   Task.Run(() => F());
来源：http://hz.mhx1999.top/gtrnafkwcq.html

[O02] 使用线程池
来源：http://hz.guowangkeji.top/gtbovkhejh.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.xziqi.cn/gtlxzwdrqd.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.hfpthk.cn/gtoqhvoros.html

JS:   // worker_threads 线程池
来源：http://hz.zhijiandao.cn/gtzlibkhmp.html

TS:   // worker_threads 线程池
来源：http://hz.nwbrower.top/gttuzsajbc.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.nanxinkj.top/gtmjtycdus.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.c1oappe.top/gtzjjfedbb.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.shanyushiyangtech.top/gtcusgvvct.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.jqgfzy.top/gtomxryljl.html

[O03] 加锁保护共享数据
来源：http://hz.svipenyu.cn/gtstrvawwn.html

Py:   with lock: shared += 1
来源：http://hz.jinyuanbaomall.cn/gtkhgaqpta.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.zhiwuduotai.top/gthinuotqt.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.0kj1m.cn/gtvbyuekbq.html

TS:   // 同 JS
来源：http://hz.mhx1999.top/gtbkcqghmn.html

Java: synchronized (this) { shared++; }
来源：http://hz.hysaishi.cn/gtplcluyfp.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.hnxiangtu.top/gtwisyuthq.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.zhoulong.xyz/gtsgdtzbel.html

C#:   lock (gate) { shared++; }
来源：http://hz.quarkkingdee.top/gtkkvmrugj.html

[O04] 定义异步函数并等待
来源：http://hz.tian-w.cn/gtvulmggot.html

Py:   async def f():⏎    await g()
来源：http://hz.sysykeji.top/gtivamirjq.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.ehwqpu.com/gtzkpnbwps.html

JS:   async function f() { await g(); }
来源：http://hz.zdqjudy.top/gtytrtxysq.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.jqgfzy.top/gtarbdnhec.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.jlsjyb.cn/gtcfkwzmbu.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.zhixingplan.top/gttmllqhgh.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.sxryk.cn/gtbvebjvat.html

C#:   async Task F() { await G(); }
来源：http://hz.nanxuanxn.top/gtkhucrvbp.html

[O05] 并发执行并等待全部完成
来源：http://hz.xylfe.cn/gtihdatxon.html

Py:   asyncio.gather(*tasks)
来源：http://hz.xziqi.cn/gtrbfbjerg.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.0kj1m.cn/gtrhojdoij.html

JS:   await Promise.all(tasks)
来源：http://hz.52xcode.cn/gtgoozxxwn.html

TS:   await Promise.all(tasks)
来源：http://hz.yuxming.cn/gtjynaautl.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.jianghu66.top/gtanagqvlq.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.kuanghao11.cn/gtdtbkxfiw.html

Ruby: threads.map(&:join)
来源：http://hz.vqdsnc.cn/gtvkspudxi.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.mhx1999.top/gtptlzckhh.html

[O06] 使用进程池
来源：http://hz.xingfuxueyuan.xyz/gtprwrjwqb.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.svipenyu.cn/gttvjvchbh.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.xuetiantiany.cn/gtfwmibwpq.html

JS:   // child_process / cluster 模块
来源：http://hz.shanyushiyangtech.top/gtldtwgpxp.html

TS:   // child_process / cluster 模块
来源：http://hz.zycfv.cn/gtbqmqjavo.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.havefunace.top/gtpvbwahxw.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.pengpengdd.cyou/gtkwjzwetw.html

Ruby: // fork 块
来源：http://hz.chenlongwang.top/gtommbaqhs.html

C#:   Parallel.For
来源：http://hz.gotoacloud.top/gtjudhkpbd.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtrdukgqlk.html

P. 常用工具函数
来源：http://hz.zhijiandao.cn/gtaereocis.html

================================================================================
来源：http://hz.tanke756.top/gtnkddyroj.html

[P01] 生成 UUID
来源：http://hz.52xcode.cn/gtbmnxijub.html

Py:   str(uuid.uuid4())
来源：http://hz.chenlongwang.top/gtoqzvbpsm.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.gzhubu.top/gtvfvtnmpk.html

JS:   crypto.randomUUID()
来源：http://hz.zhengqikj.top/gthjgkxtwe.html

TS:   crypto.randomUUID()
来源：http://hz.ydjk.org.cn/gthsznxiop.html

Java: UUID.randomUUID().toString()
来源：http://hz.dianchejie.cn/gtuwdtdspy.html

Go:   // 用 github.com/google/uuid
来源：http://hz.zhiwuduotai.top/gtdiqyjcpm.html

Ruby: SecureRandom.uuid
来源：http://hz.ybcxt.top/gtzdxnbmry.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.ydjk.org.cn/gtwwnbvine.html

[P02] MD5 / SHA256 摘要
来源：http://hz.iojbl.cn/gtwblvlgmk.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.jlsjyb.cn/gtzsxpdrfd.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.ydzc1.top/gtzwnqsrfk.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.jinqigufen.top/gtgrwldkos.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.birdmap.top/gtqmuyghlx.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.shzxlz.cn/gtlsagxkgd.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.cashguo.top/gthomanrzd.html


<!-- 参考信息 -->