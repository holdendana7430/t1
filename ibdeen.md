代发 wailian999

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.havefunace.top/gtmehwpvmh.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.52xcode.cn/gtdkwdpwek.html

[L05] 上传文件（multipart）
来源：http://hz.wangshuangyany.cn/gttnlcoxmg.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.zhixingplan.top/gtngvdbkge.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.tanke756.top/gtfqcvnbxb.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.aibaodan.cn/gteoozzqik.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.tanke756.top/gtojdvebtb.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.cdnleiting.top/gtpkmjfvqj.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.dashuyun.cn/gtglvxiojh.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.xingfuxueyuan.xyz/gtkvrehrss.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.gzhubu.top/gtkshgzrhk.html

[L06] 解析响应为 JSON
来源：http://hz.xinyue.icu/gtoiusubhs.html

Py:   resp.json()
来源：http://hz.hnqzz.top/gtsqsdkavx.html

PHP:  json_decode($body, true);
来源：http://hz.havefunace.top/gtvvngyvnc.html

JS:   await resp.json()
来源：http://hz.yj202588.top/gtzcqzydjz.html

TS:   await resp.json()
来源：http://hz.jqgufenzy.top/gtxmmxknqh.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.nanxuanxn.top/gtvwpshoub.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.9152youxi.cn/gteqkivhtf.html

Ruby: JSON.parse(resp.body)
来源：http://hz.yj20258888.top/gtfjclkyqf.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.nwbrower.top/gtfhyqejjj.html

[L07] 处理 HTTP 状态码
来源：http://hz.ivvv.top/gtqqgssjai.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.nanxinkj.top/gtrrydngtv.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.tianlin.xyz/gtumrndcqp.html

JS:   resp.ok;  resp.status
来源：http://hz.xuetiantiany.cn/gtqcnlthqr.html

TS:   resp.ok;  resp.status
来源：http://hz.dashuyun.cn/gtokcpyhys.html

Java: resp.statusCode()
来源：http://hz.hnqzz.top/gtkbeiyzbk.html

Go:   resp.StatusCode
来源：http://hz.yvedp.cn/gtulzcnusr.html

Ruby: resp.code.to_i
来源：http://hz.meibo888.top/gtsletdzqa.html

C#:   (int)resp.StatusCode
来源：http://hz.shanyushiyangtech.top/gtnqvgogwl.html

[L08] 并发请求多个地址
来源：http://hz.zhongyouzk.top/gtzbhbyqbn.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.yj202588.top/gtgeupphoc.html

PHP:  curl_multi_init() 系列
来源：http://hz.sufxvd.cn/gtjjcrervw.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.ehwqpu.com/gtmagqodxg.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jinghuilouyu.cn/gtumhvfnmw.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.shzxlz.cn/gtipxdpirg.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.jinyuanbaomall.cn/gthwztwmri.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.guowangkeji.top/gtiegrltfc.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.zycfv.cn/gtdnjkvhbn.html

================================================================================
来源：http://hz.redwolf501.top/gtllbnjuea.html

M. 命令行 / 进程 / 环境
来源：http://hz.nwbrower.top/gtdwjpbuiw.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtnewscqha.html

[M01] 读取命令行参数
来源：http://hz.jianghu66.top/gttziqkvdb.html

Py:   sys.argv[1:]
来源：http://hz.iojbl.cn/gtttogottn.html

PHP:  $argv;  $argc;
来源：http://hz.sysykeji.top/gtcqqbbwdi.html

JS:   process.argv.slice(2)
来源：http://hz.cdnleiting.top/gtgnggizbu.html

TS:   process.argv.slice(2)
来源：http://hz.xylfe.cn/gtrlloexir.html

Java: args 数组（main 方法参数）
来源：http://hz.0kj1m.cn/gtwouozcin.html

Go:   os.Args[1:]
来源：http://hz.pengpengdd.cyou/gtlvxizjqk.html

Ruby: ARGV
来源：http://hz.birdmap.top/gtuowrokuh.html

C#:   args 数组（Main 方法参数）
来源：http://hz.hysaishi.cn/gtsfiiimtl.html

[M02] 读取环境变量
来源：http://hz.tian-w.cn/gtaygdiths.html

Py:   os.environ.get("HOME")
来源：http://hz.hnqzz.top/gtdsrousbr.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.yangfankeji.com/gtihcmnxxn.html

JS:   process.env.HOME
来源：http://hz.ydzc1.top/gtvmhaamgk.html

TS:   process.env.HOME
来源：http://hz.jinqigufen.top/gtwmsnbdfc.html

Java: System.getenv("HOME")
来源：http://hz.jyoumei.cn/gtoafgeqqa.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.fengsongda.top/gtifsunrcf.html

Ruby: ENV["HOME"]
来源：http://hz.redwolf501.top/gthwodfrso.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.andypj.xyz/gthrxgehyf.html

[M03] 执行外部命令
来源：http://hz.zhijiandao.cn/gtugeyueem.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.vqdsnc.cn/gtmuqomlix.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.guannengcc.top/gtfvbllbkr.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.zdqjudy.top/gtmbazhrro.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.zhengqikj.top/gtirgtcnmq.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.yj202588.top/gttylqnkcv.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.meibo888.top/gtlcwzrklo.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.sxryk.cn/gtmncrujen.html

C#:   Process.Start("ls", "-l");
来源：http://hz.yonumen.top/gtjxzihuxn.html

[M04] 获取当前工作目录
来源：http://hz.hywenlv.cn/gtakvnjlln.html

Py:   os.getcwd()
来源：http://hz.hongshengwenyu.top/gtxkqxbjiq.html

PHP:  getcwd();
来源：http://hz.tanke756.top/gtfmnqbdps.html

JS:   process.cwd()
来源：http://hz.9152youxi.cn/gtqytzwkug.html

TS:   process.cwd()
来源：http://hz.sweek.top/gtaeufhtww.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.sweek.top/gtpnfaxepy.html

Go:   os.Getwd()
来源：http://hz.chenjidiqi.icu/gtipddijkh.html

Ruby: Dir.pwd
来源：http://hz.316326.xyz/gtejptnbtm.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.316326.xyz/gtsfzwdcjo.html

[M05] 设置退出码
来源：http://hz.zdqjudy.top/gtfuomtlek.html

Py:   sys.exit(1)
来源：http://hz.yonumen.top/gtidygvazw.html

PHP:  exit(1);
来源：http://hz.jinyuanbaomall.cn/gtndlvaqxn.html

JS:   process.exit(1)
来源：http://hz.ppjwa.cn/gtzjkpkhtt.html

TS:   process.exit(1)
来源：http://hz.jyoumei.cn/gtmhnfdkic.html

Java: System.exit(1)
来源：http://hz.c1oappe.top/gtkzkzvoxx.html

Go:   os.Exit(1)
来源：http://hz.xylfe.cn/gteooyktkk.html

Ruby: exit 1
来源：http://hz.jinqigufen.top/gtlgmkenor.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.guannengcc.top/gtqopftrtf.html

[M06] 向标准错误输出
来源：http://hz.xuetiantiany.cn/gtnzwanoig.html

Py:   print("err", file=sys.stderr)
来源：http://hz.jyoumei.cn/gteihtmvgc.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.sysykeji.top/gtlankgzpw.html

JS:   console.error("err")
来源：http://hz.ywan-chungtsiang.top/gtriukdmqc.html

TS:   console.error("err")
来源：http://hz.zhijiandao.cn/gtlhdssofw.html

Java: System.err.println("err")
来源：http://hz.sufxvd.cn/gtsbkygebu.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.havefunace.top/gtmtgvbmch.html

Ruby: warn "err"
来源：http://hz.nanxuanxn.top/gtcyovfopp.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.tanke756.top/gtwgpttied.html

[M07] 判断是否为主入口
来源：http://hz.ydjk.org.cn/gtrlthrfnh.html

Py:   if __name__ == "__main__":
来源：http://hz.zhixingplan.top/gttylplhzd.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.nanxuanxn.top/gtdkfnphwl.html

JS:   require.main === module
来源：http://hz.ydjk.org.cn/gtwcbxqjhs.html

TS:   require.main === module
来源：http://hz.cashguo.top/gtcebikoja.html

Java: public static void main(String[] args)
来源：http://hz.tanke756.top/gttgmmbldu.html

Go:   func main()
来源：http://hz.yueranfly.top/gtemnnvwwd.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.zdqjudy.top/gtkeumvtsu.html

C#:   static void Main(string[] args)
来源：http://hz.hnxiangtu.top/gtfahfbcof.html

[M08] 获取系统与运行时信息
来源：http://hz.shzxlz.cn/gtjvbvctgk.html

Py:   platform.system();  platform.python_version()
来源：http://hz.andypj.xyz/gtrtvlmvbf.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.tianlin.xyz/gtlbokpeut.html

JS:   process.platform;  process.version
来源：http://hz.sufxvd.cn/gtxsiqvapg.html

TS:   process.platform;  process.version
来源：http://hz.birdmap.top/gtftsnghcx.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.xylfe.cn/gtiwcetmlk.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.shzxlz.cn/gtejybqdso.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.ybcxt.top/gtuiokewwi.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.cucudq.cn/gtjpcjuiyr.html

================================================================================
来源：http://hz.pycfn.com/gtitknhvfg.html

N. 数据结构与算法
来源：http://hz.yuanzhike.top/gtkpicltnl.html

================================================================================
来源：http://hz.aibaodan.cn/gtmgxsjxxv.html

[N01] 二分查找（有序数组）
来源：http://hz.meibo888.top/gtfqrcvscq.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.hfpthk.cn/gtsrujsuaq.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.dashuyun.cn/gtqdslkafu.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yanxiufei.cn/gtmekzmrkl.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yj202588.top/gtzasbpqwl.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.gzhubu.top/gtsrcsmyqz.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.quarkkingdee.top/gtzoqasyqu.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.ehwqpu.com/gticyjhkzy.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.daria6918.cn/gtirncalxq.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.birdmap.top/gtkzmkrysy.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.yanxiufei.cn/gtfyiifcfj.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.pengpengdd.cyou/gtnidmjimt.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.ywan-chungtsiang.top/gtemfocutp.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.daxiang520.top/gtozosmqto.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.jqgfzy.top/gtnhjihfpq.html

Go:   slices.Sort(arr)
来源：http://hz.smart0.xyz/gtwpgzdvmf.html

Ruby: arr.sort
来源：http://hz.yj202588.top/gtplurdqvb.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.xylfe.cn/gtmozabsky.html

[N03] 快速排序（分治示例）
来源：http://hz.hfpthk.cn/gtmjtrcmft.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.xziqi.cn/gtfooxbnkr.html

PHP:  // 递归实现，或用 usort
来源：http://hz.yangfankeji.com/gtsbhegelw.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yonumen.top/gtdzapewto.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.shzxlz.cn/gtichgczoz.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.yongpay.top/gteysirjnw.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.guowangkeji.top/gtcqwyergw.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.xylfe.cn/gtuwjloaju.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.ppjwa.cn/gthbzjanpk.html

[N04] 斐波那契数列
来源：http://hz.gotoacloud.top/gticubxwgq.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.hfpthk.cn/gtcfuktusl.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.yuanzhike.top/gtxbuvoqkj.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.zycfv.cn/gtfnksusoa.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.zhiwuduotai.top/gtcajqgvei.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.wangdashe.top/gtupphseix.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.daxiang520.top/gtigwmzprm.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.ydzc1.top/gtsfgmhrkl.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.zhijiandao.cn/gttslktegl.html

[N05] 最大公约数
来源：http://hz.pengpengdd.cyou/gtgkntpfil.html

Py:   math.gcd(a, b)
来源：http://hz.zhengqikj.top/gtdfkzogrq.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.feifeiyinyue.top/gtcrtcjeeh.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.kuanghao11.cn/gtdlfkqtcw.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.tianlin.xyz/gtnnbjjfbb.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.yuanzhike.top/gtbroughos.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.gogol.net.cn/gttrzdkicb.html

Ruby: a.gcd(b)
来源：http://hz.daxiang520.top/gtxbdahlgh.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.jiagoushi.top/gtraapmbzy.html

[N06] 判断回文字符串
来源：http://hz.yvedp.cn/gttfbosxls.html

Py:   s == s[::-1]
来源：http://hz.jinqigfzy.top/gtxproeann.html

PHP:  $s === strrev($s);
来源：http://hz.chenzaomai.com/gtvsvbepvg.html

JS:   s === [...s].reverse().join("")
来源：http://hz.yueranfly.top/gtyfgbvbjo.html

TS:   s === [...s].reverse().join("")
来源：http://hz.dashuyun.cn/gtylfgstfi.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.sweek.top/gtfohaznpi.html

Go:   // 双指针从两端比较
来源：http://hz.tianlin.xyz/gtaxlaxhrs.html

Ruby: s == s.reverse
来源：http://hz.yueranfly.top/gtektpanty.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.nwbrower.top/gtvmdsdiso.html

[N07] 两数之和（返回下标）
来源：http://hz.sweek.top/gtkzrcfzyo.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.jqgfzy.top/gtvhsocilh.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.yonumen.top/gtgxdbhniz.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.xziqi.cn/gtvssizzkf.html

TS:   // 手写 Map<string, number>
来源：http://hz.shangyingyoupin.top/gtozwfzzaz.html

Java: // 手写 HashMap
来源：http://hz.jianghu66.top/gtmqjdegwk.html

Go:   // 手写 map[int]int
来源：http://hz.aizwys.cn/gtpqbmkcqm.html

Ruby: // 手写 Hash
来源：http://hz.ivvv.top/gtanvsjiso.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.ydzc1.top/gtkvdiflhl.html

[N08] 生成全排列
来源：http://hz.daria6918.cn/gthmsojrll.html

Py:   itertools.permutations(arr)
来源：http://hz.0kj1m.cn/gtiasgyfxs.html

PHP:  // 手写递归交换
来源：http://hz.shuidangran.top/gtawesmmbm.html

JS:   // 手写回溯递归
来源：http://hz.pycfn.com/gtmwvmgzha.html

TS:   // 手写回溯递归
来源：http://hz.gotoacloud.top/gtuyeesgtk.html

Java: // 手写回溯递归
来源：http://hz.yangfankeji.com/gteuhsgske.html

Go:   // 手写回溯递归
来源：http://hz.xuanzx.com/gtgvlthxce.html

Ruby: arr.permutation.to_a
来源：http://hz.9152youxi.cn/gtkflzkzxo.html

C#:   // 手写回溯递归
来源：http://hz.gzhubu.top/gtdtysypap.html

[N09] 栈与队列
来源：http://hz.jinqigufen.top/gtcigjjhmv.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.nanxinkj.top/gtlqfktvqh.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.xuanzx.com/gtewaandnz.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.iojbl.cn/gtwrubpqun.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.nwbrower.top/gtrjifgyde.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.snrcjt.cn/gtkicvwknk.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.aibaodan.cn/gtgggbthpk.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.jinqigfzy.top/gtjabflzaz.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.chenzaomai.com/gtmayevwjd.html

[N10] 链表节点定义
来源：http://hz.zhaomingkeji.xyz/gtvarzjtus.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.hammf.cn/gtixqqgbdb.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.sysykeji.top/gtpoaeahei.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.yvedp.cn/gtudsgxbmt.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.aizwys.cn/gtaaushbwi.html

Java: class Node { int v; Node next; }
来源：http://hz.zhijiandao.cn/gtpzontmpw.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.jinqigfzy.top/gtwnbtzfcz.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.hnxiangtu.top/gteokrsnih.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.bjfxy.top/gtwaceucxx.html

[N11] 二叉树中序遍历
来源：http://hz.pengpengdd.cyou/gtegqumnzi.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.316326.xyz/gtiqofrhjr.html

PHP:  // 手写递归函数
来源：http://hz.yongpay.top/gtlhcyfcnf.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yuxming.cn/gttpelbfiz.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.chenjidiqi.icu/gtzzzuxzfk.html

Java: // 手写递归
来源：http://hz.jqgfzy.top/gtcptwsrwq.html

Go:   // 手写递归
来源：http://hz.jianghu66.top/gtulbtdvhb.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.guowangkeji.top/gtrjerpwpz.html

C#:   // 手写递归
来源：http://hz.xuanzx.com/gtpgvrkmne.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.ydzc1.top/gtvvyzyvqd.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.ppjwa.cn/gtlvmaxsfr.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.yuxming.cn/gtbxdtldlw.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.zycfv.cn/gtytlnbzee.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jyoumei.cn/gtahkconqf.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yueranfly.top/gtcyewhdtn.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.vqdsnc.cn/gtjqnilujd.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.shanyushiyangtech.top/gtsxqxieou.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.tianlin.xyz/gtktitlded.html

================================================================================
来源：http://hz.smart0.xyz/gtdneczxda.html

O. 并发与异步
来源：http://hz.tianlin.xyz/gtxecqcxhq.html

================================================================================
来源：http://hz.yongpay.top/gtctyojran.html

[O01] 启动一个线程
来源：http://hz.cdnleiting.top/gtbjimvafh.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.wangdashe.top/gthzhteglt.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.zdqjudy.top/gtxgutjndo.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.aizwys.cn/gtxjbugrsg.html

TS:   // 同 JS
来源：http://hz.feifeiyinyue.top/gtluegcxdy.html

Java: new Thread(() -> f()).start()
来源：http://hz.0kj1m.cn/gtvzgojxoa.html

Go:   go f()
来源：http://hz.yueranfly.top/gtaghukuwu.html

Ruby: Thread.new { f }
来源：http://hz.havefunace.top/gtyjbazets.html

C#:   Task.Run(() => F());
来源：http://hz.zdqjudy.top/gtniuyuszm.html

[O02] 使用线程池
来源：http://hz.iojbl.cn/gthbphkffz.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.wangdashe.top/gthvnnulzs.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.aibaodan.cn/gtvevjzxzh.html

JS:   // worker_threads 线程池
来源：http://hz.fengsongda.top/gtkcxihdfs.html

TS:   // worker_threads 线程池
来源：http://hz.yangfankeji.com/gtsurnttrm.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.yuxming.cn/gtednpvrcd.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.sysykeji.top/gtpttjlmpz.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.birdmap.top/gtpcavywcz.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.sxryk.cn/gtyavyhlqf.html

[O03] 加锁保护共享数据
来源：http://hz.kuanghao11.cn/gthdjkaeeb.html

Py:   with lock: shared += 1
来源：http://hz.tanke756.top/gttyimoxle.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.316326.xyz/gtacbxfzrx.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.zhijiandao.cn/gtyupwgsfs.html

TS:   // 同 JS
来源：http://hz.zhixingplan.top/gtxekearuo.html

Java: synchronized (this) { shared++; }
来源：http://hz.kuanghao11.cn/gtvjevijhi.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.cucudq.cn/gtejiqpybk.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.ybcxt.top/gtpqcxfqcc.html

C#:   lock (gate) { shared++; }
来源：http://hz.hnxiangtu.top/gtmdqhzapo.html

[O04] 定义异步函数并等待
来源：http://hz.xingfuxueyuan.xyz/gtabwuehuu.html

Py:   async def f():⏎    await g()
来源：http://hz.hammf.cn/gtczsonnmn.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.yj202588.top/gtexvqaoep.html

JS:   async function f() { await g(); }
来源：http://hz.birdmap.top/gttotluqtn.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.dashuyun.cn/gtbgnkzdew.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.nanxuanxn.top/gtdurnzxpi.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.bjfxy.top/gtdprblcuo.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.guowangkeji.top/gtmxopgjuk.html

C#:   async Task F() { await G(); }
来源：http://hz.fengsongda.top/gtfhtbtkjg.html

[O05] 并发执行并等待全部完成
来源：http://hz.jianghu66.top/gtjcqgtqfe.html

Py:   asyncio.gather(*tasks)
来源：http://hz.nwbrower.top/gtcrnxoeoc.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.tian-w.cn/gtltutapsg.html

JS:   await Promise.all(tasks)
来源：http://hz.jqgufenzy.top/gtbigpytww.html

TS:   await Promise.all(tasks)
来源：http://hz.yvedp.cn/gtindjvvmt.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.yj20258.top/gtleihavub.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.fengsongda.top/gtwkkfqaub.html

Ruby: threads.map(&:join)
来源：http://hz.yonumen.top/gtyzoobjsg.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.zdqjudy.top/gtdfwlhngz.html

[O06] 使用进程池
来源：http://hz.aibaodan.cn/gtdwrfmjxu.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.quarkkingdee.top/gtannykdzu.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.haohaochexian.top/gttbsdtjzq.html

JS:   // child_process / cluster 模块
来源：http://hz.jinqigfzy.top/gtpqmzixhp.html

TS:   // child_process / cluster 模块
来源：http://hz.hongshengwenyu.top/gtolkvzieh.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.ppjwa.cn/gtgtdnmyvx.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.sysykeji.top/gtghptvfay.html

Ruby: // fork 块
来源：http://hz.jlsjyb.cn/gtzijsosdk.html

C#:   Parallel.For
来源：http://hz.haohaochexian.top/gtptkmwnek.html

================================================================================
来源：http://hz.52xcode.cn/gtmxhkdjlv.html

P. 常用工具函数
来源：http://hz.jlsjyb.cn/gtokyupxrk.html

================================================================================
来源：http://hz.dashuyun.cn/gttsqmfzqm.html

[P01] 生成 UUID
来源：http://hz.zycfv.cn/gtyzxtwbqu.html

Py:   str(uuid.uuid4())
来源：http://hz.daxiang520.top/gtevcivbue.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.hysaishi.cn/gtvpnnxzuz.html

JS:   crypto.randomUUID()
来源：http://hz.feifeiyinyue.top/gtgzxmnzcl.html

TS:   crypto.randomUUID()
来源：http://hz.quarkkingdee.top/gtxubooakr.html

Java: UUID.randomUUID().toString()
来源：http://hz.andypj.xyz/gtsfjenfgs.html

Go:   // 用 github.com/google/uuid
来源：http://hz.kuanghao11.cn/gtdpunhilr.html

Ruby: SecureRandom.uuid
来源：http://hz.hnqzz.top/gtazimajmy.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.chenjidiqi.icu/gtwnhwvzuh.html

[P02] MD5 / SHA256 摘要
来源：http://hz.wangshuangyany.cn/gttzwlncvw.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.yueranfly.top/gtyajfbjle.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.kuanghao11.cn/gtauvuheoy.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.fengsongda.top/gtkgqmwkam.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.nwbrower.top/gtxfjdstby.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.gaohongyu789.top/gtkjopramt.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.shangyingyoupin.top/gtleejjzad.html


<!-- 参考信息 -->