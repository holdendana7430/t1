代发 wailian999

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yueranfly.top/gtxwapzbgr.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.quarkkingdee.top/gtwreutxep.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.yonumen.top/gtgparrmtq.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.cucudq.cn/gtodulcvku.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.cdnleiting.top/gtpqizcimo.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.aibaodan.cn/gtmqlpkikc.html

[L05] 上传文件（multipart）
来源：http://hz.pycfn.com/gtctrefzpx.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.zhijiandao.cn/gtnwejifnt.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.xuanzx.com/gtrhqwsowp.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.xingfuxueyuan.xyz/gtivagzgvu.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.zhongyouzk.top/gtkgesmdds.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.fengsongda.top/gtrtxqblra.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.xingfuxueyuan.xyz/gtitzkgagn.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.yonumen.top/gtondvrilq.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.shuidangran.top/gtqhbklzex.html

[L06] 解析响应为 JSON
来源：http://hz.zhijiandao.cn/gtrltmojgi.html

Py:   resp.json()
来源：http://hz.nwbrower.top/gthljfbxnb.html

PHP:  json_decode($body, true);
来源：http://hz.shanyushiyangkeji.top/gtxpezidky.html

JS:   await resp.json()
来源：http://hz.gzhubu.top/gtnnwzqjns.html

TS:   await resp.json()
来源：http://hz.daria6918.cn/gtolbwxmpm.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.52xcode.cn/gtoqunbbha.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.svipenyu.cn/gtdnsoftqf.html

Ruby: JSON.parse(resp.body)
来源：http://hz.ybcxt.top/gtgnzxblkh.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.vqdsnc.cn/gtgjegcgoa.html

[L07] 处理 HTTP 状态码
来源：http://hz.hywenlv.cn/gtwfubjome.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.xylfe.cn/gtiklghque.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.guowangkeji.top/gtvigjbhnl.html

JS:   resp.ok;  resp.status
来源：http://hz.jqgfzy.top/gtskqpudvp.html

TS:   resp.ok;  resp.status
来源：http://hz.jianghu66.top/gtwnqhjgta.html

Java: resp.statusCode()
来源：http://hz.jiagoushi.top/gtszoxfrsw.html

Go:   resp.StatusCode
来源：http://hz.yvedp.cn/gtnwcqomqp.html

Ruby: resp.code.to_i
来源：http://hz.guannengcc.top/gtmxdxutpt.html

C#:   (int)resp.StatusCode
来源：http://hz.hnxiangtu.top/gtnpezdhrz.html

[L08] 并发请求多个地址
来源：http://hz.yueranfly.top/gtyarlbdbl.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.xingfuxueyuan.xyz/gthwfewymf.html

PHP:  curl_multi_init() 系列
来源：http://hz.svipenyu.cn/gtucvqcwwe.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.gotoacloud.top/gtonjiaqqs.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jqgfzy.top/gtbuadyuvv.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.nanxinkj.top/gtcclinrir.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.hammf.cn/gtchaknxtj.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.guannengcc.top/gtrwaqmqxa.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.52xcode.cn/gtdmsdehjp.html

================================================================================
来源：http://hz.yueranfly.top/gtigtravdo.html

M. 命令行 / 进程 / 环境
来源：http://hz.jqgfzy.top/gthunsmheg.html

================================================================================
来源：http://hz.andypj.xyz/gtcfctfzvd.html

[M01] 读取命令行参数
来源：http://hz.yonumen.top/gtsmdwvpeh.html

Py:   sys.argv[1:]
来源：http://hz.tanke756.top/gtfpdbzgyr.html

PHP:  $argv;  $argc;
来源：http://hz.yueranfly.top/gtaesfziaj.html

JS:   process.argv.slice(2)
来源：http://hz.9152youxi.cn/gtcvzdmlkj.html

TS:   process.argv.slice(2)
来源：http://hz.sweek.top/gtpuieouqw.html

Java: args 数组（main 方法参数）
来源：http://hz.zhijiandao.cn/gtafrglwkz.html

Go:   os.Args[1:]
来源：http://hz.ppjwa.cn/gtbzjonuvg.html

Ruby: ARGV
来源：http://hz.gogol.net.cn/gtwbiuqqyo.html

C#:   args 数组（Main 方法参数）
来源：http://hz.cheryme.top/gtihfhdvfp.html

[M02] 读取环境变量
来源：http://hz.fzhhl.top/gtbyvzirdq.html

Py:   os.environ.get("HOME")
来源：http://hz.yuanzhike.top/gtepnkzmsv.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.svipenyu.cn/gtkjxcvnzl.html

JS:   process.env.HOME
来源：http://hz.nwbrower.top/gtwaormnjb.html

TS:   process.env.HOME
来源：http://hz.jinqigufen.top/gthsvsflgh.html

Java: System.getenv("HOME")
来源：http://hz.kuanghao11.cn/gtthmwxivf.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.yj20258888.top/gtmduqowpy.html

Ruby: ENV["HOME"]
来源：http://hz.xinyue.icu/gtqgctomtc.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.zhongyouzk.top/gtlcsvxkzc.html

[M03] 执行外部命令
来源：http://hz.dianchejie.cn/gtotnfxhfv.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.jqgufenzy.top/gtdbasmcrl.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.shangyingyoupin.top/gtwxloyzey.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.c1oappe.top/gtcgvhqchk.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.pengpengdd.cyou/gtwmgwpwuu.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.dashuyun.cn/gtymqypbkc.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.zhixingplan.top/gtroxdqtra.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.mhx1999.top/gtkbvsuljh.html

C#:   Process.Start("ls", "-l");
来源：http://hz.mhx1999.top/gtylrkybud.html

[M04] 获取当前工作目录
来源：http://hz.sufxvd.cn/gtcxdqrtbr.html

Py:   os.getcwd()
来源：http://hz.snrcjt.cn/gtugsmrcwq.html

PHP:  getcwd();
来源：http://hz.yongpay.top/gtajfffohc.html

JS:   process.cwd()
来源：http://hz.xingfuxueyuan.xyz/gtscccbgzg.html

TS:   process.cwd()
来源：http://hz.cqqwz.cn/gtxeezqhlb.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.hysaishi.cn/gtkhscmfmt.html

Go:   os.Getwd()
来源：http://hz.vqdsnc.cn/gtiosouoce.html

Ruby: Dir.pwd
来源：http://hz.jinyuanbaomall.cn/gtoswskdbm.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.jiagoushi.top/gthpsalgom.html

[M05] 设置退出码
来源：http://hz.xinyue.icu/gtuvbgozsd.html

Py:   sys.exit(1)
来源：http://hz.shanyushiyangtech.top/gtzibbnuju.html

PHP:  exit(1);
来源：http://hz.pengpengdd.cyou/gtnmvvoxgc.html

JS:   process.exit(1)
来源：http://hz.yongpay.top/gtlgkslvku.html

TS:   process.exit(1)
来源：http://hz.fengsongda.top/gtspzcyvlj.html

Java: System.exit(1)
来源：http://hz.jinghuilouyu.cn/gtbbbulajn.html

Go:   os.Exit(1)
来源：http://hz.sufxvd.cn/gtwrorkaix.html

Ruby: exit 1
来源：http://hz.fzhhl.top/gtsctejeao.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.daria6918.cn/gtnhnlwleb.html

[M06] 向标准错误输出
来源：http://hz.nanxinkj.top/gtmxefceoc.html

Py:   print("err", file=sys.stderr)
来源：http://hz.kuanghao11.cn/gtquqnbbbf.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.hammf.cn/gtnzvuhnux.html

JS:   console.error("err")
来源：http://hz.yuxming.cn/gtsmviutwt.html

TS:   console.error("err")
来源：http://hz.jqgfzy.top/gtjnlyirqw.html

Java: System.err.println("err")
来源：http://hz.ydjk.org.cn/gtbxpdizgu.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.0kj1m.cn/gtmongboqh.html

Ruby: warn "err"
来源：http://hz.xylfe.cn/gtipamulsk.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.cdnleiting.top/gtcorqkyth.html

[M07] 判断是否为主入口
来源：http://hz.smart0.xyz/gtecztblnv.html

Py:   if __name__ == "__main__":
来源：http://hz.yj202588.top/gtsewouttb.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.chenlongwang.top/gtpzafikht.html

JS:   require.main === module
来源：http://hz.chenzaomai.com/gtvmremkgj.html

TS:   require.main === module
来源：http://hz.gogol.net.cn/gthqmtdfid.html

Java: public static void main(String[] args)
来源：http://hz.tanke756.top/gtmlnhafbg.html

Go:   func main()
来源：http://hz.sxryk.cn/gteqzpccxj.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.pycfn.com/gtilrhgnfp.html

C#:   static void Main(string[] args)
来源：http://hz.vqdsnc.cn/gtfwnkmubk.html

[M08] 获取系统与运行时信息
来源：http://hz.ehwqpu.com/gtihjnzfba.html

Py:   platform.system();  platform.python_version()
来源：http://hz.yueranfly.top/gtcqqpbqrf.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.iojbl.cn/gtxzyfboix.html

JS:   process.platform;  process.version
来源：http://hz.ybcxt.top/gtyvqrbbhz.html

TS:   process.platform;  process.version
来源：http://hz.ybcxt.top/gtwkkhfxvx.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.ywan-chungtsiang.top/gtazmwyjiv.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.jinghuilouyu.cn/gttcsejgfr.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.hfpthk.cn/gtkjpvwrhg.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.ivvv.top/gtxgokpnfk.html

================================================================================
来源：http://hz.zhongyouzk.top/gtbccaojqt.html

N. 数据结构与算法
来源：http://hz.daria6918.cn/gtqqcliboy.html

================================================================================
来源：http://hz.jinqigufen.top/gtxvobeuqr.html

[N01] 二分查找（有序数组）
来源：http://hz.daxiang520.top/gtakxjvxmk.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.ydjk.org.cn/gtuosolkes.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.jyoumei.cn/gttbcbhsxr.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zhongyouzk.top/gtjajyhrne.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yvedp.cn/gtaqosjcjp.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.meibo888.top/gtvzwydzaf.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.tian-w.cn/gtuzgttuki.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.yuanzhike.top/gtdjrohomb.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.zhengqikj.top/gtvyzjebfh.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.yueranfly.top/gtagwsxqgs.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.guannengcc.top/gtfrwabejb.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.cqqwz.cn/gtdlyocnlf.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yanxiufei.cn/gtcxhxeizp.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.chenjidiqi.icu/gtbjmssmkf.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.nanxuanxn.top/gtuamsqgxa.html

Go:   slices.Sort(arr)
来源：http://hz.9152youxi.cn/gtefpqrebf.html

Ruby: arr.sort
来源：http://hz.aizwys.cn/gtatthuwyi.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.yonumen.top/gtvohedzrm.html

[N03] 快速排序（分治示例）
来源：http://hz.jinqigufen.top/gtjbmsuovz.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.shanyushiyangtech.top/gtvertpgxw.html

PHP:  // 递归实现，或用 usort
来源：http://hz.haohaochexian.top/gtatfmjann.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.ehwqpu.com/gtwdxlcyfr.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jqgfzy.top/gtxonhawan.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.fzhhl.top/gtfjupqlgd.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.bjfxy.top/gtxncggnbc.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.hfpthk.cn/gtmgtwkikc.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.zhengqikj.top/gthotzkmyj.html

[N04] 斐波那契数列
来源：http://hz.xinyue.icu/gtagzdjjan.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.yonumen.top/gtaznzuzac.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.tian-w.cn/gthbxwaays.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.zhengqikj.top/gtkzvfgihs.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.cdnleiting.top/gthoamecir.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.yueranfly.top/gthbksghgn.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.jianghu66.top/gtbuenopvm.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.yonumen.top/gtfljgfxce.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.aibaodan.cn/gtfjxniykb.html

[N05] 最大公约数
来源：http://hz.nwbrower.top/gtipshtsmz.html

Py:   math.gcd(a, b)
来源：http://hz.iojbl.cn/gtxbdgizpj.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.ywan-chungtsiang.top/gtmieliiti.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jqgufenzy.top/gtncvxomeh.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jqgufenzy.top/gtaktuydpg.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.ppjwa.cn/gtqwqzvblj.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.aizwys.cn/gtadgjopoh.html

Ruby: a.gcd(b)
来源：http://hz.yuxming.cn/gtjhjwzrcl.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.zhiwuduotai.top/gtitcjjtoe.html

[N06] 判断回文字符串
来源：http://hz.ybcxt.top/gtevbjsboj.html

Py:   s == s[::-1]
来源：http://hz.ybcxt.top/gtezeuymtg.html

PHP:  $s === strrev($s);
来源：http://hz.pengpengdd.cyou/gtreuskwte.html

JS:   s === [...s].reverse().join("")
来源：http://hz.hywenlv.cn/gtoyuawrhj.html

TS:   s === [...s].reverse().join("")
来源：http://hz.pycfn.com/gtgigqocru.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.meibo888.top/gtjtbbyvzs.html

Go:   // 双指针从两端比较
来源：http://hz.xziqi.cn/gtoziwtjqj.html

Ruby: s == s.reverse
来源：http://hz.0kj1m.cn/gtaxzlrrcg.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.gogol.net.cn/gtlswpctho.html

[N07] 两数之和（返回下标）
来源：http://hz.zhixingplan.top/gtzmwczkxn.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.cashguo.top/gtuyzgiilw.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.quarkkingdee.top/gtzfrjayav.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.wangdashe.top/gtwvkeuqay.html

TS:   // 手写 Map<string, number>
来源：http://hz.guannengcc.top/gtchamajfo.html

Java: // 手写 HashMap
来源：http://hz.xziqi.cn/gtsdnoyfqm.html

Go:   // 手写 map[int]int
来源：http://hz.zhiwuduotai.top/gtjltsycri.html

Ruby: // 手写 Hash
来源：http://hz.haohaochexian.top/gtnfizatmc.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.jinqigfzy.top/gtkogkvotp.html

[N08] 生成全排列
来源：http://hz.jiagoushi.top/gtucrkqrco.html

Py:   itertools.permutations(arr)
来源：http://hz.svipenyu.cn/gtlzjueqxk.html

PHP:  // 手写递归交换
来源：http://hz.shzxlz.cn/gtsvkemumi.html

JS:   // 手写回溯递归
来源：http://hz.sufxvd.cn/gtuwmihfez.html

TS:   // 手写回溯递归
来源：http://hz.hnxiangtu.top/gtszxpjfir.html

Java: // 手写回溯递归
来源：http://hz.cashguo.top/gtwycsijrs.html

Go:   // 手写回溯递归
来源：http://hz.nanxinkj.top/gtnnctbqkz.html

Ruby: arr.permutation.to_a
来源：http://hz.cheryme.top/gtidapbndc.html

C#:   // 手写回溯递归
来源：http://hz.zhaomingkeji.xyz/gtxoaweupd.html

[N09] 栈与队列
来源：http://hz.shuidangran.top/gtpyoumbzy.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.jlsjyb.cn/gtakxbiyaz.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.zhongyouzk.top/gtiwfhgogb.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.tian-w.cn/gtnhbeppye.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.hammf.cn/gtxzubnjhm.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.zhixingplan.top/gtdvbfmapn.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.ivvv.top/gtyycmqaci.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.dianchejie.cn/gtxsioglgx.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.sxryk.cn/gtyhsfhszg.html

[N10] 链表节点定义
来源：http://hz.zdqjudy.top/gtswowmybh.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.guannengcc.top/gtekhgmkzp.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.xuetiantiany.cn/gtntnkzzue.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.havefunace.top/gtpillqtyk.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.daria6918.cn/gtlczgqgck.html

Java: class Node { int v; Node next; }
来源：http://hz.ivvv.top/gtphkeidhx.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.jinqigufen.top/gtukxweqqf.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.sxryk.cn/gttngqdall.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.guannengcc.top/gtuwgeicev.html

[N11] 二叉树中序遍历
来源：http://hz.shangyingyoupin.top/gthqnkplic.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.tian-w.cn/gtpafjxbay.html

PHP:  // 手写递归函数
来源：http://hz.sysykeji.top/gtdtzqhvbf.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.haohaochexian.top/gtvrurdrqe.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.cashguo.top/gtcymjnmwy.html

Java: // 手写递归
来源：http://hz.yonumen.top/gtmfhzqnly.html

Go:   // 手写递归
来源：http://hz.aizwys.cn/gtgyyhogjj.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.xziqi.cn/gtwmruuezt.html

C#:   // 手写递归
来源：http://hz.jinghuilouyu.cn/gtqzbelllw.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.feifeiyinyue.top/gtqoidwdtw.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.cucudq.cn/gtgdilkfxd.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.jinyuanbaomall.cn/gtdnobwoth.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.xuanzx.com/gteuemgkmi.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.cucudq.cn/gtleizhvpe.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.jlsjyb.cn/gtmsyvsupy.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.316326.xyz/gtuxdlbrmr.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.cashguo.top/gthpzjnghs.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.snrcjt.cn/gtcmbvebur.html

================================================================================
来源：http://hz.ydjk.org.cn/gtdxeamnme.html

O. 并发与异步
来源：http://hz.xingfuxueyuan.xyz/gtygstllho.html

================================================================================
来源：http://hz.fzhhl.top/gtobqppsan.html

[O01] 启动一个线程
来源：http://hz.yueranfly.top/gtwmuwumaa.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.snrcjt.cn/gtsauchfhx.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.ybcxt.top/gtpbnalgav.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.hongshengwenyu.top/gtcyaswabh.html

TS:   // 同 JS
来源：http://hz.tanke756.top/gtqwpxpluc.html

Java: new Thread(() -> f()).start()
来源：http://hz.jiagoushi.top/gtghhbttpq.html

Go:   go f()
来源：http://hz.hysaishi.cn/gtpouztmkn.html

Ruby: Thread.new { f }
来源：http://hz.yuxming.cn/gtnnagycpv.html

C#:   Task.Run(() => F());
来源：http://hz.haohaochexian.top/gtlfrwcrrg.html

[O02] 使用线程池
来源：http://hz.chenzaomai.com/gtkxypswvw.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.jinghuilouyu.cn/gtywiqgofz.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.shanyushiyangtech.top/gtkdgoijfx.html

JS:   // worker_threads 线程池
来源：http://hz.dashuyun.cn/gtomcfdnod.html

TS:   // worker_threads 线程池
来源：http://hz.gzhubu.top/gtwkvnfjle.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.yangfankeji.com/gtgjfjjjbr.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.dianchejie.cn/gtdiaffmrp.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.dianchejie.cn/gtpcqwxfbk.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.ydzc1.top/gttnznhavb.html

[O03] 加锁保护共享数据
来源：http://hz.cucudq.cn/gtqxvanbdt.html

Py:   with lock: shared += 1
来源：http://hz.meibo888.top/gtnfsiuoay.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.tianlin.xyz/gtozspfopp.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.snrcjt.cn/gtxummjddu.html

TS:   // 同 JS
来源：http://hz.zhaomingkeji.xyz/gtzjkpvfnh.html

Java: synchronized (this) { shared++; }
来源：http://hz.0kj1m.cn/gttlpnkmeb.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.vqdsnc.cn/gtwfspchhj.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.wangdashe.top/gtscnsfjwh.html

C#:   lock (gate) { shared++; }
来源：http://hz.shuidangran.top/gtyosydpcn.html

[O04] 定义异步函数并等待
来源：http://hz.yonumen.top/gtxinwpbak.html

Py:   async def f():⏎    await g()
来源：http://hz.ppjwa.cn/gtynnntcsj.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.yuanzhike.top/gtkjwevare.html

JS:   async function f() { await g(); }
来源：http://hz.cucudq.cn/gtxitpbsfj.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.52xcode.cn/gtfssgmlgw.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.hnxiangtu.top/gtfzjhjadh.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.ydjk.org.cn/gtsmhsttpx.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.pycfn.com/gtqjdagtvf.html

C#:   async Task F() { await G(); }
来源：http://hz.zhaomingkeji.xyz/gteylhvovd.html

[O05] 并发执行并等待全部完成
来源：http://hz.9152youxi.cn/gttzexabdi.html

Py:   asyncio.gather(*tasks)
来源：http://hz.hnxiangtu.top/gttuaajrdw.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.iojbl.cn/gtzfkfetcc.html

JS:   await Promise.all(tasks)
来源：http://hz.jianghu66.top/gtxzscagxc.html

TS:   await Promise.all(tasks)
来源：http://hz.shangyingyoupin.top/gttliajfbl.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.yonumen.top/gtyoiuudag.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.quarkkingdee.top/gtgyyaubak.html

Ruby: threads.map(&:join)
来源：http://hz.pengpengdd.cyou/gtktskhbkq.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.shangyingyoupin.top/gtewbpysfv.html

[O06] 使用进程池
来源：http://hz.0kj1m.cn/gtdvmkkoov.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.svipenyu.cn/gtysymgbfz.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.jinqigufen.top/gtpbmflwxb.html

JS:   // child_process / cluster 模块
来源：http://hz.iojbl.cn/gtwkrjcgvv.html

TS:   // child_process / cluster 模块
来源：http://hz.316326.xyz/gtscrpyvdw.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.yvedp.cn/gtphjkubok.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.jqgufenzy.top/gtcyvzftzi.html

Ruby: // fork 块
来源：http://hz.tianlin.xyz/gtbinegvcm.html

C#:   Parallel.For
来源：http://hz.sufxvd.cn/gtzydvbote.html

================================================================================
来源：http://hz.quarkkingdee.top/gtsjxnlojb.html

P. 常用工具函数
来源：http://hz.yvedp.cn/gtkpqffdoe.html

================================================================================
来源：http://hz.hfpthk.cn/gtncgdlyuy.html

[P01] 生成 UUID
来源：http://hz.tian-w.cn/gtsmywrrel.html

Py:   str(uuid.uuid4())
来源：http://hz.vqdsnc.cn/gtioixmfin.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.cqqwz.cn/gtplwzxfev.html

JS:   crypto.randomUUID()
来源：http://hz.zhaomingkeji.xyz/gtisrgxafe.html

TS:   crypto.randomUUID()
来源：http://hz.quarkkingdee.top/gtoagyzxie.html

Java: UUID.randomUUID().toString()
来源：http://hz.ybcxt.top/gtechiougs.html

Go:   // 用 github.com/google/uuid
来源：http://hz.wangshuangyany.cn/gtyqiipjag.html

Ruby: SecureRandom.uuid
来源：http://hz.xinyue.icu/gtpwcyjwjk.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.fengsongda.top/gtudmprmdg.html

[P02] MD5 / SHA256 摘要
来源：http://hz.ppjwa.cn/gtrpjtrvep.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.xinyue.icu/gtqfgrambh.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.52xcode.cn/gtotgvgiep.html


<!-- 参考信息 -->