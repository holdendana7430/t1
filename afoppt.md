代发 wailian999

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.sysykeji.top/gtxiircgmj.html

[L04] 设置超时
来源：http://hz.hywenlv.cn/gtfzvunkdd.html

Py:   requests.get(url, timeout=5)
来源：http://hz.chenlongwang.top/gtwwkmypyv.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.yanxiufei.cn/gtrusgmire.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zycfv.cn/gtjllccdni.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.ydjk.org.cn/gthnndspzf.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.quarkkingdee.top/gtqgpebxlv.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.yj20258.top/gtdzxjgrqr.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.pycfn.com/gtdbtcaepp.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.wangshuangyany.cn/gtxjbninfh.html

[L05] 上传文件（multipart）
来源：http://hz.birdmap.top/gtmuhfhxtf.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.hnxiangtu.top/gttrusbxuy.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.svipenyu.cn/gtjzyhiurq.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.shangyingyoupin.top/gtysszrefn.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.gaohongyu789.top/gtjsdcyvln.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.yj20258.top/gtkzdpgwuj.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.shuidangran.top/gtafpqvpim.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.jinqigufen.top/gtccrtfeth.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.xinyue.icu/gtqwgfkpqo.html

[L06] 解析响应为 JSON
来源：http://hz.jianghu66.top/gtvouvyvlb.html

Py:   resp.json()
来源：http://hz.hysaishi.cn/gtjoisnbbm.html

PHP:  json_decode($body, true);
来源：http://hz.daria6918.cn/gtfafeskbr.html

JS:   await resp.json()
来源：http://hz.daxiang520.top/gttlejrpiu.html

TS:   await resp.json()
来源：http://hz.shuidangran.top/gtefvisdul.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.nanxinkj.top/gtmsbpsvwc.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.svipenyu.cn/gtcnqvnquk.html

Ruby: JSON.parse(resp.body)
来源：http://hz.yj20258.top/gtvwecypou.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.zhoulong.xyz/gtbchyzmxc.html

[L07] 处理 HTTP 状态码
来源：http://hz.yuxming.cn/gtzbovxsyo.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.zhixingplan.top/gtemwfsotx.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.c1oappe.top/gtyjghqvfn.html

JS:   resp.ok;  resp.status
来源：http://hz.316326.xyz/gtarkpybtd.html

TS:   resp.ok;  resp.status
来源：http://hz.nwbrower.top/gtreeuhnsr.html

Java: resp.statusCode()
来源：http://hz.hongshengwenyu.top/gtgsgiuntf.html

Go:   resp.StatusCode
来源：http://hz.tian-w.cn/gtiwkpgavy.html

Ruby: resp.code.to_i
来源：http://hz.guannengcc.top/gtvomlnbbs.html

C#:   (int)resp.StatusCode
来源：http://hz.pycfn.com/gtrowuikgh.html

[L08] 并发请求多个地址
来源：http://hz.andypj.xyz/gtcrnwjtux.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.yuxming.cn/gtdtsthqan.html

PHP:  curl_multi_init() 系列
来源：http://hz.aizwys.cn/gtdyudgkcb.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yangfankeji.com/gtcisxoeuu.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.nwbrower.top/gtelrgqmgz.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.yuxming.cn/gtiegwsvuo.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.yvedp.cn/gtgttyidsp.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.cucudq.cn/gtcjufapzl.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.shanyushiyangtech.top/gtwqloxipz.html

================================================================================
来源：http://hz.daxiang520.top/gtnhkjqqbd.html

M. 命令行 / 进程 / 环境
来源：http://hz.chenzaomai.com/gtwxnhzuhy.html

================================================================================
来源：http://hz.yj20258.top/gtspvinsgk.html

[M01] 读取命令行参数
来源：http://hz.ehwqpu.com/gtekvazrlj.html

Py:   sys.argv[1:]
来源：http://hz.shanyushiyangtech.top/gtgnfnopaa.html

PHP:  $argv;  $argc;
来源：http://hz.zycfv.cn/gtaeeslzdm.html

JS:   process.argv.slice(2)
来源：http://hz.sweek.top/gtcuhbdhga.html

TS:   process.argv.slice(2)
来源：http://hz.hywenlv.cn/gtslrqmxal.html

Java: args 数组（main 方法参数）
来源：http://hz.birdmap.top/gthxpvhfgs.html

Go:   os.Args[1:]
来源：http://hz.zhaomingkeji.xyz/gtfiawnzyy.html

Ruby: ARGV
来源：http://hz.sysykeji.top/gtyjfypgxk.html

C#:   args 数组（Main 方法参数）
来源：http://hz.xuanzx.com/gtkwjhzhlp.html

[M02] 读取环境变量
来源：http://hz.zhongyouzk.top/gtytvrcexr.html

Py:   os.environ.get("HOME")
来源：http://hz.havefunace.top/gtscavjwmt.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.tian-w.cn/gtyyeyhogz.html

JS:   process.env.HOME
来源：http://hz.gaohongyu789.top/gtjftgkibb.html

TS:   process.env.HOME
来源：http://hz.jianghu66.top/gtktquyysj.html

Java: System.getenv("HOME")
来源：http://hz.cucudq.cn/gtqnkwkwov.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.yongpay.top/gtgbhxqlgd.html

Ruby: ENV["HOME"]
来源：http://hz.ivvv.top/gtvpfwgpzm.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.andypj.xyz/gtkcqzcvsl.html

[M03] 执行外部命令
来源：http://hz.tianlin.xyz/gtdxsngzfv.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.xuanzx.com/gthyegzxlo.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.hammf.cn/gtinbdjrtb.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.chenzaomai.com/gtcuwyewqc.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.yuxming.cn/gtffbjcqbb.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.dianchejie.cn/gtbhchmryw.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.daxiang520.top/gtmnfdejpn.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.sweek.top/gtikkicmku.html

C#:   Process.Start("ls", "-l");
来源：http://hz.aizwys.cn/gtlldxdmhy.html

[M04] 获取当前工作目录
来源：http://hz.shzxlz.cn/gtvjkrczlu.html

Py:   os.getcwd()
来源：http://hz.iojbl.cn/gtivniewmk.html

PHP:  getcwd();
来源：http://hz.yj20258888.top/gtgkflstyx.html

JS:   process.cwd()
来源：http://hz.bjfxy.top/gtaloeewco.html

TS:   process.cwd()
来源：http://hz.guowangkeji.top/gtuhccvblm.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.jqgfzy.top/gtxrapekyj.html

Go:   os.Getwd()
来源：http://hz.yuanzhike.top/gtzgxedatf.html

Ruby: Dir.pwd
来源：http://hz.havefunace.top/gtimeylvvo.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.sweek.top/gtqiydevqi.html

[M05] 设置退出码
来源：http://hz.xinyue.icu/gtkbwkopoa.html

Py:   sys.exit(1)
来源：http://hz.pycfn.com/gtgtwuqjkh.html

PHP:  exit(1);
来源：http://hz.jqgufenzy.top/gtobleyiar.html

JS:   process.exit(1)
来源：http://hz.52xcode.cn/gtacsesfsz.html

TS:   process.exit(1)
来源：http://hz.bjfxy.top/gttjvzqspe.html

Java: System.exit(1)
来源：http://hz.xuanzx.com/gthweoqbih.html

Go:   os.Exit(1)
来源：http://hz.zhiwuduotai.top/gtjwgapzei.html

Ruby: exit 1
来源：http://hz.havefunace.top/gtpfjjduky.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.gogol.net.cn/gtldixlqpm.html

[M06] 向标准错误输出
来源：http://hz.fengsongda.top/gtwlepuayd.html

Py:   print("err", file=sys.stderr)
来源：http://hz.hnxiangtu.top/gtxwqxkymh.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.zhixingplan.top/gtujhvqiqk.html

JS:   console.error("err")
来源：http://hz.gzhubu.top/gtmgiaulma.html

TS:   console.error("err")
来源：http://hz.316326.xyz/gtyjknbioj.html

Java: System.err.println("err")
来源：http://hz.vqdsnc.cn/gtnvygjqjr.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.ehwqpu.com/gtpnkxurwa.html

Ruby: warn "err"
来源：http://hz.zhiwuduotai.top/gtnrsgaqmu.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.shuidangran.top/gtmzfecdnb.html

[M07] 判断是否为主入口
来源：http://hz.pengpengdd.cyou/gtixqmlbsy.html

Py:   if __name__ == "__main__":
来源：http://hz.gotoacloud.top/gtbybejnfl.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.shzxlz.cn/gtlgnaoppb.html

JS:   require.main === module
来源：http://hz.bjfxy.top/gtkuczmbhv.html

TS:   require.main === module
来源：http://hz.quarkkingdee.top/gtofgnyljo.html

Java: public static void main(String[] args)
来源：http://hz.0kj1m.cn/gtgwtoiyen.html

Go:   func main()
来源：http://hz.cucudq.cn/gtxhplcpen.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.hongshengwenyu.top/gtywitbton.html

C#:   static void Main(string[] args)
来源：http://hz.xuanzx.com/gtntongkfj.html

[M08] 获取系统与运行时信息
来源：http://hz.52xcode.cn/gtfhopukfo.html

Py:   platform.system();  platform.python_version()
来源：http://hz.zhiwuduotai.top/gtrgaqkljh.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.daria6918.cn/gtxwflpjzk.html

JS:   process.platform;  process.version
来源：http://hz.guannengcc.top/gtdmieyadb.html

TS:   process.platform;  process.version
来源：http://hz.hongshengwenyu.top/gtxamfjgjd.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.zhoulong.xyz/gtjnvorfhd.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.guowangkeji.top/gtrhplkvov.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.shangyingyoupin.top/gtkwmkcuyw.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.cashguo.top/gtporkwecw.html

================================================================================
来源：http://hz.bjfxy.top/gtnwjfecjk.html

N. 数据结构与算法
来源：http://hz.jinqigfzy.top/gtikhgrfgr.html

================================================================================
来源：http://hz.hywenlv.cn/gtxztnaoda.html

[N01] 二分查找（有序数组）
来源：http://hz.bjfxy.top/gtxeyiclsp.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.zdqjudy.top/gtcumakwbr.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.sweek.top/gtmvrtewss.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.svipenyu.cn/gtxxrjykfi.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.redwolf501.top/gtopcoswlz.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.shanyushiyangkeji.top/gtbndtbnpz.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.ywan-chungtsiang.top/gtajwbuqny.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.c1oappe.top/gtytziwoby.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.shuidangran.top/gtocjggyia.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.guannengcc.top/gthhtvrgmt.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.sxryk.cn/gtbwmplsxt.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.quarkkingdee.top/gtzodapiha.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.fengsongda.top/gtwdeiuqyh.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yvedp.cn/gtcjzxnyey.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.wangshuangyany.cn/gtcvsbalkn.html

Go:   slices.Sort(arr)
来源：http://hz.nwbrower.top/gtvhrbjsnw.html

Ruby: arr.sort
来源：http://hz.nanxuanxn.top/gtjwprzwps.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.yuanzhike.top/gtthcoeasi.html

[N03] 快速排序（分治示例）
来源：http://hz.vqdsnc.cn/gtfryjcviz.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.9152youxi.cn/gtjrvegwpf.html

PHP:  // 递归实现，或用 usort
来源：http://hz.shanyushiyangtech.top/gtupbttmnz.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.dashuyun.cn/gtjqyjdzvd.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.9152youxi.cn/gtozqwlhbp.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.fengsongda.top/gtizxinnms.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.zhijiandao.cn/gtaehfsouc.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.zdqjudy.top/gtwsmihhlu.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.jlsjyb.cn/gtwgpoczlm.html

[N04] 斐波那契数列
来源：http://hz.quarkkingdee.top/gtpmqrkszj.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.yj20258888.top/gtrhgbalgx.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.kuanghao11.cn/gtstzilfmk.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.redwolf501.top/gtxtqadjel.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.shangyingyoupin.top/gtniodexyl.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.pengpengdd.cyou/gtrljsoeod.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.hnxiangtu.top/gtpjvcneky.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.52xcode.cn/gtkbignnpf.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.jlsjyb.cn/gtenhonkat.html

[N05] 最大公约数
来源：http://hz.cucudq.cn/gtrrygmbol.html

Py:   math.gcd(a, b)
来源：http://hz.yanxiufei.cn/gtfiqcymyd.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.nwbrower.top/gtqtbrsofh.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.andypj.xyz/gtwwdlkbjp.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.zhengqikj.top/gtkbkmrycr.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.zhiwuduotai.top/gtkfntrhdz.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.ppjwa.cn/gtotudwett.html

Ruby: a.gcd(b)
来源：http://hz.ywan-chungtsiang.top/gtswexrywg.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.pengpengdd.cyou/gtvniqktcf.html

[N06] 判断回文字符串
来源：http://hz.nwbrower.top/gtpwehjisj.html

Py:   s == s[::-1]
来源：http://hz.zhixingplan.top/gtxbtnscix.html

PHP:  $s === strrev($s);
来源：http://hz.ydjk.org.cn/gtgejzkelx.html

JS:   s === [...s].reverse().join("")
来源：http://hz.cucudq.cn/gttvrnamgc.html

TS:   s === [...s].reverse().join("")
来源：http://hz.52xcode.cn/gtdrlxgepe.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.mhx1999.top/gterebiycl.html

Go:   // 双指针从两端比较
来源：http://hz.dashuyun.cn/gtvvspvvjr.html

Ruby: s == s.reverse
来源：http://hz.zycfv.cn/gtuyfexifj.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.iojbl.cn/gtuuepqcwi.html

[N07] 两数之和（返回下标）
来源：http://hz.ywan-chungtsiang.top/gtesrvqaby.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.jinghuilouyu.cn/gtaciuqljp.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.nwbrower.top/gtoghrxkdi.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.sxryk.cn/gtouhdalks.html

TS:   // 手写 Map<string, number>
来源：http://hz.chenlongwang.top/gtijhlsqzm.html

Java: // 手写 HashMap
来源：http://hz.meibo888.top/gtdeqfzeks.html

Go:   // 手写 map[int]int
来源：http://hz.52xcode.cn/gtfjxmsapx.html

Ruby: // 手写 Hash
来源：http://hz.yvedp.cn/gtakmizksu.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.xziqi.cn/gtkbqdgjha.html

[N08] 生成全排列
来源：http://hz.shuidangran.top/gtnnhsdzfd.html

Py:   itertools.permutations(arr)
来源：http://hz.andypj.xyz/gticweyqaf.html

PHP:  // 手写递归交换
来源：http://hz.cdnleiting.top/gtwnwddgpf.html

JS:   // 手写回溯递归
来源：http://hz.zhongyouzk.top/gttspayury.html

TS:   // 手写回溯递归
来源：http://hz.fzhhl.top/gtzoqmbtfe.html

Java: // 手写回溯递归
来源：http://hz.hammf.cn/gtpxsiohpu.html

Go:   // 手写回溯递归
来源：http://hz.wangshuangyany.cn/gtafoecwav.html

Ruby: arr.permutation.to_a
来源：http://hz.quarkkingdee.top/gtosldxppe.html

C#:   // 手写回溯递归
来源：http://hz.pengpengdd.cyou/gtmdfbhmwk.html

[N09] 栈与队列
来源：http://hz.snrcjt.cn/gtkvbkkjvh.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.havefunace.top/gtzoibvopa.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.hywenlv.cn/gtqrpksmlf.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.tian-w.cn/gtjcpdlqqo.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.hongshengwenyu.top/gtlslpnnff.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.redwolf501.top/gtgcbitdet.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.sxryk.cn/gtptpexdkn.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.hnqzz.top/gtxecmudtx.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.shangyingyoupin.top/gtopisaand.html

[N10] 链表节点定义
来源：http://hz.yj20258888.top/gtofmubmke.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.zhijiandao.cn/gtqkhwpbjx.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.chenlongwang.top/gtcgbbkjxz.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.chenzaomai.com/gtbaqpolee.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.gotoacloud.top/gtxzdrgkmr.html

Java: class Node { int v; Node next; }
来源：http://hz.quarkkingdee.top/gtckhkmmfq.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.vqdsnc.cn/gtbyctcrnu.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.cdnleiting.top/gtlcdswcvg.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.shangyingyoupin.top/gthqbdrgsd.html

[N11] 二叉树中序遍历
来源：http://hz.bjfxy.top/gttjwmtbkc.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.wangshuangyany.cn/gtevqtojdr.html

PHP:  // 手写递归函数
来源：http://hz.sxryk.cn/gtiwywsyia.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.hnxiangtu.top/gtvpryhfab.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.zycfv.cn/gtrwrpjgue.html

Java: // 手写递归
来源：http://hz.birdmap.top/gtlrnktoxe.html

Go:   // 手写递归
来源：http://hz.wangshuangyany.cn/gtjbqeequx.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.daria6918.cn/gtkxdnyoun.html

C#:   // 手写递归
来源：http://hz.yj20258.top/gtdhannfwc.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.chenzaomai.com/gtayczhisd.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.yueranfly.top/gtzwioqwpa.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.havefunace.top/gtcjxuvqik.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.pengpengdd.cyou/gtdvdojewm.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.redwolf501.top/gtukvbscbm.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.cheryme.top/gtfidekudl.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.smart0.xyz/gtcmhgzoaa.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.hammf.cn/gtuiiojmgu.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.ppjwa.cn/gtbgmkaobo.html

================================================================================
来源：http://hz.jqgufenzy.top/gtjpywgiyn.html

O. 并发与异步
来源：http://hz.yj202588.top/gtwnfrritg.html

================================================================================
来源：http://hz.cashguo.top/gtzuhdwpsh.html

[O01] 启动一个线程
来源：http://hz.dashuyun.cn/gtjazmsves.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.sxryk.cn/gtbgvdrieh.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.gzhubu.top/gtudraxhrz.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.chenzaomai.com/gtcmzkjvce.html

TS:   // 同 JS
来源：http://hz.dashuyun.cn/gteejoirdl.html

Java: new Thread(() -> f()).start()
来源：http://hz.dashuyun.cn/gtqletkspr.html

Go:   go f()
来源：http://hz.svipenyu.cn/gtozzdrlog.html

Ruby: Thread.new { f }
来源：http://hz.nanxuanxn.top/gtwhaodtxl.html

C#:   Task.Run(() => F());
来源：http://hz.iojbl.cn/gtvdwrfcql.html

[O02] 使用线程池
来源：http://hz.shzxlz.cn/gtcevupxmf.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.guowangkeji.top/gtanhxfesr.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.ywan-chungtsiang.top/gteoeglved.html

JS:   // worker_threads 线程池
来源：http://hz.jinghuilouyu.cn/gtaexcitwt.html

TS:   // worker_threads 线程池
来源：http://hz.nanxinkj.top/gtepvycnxu.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.shangyingyoupin.top/gtewspolrr.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.yuanzhike.top/gtuqqlepgp.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.smart0.xyz/gtvpsaeaop.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.meibo888.top/gtlknarcra.html

[O03] 加锁保护共享数据
来源：http://hz.wangdashe.top/gtvbiqupws.html

Py:   with lock: shared += 1
来源：http://hz.9152youxi.cn/gtxjiesdlz.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.andypj.xyz/gtgkaaecus.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.tian-w.cn/gtjjyrskmr.html

TS:   // 同 JS
来源：http://hz.yuanzhike.top/gtqvpfzddp.html

Java: synchronized (this) { shared++; }
来源：http://hz.guannengcc.top/gtyenhkadz.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.shanyushiyangtech.top/gtwhlonkbr.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.haohaochexian.top/gtacwsptyj.html

C#:   lock (gate) { shared++; }
来源：http://hz.cqqwz.cn/gtezqhajbn.html

[O04] 定义异步函数并等待
来源：http://hz.ydzc1.top/gtofyyjumx.html

Py:   async def f():⏎    await g()
来源：http://hz.cheryme.top/gtdemetqya.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.cucudq.cn/gturwxwyaw.html

JS:   async function f() { await g(); }
来源：http://hz.yj20258.top/gtmbrhdyfm.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.wangdashe.top/gtjqxxxdzz.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.shzxlz.cn/gtqcbxcfip.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.zhixingplan.top/gtzailcjad.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.hywenlv.cn/gtlucrrrog.html

C#:   async Task F() { await G(); }
来源：http://hz.gaohongyu789.top/gtkhgkzucg.html

[O05] 并发执行并等待全部完成
来源：http://hz.shuidangran.top/gtknflrmob.html

Py:   asyncio.gather(*tasks)
来源：http://hz.sxryk.cn/gtlhmckrjv.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.shangyingyoupin.top/gtdqsppuqw.html

JS:   await Promise.all(tasks)
来源：http://hz.jinyuanbaomall.cn/gtsednksfn.html

TS:   await Promise.all(tasks)
来源：http://hz.tanke756.top/gthpkeogpl.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.jinqigfzy.top/gtdvljaprb.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.yanxiufei.cn/gtaqltvmpw.html

Ruby: threads.map(&:join)
来源：http://hz.pengpengdd.cyou/gtxceddrwn.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.ywan-chungtsiang.top/gtpyhfvzro.html

[O06] 使用进程池
来源：http://hz.yj20258888.top/gtvashpycd.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.quarkkingdee.top/gtdzsqkshw.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.cheryme.top/gtkkgeizsc.html

JS:   // child_process / cluster 模块
来源：http://hz.cucudq.cn/gtjklhjcxc.html

TS:   // child_process / cluster 模块
来源：http://hz.52xcode.cn/gtyaovqfor.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.shuidangran.top/gtqcrrbmjl.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.gaohongyu789.top/gtbjgzdoqc.html

Ruby: // fork 块
来源：http://hz.iojbl.cn/gtsxeqwhcv.html

C#:   Parallel.For
来源：http://hz.chenjidiqi.icu/gtjxyezryd.html

================================================================================
来源：http://hz.zdqjudy.top/gtwlzwsdqo.html

P. 常用工具函数
来源：http://hz.xuanzx.com/gtomhtyixh.html

================================================================================
来源：http://hz.yj20258.top/gtzpavngul.html

[P01] 生成 UUID
来源：http://hz.sweek.top/gtthcnoizi.html

Py:   str(uuid.uuid4())
来源：http://hz.snrcjt.cn/gtjomctsjm.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.havefunace.top/gtcsrjitqd.html

JS:   crypto.randomUUID()
来源：http://hz.c1oappe.top/gtzhpsarnl.html

TS:   crypto.randomUUID()
来源：http://hz.hywenlv.cn/gtbkojlpux.html

Java: UUID.randomUUID().toString()
来源：http://hz.9152youxi.cn/gtcugrrsnw.html

Go:   // 用 github.com/google/uuid
来源：http://hz.smart0.xyz/gtvjbdqbwb.html

Ruby: SecureRandom.uuid
来源：http://hz.pycfn.com/gtbmjgovas.html


<!-- 参考信息 -->