代发 wailian999

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.nanxuanxn.top/gtvnfpgxoa.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.xuanzx.com/gtmeqqlatr.html

[L05] 上传文件（multipart）
来源：http://hz.nanxuanxn.top/gtxlzfmotp.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.jyoumei.cn/gttmnnvwcb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.dashuyun.cn/gtrbdiowtq.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.tian-w.cn/gttwkzxueg.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.daxiang520.top/gtykmtwali.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.shanyushiyangkeji.top/gtdfrzisew.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.gaohongyu789.top/gtvldjqqni.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.smart0.xyz/gtmhzuyftb.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.guowangkeji.top/gtnvvdohhj.html

[L06] 解析响应为 JSON
来源：http://hz.jqgfzy.top/gtceduymuy.html

Py:   resp.json()
来源：http://hz.snrcjt.cn/gtpoedykva.html

PHP:  json_decode($body, true);
来源：http://hz.yueranfly.top/gtfpsshyfk.html

JS:   await resp.json()
来源：http://hz.yueranfly.top/gtdzyfhrun.html

TS:   await resp.json()
来源：http://hz.jqgfzy.top/gtmbtcvsuf.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.hywenlv.cn/gtdmzkvlui.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.haohaochexian.top/gtptdxycrq.html

Ruby: JSON.parse(resp.body)
来源：http://hz.52xcode.cn/gtxraksiah.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.aibaodan.cn/gtmdcmdlfo.html

[L07] 处理 HTTP 状态码
来源：http://hz.gzhubu.top/gtzdopwvzw.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.ywan-chungtsiang.top/gtxknknyjr.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.sxryk.cn/gtsptqrlsb.html

JS:   resp.ok;  resp.status
来源：http://hz.xuanzx.com/gtnptmhnab.html

TS:   resp.ok;  resp.status
来源：http://hz.vqdsnc.cn/gtjbfglmdy.html

Java: resp.statusCode()
来源：http://hz.tian-w.cn/gtyosawysq.html

Go:   resp.StatusCode
来源：http://hz.jyoumei.cn/gtifbkvjtr.html

Ruby: resp.code.to_i
来源：http://hz.pengpengdd.cyou/gtmcsiwqiv.html

C#:   (int)resp.StatusCode
来源：http://hz.sysykeji.top/gtoqqzgxgp.html

[L08] 并发请求多个地址
来源：http://hz.xinyue.icu/gtpmvrzcdc.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.pengpengdd.cyou/gtdwbvvjdu.html

PHP:  curl_multi_init() 系列
来源：http://hz.52xcode.cn/gtrsfapssa.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.xziqi.cn/gtiusiocsz.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.svipenyu.cn/gtjiqlvcft.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.jiagoushi.top/gtilqafqlt.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.ehwqpu.com/gtajtcyngd.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.tanke756.top/gtjnmodhnj.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.shangyingyoupin.top/gtpmtcdude.html

================================================================================
来源：http://hz.xinyue.icu/gtlmhhevtr.html

M. 命令行 / 进程 / 环境
来源：http://hz.yj202588.top/gtxvrurhqu.html

================================================================================
来源：http://hz.ivvv.top/gtwfqjfrzw.html

[M01] 读取命令行参数
来源：http://hz.vqdsnc.cn/gtzeabrgif.html

Py:   sys.argv[1:]
来源：http://hz.zhijiandao.cn/gtrxidbssn.html

PHP:  $argv;  $argc;
来源：http://hz.nwbrower.top/gtpsrjhksa.html

JS:   process.argv.slice(2)
来源：http://hz.sxryk.cn/gtltrmjtns.html

TS:   process.argv.slice(2)
来源：http://hz.jinghuilouyu.cn/gtrsmzaknx.html

Java: args 数组（main 方法参数）
来源：http://hz.hfpthk.cn/gtfqjnrdye.html

Go:   os.Args[1:]
来源：http://hz.shanyushiyangtech.top/gtchelagbp.html

Ruby: ARGV
来源：http://hz.birdmap.top/gtycjrvcit.html

C#:   args 数组（Main 方法参数）
来源：http://hz.ehwqpu.com/gtrankzpsr.html

[M02] 读取环境变量
来源：http://hz.shanyushiyangkeji.top/gtmwesdkal.html

Py:   os.environ.get("HOME")
来源：http://hz.wangdashe.top/gtxnefazua.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.c1oappe.top/gtqsxuygbl.html

JS:   process.env.HOME
来源：http://hz.9152youxi.cn/gtkovgkwvr.html

TS:   process.env.HOME
来源：http://hz.ivvv.top/gtvkquywyl.html

Java: System.getenv("HOME")
来源：http://hz.hywenlv.cn/gtwswlfvwy.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.yueranfly.top/gtuddlujgr.html

Ruby: ENV["HOME"]
来源：http://hz.ehwqpu.com/gtockriavu.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.sysykeji.top/gtlpfywbxs.html

[M03] 执行外部命令
来源：http://hz.gogol.net.cn/gtdgomhopa.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.gaohongyu789.top/gtfmudnsxv.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.jianghu66.top/gtmkhpumsa.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.wangdashe.top/gtroooazrr.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.bjfxy.top/gtdwmiiprf.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.tian-w.cn/gtegikgmkk.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.guowangkeji.top/gthrjwpkzx.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.hywenlv.cn/gtyrezimxy.html

C#:   Process.Start("ls", "-l");
来源：http://hz.xylfe.cn/gtpfgjarwu.html

[M04] 获取当前工作目录
来源：http://hz.cheryme.top/gtcmjnuqtf.html

Py:   os.getcwd()
来源：http://hz.meibo888.top/gtsvodulls.html

PHP:  getcwd();
来源：http://hz.xuetiantiany.cn/gtqaqlbjkr.html

JS:   process.cwd()
来源：http://hz.sysykeji.top/gtqaxpjkrg.html

TS:   process.cwd()
来源：http://hz.yongpay.top/gtwyhqincd.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.ybcxt.top/gttnziiwkm.html

Go:   os.Getwd()
来源：http://hz.aibaodan.cn/gtuzisosij.html

Ruby: Dir.pwd
来源：http://hz.ybcxt.top/gtgckpnucw.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.316326.xyz/gtljrihzuv.html

[M05] 设置退出码
来源：http://hz.zhijiandao.cn/gtyxhmimhr.html

Py:   sys.exit(1)
来源：http://hz.gotoacloud.top/gtkzfuakjj.html

PHP:  exit(1);
来源：http://hz.52xcode.cn/gteisrtjhi.html

JS:   process.exit(1)
来源：http://hz.andypj.xyz/gtnmvteezl.html

TS:   process.exit(1)
来源：http://hz.ywan-chungtsiang.top/gtpzkqzezt.html

Java: System.exit(1)
来源：http://hz.zdqjudy.top/gtqyiovrvk.html

Go:   os.Exit(1)
来源：http://hz.c1oappe.top/gtppyicwlu.html

Ruby: exit 1
来源：http://hz.ybcxt.top/gtfjhrmdwv.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.jyoumei.cn/gtbhiafdex.html

[M06] 向标准错误输出
来源：http://hz.316326.xyz/gtyqncaill.html

Py:   print("err", file=sys.stderr)
来源：http://hz.sysykeji.top/gtrcjnxoum.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.xinyue.icu/gtweezavvu.html

JS:   console.error("err")
来源：http://hz.kuanghao11.cn/gtrictiten.html

TS:   console.error("err")
来源：http://hz.aibaodan.cn/gtlhrlrmry.html

Java: System.err.println("err")
来源：http://hz.tian-w.cn/gtdqgoxudp.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.yueranfly.top/gtfxtefasm.html

Ruby: warn "err"
来源：http://hz.gaohongyu789.top/gtkcgvknij.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.shzxlz.cn/gtqzrqnked.html

[M07] 判断是否为主入口
来源：http://hz.yj202588.top/gtkrbisvob.html

Py:   if __name__ == "__main__":
来源：http://hz.hfpthk.cn/gtwnhpjjno.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.yangfankeji.com/gtsrxlzxqw.html

JS:   require.main === module
来源：http://hz.hysaishi.cn/gtzdvpcxqe.html

TS:   require.main === module
来源：http://hz.sysykeji.top/gtrrqdxnts.html

Java: public static void main(String[] args)
来源：http://hz.jinghuilouyu.cn/gtsdmzpqqn.html

Go:   func main()
来源：http://hz.jinqigufen.top/gtxvhvlzit.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.yvedp.cn/gtaeudomzl.html

C#:   static void Main(string[] args)
来源：http://hz.yuanzhike.top/gtxcnfxabv.html

[M08] 获取系统与运行时信息
来源：http://hz.zdqjudy.top/gtnqisrcrb.html

Py:   platform.system();  platform.python_version()
来源：http://hz.quarkkingdee.top/gtbbhygyzm.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.chenjidiqi.icu/gthbywpjwy.html

JS:   process.platform;  process.version
来源：http://hz.ydjk.org.cn/gtnxvxjsmv.html

TS:   process.platform;  process.version
来源：http://hz.cucudq.cn/gtxfssicxp.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.andypj.xyz/gtufvfduax.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.ivvv.top/gtoerbehba.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.sxryk.cn/gtsjqahxvi.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.svipenyu.cn/gtkrmhymmr.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtmqnlywwi.html

N. 数据结构与算法
来源：http://hz.iojbl.cn/gtfbdwvyfd.html

================================================================================
来源：http://hz.ydzc1.top/gtktoreqzz.html

[N01] 二分查找（有序数组）
来源：http://hz.c1oappe.top/gthvgztkpu.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.pycfn.com/gthoieinee.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.nanxuanxn.top/gtsgwpskdv.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.sxryk.cn/gtpkzefdww.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.9152youxi.cn/gtyabchbyk.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.cucudq.cn/gteydechvd.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.feifeiyinyue.top/gtphapmohg.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.cheryme.top/gtzejkpqhb.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.hfpthk.cn/gtbspdwjgx.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.cashguo.top/gtfrsholvy.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.xziqi.cn/gtpqmzoebs.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.jlsjyb.cn/gtnogjnqqe.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.guowangkeji.top/gtapcjfjpu.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.feifeiyinyue.top/gtsejcavfo.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.hfpthk.cn/gtygahirtq.html

Go:   slices.Sort(arr)
来源：http://hz.chenlongwang.top/gtzhgwsohy.html

Ruby: arr.sort
来源：http://hz.ybcxt.top/gtxautpfto.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.mhx1999.top/gtxljgtcvm.html

[N03] 快速排序（分治示例）
来源：http://hz.fengsongda.top/gtfqvpsdvk.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.jiagoushi.top/gtzwleevpz.html

PHP:  // 递归实现，或用 usort
来源：http://hz.nanxinkj.top/gtfmnamwcj.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yuanzhike.top/gttywwtuvj.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.tanke756.top/gtmpwfuwpq.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.shanyushiyangtech.top/gtckucsock.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.jianghu66.top/gtdrzhpzeg.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.feifeiyinyue.top/gtmzmyptsc.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.xuetiantiany.cn/gtgokhsuzd.html

[N04] 斐波那契数列
来源：http://hz.kuanghao11.cn/gtviasdufo.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.shanyushiyangtech.top/gtbkbwzixk.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.jinqigufen.top/gtcuifdhff.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yj20258888.top/gtpvlxwska.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.shangyingyoupin.top/gtuofvnsqa.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.iojbl.cn/gtcmwtksaj.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.jyoumei.cn/gtnyrphwbu.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.jlsjyb.cn/gtfpvuumrm.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.hnqzz.top/gtzqyplloj.html

[N05] 最大公约数
来源：http://hz.hfpthk.cn/gtyidghimc.html

Py:   math.gcd(a, b)
来源：http://hz.bjfxy.top/gtefyzmnro.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.sysykeji.top/gtsktimosa.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jinqigufen.top/gtyjjqxzye.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.redwolf501.top/gtmovrwfbi.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.52xcode.cn/gtdebvxttk.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.fzhhl.top/gtfsnlhfrb.html

Ruby: a.gcd(b)
来源：http://hz.dashuyun.cn/gtsiyfqief.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.cqqwz.cn/gtonrmmmgn.html

[N06] 判断回文字符串
来源：http://hz.ybcxt.top/gtsxwkwgeu.html

Py:   s == s[::-1]
来源：http://hz.havefunace.top/gtmpwqjsku.html

PHP:  $s === strrev($s);
来源：http://hz.zhaomingkeji.xyz/gtwqmmtvmb.html

JS:   s === [...s].reverse().join("")
来源：http://hz.cucudq.cn/gtpuypxzqv.html

TS:   s === [...s].reverse().join("")
来源：http://hz.9152youxi.cn/gtihgptaap.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.fengsongda.top/gtqpzksmlm.html

Go:   // 双指针从两端比较
来源：http://hz.chenjidiqi.icu/gtmbhxhdxx.html

Ruby: s == s.reverse
来源：http://hz.yj20258888.top/gtmazayaco.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.vqdsnc.cn/gtfjvajayk.html

[N07] 两数之和（返回下标）
来源：http://hz.pengpengdd.cyou/gtoytphnbm.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.guowangkeji.top/gtndkbwavu.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.xuanzx.com/gthrfhkcfo.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.jyoumei.cn/gthwpftoyc.html

TS:   // 手写 Map<string, number>
来源：http://hz.yj20258.top/gtlufgvbfr.html

Java: // 手写 HashMap
来源：http://hz.316326.xyz/gtgycosyja.html

Go:   // 手写 map[int]int
来源：http://hz.yj20258.top/gtplqpalur.html

Ruby: // 手写 Hash
来源：http://hz.kuanghao11.cn/gtyslwiqlo.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.gzhubu.top/gticddfuwn.html

[N08] 生成全排列
来源：http://hz.jlsjyb.cn/gtiixdrokh.html

Py:   itertools.permutations(arr)
来源：http://hz.vqdsnc.cn/gtwswstcnr.html

PHP:  // 手写递归交换
来源：http://hz.yj20258.top/gtzhtjgcek.html

JS:   // 手写回溯递归
来源：http://hz.sxryk.cn/gtcvqrngfn.html

TS:   // 手写回溯递归
来源：http://hz.zhoulong.xyz/gtitutecys.html

Java: // 手写回溯递归
来源：http://hz.jianghu66.top/gtawzzxsri.html

Go:   // 手写回溯递归
来源：http://hz.havefunace.top/gtbhodwvhj.html

Ruby: arr.permutation.to_a
来源：http://hz.hongshengwenyu.top/gtoeqkwveg.html

C#:   // 手写回溯递归
来源：http://hz.tianlin.xyz/gtfehkcrmn.html

[N09] 栈与队列
来源：http://hz.9152youxi.cn/gtayykqbof.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.cqqwz.cn/gtwxhyiasn.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.yonumen.top/gtmgrocucq.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.sufxvd.cn/gtaixsablt.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.aizwys.cn/gtpfarodqw.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.dianchejie.cn/gteezypmwd.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.yuxming.cn/gtgyexnrgg.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.cdnleiting.top/gtqbacofzk.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.xuetiantiany.cn/gtdzfwakyw.html

[N10] 链表节点定义
来源：http://hz.yueranfly.top/gtnxgehlzi.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.yongpay.top/gticfkbrbp.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.gotoacloud.top/gtrppxpvly.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.snrcjt.cn/gtgxnalnci.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.cucudq.cn/gthkuhkmrv.html

Java: class Node { int v; Node next; }
来源：http://hz.zhoulong.xyz/gtmhgpclzu.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.yueranfly.top/gtgcwevnui.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.hnxiangtu.top/gtiounhuzc.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.hysaishi.cn/gtghsaicdg.html

[N11] 二叉树中序遍历
来源：http://hz.nanxuanxn.top/gthykxkgbl.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.zhaomingkeji.xyz/gtdwlmkcqe.html

PHP:  // 手写递归函数
来源：http://hz.yvedp.cn/gtzfeosmnm.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.haohaochexian.top/gtabbltezp.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jinyuanbaomall.cn/gtlwzacokp.html

Java: // 手写递归
来源：http://hz.yj20258888.top/gtbjwuycgy.html

Go:   // 手写递归
来源：http://hz.redwolf501.top/gtfnrbkzwb.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.guowangkeji.top/gtjywchlsf.html

C#:   // 手写递归
来源：http://hz.cashguo.top/gtdpqrbrqk.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.tian-w.cn/gtlkjgakuc.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.xinyue.icu/gttrgaclwt.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.zhongyouzk.top/gtlhfycgqs.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.havefunace.top/gtssqrfucp.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.sysykeji.top/gttjhkfsit.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.ivvv.top/gtsjktmazj.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.jianghu66.top/gtqpkzujpz.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.nwbrower.top/gttjhuvnzo.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.zhengqikj.top/gtfffmezmu.html

================================================================================
来源：http://hz.jiagoushi.top/gtcxyhzowu.html

O. 并发与异步
来源：http://hz.chenlongwang.top/gtodaybqmp.html

================================================================================
来源：http://hz.fzhhl.top/gtvmlnuenj.html

[O01] 启动一个线程
来源：http://hz.gaohongyu789.top/gtxasvgdls.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.zhengqikj.top/gtyukygjqz.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.aibaodan.cn/gtaimaahsu.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.fzhhl.top/gtgevhfhrq.html

TS:   // 同 JS
来源：http://hz.chenlongwang.top/gtdxqcgnqu.html

Java: new Thread(() -> f()).start()
来源：http://hz.jinghuilouyu.cn/gtuoidqedw.html

Go:   go f()
来源：http://hz.cucudq.cn/gtklxqiize.html

Ruby: Thread.new { f }
来源：http://hz.zhaomingkeji.xyz/gtpezgqfpl.html

C#:   Task.Run(() => F());
来源：http://hz.jinqigufen.top/gtvfxpxfiw.html

[O02] 使用线程池
来源：http://hz.nanxinkj.top/gtddhskhfx.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.ybcxt.top/gtjrhhprav.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.daxiang520.top/gtxttccfbh.html

JS:   // worker_threads 线程池
来源：http://hz.jinqigfzy.top/gtznyfqjqs.html

TS:   // worker_threads 线程池
来源：http://hz.andypj.xyz/gtvbcxhaek.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.zycfv.cn/gtqlxblrzj.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.zhixingplan.top/gthswpbjar.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.gogol.net.cn/gtqxetafsk.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.jianghu66.top/gtxvdzmwxa.html

[O03] 加锁保护共享数据
来源：http://hz.hammf.cn/gtxtdliiwz.html

Py:   with lock: shared += 1
来源：http://hz.zhixingplan.top/gtmulknzsq.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.shzxlz.cn/gtgsworxrc.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.cashguo.top/gthcwnwvyx.html

TS:   // 同 JS
来源：http://hz.yj20258.top/gtrwvbtsmb.html

Java: synchronized (this) { shared++; }
来源：http://hz.nwbrower.top/gtzxtpznkn.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.sysykeji.top/gtbuftvnxi.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.xuetiantiany.cn/gtxyxanlzj.html

C#:   lock (gate) { shared++; }
来源：http://hz.hnxiangtu.top/gtqotfntpo.html

[O04] 定义异步函数并等待
来源：http://hz.birdmap.top/gtxrbqrbsu.html

Py:   async def f():⏎    await g()
来源：http://hz.yj20258888.top/gtzafhoahi.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.shanyushiyangtech.top/gtesrdiufh.html

JS:   async function f() { await g(); }
来源：http://hz.jiagoushi.top/gtkbacowgw.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.jiagoushi.top/gtaovjiakh.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.shangyingyoupin.top/gtjogjjdcm.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.snrcjt.cn/gtxgccmgho.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.redwolf501.top/gtaqujlrle.html

C#:   async Task F() { await G(); }
来源：http://hz.cucudq.cn/gtiudpgnhr.html

[O05] 并发执行并等待全部完成
来源：http://hz.quarkkingdee.top/gtxskrswbu.html

Py:   asyncio.gather(*tasks)
来源：http://hz.nwbrower.top/gtsbpisjzd.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.redwolf501.top/gtawetiunb.html

JS:   await Promise.all(tasks)
来源：http://hz.cashguo.top/gtvmcdfkur.html

TS:   await Promise.all(tasks)
来源：http://hz.hongshengwenyu.top/gtlrrhbykt.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.guannengcc.top/gtsthibjxm.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.nanxuanxn.top/gtqhmjcaug.html

Ruby: threads.map(&:join)
来源：http://hz.andypj.xyz/gthctzbvby.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.nwbrower.top/gttljlohcf.html

[O06] 使用进程池
来源：http://hz.jyoumei.cn/gtsxvnpvfh.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.xuetiantiany.cn/gtxmyjvuna.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.fzhhl.top/gtcqrgwvkg.html

JS:   // child_process / cluster 模块
来源：http://hz.shanyushiyangtech.top/gtcjdvpdxd.html

TS:   // child_process / cluster 模块
来源：http://hz.aizwys.cn/gtrxsyaqbd.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.ppjwa.cn/gtjmgiazjd.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.zhengqikj.top/gtzyfvmlad.html

Ruby: // fork 块
来源：http://hz.yonumen.top/gtpsypggpp.html

C#:   Parallel.For
来源：http://hz.gotoacloud.top/gtbyquaunl.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtacozjdzh.html

P. 常用工具函数
来源：http://hz.0kj1m.cn/gttbxfsiua.html

================================================================================
来源：http://hz.sufxvd.cn/gtpkjrtfhr.html

[P01] 生成 UUID
来源：http://hz.zycfv.cn/gtqweyvsja.html

Py:   str(uuid.uuid4())
来源：http://hz.sweek.top/gtupemftly.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.ppjwa.cn/gtszloufuf.html

JS:   crypto.randomUUID()
来源：http://hz.yueranfly.top/gtfqrveolp.html

TS:   crypto.randomUUID()
来源：http://hz.fzhhl.top/gtquagbnyi.html

Java: UUID.randomUUID().toString()
来源：http://hz.jyoumei.cn/gtltumlzmg.html

Go:   // 用 github.com/google/uuid
来源：http://hz.hfpthk.cn/gtjxzuujml.html

Ruby: SecureRandom.uuid
来源：http://hz.316326.xyz/gtsdernfyq.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.shanyushiyangtech.top/gtbjshbhpm.html

[P02] MD5 / SHA256 摘要
来源：http://hz.zhiwuduotai.top/gtmlddaltf.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.xinyue.icu/gteshhxxuc.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.shangyingyoupin.top/gtfcqidgyz.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.pengpengdd.cyou/gtcrmvonyn.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.xingfuxueyuan.xyz/gtpbfwzpjp.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.yj20258888.top/gtoshzcort.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.52xcode.cn/gtcsjhmeso.html


<!-- 参考信息 -->