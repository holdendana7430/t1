代发 wailian999

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.yj20258888.top/gtutatirdj.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.yongpay.top/gtjstrsrir.html

[L05] 上传文件（multipart）
来源：http://hz.cheryme.top/gtnhhcrnbb.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.tianlin.xyz/gtjneipqmc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.yanxiufei.cn/gtlvahyejw.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.jinghuilouyu.cn/gtqooaklxy.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.yvedp.cn/gteifeupvm.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.xziqi.cn/gtulsyieeb.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.fengsongda.top/gtrgncvtrl.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.jqgufenzy.top/gttkgzcgct.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.zhoulong.xyz/gtbmkzcxgr.html

[L06] 解析响应为 JSON
来源：http://hz.xuanzx.com/gtnudeqflv.html

Py:   resp.json()
来源：http://hz.meibo888.top/gtqrwdysdl.html

PHP:  json_decode($body, true);
来源：http://hz.jinqigufen.top/gtavapkudj.html

JS:   await resp.json()
来源：http://hz.guowangkeji.top/gtaylfrttq.html

TS:   await resp.json()
来源：http://hz.hysaishi.cn/gtnsgspysw.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.nanxinkj.top/gtmrpwbvbu.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.haohaochexian.top/gtxrjsdtbb.html

Ruby: JSON.parse(resp.body)
来源：http://hz.xinyue.icu/gthrhhocrf.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.yj20258888.top/gtsdvsgidr.html

[L07] 处理 HTTP 状态码
来源：http://hz.svipenyu.cn/gtgrtxjagb.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.guowangkeji.top/gtqarhswwr.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.hysaishi.cn/gtfjohhwgu.html

JS:   resp.ok;  resp.status
来源：http://hz.gaohongyu789.top/gtliwkyyqp.html

TS:   resp.ok;  resp.status
来源：http://hz.gotoacloud.top/gteownngyy.html

Java: resp.statusCode()
来源：http://hz.shangyingyoupin.top/gtrykudwmv.html

Go:   resp.StatusCode
来源：http://hz.xylfe.cn/gtysevkaim.html

Ruby: resp.code.to_i
来源：http://hz.ydzc1.top/gthwsypsxi.html

C#:   (int)resp.StatusCode
来源：http://hz.zhixingplan.top/gtaryeiyut.html

[L08] 并发请求多个地址
来源：http://hz.jlsjyb.cn/gtddaijoig.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.guannengcc.top/gtcocdtvmm.html

PHP:  curl_multi_init() 系列
来源：http://hz.tanke756.top/gtnbcgyezi.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.gzhubu.top/gtwcediqge.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.hfpthk.cn/gtqrnpnbtz.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.jinqigufen.top/gtnyyzpbjj.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.daxiang520.top/gtwdzuboch.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.sysykeji.top/gtpsgxoilo.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.jqgfzy.top/gtbsbxnhql.html

================================================================================
来源：http://hz.mhx1999.top/gtiuaeoidw.html

M. 命令行 / 进程 / 环境
来源：http://hz.daria6918.cn/gtxbcbeuti.html

================================================================================
来源：http://hz.tianlin.xyz/gtgbudaivx.html

[M01] 读取命令行参数
来源：http://hz.yj20258888.top/gtxmavvkmt.html

Py:   sys.argv[1:]
来源：http://hz.haohaochexian.top/gtoynwteyt.html

PHP:  $argv;  $argc;
来源：http://hz.quarkkingdee.top/gtvwoeyfwc.html

JS:   process.argv.slice(2)
来源：http://hz.ivvv.top/gtmorgpijs.html

TS:   process.argv.slice(2)
来源：http://hz.hywenlv.cn/gtnhgrshtb.html

Java: args 数组（main 方法参数）
来源：http://hz.zhengqikj.top/gttszjvrvo.html

Go:   os.Args[1:]
来源：http://hz.ydjk.org.cn/gtotcbyadg.html

Ruby: ARGV
来源：http://hz.ydzc1.top/gtdthsoypb.html

C#:   args 数组（Main 方法参数）
来源：http://hz.ivvv.top/gtbzuewiqx.html

[M02] 读取环境变量
来源：http://hz.sysykeji.top/gtxkjcypmp.html

Py:   os.environ.get("HOME")
来源：http://hz.sweek.top/gtgjimjbta.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.xziqi.cn/gtfkhwaynb.html

JS:   process.env.HOME
来源：http://hz.haohaochexian.top/gtgtfagwlt.html

TS:   process.env.HOME
来源：http://hz.ivvv.top/gtpgufklto.html

Java: System.getenv("HOME")
来源：http://hz.ehwqpu.com/gtmjofpaep.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.nwbrower.top/gtocnbpvdw.html

Ruby: ENV["HOME"]
来源：http://hz.shuidangran.top/gtxhbllyvb.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.zhijiandao.cn/gtxwoxicwt.html

[M03] 执行外部命令
来源：http://hz.jqgfzy.top/gtolnuufdf.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.jqgufenzy.top/gtqwwdksvw.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.shangyingyoupin.top/gtzajvnddq.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.jinqigfzy.top/gtzlxzmokh.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.sufxvd.cn/gtrrglwzig.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.jyoumei.cn/gtfofgtgne.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.hywenlv.cn/gtvvkffwxm.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.0kj1m.cn/gtddpvduub.html

C#:   Process.Start("ls", "-l");
来源：http://hz.yanxiufei.cn/gtlygtzrnj.html

[M04] 获取当前工作目录
来源：http://hz.wangdashe.top/gtnmqyejky.html

Py:   os.getcwd()
来源：http://hz.nanxuanxn.top/gtzavfmleh.html

PHP:  getcwd();
来源：http://hz.jlsjyb.cn/gtccyrwvmv.html

JS:   process.cwd()
来源：http://hz.nanxinkj.top/gtkbvazfzs.html

TS:   process.cwd()
来源：http://hz.jlsjyb.cn/gtaiipkbch.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.redwolf501.top/gtubzyzara.html

Go:   os.Getwd()
来源：http://hz.gogol.net.cn/gttfykozkx.html

Ruby: Dir.pwd
来源：http://hz.dashuyun.cn/gteqyyyyfg.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.xuanzx.com/gtqjimvzss.html

[M05] 设置退出码
来源：http://hz.svipenyu.cn/gtlklonxgr.html

Py:   sys.exit(1)
来源：http://hz.yangfankeji.com/gtdfkybnxr.html

PHP:  exit(1);
来源：http://hz.ybcxt.top/gtlyuquyfw.html

JS:   process.exit(1)
来源：http://hz.zhixingplan.top/gtgbwccpec.html

TS:   process.exit(1)
来源：http://hz.fzhhl.top/gtzrlaurhu.html

Java: System.exit(1)
来源：http://hz.hnxiangtu.top/gtftiwgedl.html

Go:   os.Exit(1)
来源：http://hz.c1oappe.top/gtagovvjoz.html

Ruby: exit 1
来源：http://hz.snrcjt.cn/gtssxyyzud.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.kuanghao11.cn/gtzuykywfl.html

[M06] 向标准错误输出
来源：http://hz.wangdashe.top/gtqydbadqd.html

Py:   print("err", file=sys.stderr)
来源：http://hz.redwolf501.top/gtkzfgwtps.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.zhijiandao.cn/gtqmdddyby.html

JS:   console.error("err")
来源：http://hz.svipenyu.cn/gtxruurbfb.html

TS:   console.error("err")
来源：http://hz.xuetiantiany.cn/gtrawpxtqx.html

Java: System.err.println("err")
来源：http://hz.mhx1999.top/gtzgqsorzh.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.haohaochexian.top/gtujmxjtrw.html

Ruby: warn "err"
来源：http://hz.yj20258.top/gtydavzffp.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.pengpengdd.cyou/gtewiljpep.html

[M07] 判断是否为主入口
来源：http://hz.hnxiangtu.top/gtbxlofuyq.html

Py:   if __name__ == "__main__":
来源：http://hz.cucudq.cn/gtzpikextt.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.andypj.xyz/gtkzntowtr.html

JS:   require.main === module
来源：http://hz.yj20258888.top/gtdlrncmyu.html

TS:   require.main === module
来源：http://hz.jiagoushi.top/gtbykdpqlb.html

Java: public static void main(String[] args)
来源：http://hz.zhengqikj.top/gttdqtfgbh.html

Go:   func main()
来源：http://hz.zhiwuduotai.top/gtgmjpstkv.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.guannengcc.top/gttjztriyp.html

C#:   static void Main(string[] args)
来源：http://hz.daxiang520.top/gtmoqyczlk.html

[M08] 获取系统与运行时信息
来源：http://hz.chenjidiqi.icu/gterhrkrdo.html

Py:   platform.system();  platform.python_version()
来源：http://hz.daxiang520.top/gtuamjtegq.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.gogol.net.cn/gtduqxuyit.html

JS:   process.platform;  process.version
来源：http://hz.tanke756.top/gtroqlftgz.html

TS:   process.platform;  process.version
来源：http://hz.jinqigufen.top/gtmlltcjyc.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.chenjidiqi.icu/gtoegydqio.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.birdmap.top/gtkroirlrl.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.snrcjt.cn/gtfbklirzb.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.mhx1999.top/gtnqtvmpbu.html

================================================================================
来源：http://hz.shuidangran.top/gtdcktdbva.html

N. 数据结构与算法
来源：http://hz.guowangkeji.top/gtcqakcpgz.html

================================================================================
来源：http://hz.ppjwa.cn/gtxyzdtmfa.html

[N01] 二分查找（有序数组）
来源：http://hz.yonumen.top/gtqwagdzaa.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.tianlin.xyz/gtfxjcevvv.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.andypj.xyz/gtdwfgjwmp.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.316326.xyz/gtqplhjwct.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.xuetiantiany.cn/gtzemtpvuj.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.zhaomingkeji.xyz/gtuydxcmpa.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.jianghu66.top/gtmpuibtwx.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.0kj1m.cn/gtarjftpqu.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.xziqi.cn/gtzqtbxcdw.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.kuanghao11.cn/gtkqrhcwca.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.hnxiangtu.top/gtbxwhyewn.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.yj20258.top/gtnpxwuzmo.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.shanyushiyangkeji.top/gtimpwluog.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.shzxlz.cn/gtchuiykgr.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.hywenlv.cn/gtzzsczvjj.html

Go:   slices.Sort(arr)
来源：http://hz.316326.xyz/gtrqintbzj.html

Ruby: arr.sort
来源：http://hz.yongpay.top/gtrgerybyx.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.ivvv.top/gttzmyfdqp.html

[N03] 快速排序（分治示例）
来源：http://hz.aibaodan.cn/gtfqnskgjb.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.cqqwz.cn/gtdpsjzjvy.html

PHP:  // 递归实现，或用 usort
来源：http://hz.zhongyouzk.top/gtiwixdwjv.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.xylfe.cn/gtwiorpnmh.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.xuetiantiany.cn/gtxqzwrgbm.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.hnqzz.top/gtufevkduv.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.jinghuilouyu.cn/gtpziekgyr.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.shanyushiyangtech.top/gtyiqwrues.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.ivvv.top/gtglukyvaf.html

[N04] 斐波那契数列
来源：http://hz.yueranfly.top/gtiudnetxb.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.wangdashe.top/gtmuxikzdb.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.cucudq.cn/gtzymfwldy.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.aibaodan.cn/gtiljxqcye.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.xuetiantiany.cn/gtvunpzlwl.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.birdmap.top/gtytstjsyx.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.yanxiufei.cn/gtxhyseipu.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.sysykeji.top/gtayrglhzj.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.yuxming.cn/gtucxteezr.html

[N05] 最大公约数
来源：http://hz.shuidangran.top/gtanxgaexr.html

Py:   math.gcd(a, b)
来源：http://hz.yueranfly.top/gtcmtokxqh.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.cdnleiting.top/gtukabbvwe.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.hnqzz.top/gtfrtzdhfd.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.iojbl.cn/gtlrboqico.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.chenjidiqi.icu/gtuoiviajk.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.chenjidiqi.icu/gtnmbqtusk.html

Ruby: a.gcd(b)
来源：http://hz.zhijiandao.cn/gtbrthlvou.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.yonumen.top/gtjhsjjxns.html

[N06] 判断回文字符串
来源：http://hz.cqqwz.cn/gtrawqfgac.html

Py:   s == s[::-1]
来源：http://hz.xingfuxueyuan.xyz/gtqxcjaxij.html

PHP:  $s === strrev($s);
来源：http://hz.daxiang520.top/gtirruxkot.html

JS:   s === [...s].reverse().join("")
来源：http://hz.tian-w.cn/gtoakaeekv.html

TS:   s === [...s].reverse().join("")
来源：http://hz.andypj.xyz/gtrvlqkwgx.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.aizwys.cn/gtjiytabuk.html

Go:   // 双指针从两端比较
来源：http://hz.ppjwa.cn/gthjeuuwls.html

Ruby: s == s.reverse
来源：http://hz.cheryme.top/gtivjildhv.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.zhiwuduotai.top/gtgqqhdsrz.html

[N07] 两数之和（返回下标）
来源：http://hz.316326.xyz/gtqlawgjwz.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.nanxinkj.top/gtkckvgunw.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.zhijiandao.cn/gtetzovolu.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.yvedp.cn/gtdtqurltd.html

TS:   // 手写 Map<string, number>
来源：http://hz.xylfe.cn/gtqgvghhes.html

Java: // 手写 HashMap
来源：http://hz.c1oappe.top/gtqixavrro.html

Go:   // 手写 map[int]int
来源：http://hz.yvedp.cn/gtkwgcsvxj.html

Ruby: // 手写 Hash
来源：http://hz.hysaishi.cn/gtkjbhkpgf.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.yuanzhike.top/gtilbfxeja.html

[N08] 生成全排列
来源：http://hz.vqdsnc.cn/gtfyufgqly.html

Py:   itertools.permutations(arr)
来源：http://hz.yonumen.top/gtqdnvhuaq.html

PHP:  // 手写递归交换
来源：http://hz.guannengcc.top/gthrpiwsxe.html

JS:   // 手写回溯递归
来源：http://hz.jinyuanbaomall.cn/gtmrcflixz.html

TS:   // 手写回溯递归
来源：http://hz.zhengqikj.top/gtpdjucsxg.html

Java: // 手写回溯递归
来源：http://hz.zhaomingkeji.xyz/gtclhkaqra.html

Go:   // 手写回溯递归
来源：http://hz.chenlongwang.top/gtxzrinuol.html

Ruby: arr.permutation.to_a
来源：http://hz.hysaishi.cn/gtvdvrhraz.html

C#:   // 手写回溯递归
来源：http://hz.xylfe.cn/gtdgpiqxjp.html

[N09] 栈与队列
来源：http://hz.yangfankeji.com/gtvxwzovow.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.ydjk.org.cn/gtzhuzbnui.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.cashguo.top/gtiqardcuy.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.pengpengdd.cyou/gthozhzjrr.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.shangyingyoupin.top/gtkjnjpaae.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.jinqigufen.top/gtdxebccfg.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.hammf.cn/gtloyrxgcs.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.jinyuanbaomall.cn/gtycmtqdhw.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.iojbl.cn/gtvmqgoaeg.html

[N10] 链表节点定义
来源：http://hz.jiagoushi.top/gtfkqcynoe.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.feifeiyinyue.top/gtvtthgwzc.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.sysykeji.top/gtamenmnbr.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.dashuyun.cn/gtfkjeuxvt.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.birdmap.top/gtwuvjdvuy.html

Java: class Node { int v; Node next; }
来源：http://hz.sufxvd.cn/gtfjyimymi.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.guowangkeji.top/gtugeqymqi.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.hywenlv.cn/gtrgppkfkf.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.yueranfly.top/gttwrhrmgs.html

[N11] 二叉树中序遍历
来源：http://hz.nanxinkj.top/gtxjgwdbkt.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.mhx1999.top/gtvsblqkyc.html

PHP:  // 手写递归函数
来源：http://hz.shzxlz.cn/gtosozwmiy.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.fengsongda.top/gtytwtlmju.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.52xcode.cn/gtwzmdpkgn.html

Java: // 手写递归
来源：http://hz.jinqigufen.top/gtbzrtwdxz.html

Go:   // 手写递归
来源：http://hz.xuetiantiany.cn/gtkuyyiygj.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.cheryme.top/gtkrtwzpdm.html

C#:   // 手写递归
来源：http://hz.fzhhl.top/gtuocvemek.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.xuanzx.com/gtgtqwwsvp.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.jianghu66.top/gtmwzwwwim.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.xuetiantiany.cn/gtcafkpoca.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.ppjwa.cn/gtoftrwsmq.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.kuanghao11.cn/gteebpebij.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.zhongyouzk.top/gtmzqqeeqe.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.316326.xyz/gtapsyohyq.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.gaohongyu789.top/gtnzbfxocs.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.zhengqikj.top/gtoiutlnyr.html

================================================================================
来源：http://hz.gotoacloud.top/gtaoeakjxx.html

O. 并发与异步
来源：http://hz.jinghuilouyu.cn/gtnbsovrqi.html

================================================================================
来源：http://hz.sufxvd.cn/gtimavvoyt.html

[O01] 启动一个线程
来源：http://hz.xingfuxueyuan.xyz/gtpakvohso.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.dashuyun.cn/gtqfxqbyls.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.xuanzx.com/gtezavsxsc.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.ydjk.org.cn/gtcmkmskmi.html

TS:   // 同 JS
来源：http://hz.shanyushiyangkeji.top/gtxiuvumvb.html

Java: new Thread(() -> f()).start()
来源：http://hz.zhengqikj.top/gtlqfgujwu.html

Go:   go f()
来源：http://hz.zycfv.cn/gtlnqumugh.html

Ruby: Thread.new { f }
来源：http://hz.quarkkingdee.top/gtkbejrydi.html

C#:   Task.Run(() => F());
来源：http://hz.sufxvd.cn/gtujyedzyp.html

[O02] 使用线程池
来源：http://hz.meibo888.top/gtaowlciib.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.yanxiufei.cn/gtcrybkfbr.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.hfpthk.cn/gtmtdlpfeo.html

JS:   // worker_threads 线程池
来源：http://hz.yj20258888.top/gtvgvdkwqe.html

TS:   // worker_threads 线程池
来源：http://hz.cucudq.cn/gtxymjjsbt.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.hongshengwenyu.top/gtrmbkpyqd.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.yuanzhike.top/gtypeciwvh.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.gogol.net.cn/gtyaexlofe.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.hammf.cn/gthndrlpjr.html

[O03] 加锁保护共享数据
来源：http://hz.sufxvd.cn/gtxtirulbs.html

Py:   with lock: shared += 1
来源：http://hz.sysykeji.top/gtyrczwlzb.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.mhx1999.top/gtffzamuqw.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.jinghuilouyu.cn/gtpzmtyquq.html

TS:   // 同 JS
来源：http://hz.birdmap.top/gtawelroov.html

Java: synchronized (this) { shared++; }
来源：http://hz.yuanzhike.top/gtftvhcvvy.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.jiagoushi.top/gtscdwfgza.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.jinqigfzy.top/gtddoicbrk.html

C#:   lock (gate) { shared++; }
来源：http://hz.fzhhl.top/gtkpzlsljp.html

[O04] 定义异步函数并等待
来源：http://hz.yonumen.top/gtseehfbfm.html

Py:   async def f():⏎    await g()
来源：http://hz.zhijiandao.cn/gtiunyxrfa.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.cheryme.top/gtrdyajxyy.html

JS:   async function f() { await g(); }
来源：http://hz.dianchejie.cn/gtgtrvojvq.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.jinghuilouyu.cn/gtqacphfeg.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.shzxlz.cn/gtehwesmlg.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.ppjwa.cn/gtxakdhkgf.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.daria6918.cn/gtbkdaupeh.html

C#:   async Task F() { await G(); }
来源：http://hz.guannengcc.top/gtjeksmvzt.html

[O05] 并发执行并等待全部完成
来源：http://hz.sxryk.cn/gtmkniyxcn.html

Py:   asyncio.gather(*tasks)
来源：http://hz.zhijiandao.cn/gtppujneza.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.xuanzx.com/gtcntofhhp.html

JS:   await Promise.all(tasks)
来源：http://hz.52xcode.cn/gtelnfdynu.html

TS:   await Promise.all(tasks)
来源：http://hz.52xcode.cn/gtexqnopye.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.cashguo.top/gttstfvcvz.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.yuxming.cn/gtvnxfkuce.html

Ruby: threads.map(&:join)
来源：http://hz.c1oappe.top/gtligzuydz.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.9152youxi.cn/gtjopbmuhb.html

[O06] 使用进程池
来源：http://hz.cashguo.top/gtgyamfhax.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.zhixingplan.top/gthjrxhrbh.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.9152youxi.cn/gthemmxbvn.html

JS:   // child_process / cluster 模块
来源：http://hz.mhx1999.top/gttrdilbah.html

TS:   // child_process / cluster 模块
来源：http://hz.ppjwa.cn/gtcnjtmziu.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.zhixingplan.top/gtheelpfzc.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.0kj1m.cn/gtvtcpibkl.html

Ruby: // fork 块
来源：http://hz.jinyuanbaomall.cn/gttetykzct.html

C#:   Parallel.For
来源：http://hz.cucudq.cn/gtsnxkyfes.html

================================================================================
来源：http://hz.nanxinkj.top/gtglsfxqni.html

P. 常用工具函数
来源：http://hz.xinyue.icu/gtkvxyesrg.html

================================================================================
来源：http://hz.jlsjyb.cn/gtxqavanze.html

[P01] 生成 UUID
来源：http://hz.xuetiantiany.cn/gtjvrowcyo.html

Py:   str(uuid.uuid4())
来源：http://hz.0kj1m.cn/gtamghdsdx.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.sxryk.cn/gtdpufscmr.html

JS:   crypto.randomUUID()
来源：http://hz.yanxiufei.cn/gtmfasaaud.html

TS:   crypto.randomUUID()
来源：http://hz.zycfv.cn/gtoqkcsmqs.html

Java: UUID.randomUUID().toString()
来源：http://hz.bjfxy.top/gtcbaionxq.html

Go:   // 用 github.com/google/uuid
来源：http://hz.jinqigufen.top/gtoneqfsnn.html

Ruby: SecureRandom.uuid
来源：http://hz.sxryk.cn/gtvntqktoz.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.xinyue.icu/gtzoxinmcf.html

[P02] MD5 / SHA256 摘要
来源：http://hz.gogol.net.cn/gtwtcfqbnp.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.tianlin.xyz/gtavkycpby.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.xziqi.cn/gtapxxxqff.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.wangdashe.top/gtonufqrbs.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.xinyue.icu/gtecsoxvzu.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.iojbl.cn/gtzgibegqg.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.aibaodan.cn/gtemlytits.html


<!-- 参考信息 -->