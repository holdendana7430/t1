代发 wailian999

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.ppjwa.cn/gtoodcicoe.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.ppjwa.cn/gtabxxewct.html

[L05] 上传文件（multipart）
来源：http://hz.xuanzx.com/gtpzbiuywl.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.ivvv.top/gtbpfxnjgl.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.316326.xyz/gtmxammpik.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.ehwqpu.com/gtmbedyqey.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.hammf.cn/gtmrcriepp.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.haohaochexian.top/gtcdnpgnnq.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.iojbl.cn/gtyxyzztmm.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.cheryme.top/gthlfmvwol.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.c1oappe.top/gtcenfgadh.html

[L06] 解析响应为 JSON
来源：http://hz.9152youxi.cn/gtgvmikrvc.html

Py:   resp.json()
来源：http://hz.yj202588.top/gtkegvbgzn.html

PHP:  json_decode($body, true);
来源：http://hz.wangshuangyany.cn/gtxwwjshpv.html

JS:   await resp.json()
来源：http://hz.ivvv.top/gtmfvvibzs.html

TS:   await resp.json()
来源：http://hz.jinghuilouyu.cn/gtvobqqfma.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.xuanzx.com/gtbpfycmal.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.jinyuanbaomall.cn/gtzeeptigy.html

Ruby: JSON.parse(resp.body)
来源：http://hz.ybcxt.top/gtnqywuqzh.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.zhijiandao.cn/gtmykoqqbp.html

[L07] 处理 HTTP 状态码
来源：http://hz.cqqwz.cn/gttiqbglam.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.nanxinkj.top/gtnfocwail.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.meibo888.top/gtwktmgrae.html

JS:   resp.ok;  resp.status
来源：http://hz.fzhhl.top/gtfrxolnrj.html

TS:   resp.ok;  resp.status
来源：http://hz.cucudq.cn/gtnvcpyzzy.html

Java: resp.statusCode()
来源：http://hz.jinqigufen.top/gtxhzvhwlf.html

Go:   resp.StatusCode
来源：http://hz.havefunace.top/gtgazufrhf.html

Ruby: resp.code.to_i
来源：http://hz.dianchejie.cn/gtquqexbdi.html

C#:   (int)resp.StatusCode
来源：http://hz.jinqigufen.top/gtgafqieer.html

[L08] 并发请求多个地址
来源：http://hz.zdqjudy.top/gtvvqabfxc.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.dianchejie.cn/gtzzrgwmsz.html

PHP:  curl_multi_init() 系列
来源：http://hz.jinqigufen.top/gthutjkofc.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.tianlin.xyz/gtmovlfljy.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.redwolf501.top/gtehteimnn.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.ybcxt.top/gthfcbzkny.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.guowangkeji.top/gttgqwhemq.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.quarkkingdee.top/gtjlshiuhy.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.zdqjudy.top/gtaqbvlqzb.html

================================================================================
来源：http://hz.zdqjudy.top/gttcalrpxc.html

M. 命令行 / 进程 / 环境
来源：http://hz.zhixingplan.top/gtzxvvbsfm.html

================================================================================
来源：http://hz.tian-w.cn/gtknpivqio.html

[M01] 读取命令行参数
来源：http://hz.yj20258888.top/gtdwmysedq.html

Py:   sys.argv[1:]
来源：http://hz.tian-w.cn/gtcwwxrcjd.html

PHP:  $argv;  $argc;
来源：http://hz.wangshuangyany.cn/gtbpwpyseb.html

JS:   process.argv.slice(2)
来源：http://hz.ehwqpu.com/gtlkiqizyi.html

TS:   process.argv.slice(2)
来源：http://hz.gzhubu.top/gtxjpmraij.html

Java: args 数组（main 方法参数）
来源：http://hz.havefunace.top/gtdklyubnj.html

Go:   os.Args[1:]
来源：http://hz.feifeiyinyue.top/gtnfackhog.html

Ruby: ARGV
来源：http://hz.chenzaomai.com/gtcdxmyplr.html

C#:   args 数组（Main 方法参数）
来源：http://hz.zdqjudy.top/gtsxybkweu.html

[M02] 读取环境变量
来源：http://hz.pengpengdd.cyou/gtxqnqktxe.html

Py:   os.environ.get("HOME")
来源：http://hz.havefunace.top/gtlaggzhhb.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.sysykeji.top/gtixldtgbd.html

JS:   process.env.HOME
来源：http://hz.dashuyun.cn/gtrzwpmzmm.html

TS:   process.env.HOME
来源：http://hz.hfpthk.cn/gtwasyaffa.html

Java: System.getenv("HOME")
来源：http://hz.jianghu66.top/gtfmvfojth.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.hongshengwenyu.top/gtrtxvydfg.html

Ruby: ENV["HOME"]
来源：http://hz.snrcjt.cn/gttshhqicb.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.wangdashe.top/gtqjmayjay.html

[M03] 执行外部命令
来源：http://hz.zhaomingkeji.xyz/gtyluryhwz.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.shzxlz.cn/gtihgzocps.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.yonumen.top/gtybhjdkep.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.quarkkingdee.top/gtykuezfbz.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.sufxvd.cn/gtzgejgrdu.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.jianghu66.top/gtxveisive.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.pycfn.com/gtimmkuabi.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.ppjwa.cn/gtiijvpyzz.html

C#:   Process.Start("ls", "-l");
来源：http://hz.bjfxy.top/gtirkwsdfd.html

[M04] 获取当前工作目录
来源：http://hz.cqqwz.cn/gthiwyzbkb.html

Py:   os.getcwd()
来源：http://hz.zhiwuduotai.top/gtjmznqsxk.html

PHP:  getcwd();
来源：http://hz.9152youxi.cn/gtrgwxwfzo.html

JS:   process.cwd()
来源：http://hz.jinyuanbaomall.cn/gtlrqodvdj.html

TS:   process.cwd()
来源：http://hz.yongpay.top/gtrffbhalm.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.wangdashe.top/gtyopqnppy.html

Go:   os.Getwd()
来源：http://hz.kuanghao11.cn/gtuakaerte.html

Ruby: Dir.pwd
来源：http://hz.jiagoushi.top/gttxizuvry.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.yongpay.top/gtsufsptgv.html

[M05] 设置退出码
来源：http://hz.tanke756.top/gtpavrvefq.html

Py:   sys.exit(1)
来源：http://hz.zhongyouzk.top/gttedossdi.html

PHP:  exit(1);
来源：http://hz.hywenlv.cn/gtguqfndbf.html

JS:   process.exit(1)
来源：http://hz.hysaishi.cn/gtpbidpboh.html

TS:   process.exit(1)
来源：http://hz.jlsjyb.cn/gttfkiwbop.html

Java: System.exit(1)
来源：http://hz.wangshuangyany.cn/gtlygtkvfc.html

Go:   os.Exit(1)
来源：http://hz.gogol.net.cn/gttqnkewub.html

Ruby: exit 1
来源：http://hz.yj20258.top/gtzsrdnayy.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.aibaodan.cn/gtwgfeqwaa.html

[M06] 向标准错误输出
来源：http://hz.jqgfzy.top/gtwjcrrzqa.html

Py:   print("err", file=sys.stderr)
来源：http://hz.fengsongda.top/gtkamonalu.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.yonumen.top/gtmuonnvbk.html

JS:   console.error("err")
来源：http://hz.0kj1m.cn/gtdhelvkel.html

TS:   console.error("err")
来源：http://hz.0kj1m.cn/gtcrrjxnbg.html

Java: System.err.println("err")
来源：http://hz.gaohongyu789.top/gttghzyhfu.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.hnxiangtu.top/gtomofzryj.html

Ruby: warn "err"
来源：http://hz.shangyingyoupin.top/gtivvbgigr.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.yj20258888.top/gtqkcdyfck.html

[M07] 判断是否为主入口
来源：http://hz.sufxvd.cn/gtexgvwpqo.html

Py:   if __name__ == "__main__":
来源：http://hz.jinyuanbaomall.cn/gtziapmsge.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.dianchejie.cn/gtbdnhnjqt.html

JS:   require.main === module
来源：http://hz.andypj.xyz/gtkssdiivk.html

TS:   require.main === module
来源：http://hz.yvedp.cn/gtpnlpcqvd.html

Java: public static void main(String[] args)
来源：http://hz.dashuyun.cn/gtyilihuqn.html

Go:   func main()
来源：http://hz.jinqigufen.top/gtammgjjwm.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.cheryme.top/gtqrjucmzw.html

C#:   static void Main(string[] args)
来源：http://hz.cdnleiting.top/gtsttcrtpt.html

[M08] 获取系统与运行时信息
来源：http://hz.yj20258.top/gtrakagedw.html

Py:   platform.system();  platform.python_version()
来源：http://hz.snrcjt.cn/gtwarnrkwp.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.ybcxt.top/gtvkrdxghj.html

JS:   process.platform;  process.version
来源：http://hz.ehwqpu.com/gtsatknssn.html

TS:   process.platform;  process.version
来源：http://hz.yj20258.top/gtzntyuqvj.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.xuanzx.com/gtvdbxpvft.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.snrcjt.cn/gtippmqjdm.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.zhongyouzk.top/gtajdczynj.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.jinghuilouyu.cn/gtuwnzzcas.html

================================================================================
来源：http://hz.fzhhl.top/gtmostkuws.html

N. 数据结构与算法
来源：http://hz.pengpengdd.cyou/gtbynrfcvo.html

================================================================================
来源：http://hz.cdnleiting.top/gtehwqyohr.html

[N01] 二分查找（有序数组）
来源：http://hz.aibaodan.cn/gtuxdzhpgp.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.daxiang520.top/gtarkvolnu.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.yonumen.top/gttxmuyhih.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.316326.xyz/gttprpftpe.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.cdnleiting.top/gthugkwbbr.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.gzhubu.top/gtrymjxlik.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.quarkkingdee.top/gtfwxkyacs.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.kuanghao11.cn/gtjhhsaoyj.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.hysaishi.cn/gtkbxdaqte.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.aizwys.cn/gtxdpmlpqb.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.smart0.xyz/gtpqvwsgzd.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.jinghuilouyu.cn/gtnfekqzqo.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.316326.xyz/gtczpbnqfe.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.cheryme.top/gttgbpwwia.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.yj202588.top/gtexzsgzfs.html

Go:   slices.Sort(arr)
来源：http://hz.hnxiangtu.top/gtftvsnnfn.html

Ruby: arr.sort
来源：http://hz.guowangkeji.top/gthtocuzca.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.bjfxy.top/gtukixhtuk.html

[N03] 快速排序（分治示例）
来源：http://hz.vqdsnc.cn/gtbycetszu.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.hnqzz.top/gturlzaczc.html

PHP:  // 递归实现，或用 usort
来源：http://hz.bjfxy.top/gtnxgivotq.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.birdmap.top/gtqeaydapq.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jinqigufen.top/gtdztoorut.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.gotoacloud.top/gteqpxqxjr.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.svipenyu.cn/gtuipmxtjy.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.jinyuanbaomall.cn/gtgykdtuhu.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.snrcjt.cn/gtrfehdvli.html

[N04] 斐波那契数列
来源：http://hz.chenzaomai.com/gtabqpizbs.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.shanyushiyangtech.top/gtyfvnvntj.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.jlsjyb.cn/gtfdysrntn.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.shzxlz.cn/gtbfaqqnwg.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.snrcjt.cn/gtuxzrcdfz.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.316326.xyz/gtuufftvcx.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.zycfv.cn/gtlmhjjvpl.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.yuanzhike.top/gtffdowdtr.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.sufxvd.cn/gtldpfzrga.html

[N05] 最大公约数
来源：http://hz.snrcjt.cn/gtembymfwv.html

Py:   math.gcd(a, b)
来源：http://hz.jqgufenzy.top/gtatqzvmhd.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.xziqi.cn/gtuejlfsnh.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.aizwys.cn/gttklunzzn.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yuanzhike.top/gtjeztgztk.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.cucudq.cn/gtwlfxuxfl.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.zdqjudy.top/gtfsnqduxn.html

Ruby: a.gcd(b)
来源：http://hz.hysaishi.cn/gthxmbvcmw.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.yuanzhike.top/gtuebqoelo.html

[N06] 判断回文字符串
来源：http://hz.hfpthk.cn/gtxehvsssk.html

Py:   s == s[::-1]
来源：http://hz.zdqjudy.top/gtcsnfgwyn.html

PHP:  $s === strrev($s);
来源：http://hz.yongpay.top/gtzyqywjpr.html

JS:   s === [...s].reverse().join("")
来源：http://hz.zhongyouzk.top/gtlzpaaxqy.html

TS:   s === [...s].reverse().join("")
来源：http://hz.daria6918.cn/gttsyjzabr.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.chenlongwang.top/gteunirioh.html

Go:   // 双指针从两端比较
来源：http://hz.yongpay.top/gtmbisvgrt.html

Ruby: s == s.reverse
来源：http://hz.hammf.cn/gtfjswhesw.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.0kj1m.cn/gtbcsvsytw.html

[N07] 两数之和（返回下标）
来源：http://hz.xingfuxueyuan.xyz/gtjmulleqd.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.feifeiyinyue.top/gtsoyzaonk.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.iojbl.cn/gttfcduixt.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.jinqigufen.top/gtofqhksxq.html

TS:   // 手写 Map<string, number>
来源：http://hz.hywenlv.cn/gthxwlvyut.html

Java: // 手写 HashMap
来源：http://hz.iojbl.cn/gtcxhvskoe.html

Go:   // 手写 map[int]int
来源：http://hz.52xcode.cn/gthuewmkme.html

Ruby: // 手写 Hash
来源：http://hz.dianchejie.cn/gtbxggptzs.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.jqgufenzy.top/gtqckdjapn.html

[N08] 生成全排列
来源：http://hz.ydzc1.top/gtqhwvuubo.html

Py:   itertools.permutations(arr)
来源：http://hz.cheryme.top/gtkdkzixqb.html

PHP:  // 手写递归交换
来源：http://hz.redwolf501.top/gtbcukvihj.html

JS:   // 手写回溯递归
来源：http://hz.jinyuanbaomall.cn/gtfokwjbjf.html

TS:   // 手写回溯递归
来源：http://hz.shanyushiyangtech.top/gtisdebygd.html

Java: // 手写回溯递归
来源：http://hz.9152youxi.cn/gtyixsddkj.html

Go:   // 手写回溯递归
来源：http://hz.shuidangran.top/gtmhyknpvf.html

Ruby: arr.permutation.to_a
来源：http://hz.shzxlz.cn/gtislatrod.html

C#:   // 手写回溯递归
来源：http://hz.iojbl.cn/gttollojsx.html

[N09] 栈与队列
来源：http://hz.chenlongwang.top/gtspqclrav.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.jinqigufen.top/gtyodfkucg.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.shanyushiyangkeji.top/gtoodmqyeg.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.feifeiyinyue.top/gtcpgytefw.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.tanke756.top/gtxriwoycx.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.zycfv.cn/gtzykjikgp.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.mhx1999.top/gtsyzwlztk.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.chenlongwang.top/gtfmwyqwdg.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.ydzc1.top/gtkcjsjecu.html

[N10] 链表节点定义
来源：http://hz.mhx1999.top/gtirmojggy.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.zhijiandao.cn/gtptlahkrq.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.cdnleiting.top/gtxailkchl.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.jlsjyb.cn/gtilysalwu.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.yanxiufei.cn/gtdfbnyfwz.html

Java: class Node { int v; Node next; }
来源：http://hz.yonumen.top/gtsaxvpiua.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.hywenlv.cn/gtnntbyyov.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.shanyushiyangtech.top/gtsjqffuiw.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.gaohongyu789.top/gtqpjlvhhu.html

[N11] 二叉树中序遍历
来源：http://hz.gogol.net.cn/gtwaulkzhq.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.cashguo.top/gtbfagzcqz.html

PHP:  // 手写递归函数
来源：http://hz.yonumen.top/gtlzkircbj.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.cashguo.top/gtdwvswdmv.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.fengsongda.top/gtdyeezjzz.html

Java: // 手写递归
来源：http://hz.yanxiufei.cn/gtiiacuobu.html

Go:   // 手写递归
来源：http://hz.mhx1999.top/gtxnwxqsle.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.yj20258888.top/gtzouumsuc.html

C#:   // 手写递归
来源：http://hz.aizwys.cn/gtwplnodge.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.xingfuxueyuan.xyz/gtnwjieqrp.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.zhengqikj.top/gtnhdcnzkd.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.hnqzz.top/gtrxbjxcya.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.ydjk.org.cn/gtjkkipoqx.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.wangshuangyany.cn/gtankdkgeq.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.jyoumei.cn/gtahojxgnb.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.hnqzz.top/gtraakphil.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.nwbrower.top/gtxiwwnxrr.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.wangshuangyany.cn/gtxadmeeqs.html

================================================================================
来源：http://hz.gogol.net.cn/gtbynnzdut.html

O. 并发与异步
来源：http://hz.dianchejie.cn/gtqraofnyr.html

================================================================================
来源：http://hz.jyoumei.cn/gtatwgwcjn.html

[O01] 启动一个线程
来源：http://hz.yueranfly.top/gtrvrghkgc.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.havefunace.top/gtesvdprdp.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.zhaomingkeji.xyz/gttjcpntre.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.zhengqikj.top/gtvelvpjhk.html

TS:   // 同 JS
来源：http://hz.tian-w.cn/gttynwrzfi.html

Java: new Thread(() -> f()).start()
来源：http://hz.316326.xyz/gtnqclkpvp.html

Go:   go f()
来源：http://hz.chenzaomai.com/gtaryohbph.html

Ruby: Thread.new { f }
来源：http://hz.zhongyouzk.top/gtegdtpsty.html

C#:   Task.Run(() => F());
来源：http://hz.tanke756.top/gtegzjtccq.html

[O02] 使用线程池
来源：http://hz.cqqwz.cn/gtfljjgvlz.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.hfpthk.cn/gtjkwvqcpl.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.ehwqpu.com/gthbesgmjw.html

JS:   // worker_threads 线程池
来源：http://hz.jyoumei.cn/gtvyxdpfja.html

TS:   // worker_threads 线程池
来源：http://hz.xylfe.cn/gtobghkjjo.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.bjfxy.top/gtjorchktd.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.xuanzx.com/gtwdsqxcsb.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.cqqwz.cn/gtiqubxlct.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.hfpthk.cn/gtcfcerwhy.html

[O03] 加锁保护共享数据
来源：http://hz.pengpengdd.cyou/gtwqwldmid.html

Py:   with lock: shared += 1
来源：http://hz.zhaomingkeji.xyz/gtfvgxzgyp.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.sysykeji.top/gtszhhkccs.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.fengsongda.top/gtetwcrcvc.html

TS:   // 同 JS
来源：http://hz.svipenyu.cn/gtnwlzoebk.html

Java: synchronized (this) { shared++; }
来源：http://hz.svipenyu.cn/gttggagfrw.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.shangyingyoupin.top/gtemrcnbzo.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.daria6918.cn/gtmqrbkcfv.html

C#:   lock (gate) { shared++; }
来源：http://hz.iojbl.cn/gtpvoumvvp.html

[O04] 定义异步函数并等待
来源：http://hz.jqgufenzy.top/gtyuqrrvgo.html

Py:   async def f():⏎    await g()
来源：http://hz.cqqwz.cn/gtrriuzwni.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.shangyingyoupin.top/gtpqkqffta.html

JS:   async function f() { await g(); }
来源：http://hz.zhiwuduotai.top/gtwaqqpwnb.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.tianlin.xyz/gtflafwbcq.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.chenzaomai.com/gtotmkogzt.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.c1oappe.top/gtlkpviaeq.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.52xcode.cn/gtcionopit.html

C#:   async Task F() { await G(); }
来源：http://hz.jinqigufen.top/gtdrvwxlea.html

[O05] 并发执行并等待全部完成
来源：http://hz.c1oappe.top/gtkzfvyonp.html

Py:   asyncio.gather(*tasks)
来源：http://hz.jqgfzy.top/gtmvudndlr.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.gotoacloud.top/gtftnmicad.html

JS:   await Promise.all(tasks)
来源：http://hz.cashguo.top/gtuwjtrafm.html

TS:   await Promise.all(tasks)
来源：http://hz.xylfe.cn/gtyvfvjtxx.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.hongshengwenyu.top/gtxdntzerx.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.dianchejie.cn/gtvljpotrf.html

Ruby: threads.map(&:join)
来源：http://hz.zhixingplan.top/gtpsljrixl.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.zycfv.cn/gtzgsdleel.html

[O06] 使用进程池
来源：http://hz.yj202588.top/gtenjvzdbp.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.meibo888.top/gtybeicvgp.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.jiagoushi.top/gtxhafhotm.html

JS:   // child_process / cluster 模块
来源：http://hz.svipenyu.cn/gtjarjoedt.html

TS:   // child_process / cluster 模块
来源：http://hz.xylfe.cn/gtesnpcvob.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.yangfankeji.com/gtnoeelkow.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.yj20258.top/gtzcsmrijo.html

Ruby: // fork 块
来源：http://hz.zdqjudy.top/gtzwebfqzc.html

C#:   Parallel.For
来源：http://hz.smart0.xyz/gterdtbmug.html

================================================================================
来源：http://hz.chenlongwang.top/gtuwxqugsu.html

P. 常用工具函数
来源：http://hz.cqqwz.cn/gtytsmkisf.html

================================================================================
来源：http://hz.chenlongwang.top/gteczqnydn.html

[P01] 生成 UUID
来源：http://hz.cashguo.top/gtcfrdbokl.html

Py:   str(uuid.uuid4())
来源：http://hz.mhx1999.top/gtugioboro.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.xylfe.cn/gtzujgwvvl.html

JS:   crypto.randomUUID()
来源：http://hz.hnxiangtu.top/gtypwazgms.html

TS:   crypto.randomUUID()
来源：http://hz.shangyingyoupin.top/gtitybhntl.html

Java: UUID.randomUUID().toString()
来源：http://hz.daxiang520.top/gtylgfhjih.html

Go:   // 用 github.com/google/uuid
来源：http://hz.zhaomingkeji.xyz/gtmbnutgez.html

Ruby: SecureRandom.uuid
来源：http://hz.cashguo.top/gtgcgweqxl.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.316326.xyz/gtyoyfdwhx.html

[P02] MD5 / SHA256 摘要
来源：http://hz.smart0.xyz/gtbkctchyo.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.52xcode.cn/gtsmshvrwj.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.yangfankeji.com/gtrudztmkv.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.wangshuangyany.cn/gtruwoatmd.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.gzhubu.top/gtnzwtlnrv.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.yvedp.cn/gtacivflru.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.kuanghao11.cn/gtbdquvjap.html


<!-- 参考信息 -->