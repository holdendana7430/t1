代发 wailian999

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.9152youxi.cn/gtqylhrwbb.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.52xcode.cn/gtelcmmgnh.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.guannengcc.top/gtkvkpxjkf.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.ehwqpu.com/gtxstokknn.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.aizwys.cn/gtfnkhuakn.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.redwolf501.top/gtbpxlgfua.html

[L05] 上传文件（multipart）
来源：http://hz.shanyushiyangkeji.top/gtipjlvetp.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.zhengqikj.top/gtwfwhbkvj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.yueranfly.top/gtqykytkow.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.dianchejie.cn/gtkqwftwhq.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.andypj.xyz/gtmmvegbxj.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.hnqzz.top/gtajfdqtik.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.hywenlv.cn/gtuwgotuns.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.sweek.top/gthjceqmjr.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.tianlin.xyz/gtblrppexf.html

[L06] 解析响应为 JSON
来源：http://hz.aibaodan.cn/gtvspsvhhs.html

Py:   resp.json()
来源：http://hz.c1oappe.top/gtueshrzpm.html

PHP:  json_decode($body, true);
来源：http://hz.zycfv.cn/gtkldcfvkh.html

JS:   await resp.json()
来源：http://hz.xylfe.cn/gtuktorwad.html

TS:   await resp.json()
来源：http://hz.xingfuxueyuan.xyz/gtsmgzucbx.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.snrcjt.cn/gtjwaupduf.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.cucudq.cn/gtdsvmrcxs.html

Ruby: JSON.parse(resp.body)
来源：http://hz.iojbl.cn/gtggfgpliw.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.nanxuanxn.top/gtwvxggajo.html

[L07] 处理 HTTP 状态码
来源：http://hz.dashuyun.cn/gtssdnwcel.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.chenjidiqi.icu/gtuvsztwxg.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.yanxiufei.cn/gtopcsrclr.html

JS:   resp.ok;  resp.status
来源：http://hz.yuanzhike.top/gtuwisrbsm.html

TS:   resp.ok;  resp.status
来源：http://hz.316326.xyz/gtjebsukzk.html

Java: resp.statusCode()
来源：http://hz.cqqwz.cn/gtbqcesiaj.html

Go:   resp.StatusCode
来源：http://hz.yj20258888.top/gtbshgnjxr.html

Ruby: resp.code.to_i
来源：http://hz.svipenyu.cn/gttehwuzir.html

C#:   (int)resp.StatusCode
来源：http://hz.quarkkingdee.top/gtczazapql.html

[L08] 并发请求多个地址
来源：http://hz.nanxinkj.top/gtoupqwevq.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.nwbrower.top/gteburbkrk.html

PHP:  curl_multi_init() 系列
来源：http://hz.redwolf501.top/gtxsozkhiu.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.dianchejie.cn/gtcuxdbbpc.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.pengpengdd.cyou/gtqbrumfkl.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.jlsjyb.cn/gtpgwfgbms.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.zhaomingkeji.xyz/gtmgezveoi.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.tianlin.xyz/gtafwmjabt.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.chenzaomai.com/gttshmzosk.html

================================================================================
来源：http://hz.xinyue.icu/gtklfiatix.html

M. 命令行 / 进程 / 环境
来源：http://hz.snrcjt.cn/gtjtfcbggy.html

================================================================================
来源：http://hz.yj20258888.top/gtxehnrdhy.html

[M01] 读取命令行参数
来源：http://hz.daria6918.cn/gtvxjyfmha.html

Py:   sys.argv[1:]
来源：http://hz.sxryk.cn/gtdplalhig.html

PHP:  $argv;  $argc;
来源：http://hz.daxiang520.top/gtsmqfkmsu.html

JS:   process.argv.slice(2)
来源：http://hz.xylfe.cn/gtyhgrljwq.html

TS:   process.argv.slice(2)
来源：http://hz.redwolf501.top/gtjpkokaja.html

Java: args 数组（main 方法参数）
来源：http://hz.52xcode.cn/gtwrtsqclc.html

Go:   os.Args[1:]
来源：http://hz.zycfv.cn/gtbypkyelw.html

Ruby: ARGV
来源：http://hz.jqgufenzy.top/gtreqikftl.html

C#:   args 数组（Main 方法参数）
来源：http://hz.redwolf501.top/gtwogsuzgp.html

[M02] 读取环境变量
来源：http://hz.jinghuilouyu.cn/gtbezydtoa.html

Py:   os.environ.get("HOME")
来源：http://hz.gogol.net.cn/gtcrxsxqyi.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.shanyushiyangkeji.top/gtlnljkjlz.html

JS:   process.env.HOME
来源：http://hz.zhijiandao.cn/gtqpnwvwox.html

TS:   process.env.HOME
来源：http://hz.sysykeji.top/gtihmvelxt.html

Java: System.getenv("HOME")
来源：http://hz.havefunace.top/gtvybqsbtx.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.sysykeji.top/gtnbygrryt.html

Ruby: ENV["HOME"]
来源：http://hz.aibaodan.cn/gtsaynuxgp.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.xuetiantiany.cn/gtnlocgmhn.html

[M03] 执行外部命令
来源：http://hz.yvedp.cn/gtourzojje.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.hywenlv.cn/gtolskslut.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.hfpthk.cn/gtkbsunxtd.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.ydjk.org.cn/gtqaxsfgbs.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.zycfv.cn/gtssezfaty.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.hnqzz.top/gtzwdkabki.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.wangdashe.top/gtjuyzkype.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.316326.xyz/gtikeorjfv.html

C#:   Process.Start("ls", "-l");
来源：http://hz.pengpengdd.cyou/gtleyclayn.html

[M04] 获取当前工作目录
来源：http://hz.chenjidiqi.icu/gtgbngcqsf.html

Py:   os.getcwd()
来源：http://hz.svipenyu.cn/gtarcnajts.html

PHP:  getcwd();
来源：http://hz.yj20258.top/gtarcizpjv.html

JS:   process.cwd()
来源：http://hz.cdnleiting.top/gtdkjrndtk.html

TS:   process.cwd()
来源：http://hz.xingfuxueyuan.xyz/gtsmxihrlp.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.xuanzx.com/gtimubndor.html

Go:   os.Getwd()
来源：http://hz.fzhhl.top/gtylkyrzbc.html

Ruby: Dir.pwd
来源：http://hz.cucudq.cn/gtmzcrwmjp.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.hysaishi.cn/gtjoeagoij.html

[M05] 设置退出码
来源：http://hz.gzhubu.top/gtjgmhfabd.html

Py:   sys.exit(1)
来源：http://hz.shanyushiyangtech.top/gtzchqwxmd.html

PHP:  exit(1);
来源：http://hz.jinyuanbaomall.cn/gtrjrjqnyh.html

JS:   process.exit(1)
来源：http://hz.jqgufenzy.top/gtsulnkpbw.html

TS:   process.exit(1)
来源：http://hz.pycfn.com/gttxjibrkp.html

Java: System.exit(1)
来源：http://hz.gaohongyu789.top/gturamyhxd.html

Go:   os.Exit(1)
来源：http://hz.yangfankeji.com/gtqtyyutta.html

Ruby: exit 1
来源：http://hz.zhixingplan.top/gtikrgmffc.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.vqdsnc.cn/gtfaigjgfc.html

[M06] 向标准错误输出
来源：http://hz.wangshuangyany.cn/gtuouitjya.html

Py:   print("err", file=sys.stderr)
来源：http://hz.jianghu66.top/gtyhmpwvov.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.hfpthk.cn/gtkhcwqhdk.html

JS:   console.error("err")
来源：http://hz.c1oappe.top/gttzdvofja.html

TS:   console.error("err")
来源：http://hz.shuidangran.top/gtdifciljb.html

Java: System.err.println("err")
来源：http://hz.wangshuangyany.cn/gtjqdqewto.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.gogol.net.cn/gtklluoldk.html

Ruby: warn "err"
来源：http://hz.sweek.top/gtdduwwgty.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.ywan-chungtsiang.top/gtgqolumfe.html

[M07] 判断是否为主入口
来源：http://hz.jinyuanbaomall.cn/gtrmuuwqzi.html

Py:   if __name__ == "__main__":
来源：http://hz.nanxuanxn.top/gtqmwvcvgp.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.jinghuilouyu.cn/gtikdmnfqg.html

JS:   require.main === module
来源：http://hz.pengpengdd.cyou/gtdjscrtjj.html

TS:   require.main === module
来源：http://hz.ivvv.top/gthbumwhpl.html

Java: public static void main(String[] args)
来源：http://hz.hysaishi.cn/gtsiygowhg.html

Go:   func main()
来源：http://hz.yj202588.top/gtvngxcxyj.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.hysaishi.cn/gtpygkpxsq.html

C#:   static void Main(string[] args)
来源：http://hz.jianghu66.top/gtfocjjwpm.html

[M08] 获取系统与运行时信息
来源：http://hz.nanxinkj.top/gtpxzzvcny.html

Py:   platform.system();  platform.python_version()
来源：http://hz.yj20258.top/gtijbzbsyd.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.nanxinkj.top/gtiqszwpee.html

JS:   process.platform;  process.version
来源：http://hz.iojbl.cn/gtgdcdxshi.html

TS:   process.platform;  process.version
来源：http://hz.shanyushiyangtech.top/gtegwdogxm.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.yj20258.top/gtpnbzkess.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.sufxvd.cn/gtraiwxzsq.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.ywan-chungtsiang.top/gtstqnuolx.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.aibaodan.cn/gtxcsprglz.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtctzmjszs.html

N. 数据结构与算法
来源：http://hz.zhijiandao.cn/gtuvjdwmrf.html

================================================================================
来源：http://hz.pycfn.com/gtrquqfdnt.html

[N01] 二分查找（有序数组）
来源：http://hz.shuidangran.top/gtoxahuedz.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.zhiwuduotai.top/gtqyvzrjnr.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.xinyue.icu/gtiiaekmzh.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jinghuilouyu.cn/gtyswbowsu.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.snrcjt.cn/gtjpnwzrpb.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.ywan-chungtsiang.top/gtkrrkofaz.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.52xcode.cn/gtkvjyspla.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.ehwqpu.com/gtsjtrwcjz.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.havefunace.top/gtqparhhhv.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.gotoacloud.top/gtugcwomyl.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.hysaishi.cn/gtbevjeynn.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.hnqzz.top/gtdqkhdhtl.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.hywenlv.cn/gtpfjrlfth.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.gotoacloud.top/gtgyiviapo.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.guannengcc.top/gthzqqmkwq.html

Go:   slices.Sort(arr)
来源：http://hz.xingfuxueyuan.xyz/gtqgtczope.html

Ruby: arr.sort
来源：http://hz.wangdashe.top/gtjdagbjlh.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.hnqzz.top/gtknqvxhgq.html

[N03] 快速排序（分治示例）
来源：http://hz.daxiang520.top/gtztwliysi.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.havefunace.top/gtexpckrra.html

PHP:  // 递归实现，或用 usort
来源：http://hz.wangshuangyany.cn/gtiazxahjg.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.chenzaomai.com/gthfjjomcw.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.fzhhl.top/gtihxvdvsi.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.jinqigfzy.top/gtzlsxrven.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.shangyingyoupin.top/gtukjdrnkh.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.ybcxt.top/gtpxenolta.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.guannengcc.top/gtpykqhrho.html

[N04] 斐波那契数列
来源：http://hz.zhixingplan.top/gtgmfmohkb.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.shangyingyoupin.top/gtochumxir.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.jinyuanbaomall.cn/gtnvgexoll.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yvedp.cn/gtojttkria.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.hywenlv.cn/gteirxtzdo.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.gogol.net.cn/gtcxuhygdg.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.meibo888.top/gtkbjgusjg.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.shangyingyoupin.top/gtuetpnmiv.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.cashguo.top/gtuenfmsnq.html

[N05] 最大公约数
来源：http://hz.tanke756.top/gtpypqiqvv.html

Py:   math.gcd(a, b)
来源：http://hz.zhoulong.xyz/gtbtzryjxt.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.9152youxi.cn/gtdjpgptzw.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.sxryk.cn/gtljerxtyv.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.havefunace.top/gtaaryucau.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.jianghu66.top/gtvpbsolgb.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.gaohongyu789.top/gtyyietgmo.html

Ruby: a.gcd(b)
来源：http://hz.cucudq.cn/gtcffrcxip.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.xingfuxueyuan.xyz/gtufutxveu.html

[N06] 判断回文字符串
来源：http://hz.yuxming.cn/gtsezceaad.html

Py:   s == s[::-1]
来源：http://hz.daria6918.cn/gthermzqdr.html

PHP:  $s === strrev($s);
来源：http://hz.aizwys.cn/gtqnubvpko.html

JS:   s === [...s].reverse().join("")
来源：http://hz.jqgfzy.top/gtsrydjlvp.html

TS:   s === [...s].reverse().join("")
来源：http://hz.chenjidiqi.icu/gtqefhfgaq.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.aibaodan.cn/gtnqfiyxzr.html

Go:   // 双指针从两端比较
来源：http://hz.xuetiantiany.cn/gtadzchaen.html

Ruby: s == s.reverse
来源：http://hz.aizwys.cn/gtwcazqqqr.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.hnxiangtu.top/gtnfcrnsku.html

[N07] 两数之和（返回下标）
来源：http://hz.zhixingplan.top/gtaxtunlwv.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.316326.xyz/gtqdqwnoaq.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.jlsjyb.cn/gtgehkwlzy.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.shzxlz.cn/gtptzcfjre.html

TS:   // 手写 Map<string, number>
来源：http://hz.ehwqpu.com/gteqqjwsqm.html

Java: // 手写 HashMap
来源：http://hz.shzxlz.cn/gtmpdddjsz.html

Go:   // 手写 map[int]int
来源：http://hz.c1oappe.top/gtfhitbryc.html

Ruby: // 手写 Hash
来源：http://hz.xinyue.icu/gtmltxzleo.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.jinghuilouyu.cn/gtzvjtxggi.html

[N08] 生成全排列
来源：http://hz.kuanghao11.cn/gtxyxuaqut.html

Py:   itertools.permutations(arr)
来源：http://hz.shuidangran.top/gtlglpdxfk.html

PHP:  // 手写递归交换
来源：http://hz.shanyushiyangkeji.top/gtuuizaxjh.html

JS:   // 手写回溯递归
来源：http://hz.yuxming.cn/gtjcxbhbso.html

TS:   // 手写回溯递归
来源：http://hz.havefunace.top/gttwalawtl.html

Java: // 手写回溯递归
来源：http://hz.ywan-chungtsiang.top/gtyutgmdzt.html

Go:   // 手写回溯递归
来源：http://hz.zhaomingkeji.xyz/gthgodxwnd.html

Ruby: arr.permutation.to_a
来源：http://hz.hongshengwenyu.top/gtdhzjrhnv.html

C#:   // 手写回溯递归
来源：http://hz.pycfn.com/gtavndcfjf.html

[N09] 栈与队列
来源：http://hz.jinyuanbaomall.cn/gtpmygknvb.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.kuanghao11.cn/gtjiptqmhr.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.hnqzz.top/gtsyjsbrik.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.hammf.cn/gtgvwgplak.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.jinyuanbaomall.cn/gtedhzfgsl.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.dianchejie.cn/gtomfqdwee.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.jqgfzy.top/gtjzeauldx.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.jinyuanbaomall.cn/gtibcoggaa.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.shanyushiyangkeji.top/gtwimcrjar.html

[N10] 链表节点定义
来源：http://hz.zycfv.cn/gtigkochmp.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.zhaomingkeji.xyz/gtlymilyki.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.havefunace.top/gtmzswitoo.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.52xcode.cn/gtwxgjwhrl.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.hammf.cn/gtvdtdnile.html

Java: class Node { int v; Node next; }
来源：http://hz.shanyushiyangtech.top/gtddpmtemm.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.hysaishi.cn/gtzegsoazo.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.cdnleiting.top/gtuobweahe.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.mhx1999.top/gtpwwcfziy.html

[N11] 二叉树中序遍历
来源：http://hz.feifeiyinyue.top/gtzkosdwyw.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.feifeiyinyue.top/gtitdtqolg.html

PHP:  // 手写递归函数
来源：http://hz.nwbrower.top/gtbdianbyi.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.sxryk.cn/gtepdexfms.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.tian-w.cn/gtgyzrktjh.html

Java: // 手写递归
来源：http://hz.zhiwuduotai.top/gtrlhrkzhg.html

Go:   // 手写递归
来源：http://hz.daria6918.cn/gtwmbogppq.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.yvedp.cn/gtrewqdglv.html

C#:   // 手写递归
来源：http://hz.jyoumei.cn/gtpciaorix.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.zhoulong.xyz/gtqqadubwv.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.meibo888.top/gtcnambazh.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.nwbrower.top/gtoknrfsxk.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.zhongyouzk.top/gtzbxgiute.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.tanke756.top/gtjdhuyhmn.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.gzhubu.top/gtgujowwmv.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.chenlongwang.top/gthcgwwdpo.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.zdqjudy.top/gtzzqmewry.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.jinghuilouyu.cn/gtdpjyckyz.html

================================================================================
来源：http://hz.hnqzz.top/gtdnuliegi.html

O. 并发与异步
来源：http://hz.cucudq.cn/gtuioymkpx.html

================================================================================
来源：http://hz.aibaodan.cn/gtcgnhqriq.html

[O01] 启动一个线程
来源：http://hz.yj20258.top/gtumifstua.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.cashguo.top/gthaeqsrie.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.bjfxy.top/gthymhfmnh.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.xylfe.cn/gthwkxijys.html

TS:   // 同 JS
来源：http://hz.hongshengwenyu.top/gtxhmlxlop.html

Java: new Thread(() -> f()).start()
来源：http://hz.chenjidiqi.icu/gtwnertrle.html

Go:   go f()
来源：http://hz.shanyushiyangtech.top/gtdqiwziyh.html

Ruby: Thread.new { f }
来源：http://hz.ydjk.org.cn/gtoyinaeaj.html

C#:   Task.Run(() => F());
来源：http://hz.gaohongyu789.top/gtjwrqezqi.html

[O02] 使用线程池
来源：http://hz.0kj1m.cn/gtvqxpheee.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.wangshuangyany.cn/gtymlvvibc.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.9152youxi.cn/gtlfpeydjw.html

JS:   // worker_threads 线程池
来源：http://hz.yvedp.cn/gtjctynurj.html

TS:   // worker_threads 线程池
来源：http://hz.ivvv.top/gtjbijrexo.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.smart0.xyz/gtwbrrzmao.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.shangyingyoupin.top/gtchnbwbaw.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.xuanzx.com/gtgepvietc.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.cqqwz.cn/gtmxxcntnf.html

[O03] 加锁保护共享数据
来源：http://hz.xingfuxueyuan.xyz/gtprqpfowy.html

Py:   with lock: shared += 1
来源：http://hz.chenjidiqi.icu/gtjvdmxmrb.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.yanxiufei.cn/gtfznakocb.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.0kj1m.cn/gtypmsoajd.html

TS:   // 同 JS
来源：http://hz.tian-w.cn/gtfrqchuct.html

Java: synchronized (this) { shared++; }
来源：http://hz.c1oappe.top/gtwlgjegeu.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.gzhubu.top/gtpemmtydg.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.pycfn.com/gtlabagkiw.html

C#:   lock (gate) { shared++; }
来源：http://hz.zdqjudy.top/gtjnfvlczr.html

[O04] 定义异步函数并等待
来源：http://hz.fengsongda.top/gtpcjxcswc.html

Py:   async def f():⏎    await g()
来源：http://hz.cashguo.top/gtvjhmxtko.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.cdnleiting.top/gthcdwhdeu.html

JS:   async function f() { await g(); }
来源：http://hz.9152youxi.cn/gtuhxzkzqf.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.yvedp.cn/gtpiqvyllo.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.sufxvd.cn/gttmrjphfe.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.pycfn.com/gtawzwyuwr.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.birdmap.top/gtbpzeluro.html

C#:   async Task F() { await G(); }
来源：http://hz.jqgfzy.top/gttjfbyewh.html

[O05] 并发执行并等待全部完成
来源：http://hz.yueranfly.top/gtdxxxrnyt.html

Py:   asyncio.gather(*tasks)
来源：http://hz.chenlongwang.top/gtsjyksrgm.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.xinyue.icu/gtlizbgxfg.html

JS:   await Promise.all(tasks)
来源：http://hz.ehwqpu.com/gtolpjuved.html

TS:   await Promise.all(tasks)
来源：http://hz.shuidangran.top/gtreokimkw.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.ivvv.top/gtbestasro.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.hfpthk.cn/gtdogipcpa.html

Ruby: threads.map(&:join)
来源：http://hz.cqqwz.cn/gthllizovk.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.zhijiandao.cn/gtwoyqcdme.html

[O06] 使用进程池
来源：http://hz.tianlin.xyz/gteoqfjcfi.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.0kj1m.cn/gtwofcbjav.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.ppjwa.cn/gtreiwinzy.html

JS:   // child_process / cluster 模块
来源：http://hz.jqgfzy.top/gtnmyvakmc.html

TS:   // child_process / cluster 模块
来源：http://hz.haohaochexian.top/gtuihjarog.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.nanxinkj.top/gtnrpsbpmz.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.jinqigufen.top/gtucruwxlh.html

Ruby: // fork 块
来源：http://hz.ybcxt.top/gttxgesots.html

C#:   Parallel.For
来源：http://hz.yuxming.cn/gtfcukgnmi.html

================================================================================
来源：http://hz.redwolf501.top/gtgbssiyas.html

P. 常用工具函数
来源：http://hz.kuanghao11.cn/gtxfhufjsg.html

================================================================================
来源：http://hz.quarkkingdee.top/gtgqhjfeeo.html

[P01] 生成 UUID
来源：http://hz.svipenyu.cn/gtjltytdsz.html

Py:   str(uuid.uuid4())
来源：http://hz.guowangkeji.top/gtcepopizp.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.zhixingplan.top/gtwlhmazny.html

JS:   crypto.randomUUID()
来源：http://hz.mhx1999.top/gtorrbfxad.html

TS:   crypto.randomUUID()
来源：http://hz.smart0.xyz/gtlafnhiza.html

Java: UUID.randomUUID().toString()
来源：http://hz.daxiang520.top/gthchzpvly.html

Go:   // 用 github.com/google/uuid
来源：http://hz.yongpay.top/gtjhnpktjj.html

Ruby: SecureRandom.uuid
来源：http://hz.zycfv.cn/gtweeejdkd.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.gogol.net.cn/gtgmaumwkc.html

[P02] MD5 / SHA256 摘要
来源：http://hz.aibaodan.cn/gtnngwubux.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.xylfe.cn/gthzyihkzp.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.smart0.xyz/gtzfbkqxpp.html


<!-- 参考信息 -->