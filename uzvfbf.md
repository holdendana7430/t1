代发 wailian999

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.dashuyun.cn/gtyssojtuj.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.smart0.xyz/gtkcagzlvc.html

[L05] 上传文件（multipart）
来源：http://hz.shzxlz.cn/gtdenhhiwd.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.fzhhl.top/gtemqymywh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.ybcxt.top/gtqfcncahf.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.xuanzx.com/gtckqxogzt.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.sysykeji.top/gtafbjdrrw.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.sxryk.cn/gtsylhqbeq.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.pycfn.com/gtznpwhuaq.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.shanyushiyangtech.top/gtmethjhuw.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.birdmap.top/gtaazdplqb.html

[L06] 解析响应为 JSON
来源：http://hz.gaohongyu789.top/gtautqvtbg.html

Py:   resp.json()
来源：http://hz.jinyuanbaomall.cn/gtwdsfrcfi.html

PHP:  json_decode($body, true);
来源：http://hz.jqgufenzy.top/gtpquqaqaa.html

JS:   await resp.json()
来源：http://hz.cheryme.top/gtwejthhkw.html

TS:   await resp.json()
来源：http://hz.0kj1m.cn/gtdpwifewd.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.birdmap.top/gtmndytbuz.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.shangyingyoupin.top/gthcymolaa.html

Ruby: JSON.parse(resp.body)
来源：http://hz.yueranfly.top/gthpufkfbp.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.ppjwa.cn/gthbucishm.html

[L07] 处理 HTTP 状态码
来源：http://hz.yuxming.cn/gtssishbkq.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.yj20258888.top/gttdvjrenc.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.wangdashe.top/gtguyzobmj.html

JS:   resp.ok;  resp.status
来源：http://hz.yj20258.top/gthjtrircz.html

TS:   resp.ok;  resp.status
来源：http://hz.snrcjt.cn/gtierbhafe.html

Java: resp.statusCode()
来源：http://hz.yj20258888.top/gtjbfsdcms.html

Go:   resp.StatusCode
来源：http://hz.zhongyouzk.top/gtndbskytz.html

Ruby: resp.code.to_i
来源：http://hz.jinyuanbaomall.cn/gtubjwlnes.html

C#:   (int)resp.StatusCode
来源：http://hz.guannengcc.top/gtvniiwvnu.html

[L08] 并发请求多个地址
来源：http://hz.pycfn.com/gtwlrplbdp.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.yuanzhike.top/gtelfaxkpa.html

PHP:  curl_multi_init() 系列
来源：http://hz.mhx1999.top/gtqolqheug.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.c1oappe.top/gtyhapsdsp.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.dashuyun.cn/gtkkofzhrd.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.yvedp.cn/gtfxmwjhrb.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.jianghu66.top/gtcbontzwe.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.hnqzz.top/gtqmexkqiy.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.hysaishi.cn/gtfmmabmhx.html

================================================================================
来源：http://hz.chenlongwang.top/gtkfwvwndo.html

M. 命令行 / 进程 / 环境
来源：http://hz.xylfe.cn/gtxptdoxhd.html

================================================================================
来源：http://hz.cqqwz.cn/gtdmakoqzr.html

[M01] 读取命令行参数
来源：http://hz.tianlin.xyz/gtpvmtgzhz.html

Py:   sys.argv[1:]
来源：http://hz.guannengcc.top/gtcjtphxzc.html

PHP:  $argv;  $argc;
来源：http://hz.jinqigufen.top/gtalnnpybm.html

JS:   process.argv.slice(2)
来源：http://hz.quarkkingdee.top/gtjtrzydlk.html

TS:   process.argv.slice(2)
来源：http://hz.hysaishi.cn/gtwoznulmo.html

Java: args 数组（main 方法参数）
来源：http://hz.ppjwa.cn/gtnkpplqxy.html

Go:   os.Args[1:]
来源：http://hz.tianlin.xyz/gtauwactfr.html

Ruby: ARGV
来源：http://hz.jlsjyb.cn/gtfdfkrarj.html

C#:   args 数组（Main 方法参数）
来源：http://hz.zhoulong.xyz/gtxnvnqdbe.html

[M02] 读取环境变量
来源：http://hz.xziqi.cn/gtrccfhend.html

Py:   os.environ.get("HOME")
来源：http://hz.meibo888.top/gtwibaaufb.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.nanxinkj.top/gtnqtpqeto.html

JS:   process.env.HOME
来源：http://hz.yonumen.top/gtxknceznh.html

TS:   process.env.HOME
来源：http://hz.redwolf501.top/gtedymblqg.html

Java: System.getenv("HOME")
来源：http://hz.redwolf501.top/gtrfovihmi.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.jinghuilouyu.cn/gtgrzcbhcn.html

Ruby: ENV["HOME"]
来源：http://hz.xuetiantiany.cn/gtnmnpejow.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.mhx1999.top/gtjpckyegb.html

[M03] 执行外部命令
来源：http://hz.zhixingplan.top/gtxsfxeycy.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.9152youxi.cn/gtoaegouve.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.yj202588.top/gtfheqfaub.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.guowangkeji.top/gtxsvxdxci.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.sxryk.cn/gtfwykybxb.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.xuetiantiany.cn/gtdvwzrnla.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.jlsjyb.cn/gtvqixzqlo.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.zhongyouzk.top/gthlemsvbv.html

C#:   Process.Start("ls", "-l");
来源：http://hz.yj202588.top/gttyoxdxub.html

[M04] 获取当前工作目录
来源：http://hz.jinqigufen.top/gtljfrczxw.html

Py:   os.getcwd()
来源：http://hz.ydzc1.top/gtwipnvmgt.html

PHP:  getcwd();
来源：http://hz.zhixingplan.top/gttxdcnxdk.html

JS:   process.cwd()
来源：http://hz.tanke756.top/gtwesweydp.html

TS:   process.cwd()
来源：http://hz.pycfn.com/gtjgtdekga.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.jianghu66.top/gthqrbuicb.html

Go:   os.Getwd()
来源：http://hz.cqqwz.cn/gttyrrowtr.html

Ruby: Dir.pwd
来源：http://hz.vqdsnc.cn/gtojkmrxrb.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.haohaochexian.top/gthvsyhiug.html

[M05] 设置退出码
来源：http://hz.xuetiantiany.cn/gtnkqzbdlk.html

Py:   sys.exit(1)
来源：http://hz.wangdashe.top/gtjjoyweqa.html

PHP:  exit(1);
来源：http://hz.zhixingplan.top/gthfmcaoha.html

JS:   process.exit(1)
来源：http://hz.zhoulong.xyz/gtawuprcho.html

TS:   process.exit(1)
来源：http://hz.ehwqpu.com/gtnixkpolx.html

Java: System.exit(1)
来源：http://hz.bjfxy.top/gtkfzonxxl.html

Go:   os.Exit(1)
来源：http://hz.sysykeji.top/gtuxnonhxv.html

Ruby: exit 1
来源：http://hz.tanke756.top/gtcveglhau.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.jqgufenzy.top/gtswrpcpnd.html

[M06] 向标准错误输出
来源：http://hz.52xcode.cn/gtciituhnj.html

Py:   print("err", file=sys.stderr)
来源：http://hz.jinghuilouyu.cn/gttztlbpbt.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.ehwqpu.com/gtrkihellq.html

JS:   console.error("err")
来源：http://hz.hysaishi.cn/gtiradmnii.html

TS:   console.error("err")
来源：http://hz.shanyushiyangkeji.top/gtexdzlyrx.html

Java: System.err.println("err")
来源：http://hz.yanxiufei.cn/gtwvnbflxf.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.zhijiandao.cn/gtijxhwgwa.html

Ruby: warn "err"
来源：http://hz.fzhhl.top/gtskjkpwod.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.zhiwuduotai.top/gtfkmhmpao.html

[M07] 判断是否为主入口
来源：http://hz.sufxvd.cn/gtzsrnlvqj.html

Py:   if __name__ == "__main__":
来源：http://hz.zhaomingkeji.xyz/gtrldvphfz.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.jlsjyb.cn/gthcderxjz.html

JS:   require.main === module
来源：http://hz.chenzaomai.com/gtibeqnluk.html

TS:   require.main === module
来源：http://hz.tanke756.top/gtbtfjkska.html

Java: public static void main(String[] args)
来源：http://hz.chenjidiqi.icu/gthadhzgis.html

Go:   func main()
来源：http://hz.nwbrower.top/gtfitphmpr.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.hnxiangtu.top/gtpkymmlra.html

C#:   static void Main(string[] args)
来源：http://hz.jinghuilouyu.cn/gtvaeqajyx.html

[M08] 获取系统与运行时信息
来源：http://hz.dashuyun.cn/gtdbkhxwbt.html

Py:   platform.system();  platform.python_version()
来源：http://hz.snrcjt.cn/gtbgmlgvtt.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.jinqigufen.top/gtdqjnkrrb.html

JS:   process.platform;  process.version
来源：http://hz.dianchejie.cn/gtpyzmvcsh.html

TS:   process.platform;  process.version
来源：http://hz.meibo888.top/gtlinfigdp.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.svipenyu.cn/gtuovtjlbq.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.birdmap.top/gtryvoyslm.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.yj20258.top/gtpttrfqkz.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.yuxming.cn/gtfprzhllr.html

================================================================================
来源：http://hz.chenzaomai.com/gtltwhpngk.html

N. 数据结构与算法
来源：http://hz.zhiwuduotai.top/gtfxpwgcdh.html

================================================================================
来源：http://hz.jqgufenzy.top/gteiarhdar.html

[N01] 二分查找（有序数组）
来源：http://hz.aibaodan.cn/gtanjhhkvo.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.zhengqikj.top/gtfxylhifa.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.cqqwz.cn/gttgvafcos.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.cashguo.top/gtqozwqeaq.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.snrcjt.cn/gtybsimlfe.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.zhijiandao.cn/gtavcdlbzo.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.tianlin.xyz/gtiyirclpl.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.yuanzhike.top/gtpcjjzwmy.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.jianghu66.top/gtnjltvodm.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.yueranfly.top/gtwwglrfmy.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.yj20258888.top/gtjickjwop.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.shangyingyoupin.top/gtbedzzhxw.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jinghuilouyu.cn/gtthauisxa.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yj20258.top/gtspwzzcad.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.chenzaomai.com/gtpfltksbk.html

Go:   slices.Sort(arr)
来源：http://hz.ydjk.org.cn/gtpinpuybx.html

Ruby: arr.sort
来源：http://hz.zhiwuduotai.top/gtuomskmum.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.yuxming.cn/gttipwesls.html

[N03] 快速排序（分治示例）
来源：http://hz.wangdashe.top/gtfkpgabfh.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.andypj.xyz/gtelkxfxbj.html

PHP:  // 递归实现，或用 usort
来源：http://hz.9152youxi.cn/gttycbktaq.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yanxiufei.cn/gtxtikdapb.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zhengqikj.top/gtehbqfsbj.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.redwolf501.top/gticvoonpb.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.yj202588.top/gtgxzfwmun.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.hnxiangtu.top/gtvdfxljyv.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.zhoulong.xyz/gtltyfgpef.html

[N04] 斐波那契数列
来源：http://hz.sysykeji.top/gtzwhqfezf.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.hongshengwenyu.top/gtohqfsnoy.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.hnqzz.top/gtplculfph.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.bjfxy.top/gtijxyhrsn.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yvedp.cn/gttgswfoyg.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.zhoulong.xyz/gtjksvpiep.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.gaohongyu789.top/gtuhfznuwo.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.fengsongda.top/gtgxusfxkv.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.yj202588.top/gtgcaxtwbp.html

[N05] 最大公约数
来源：http://hz.52xcode.cn/gtlheahbrv.html

Py:   math.gcd(a, b)
来源：http://hz.yongpay.top/gthleikthy.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.316326.xyz/gtqrfyzjrh.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.aibaodan.cn/gtocbjhxij.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.mhx1999.top/gtfuadbfor.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.jyoumei.cn/gtsdkmfaqx.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.wangshuangyany.cn/gtzsgtvdtx.html

Ruby: a.gcd(b)
来源：http://hz.wangdashe.top/gtztqegwsk.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.tianlin.xyz/gtvmiqjcbg.html

[N06] 判断回文字符串
来源：http://hz.xinyue.icu/gtdhfprxei.html

Py:   s == s[::-1]
来源：http://hz.nanxinkj.top/gtillqcbip.html

PHP:  $s === strrev($s);
来源：http://hz.cucudq.cn/gtqiulqsxq.html

JS:   s === [...s].reverse().join("")
来源：http://hz.guowangkeji.top/gtrchttdmq.html

TS:   s === [...s].reverse().join("")
来源：http://hz.yueranfly.top/gttlmlqrbt.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.yanxiufei.cn/gtearpwwsn.html

Go:   // 双指针从两端比较
来源：http://hz.pengpengdd.cyou/gtfhxblcna.html

Ruby: s == s.reverse
来源：http://hz.aizwys.cn/gttxnsfuzn.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.shangyingyoupin.top/gtcmuszgih.html

[N07] 两数之和（返回下标）
来源：http://hz.dianchejie.cn/gtnovykjlw.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.sysykeji.top/gtqrqpwyen.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.jiagoushi.top/gtutsschqw.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.jlsjyb.cn/gtbjwskrye.html

TS:   // 手写 Map<string, number>
来源：http://hz.zhixingplan.top/gtcuknqjmj.html

Java: // 手写 HashMap
来源：http://hz.chenlongwang.top/gtycsvxpql.html

Go:   // 手写 map[int]int
来源：http://hz.chenlongwang.top/gtyoxgplfn.html

Ruby: // 手写 Hash
来源：http://hz.fengsongda.top/gtwjmeknzj.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.shangyingyoupin.top/gtlegcxhuo.html

[N08] 生成全排列
来源：http://hz.daria6918.cn/gtwvgnyilu.html

Py:   itertools.permutations(arr)
来源：http://hz.jinyuanbaomall.cn/gtxoacrrpu.html

PHP:  // 手写递归交换
来源：http://hz.hammf.cn/gtjkutzccc.html

JS:   // 手写回溯递归
来源：http://hz.aibaodan.cn/gtirbukbdd.html

TS:   // 手写回溯递归
来源：http://hz.sxryk.cn/gthpdmwgki.html

Java: // 手写回溯递归
来源：http://hz.shanyushiyangkeji.top/gtzqapygwg.html

Go:   // 手写回溯递归
来源：http://hz.xziqi.cn/gtkfrvsuwl.html

Ruby: arr.permutation.to_a
来源：http://hz.bjfxy.top/gtvvjnchyc.html

C#:   // 手写回溯递归
来源：http://hz.hnxiangtu.top/gtpysbeppi.html

[N09] 栈与队列
来源：http://hz.0kj1m.cn/gtebxrgqry.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.zhongyouzk.top/gtvitixwtn.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.iojbl.cn/gtvqzawyxe.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.316326.xyz/gtabaslbom.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.yueranfly.top/gtboaxnmos.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.hysaishi.cn/gtclwqxlhj.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.yanxiufei.cn/gttmzhboej.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.iojbl.cn/gtfoasraka.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.guannengcc.top/gtmyemefxx.html

[N10] 链表节点定义
来源：http://hz.redwolf501.top/gtqdxkqoks.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.guowangkeji.top/gtsdjdutkb.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.tanke756.top/gtvirrrdxz.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.jianghu66.top/gtefaylure.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.aibaodan.cn/gtuagyjbai.html

Java: class Node { int v; Node next; }
来源：http://hz.xziqi.cn/gttbgseyqn.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.birdmap.top/gtoysdxaas.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.zycfv.cn/gtuejjanom.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.cheryme.top/gtvlewmnnz.html

[N11] 二叉树中序遍历
来源：http://hz.yvedp.cn/gtvmcnqvqz.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.jinqigfzy.top/gtnsgyqyfn.html

PHP:  // 手写递归函数
来源：http://hz.tanke756.top/gtorjeaecl.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.hfpthk.cn/gtpqrpxojj.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.xingfuxueyuan.xyz/gtshrsqini.html

Java: // 手写递归
来源：http://hz.jqgufenzy.top/gtsgavvxmk.html

Go:   // 手写递归
来源：http://hz.shanyushiyangtech.top/gtbmuckhbh.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.nanxinkj.top/gtyedhuijc.html

C#:   // 手写递归
来源：http://hz.ywan-chungtsiang.top/gtgzaetfmf.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.cucudq.cn/gtyfwdwcto.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.c1oappe.top/gttsawoqtv.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.52xcode.cn/gtzhwlijoc.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yvedp.cn/gtbqlejylz.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.hywenlv.cn/gtlqtulrtv.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.sxryk.cn/gtmvwbbuvf.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.ybcxt.top/gtonoqhtkr.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.chenzaomai.com/gtrsnflnoz.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yvedp.cn/gtvkbijhll.html

================================================================================
来源：http://hz.sxryk.cn/gtoberiqgy.html

O. 并发与异步
来源：http://hz.xziqi.cn/gtctuapjmf.html

================================================================================
来源：http://hz.zycfv.cn/gtzqcmngon.html

[O01] 启动一个线程
来源：http://hz.nanxuanxn.top/gtbsawvviu.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.jinyuanbaomall.cn/gtxydxyhkv.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.nanxinkj.top/gtxknbhtha.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.cashguo.top/gtialstpot.html

TS:   // 同 JS
来源：http://hz.jinqigfzy.top/gtirfqspct.html

Java: new Thread(() -> f()).start()
来源：http://hz.yj202588.top/gtkwkynegn.html

Go:   go f()
来源：http://hz.aibaodan.cn/gtilznidqa.html

Ruby: Thread.new { f }
来源：http://hz.haohaochexian.top/gttxlckwwf.html

C#:   Task.Run(() => F());
来源：http://hz.yuxming.cn/gtsrfkjgyi.html

[O02] 使用线程池
来源：http://hz.svipenyu.cn/gtxijezdnx.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.bjfxy.top/gtesghchcc.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.hnqzz.top/gtdxeqgurv.html

JS:   // worker_threads 线程池
来源：http://hz.jinqigufen.top/gtbqfqlxql.html

TS:   // worker_threads 线程池
来源：http://hz.ivvv.top/gtcfcrvhif.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.tanke756.top/gtwltigvzp.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.bjfxy.top/gtwyamhyiq.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.hammf.cn/gthpcdnodf.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.meibo888.top/gtkezibwek.html

[O03] 加锁保护共享数据
来源：http://hz.316326.xyz/gtflcuveus.html

Py:   with lock: shared += 1
来源：http://hz.cqqwz.cn/gtnipnmwjx.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.yj20258.top/gtpazrduic.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.yueranfly.top/gttlacjyvk.html

TS:   // 同 JS
来源：http://hz.xziqi.cn/gtzjfywqsd.html

Java: synchronized (this) { shared++; }
来源：http://hz.zhengqikj.top/gtkdtlhrkq.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.c1oappe.top/gtqsvpijya.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.havefunace.top/gtvbxvscqw.html

C#:   lock (gate) { shared++; }
来源：http://hz.yj202588.top/gtvvqekzef.html

[O04] 定义异步函数并等待
来源：http://hz.jinqigufen.top/gthwaxnjck.html

Py:   async def f():⏎    await g()
来源：http://hz.daxiang520.top/gtgfsjckwm.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.316326.xyz/gtloeltoqd.html

JS:   async function f() { await g(); }
来源：http://hz.zdqjudy.top/gtapsybcfd.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.ivvv.top/gtpkppkaso.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.nanxinkj.top/gtaciukybp.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.hywenlv.cn/gteoedrbxr.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.tian-w.cn/gtyprtamjl.html

C#:   async Task F() { await G(); }
来源：http://hz.jlsjyb.cn/gtzdlfnuxa.html

[O05] 并发执行并等待全部完成
来源：http://hz.jinghuilouyu.cn/gtscoemrec.html

Py:   asyncio.gather(*tasks)
来源：http://hz.sxryk.cn/gtwfphvmsv.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.dianchejie.cn/gtxeplqapc.html

JS:   await Promise.all(tasks)
来源：http://hz.shuidangran.top/gtqaoohdzb.html

TS:   await Promise.all(tasks)
来源：http://hz.zdqjudy.top/gtsmacmpva.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.gzhubu.top/gtorpysuhd.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.zhijiandao.cn/gtlanmbzki.html

Ruby: threads.map(&:join)
来源：http://hz.sufxvd.cn/gtsvhtqadj.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.xuanzx.com/gthznqvdtn.html

[O06] 使用进程池
来源：http://hz.daxiang520.top/gtynguivpr.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.shzxlz.cn/gtcmjitdja.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.fzhhl.top/gttgxbhyis.html

JS:   // child_process / cluster 模块
来源：http://hz.cheryme.top/gtzqkkrcfs.html

TS:   // child_process / cluster 模块
来源：http://hz.gogol.net.cn/gtmbmyygvv.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.yongpay.top/gtwngizukq.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.zhaomingkeji.xyz/gtrxrjkbpk.html

Ruby: // fork 块
来源：http://hz.shangyingyoupin.top/gtmkdnpbya.html

C#:   Parallel.For
来源：http://hz.quarkkingdee.top/gthwmcovfz.html

================================================================================
来源：http://hz.zhijiandao.cn/gthssowzhy.html

P. 常用工具函数
来源：http://hz.yanxiufei.cn/gtqdldtghq.html

================================================================================
来源：http://hz.c1oappe.top/gtxyqgovzw.html

[P01] 生成 UUID
来源：http://hz.tianlin.xyz/gtwdozpkkd.html

Py:   str(uuid.uuid4())
来源：http://hz.316326.xyz/gtiqcpucpe.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.zdqjudy.top/gttbvckefq.html

JS:   crypto.randomUUID()
来源：http://hz.cheryme.top/gtuqaccbka.html

TS:   crypto.randomUUID()
来源：http://hz.haohaochexian.top/gtiyrztltt.html

Java: UUID.randomUUID().toString()
来源：http://hz.aibaodan.cn/gtvzfsplwb.html

Go:   // 用 github.com/google/uuid
来源：http://hz.yj202588.top/gtfhsrjnck.html

Ruby: SecureRandom.uuid
来源：http://hz.smart0.xyz/gtmwosbgvm.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.xylfe.cn/gttetweehx.html

[P02] MD5 / SHA256 摘要
来源：http://hz.zdqjudy.top/gtmasnuzit.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.xylfe.cn/gtwlayhago.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.jqgfzy.top/gtovbrkfuc.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.52xcode.cn/gthlhzzyvv.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.aizwys.cn/gtpabxqzmq.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.yanxiufei.cn/gtwixrlujo.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.zycfv.cn/gthnvkrsde.html


<!-- 参考信息 -->