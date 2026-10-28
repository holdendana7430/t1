代发 wailian999

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.daria6918.cn/gthxkbvusl.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.xingfuxueyuan.xyz/gtqhlektdb.html

[L05] 上传文件（multipart）
来源：http://hz.0kj1m.cn/gtlsxfaxmd.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.ppjwa.cn/gtnxqkmkqq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.yvedp.cn/gtobwlbqjm.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.ppjwa.cn/gtidirkmnw.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.0kj1m.cn/gtrgcuerll.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.yj20258.top/gtxjolgyto.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.zhaomingkeji.xyz/gtxydqvfzd.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.hongshengwenyu.top/gtqeqlmlbf.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.jianghu66.top/gtiqkzzcvx.html

[L06] 解析响应为 JSON
来源：http://hz.kuanghao11.cn/gttvbbsuof.html

Py:   resp.json()
来源：http://hz.pengpengdd.cyou/gtrlgrmcds.html

PHP:  json_decode($body, true);
来源：http://hz.xuetiantiany.cn/gtatzgjoqc.html

JS:   await resp.json()
来源：http://hz.shanyushiyangkeji.top/gtjdrujgjk.html

TS:   await resp.json()
来源：http://hz.yueranfly.top/gterpvalgz.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.ydzc1.top/gtqgackikb.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.sweek.top/gtrbfuelpi.html

Ruby: JSON.parse(resp.body)
来源：http://hz.pengpengdd.cyou/gtqpqgokct.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.hongshengwenyu.top/gtqejvcela.html

[L07] 处理 HTTP 状态码
来源：http://hz.guowangkeji.top/gtvaulhrmf.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.hysaishi.cn/gtvwfjiqar.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.xingfuxueyuan.xyz/gtsrjeboss.html

JS:   resp.ok;  resp.status
来源：http://hz.yj20258888.top/gtvssyontm.html

TS:   resp.ok;  resp.status
来源：http://hz.wangdashe.top/gthxpvkslq.html

Java: resp.statusCode()
来源：http://hz.sxryk.cn/gtqzmlddsm.html

Go:   resp.StatusCode
来源：http://hz.ppjwa.cn/gtyrxjsmmi.html

Ruby: resp.code.to_i
来源：http://hz.daxiang520.top/gtikablmcw.html

C#:   (int)resp.StatusCode
来源：http://hz.jqgfzy.top/gtzlutrsrj.html

[L08] 并发请求多个地址
来源：http://hz.jyoumei.cn/gthluzxdem.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.jqgfzy.top/gtjxfuxtut.html

PHP:  curl_multi_init() 系列
来源：http://hz.yj202588.top/gtwmsitsve.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.316326.xyz/gtlagjokqb.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.hywenlv.cn/gtqmfpfwak.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.svipenyu.cn/gtdbrntsow.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.yongpay.top/gttxpubxkx.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.ybcxt.top/gtytwrobmi.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.fzhhl.top/gtoklidqeu.html

================================================================================
来源：http://hz.pengpengdd.cyou/gttsenxjsy.html

M. 命令行 / 进程 / 环境
来源：http://hz.fengsongda.top/gtkxtkypux.html

================================================================================
来源：http://hz.xziqi.cn/gtovsskfnz.html

[M01] 读取命令行参数
来源：http://hz.zhengqikj.top/gtrzbuoyqn.html

Py:   sys.argv[1:]
来源：http://hz.hnqzz.top/gthdvxjskc.html

PHP:  $argv;  $argc;
来源：http://hz.cdnleiting.top/gtgraxufmu.html

JS:   process.argv.slice(2)
来源：http://hz.cdnleiting.top/gtizchomft.html

TS:   process.argv.slice(2)
来源：http://hz.birdmap.top/gtkgrdyfkt.html

Java: args 数组（main 方法参数）
来源：http://hz.jianghu66.top/gtbnrsymfc.html

Go:   os.Args[1:]
来源：http://hz.snrcjt.cn/gtbxajxvpi.html

Ruby: ARGV
来源：http://hz.zhijiandao.cn/gtwkqprdvv.html

C#:   args 数组（Main 方法参数）
来源：http://hz.yvedp.cn/gtczipjtkn.html

[M02] 读取环境变量
来源：http://hz.c1oappe.top/gtqrpzylhc.html

Py:   os.environ.get("HOME")
来源：http://hz.havefunace.top/gtotvpqkaq.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.jiagoushi.top/gtxytstoec.html

JS:   process.env.HOME
来源：http://hz.chenzaomai.com/gtbpcaaxlf.html

TS:   process.env.HOME
来源：http://hz.hysaishi.cn/gtawthccbd.html

Java: System.getenv("HOME")
来源：http://hz.pengpengdd.cyou/gtgjfkwcki.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.shangyingyoupin.top/gtczpmsbss.html

Ruby: ENV["HOME"]
来源：http://hz.birdmap.top/gtksavvhvm.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.yonumen.top/gtzlhzvzwj.html

[M03] 执行外部命令
来源：http://hz.ppjwa.cn/gtsevblcbe.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.tianlin.xyz/gtyilrhftx.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.gotoacloud.top/gthnfppgmm.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.sxryk.cn/gtmzaldmcz.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.shanyushiyangkeji.top/gtoyefxrhk.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.yj202588.top/gtwzotcsrt.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.yueranfly.top/gtysbinqwx.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.ybcxt.top/gtdnvlnfit.html

C#:   Process.Start("ls", "-l");
来源：http://hz.yueranfly.top/gtktkwaflz.html

[M04] 获取当前工作目录
来源：http://hz.havefunace.top/gtdwnsxjwx.html

Py:   os.getcwd()
来源：http://hz.yongpay.top/gtjreqjhxv.html

PHP:  getcwd();
来源：http://hz.daria6918.cn/gtcbjhysem.html

JS:   process.cwd()
来源：http://hz.sxryk.cn/gtrnfzonxu.html

TS:   process.cwd()
来源：http://hz.daxiang520.top/gtkmnauuvq.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.jqgfzy.top/gthjklimqr.html

Go:   os.Getwd()
来源：http://hz.sysykeji.top/gtygjfjqdx.html

Ruby: Dir.pwd
来源：http://hz.yj20258888.top/gtsqjopcjf.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.jiagoushi.top/gtwfjrugwj.html

[M05] 设置退出码
来源：http://hz.guannengcc.top/gtjcmkcedt.html

Py:   sys.exit(1)
来源：http://hz.hfpthk.cn/gtjmkpdwnw.html

PHP:  exit(1);
来源：http://hz.haohaochexian.top/gtfmbtavpj.html

JS:   process.exit(1)
来源：http://hz.hongshengwenyu.top/gtnrsozjns.html

TS:   process.exit(1)
来源：http://hz.hongshengwenyu.top/gtoamlkvsk.html

Java: System.exit(1)
来源：http://hz.haohaochexian.top/gtuvkmqvmb.html

Go:   os.Exit(1)
来源：http://hz.dashuyun.cn/gtguoiucxf.html

Ruby: exit 1
来源：http://hz.fengsongda.top/gtvwyegegz.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.andypj.xyz/gtitunnhyr.html

[M06] 向标准错误输出
来源：http://hz.pycfn.com/gtheealrzk.html

Py:   print("err", file=sys.stderr)
来源：http://hz.zhaomingkeji.xyz/gtrlhfutrs.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.yangfankeji.com/gtltjmifwo.html

JS:   console.error("err")
来源：http://hz.jqgufenzy.top/gtxkobzwvb.html

TS:   console.error("err")
来源：http://hz.tianlin.xyz/gtkqjhxvxc.html

Java: System.err.println("err")
来源：http://hz.iojbl.cn/gtpdkryxrw.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.aizwys.cn/gtuqkiloqc.html

Ruby: warn "err"
来源：http://hz.guannengcc.top/gtxhpqryxr.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.jqgfzy.top/gtqgayssfp.html

[M07] 判断是否为主入口
来源：http://hz.svipenyu.cn/gtjxjzhvfm.html

Py:   if __name__ == "__main__":
来源：http://hz.yj20258.top/gtbzsmojct.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.mhx1999.top/gtxpqvridi.html

JS:   require.main === module
来源：http://hz.shuidangran.top/gtapkzyxjl.html

TS:   require.main === module
来源：http://hz.zhengqikj.top/gthznacykm.html

Java: public static void main(String[] args)
来源：http://hz.jinqigfzy.top/gtmmulqebb.html

Go:   func main()
来源：http://hz.xziqi.cn/gtmtpfqzqr.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.feifeiyinyue.top/gtcqiwrnee.html

C#:   static void Main(string[] args)
来源：http://hz.vqdsnc.cn/gtrtzjcfhu.html

[M08] 获取系统与运行时信息
来源：http://hz.shanyushiyangtech.top/gtxmeltncd.html

Py:   platform.system();  platform.python_version()
来源：http://hz.ydjk.org.cn/gtmmqpooex.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.zhongyouzk.top/gtbiaqjxub.html

JS:   process.platform;  process.version
来源：http://hz.vqdsnc.cn/gtssdxnswt.html

TS:   process.platform;  process.version
来源：http://hz.tian-w.cn/gtscszyzpp.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.hywenlv.cn/gtvrruccbr.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.yanxiufei.cn/gtqseokadq.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.guannengcc.top/gtpcoyffjl.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.zhoulong.xyz/gtatlksdei.html

================================================================================
来源：http://hz.haohaochexian.top/gtxssfohoi.html

N. 数据结构与算法
来源：http://hz.zhoulong.xyz/gtoskpfxpz.html

================================================================================
来源：http://hz.aizwys.cn/gtkpoovghp.html

[N01] 二分查找（有序数组）
来源：http://hz.kuanghao11.cn/gtevubesly.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.shuidangran.top/gtilxkpnbd.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.dianchejie.cn/gtdsorwaxm.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.ywan-chungtsiang.top/gtxszkzuzx.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.ydzc1.top/gtnlompdky.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.kuanghao11.cn/gtetbjhuak.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.pengpengdd.cyou/gtwvoahxst.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.fengsongda.top/gtmulogpny.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.svipenyu.cn/gttyomlwol.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.xuanzx.com/gtvsrrtmwx.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.cdnleiting.top/gthefcfgiw.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.tanke756.top/gtppnpnran.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yuanzhike.top/gteczlskri.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.hnxiangtu.top/gtdcqalrgt.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.cdnleiting.top/gtjtcifpiy.html

Go:   slices.Sort(arr)
来源：http://hz.ydzc1.top/gtkernpeuv.html

Ruby: arr.sort
来源：http://hz.pengpengdd.cyou/gtoorbmmca.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.jinghuilouyu.cn/gtakymynul.html

[N03] 快速排序（分治示例）
来源：http://hz.xziqi.cn/gtkofkcpzf.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.gaohongyu789.top/gtqlcalnbr.html

PHP:  // 递归实现，或用 usort
来源：http://hz.zhiwuduotai.top/gtspxbseci.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.c1oappe.top/gtvajbqfrj.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.hammf.cn/gtdlkrsfmr.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.yangfankeji.com/gtqkfbrdme.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.xingfuxueyuan.xyz/gtzcimrgat.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.aibaodan.cn/gtsuovxsbc.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.aizwys.cn/gtmjrzcimr.html

[N04] 斐波那契数列
来源：http://hz.kuanghao11.cn/gtrdvmcjob.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.guannengcc.top/gtbxsyictn.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.hongshengwenyu.top/gtjvebyoxq.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.zhengqikj.top/gtfiinxool.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.tianlin.xyz/gtzolbxxhp.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.mhx1999.top/gtihbyvcth.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.hysaishi.cn/gthnjtpafk.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.chenjidiqi.icu/gtaytoljql.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.shangyingyoupin.top/gtbhlmudlt.html

[N05] 最大公约数
来源：http://hz.svipenyu.cn/gtewehatch.html

Py:   math.gcd(a, b)
来源：http://hz.ydzc1.top/gtawlfeuwv.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.sweek.top/gtpvtvygcc.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yuxming.cn/gtezpjfcyn.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.shanyushiyangtech.top/gtqalgdamb.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.ivvv.top/gtommfhdrd.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.sysykeji.top/gtcltkkhlz.html

Ruby: a.gcd(b)
来源：http://hz.yueranfly.top/gtsanegjdh.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.dianchejie.cn/gtcvaxmtjp.html

[N06] 判断回文字符串
来源：http://hz.hnxiangtu.top/gtsphmuvxo.html

Py:   s == s[::-1]
来源：http://hz.andypj.xyz/gtcmeylxdo.html

PHP:  $s === strrev($s);
来源：http://hz.snrcjt.cn/gtnqggvjcb.html

JS:   s === [...s].reverse().join("")
来源：http://hz.tianlin.xyz/gtgpbqwqra.html

TS:   s === [...s].reverse().join("")
来源：http://hz.dashuyun.cn/gtxokdkzev.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.wangshuangyany.cn/gtpiffgnkh.html

Go:   // 双指针从两端比较
来源：http://hz.xziqi.cn/gtzsxvbcbm.html

Ruby: s == s.reverse
来源：http://hz.nanxinkj.top/gtrghdykxd.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.ivvv.top/gtzgqxkxpd.html

[N07] 两数之和（返回下标）
来源：http://hz.cdnleiting.top/gtgkvwwvta.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.chenlongwang.top/gtfwhfxrqz.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.hysaishi.cn/gtjjosymrc.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.xuetiantiany.cn/gtlycheacj.html

TS:   // 手写 Map<string, number>
来源：http://hz.yuanzhike.top/gtqgekjojw.html

Java: // 手写 HashMap
来源：http://hz.shangyingyoupin.top/gtjlqdngxx.html

Go:   // 手写 map[int]int
来源：http://hz.hnqzz.top/gtrocpazhf.html

Ruby: // 手写 Hash
来源：http://hz.jyoumei.cn/gtfhawzcuh.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.daxiang520.top/gtzrgglbyr.html

[N08] 生成全排列
来源：http://hz.ydjk.org.cn/gtszakyrds.html

Py:   itertools.permutations(arr)
来源：http://hz.316326.xyz/gtywmcynih.html

PHP:  // 手写递归交换
来源：http://hz.havefunace.top/gticdtmnkx.html

JS:   // 手写回溯递归
来源：http://hz.shanyushiyangkeji.top/gtitcsyqik.html

TS:   // 手写回溯递归
来源：http://hz.9152youxi.cn/gtvroddnpm.html

Java: // 手写回溯递归
来源：http://hz.gaohongyu789.top/gtbmrswral.html

Go:   // 手写回溯递归
来源：http://hz.xingfuxueyuan.xyz/gtgabulsjb.html

Ruby: arr.permutation.to_a
来源：http://hz.quarkkingdee.top/gtfjagzfwb.html

C#:   // 手写回溯递归
来源：http://hz.jiagoushi.top/gtjtczehrz.html

[N09] 栈与队列
来源：http://hz.yonumen.top/gtauitvsde.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.zycfv.cn/gtqxccthob.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.cashguo.top/gtgyyhxzah.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.yj202588.top/gtfboxkvir.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.guannengcc.top/gtayqyeyyp.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.feifeiyinyue.top/gtyvkeodfu.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.ydzc1.top/gtkwdswykl.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.gaohongyu789.top/gtcaxtafbd.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.yonumen.top/gtmqazxyjr.html

[N10] 链表节点定义
来源：http://hz.zhoulong.xyz/gtzghfuljr.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.jlsjyb.cn/gtgxrmsffm.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.9152youxi.cn/gtwbawmiax.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.gzhubu.top/gtimggkqbh.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.yj20258888.top/gtvyplpnoe.html

Java: class Node { int v; Node next; }
来源：http://hz.ppjwa.cn/gtasujgxcm.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.ivvv.top/gtkijncyaj.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.52xcode.cn/gtlruzjraf.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.yj202588.top/gttekgkaqt.html

[N11] 二叉树中序遍历
来源：http://hz.xuanzx.com/gtgxeznmwb.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.jinqigfzy.top/gtmpnviqlo.html

PHP:  // 手写递归函数
来源：http://hz.meibo888.top/gtzielrjer.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.quarkkingdee.top/gtopxgodgr.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.xuetiantiany.cn/gtqibvnezo.html

Java: // 手写递归
来源：http://hz.jinqigufen.top/gtwfyibzpo.html

Go:   // 手写递归
来源：http://hz.shangyingyoupin.top/gtpqtdjszy.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.yuxming.cn/gtrnthchgb.html

C#:   // 手写递归
来源：http://hz.jinyuanbaomall.cn/gtuyrdxkuy.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.gogol.net.cn/gtcbnmjrdh.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.yonumen.top/gtishdwwqg.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.quarkkingdee.top/gtxomimgau.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yonumen.top/gtakcbtvnm.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.sweek.top/gtjikvllwm.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.hysaishi.cn/gthubyvmne.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.yongpay.top/gtjchnvyct.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.daxiang520.top/gtwalacuvf.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.jinqigufen.top/gtvsfqmsvz.html

================================================================================
来源：http://hz.cqqwz.cn/gtkpihyprj.html

O. 并发与异步
来源：http://hz.chenjidiqi.icu/gtsnjawgga.html

================================================================================
来源：http://hz.hysaishi.cn/gtvpdjxvaa.html

[O01] 启动一个线程
来源：http://hz.chenjidiqi.icu/gtdbqwixbv.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.snrcjt.cn/gtwpjjdmrd.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.zhongyouzk.top/gtkyhrcyvr.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.zdqjudy.top/gtqqighuyr.html

TS:   // 同 JS
来源：http://hz.sxryk.cn/gthvyhntjo.html

Java: new Thread(() -> f()).start()
来源：http://hz.zhaomingkeji.xyz/gtrpkhmpdh.html

Go:   go f()
来源：http://hz.yuxming.cn/gtfdsnqbmo.html

Ruby: Thread.new { f }
来源：http://hz.pengpengdd.cyou/gtpchfaiii.html

C#:   Task.Run(() => F());
来源：http://hz.jqgfzy.top/gtbnxaojbh.html

[O02] 使用线程池
来源：http://hz.sysykeji.top/gtxcxiivcz.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.havefunace.top/gtjthxincr.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.hongshengwenyu.top/gtcyxslviq.html

JS:   // worker_threads 线程池
来源：http://hz.wangdashe.top/gtmsoxeleu.html

TS:   // worker_threads 线程池
来源：http://hz.fzhhl.top/gtjsnwqdzn.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.dashuyun.cn/gtniyhrsow.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.jiagoushi.top/gtsmymwzay.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.havefunace.top/gtexowgrzv.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.shangyingyoupin.top/gtjlzdpvxj.html

[O03] 加锁保护共享数据
来源：http://hz.jlsjyb.cn/gtmzxrssxh.html

Py:   with lock: shared += 1
来源：http://hz.aizwys.cn/gtoqywlpka.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.jinqigfzy.top/gtyqjghdtt.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.tianlin.xyz/gtovaswzfn.html

TS:   // 同 JS
来源：http://hz.yangfankeji.com/gtnpyrtvbc.html

Java: synchronized (this) { shared++; }
来源：http://hz.sweek.top/gtbzwalabt.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.zhongyouzk.top/gtpddqdivr.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.cdnleiting.top/gtcpplpvhv.html

C#:   lock (gate) { shared++; }
来源：http://hz.shuidangran.top/gtvnavzmwy.html

[O04] 定义异步函数并等待
来源：http://hz.cqqwz.cn/gtpzpobzlp.html

Py:   async def f():⏎    await g()
来源：http://hz.sysykeji.top/gtonammwdn.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.redwolf501.top/gtiovflsyz.html

JS:   async function f() { await g(); }
来源：http://hz.yangfankeji.com/gtkvjzrcgy.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.cashguo.top/gtbwnxdpcn.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.birdmap.top/gtkqzyryag.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.sysykeji.top/gtmzqphqqn.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.tianlin.xyz/gtqgsjqcyp.html

C#:   async Task F() { await G(); }
来源：http://hz.meibo888.top/gtwjemuwee.html

[O05] 并发执行并等待全部完成
来源：http://hz.nwbrower.top/gtmodndbug.html

Py:   asyncio.gather(*tasks)
来源：http://hz.ppjwa.cn/gtzawhkazu.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.haohaochexian.top/gtcyyhyvfv.html

JS:   await Promise.all(tasks)
来源：http://hz.tian-w.cn/gtomgyovzb.html

TS:   await Promise.all(tasks)
来源：http://hz.yangfankeji.com/gtatimsfag.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.hywenlv.cn/gtgvzvlwbr.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.shanyushiyangtech.top/gtjrihpmiw.html

Ruby: threads.map(&:join)
来源：http://hz.cdnleiting.top/gtwzsvhysx.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.fengsongda.top/gtkeyrseox.html

[O06] 使用进程池
来源：http://hz.chenjidiqi.icu/gttlijbcvn.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.shanyushiyangkeji.top/gtlzghowvj.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.sxryk.cn/gtlaueloeb.html

JS:   // child_process / cluster 模块
来源：http://hz.shangyingyoupin.top/gtpedlsfmx.html

TS:   // child_process / cluster 模块
来源：http://hz.ywan-chungtsiang.top/gtvrsiuqew.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.sufxvd.cn/gtsgkadohg.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.wangshuangyany.cn/gtzuvwzahh.html

Ruby: // fork 块
来源：http://hz.nanxinkj.top/gtgajhrwnk.html

C#:   Parallel.For
来源：http://hz.jlsjyb.cn/gtvnosdjit.html

================================================================================
来源：http://hz.fengsongda.top/gtxavtzvrt.html

P. 常用工具函数
来源：http://hz.yongpay.top/gttqxbxvyq.html

================================================================================
来源：http://hz.cucudq.cn/gtkfzhnaqt.html

[P01] 生成 UUID
来源：http://hz.jinyuanbaomall.cn/gthmmdqzsn.html

Py:   str(uuid.uuid4())
来源：http://hz.tanke756.top/gttcgseznw.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.aibaodan.cn/gtlngdngla.html

JS:   crypto.randomUUID()
来源：http://hz.yj20258888.top/gtkvqqangs.html

TS:   crypto.randomUUID()
来源：http://hz.ywan-chungtsiang.top/gtmilwroxl.html

Java: UUID.randomUUID().toString()
来源：http://hz.9152youxi.cn/gtoegmxemn.html

Go:   // 用 github.com/google/uuid
来源：http://hz.yongpay.top/gtjitulfbd.html

Ruby: SecureRandom.uuid
来源：http://hz.wangshuangyany.cn/gtxorkfwyo.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.chenzaomai.com/gtemaceyzb.html

[P02] MD5 / SHA256 摘要
来源：http://hz.haohaochexian.top/gtcwyiassl.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.gotoacloud.top/gthsojukgh.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.pycfn.com/gtjonaxdxj.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.tanke756.top/gtynipbdwv.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.jinghuilouyu.cn/gtbhaumoyw.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.bjfxy.top/gtdtepueaz.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.jqgufenzy.top/gtmqujbhvd.html


<!-- 参考信息 -->