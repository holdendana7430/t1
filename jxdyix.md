代发 wailian999

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.svipenyu.cn/gtnehvjhwa.html

[L04] 设置超时
来源：http://hz.gotoacloud.top/gttdbgssiv.html

Py:   requests.get(url, timeout=5)
来源：http://hz.zhongyouzk.top/gtigikxhrs.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.smart0.xyz/gtnedhqefr.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.gotoacloud.top/gtebkcbenw.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zhengqikj.top/gtfwnnlvzp.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.redwolf501.top/gtgdqbxyvs.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.shanyushiyangkeji.top/gtbowgodzv.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.iojbl.cn/gtfdbqksxk.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.daria6918.cn/gtfcxhfilh.html

[L05] 上传文件（multipart）
来源：http://hz.zhengqikj.top/gtwxdzjauy.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.redwolf501.top/gtuvzydqoy.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.jinyuanbaomall.cn/gtutybmerm.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.mhx1999.top/gttwjyghkk.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.dashuyun.cn/gtemhprikl.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.guowangkeji.top/gtacurzawz.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.jiagoushi.top/gtlvqlaboj.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.quarkkingdee.top/gtggkccphf.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.tian-w.cn/gtksiwowfz.html

[L06] 解析响应为 JSON
来源：http://hz.yj202588.top/gtnkayjgqr.html

Py:   resp.json()
来源：http://hz.sysykeji.top/gtfxcnufsz.html

PHP:  json_decode($body, true);
来源：http://hz.jyoumei.cn/gtbgqbbtfp.html

JS:   await resp.json()
来源：http://hz.316326.xyz/gtkagudbyz.html

TS:   await resp.json()
来源：http://hz.birdmap.top/gthqdhznvq.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.yueranfly.top/gtastftgiv.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.shuidangran.top/gtgtpolxgg.html

Ruby: JSON.parse(resp.body)
来源：http://hz.316326.xyz/gtesxfdccs.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.xinyue.icu/gtsyablgej.html

[L07] 处理 HTTP 状态码
来源：http://hz.tian-w.cn/gthoqwadlw.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.jinghuilouyu.cn/gtvickagnc.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.nanxuanxn.top/gtkvzjzrom.html

JS:   resp.ok;  resp.status
来源：http://hz.jinqigfzy.top/gtksmkqald.html

TS:   resp.ok;  resp.status
来源：http://hz.zhixingplan.top/gtshzelbqr.html

Java: resp.statusCode()
来源：http://hz.tianlin.xyz/gtbsvpngis.html

Go:   resp.StatusCode
来源：http://hz.zhongyouzk.top/gtabfauwuu.html

Ruby: resp.code.to_i
来源：http://hz.tianlin.xyz/gtsbutvrec.html

C#:   (int)resp.StatusCode
来源：http://hz.zhijiandao.cn/gtpycdorec.html

[L08] 并发请求多个地址
来源：http://hz.ydzc1.top/gtecdijjxq.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.sufxvd.cn/gtbjrfluod.html

PHP:  curl_multi_init() 系列
来源：http://hz.yj20258888.top/gtdgwanllo.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jqgufenzy.top/gtdximptzk.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yj202588.top/gtcagubxxb.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.zhaomingkeji.xyz/gtjanatzam.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.c1oappe.top/gtcqpvqiui.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.havefunace.top/gtaccvxqqk.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.kuanghao11.cn/gtggeydlef.html

================================================================================
来源：http://hz.cheryme.top/gtcxrlegmp.html

M. 命令行 / 进程 / 环境
来源：http://hz.52xcode.cn/gtitecrulc.html

================================================================================
来源：http://hz.jqgfzy.top/gtsufyajgy.html

[M01] 读取命令行参数
来源：http://hz.yj202588.top/gtxwwrnsaa.html

Py:   sys.argv[1:]
来源：http://hz.yj202588.top/gttbhnrqkr.html

PHP:  $argv;  $argc;
来源：http://hz.birdmap.top/gtngygptwm.html

JS:   process.argv.slice(2)
来源：http://hz.guannengcc.top/gtspaatixq.html

TS:   process.argv.slice(2)
来源：http://hz.pycfn.com/gtrfqbbfdc.html

Java: args 数组（main 方法参数）
来源：http://hz.zycfv.cn/gtdzmgxqmr.html

Go:   os.Args[1:]
来源：http://hz.9152youxi.cn/gtbqeuqcfd.html

Ruby: ARGV
来源：http://hz.pycfn.com/gtwdavvgjs.html

C#:   args 数组（Main 方法参数）
来源：http://hz.yueranfly.top/gtdifsvpwp.html

[M02] 读取环境变量
来源：http://hz.dianchejie.cn/gtxbzlkmni.html

Py:   os.environ.get("HOME")
来源：http://hz.snrcjt.cn/gtohhmmclc.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.yongpay.top/gtqvulolxb.html

JS:   process.env.HOME
来源：http://hz.c1oappe.top/gtvjsnhjws.html

TS:   process.env.HOME
来源：http://hz.xingfuxueyuan.xyz/gttaatstoj.html

Java: System.getenv("HOME")
来源：http://hz.daria6918.cn/gtajochnlc.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.cashguo.top/gtgelnzecf.html

Ruby: ENV["HOME"]
来源：http://hz.shanyushiyangtech.top/gtjewaagiz.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.shanyushiyangtech.top/gtikzgscna.html

[M03] 执行外部命令
来源：http://hz.hysaishi.cn/gtbiuqjdbx.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.zdqjudy.top/gteoqokwut.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.9152youxi.cn/gtnojdijwv.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.yanxiufei.cn/gtvqobbjfn.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.zdqjudy.top/gtemoxysim.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.zhijiandao.cn/gtwkreuxfp.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.hongshengwenyu.top/gtpzfrcuew.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.vqdsnc.cn/gtrstqhzrb.html

C#:   Process.Start("ls", "-l");
来源：http://hz.kuanghao11.cn/gtyqrrfvzw.html

[M04] 获取当前工作目录
来源：http://hz.zhixingplan.top/gtsgarldco.html

Py:   os.getcwd()
来源：http://hz.zhoulong.xyz/gtxyjxqbke.html

PHP:  getcwd();
来源：http://hz.wangdashe.top/gtkxmpkouo.html

JS:   process.cwd()
来源：http://hz.yuanzhike.top/gtumcctlig.html

TS:   process.cwd()
来源：http://hz.shanyushiyangtech.top/gtldsgemuj.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.xingfuxueyuan.xyz/gtqlnqqwev.html

Go:   os.Getwd()
来源：http://hz.aizwys.cn/gtsajixaob.html

Ruby: Dir.pwd
来源：http://hz.sufxvd.cn/gtewkerojp.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.chenjidiqi.icu/gtdcxnirwy.html

[M05] 设置退出码
来源：http://hz.ppjwa.cn/gtwunrndcn.html

Py:   sys.exit(1)
来源：http://hz.zhongyouzk.top/gtkrlrftkk.html

PHP:  exit(1);
来源：http://hz.jiagoushi.top/gtvnmichpk.html

JS:   process.exit(1)
来源：http://hz.hongshengwenyu.top/gthvjmnqtt.html

TS:   process.exit(1)
来源：http://hz.wangdashe.top/gtqnkjffhq.html

Java: System.exit(1)
来源：http://hz.gzhubu.top/gtfppvwlug.html

Go:   os.Exit(1)
来源：http://hz.yj20258.top/gtnefpydtc.html

Ruby: exit 1
来源：http://hz.yongpay.top/gtuxkkccew.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.ivvv.top/gtgislpnee.html

[M06] 向标准错误输出
来源：http://hz.cashguo.top/gtkddizcib.html

Py:   print("err", file=sys.stderr)
来源：http://hz.yvedp.cn/gtxpugviat.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.feifeiyinyue.top/gtfwpfojci.html

JS:   console.error("err")
来源：http://hz.ivvv.top/gtjzughrvv.html

TS:   console.error("err")
来源：http://hz.dianchejie.cn/gtrgnufmde.html

Java: System.err.println("err")
来源：http://hz.havefunace.top/gtxdejdebn.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.ppjwa.cn/gtkheuirid.html

Ruby: warn "err"
来源：http://hz.pycfn.com/gtofoxzmmv.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.haohaochexian.top/gtbympnbfx.html

[M07] 判断是否为主入口
来源：http://hz.smart0.xyz/gthwebhlnd.html

Py:   if __name__ == "__main__":
来源：http://hz.tanke756.top/gtvaerpqsx.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.gzhubu.top/gtlpcwisuc.html

JS:   require.main === module
来源：http://hz.hfpthk.cn/gtokkvfxjt.html

TS:   require.main === module
来源：http://hz.jinghuilouyu.cn/gtdmmsrnqf.html

Java: public static void main(String[] args)
来源：http://hz.shanyushiyangkeji.top/gtumqitnye.html

Go:   func main()
来源：http://hz.ppjwa.cn/gttluxievj.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.zhijiandao.cn/gtdkojylal.html

C#:   static void Main(string[] args)
来源：http://hz.yuxming.cn/gtcrciabvp.html

[M08] 获取系统与运行时信息
来源：http://hz.daria6918.cn/gtgggitreg.html

Py:   platform.system();  platform.python_version()
来源：http://hz.sweek.top/gtorpwnmlk.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.zhongyouzk.top/gtexsxjcuj.html

JS:   process.platform;  process.version
来源：http://hz.9152youxi.cn/gtktbmetvx.html

TS:   process.platform;  process.version
来源：http://hz.nanxuanxn.top/gtorzxkgac.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.hongshengwenyu.top/gtszwuozlu.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.pycfn.com/gtdttkptvk.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.gogol.net.cn/gtjjfhffuh.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.tianlin.xyz/gtejbkpxqh.html

================================================================================
来源：http://hz.jqgfzy.top/gtxrhonump.html

N. 数据结构与算法
来源：http://hz.zdqjudy.top/gtgabcukuo.html

================================================================================
来源：http://hz.guowangkeji.top/gtlfbzviww.html

[N01] 二分查找（有序数组）
来源：http://hz.guannengcc.top/gtuxpnfiic.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.yuanzhike.top/gtdxsvxnjv.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.yj20258888.top/gtcvlaoglp.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.xuanzx.com/gtdybgdoiq.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.hysaishi.cn/gttndnmaie.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.jinyuanbaomall.cn/gtuljrqlso.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.andypj.xyz/gtwzuqyxsg.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.pycfn.com/gtdrmzgnkp.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.xuanzx.com/gtabomwpuy.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.jinyuanbaomall.cn/gtmkgzrsfj.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.yonumen.top/gtqtdzeznu.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.yj20258.top/gtvvgtrudy.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.zhiwuduotai.top/gtxphyyyla.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yuanzhike.top/gtmmcslfwo.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.hfpthk.cn/gtdwaolqdm.html

Go:   slices.Sort(arr)
来源：http://hz.haohaochexian.top/gtbwjviedc.html

Ruby: arr.sort
来源：http://hz.zhaomingkeji.xyz/gtysokvlos.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.chenlongwang.top/gtiyjzllxm.html

[N03] 快速排序（分治示例）
来源：http://hz.nanxuanxn.top/gtpbipqbwx.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.sysykeji.top/gtbsxzvbgi.html

PHP:  // 递归实现，或用 usort
来源：http://hz.dianchejie.cn/gtthnamcfl.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.wangdashe.top/gtknowtopd.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.gaohongyu789.top/gtzpjtwizg.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.zhengqikj.top/gtzkuthkvz.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.jianghu66.top/gtxjkottqm.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.52xcode.cn/gteqlpfdrn.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.jyoumei.cn/gtnocxppiw.html

[N04] 斐波那契数列
来源：http://hz.pengpengdd.cyou/gtmqmvhfnz.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.hongshengwenyu.top/gtwxlefibb.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.daria6918.cn/gtkszywvca.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.cucudq.cn/gtunjzhdxh.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.cheryme.top/gtozqmpuyf.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.xinyue.icu/gtnmqzwpwk.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.shuidangran.top/gtrieauikb.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.nwbrower.top/gtcjoxadwb.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.meibo888.top/gtpbnhqdet.html

[N05] 最大公约数
来源：http://hz.smart0.xyz/gtcwquzbor.html

Py:   math.gcd(a, b)
来源：http://hz.zhaomingkeji.xyz/gtctrpchft.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.tianlin.xyz/gtxsmzmiul.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.ydzc1.top/gtgvetjdmx.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.aizwys.cn/gtksqfdcll.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.andypj.xyz/gteajeaygt.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.cqqwz.cn/gtrnnocvjz.html

Ruby: a.gcd(b)
来源：http://hz.zdqjudy.top/gtviwkbyxi.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.9152youxi.cn/gtzfimmxrg.html

[N06] 判断回文字符串
来源：http://hz.xylfe.cn/gtgikdvlut.html

Py:   s == s[::-1]
来源：http://hz.jinghuilouyu.cn/gtcjmedeml.html

PHP:  $s === strrev($s);
来源：http://hz.shuidangran.top/gtqvvnjznc.html

JS:   s === [...s].reverse().join("")
来源：http://hz.daria6918.cn/gtzptirzdr.html

TS:   s === [...s].reverse().join("")
来源：http://hz.cucudq.cn/gtkqvxldel.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.aibaodan.cn/gtntdklcbt.html

Go:   // 双指针从两端比较
来源：http://hz.jinghuilouyu.cn/gtvjkltceu.html

Ruby: s == s.reverse
来源：http://hz.yuxming.cn/gtueupotsp.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.daxiang520.top/gtgddlpiyo.html

[N07] 两数之和（返回下标）
来源：http://hz.xinyue.icu/gtdqbdurwh.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.ydzc1.top/gtxsbmdcwb.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.shzxlz.cn/gtdswciwmy.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.shuidangran.top/gtmmgcdotd.html

TS:   // 手写 Map<string, number>
来源：http://hz.cheryme.top/gtgbhrkclr.html

Java: // 手写 HashMap
来源：http://hz.zhixingplan.top/gtjyorzkun.html

Go:   // 手写 map[int]int
来源：http://hz.gotoacloud.top/gtjvipecto.html

Ruby: // 手写 Hash
来源：http://hz.ppjwa.cn/gtohohcudp.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.zhijiandao.cn/gtnulywppx.html

[N08] 生成全排列
来源：http://hz.jinyuanbaomall.cn/gtlprulzod.html

Py:   itertools.permutations(arr)
来源：http://hz.zhijiandao.cn/gtosuyzsnw.html

PHP:  // 手写递归交换
来源：http://hz.dianchejie.cn/gtxpnfgodb.html

JS:   // 手写回溯递归
来源：http://hz.nanxuanxn.top/gtdrjssoyz.html

TS:   // 手写回溯递归
来源：http://hz.yonumen.top/gtyclskynb.html

Java: // 手写回溯递归
来源：http://hz.jinqigfzy.top/gteyrtlyqq.html

Go:   // 手写回溯递归
来源：http://hz.yj20258.top/gthxdimhft.html

Ruby: arr.permutation.to_a
来源：http://hz.hnqzz.top/gtdgjapbjt.html

C#:   // 手写回溯递归
来源：http://hz.0kj1m.cn/gttkxdmylq.html

[N09] 栈与队列
来源：http://hz.hnxiangtu.top/gtyzuiazws.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.bjfxy.top/gtcsyqwrei.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.yangfankeji.com/gtqgfidlks.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.zhiwuduotai.top/gtuppgkrbr.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.wangshuangyany.cn/gtkozqbsyz.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.zhixingplan.top/gtpwzcsjxe.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.havefunace.top/gtptsixown.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.svipenyu.cn/gtxuxhlojy.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.ppjwa.cn/gtbzqwhltf.html

[N10] 链表节点定义
来源：http://hz.ydjk.org.cn/gtwgnxvwtp.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.gzhubu.top/gtqmbgzaww.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.snrcjt.cn/gtwedpmcyo.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.xinyue.icu/gtheofaxts.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.hnxiangtu.top/gtngyzxabn.html

Java: class Node { int v; Node next; }
来源：http://hz.bjfxy.top/gtexxoukvl.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.shzxlz.cn/gtpvibswqo.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.andypj.xyz/gthrrhkvjv.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.redwolf501.top/gtkqowzgkd.html

[N11] 二叉树中序遍历
来源：http://hz.xylfe.cn/gtkfrxbnts.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.redwolf501.top/gtchpqwbps.html

PHP:  // 手写递归函数
来源：http://hz.daria6918.cn/gtkarxzbex.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.cheryme.top/gtoicifase.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.hongshengwenyu.top/gtwuogjfqn.html

Java: // 手写递归
来源：http://hz.jlsjyb.cn/gtdjyrycuj.html

Go:   // 手写递归
来源：http://hz.zycfv.cn/gtiiwheudv.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.xuanzx.com/gtdyaonyon.html

C#:   // 手写递归
来源：http://hz.guowangkeji.top/gtadarrkwt.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.zhoulong.xyz/gtzfstlwmy.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.gotoacloud.top/gtsvlngrlf.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.jyoumei.cn/gtymocjsyo.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.havefunace.top/gtpwdhdlkt.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yj20258.top/gtzzvsrokt.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.hywenlv.cn/gtyhpkrydq.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.ehwqpu.com/gtvzkgxlqz.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.hongshengwenyu.top/gtvcxueccs.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.feifeiyinyue.top/gtbkagjphz.html

================================================================================
来源：http://hz.fzhhl.top/gtbixyijsf.html

O. 并发与异步
来源：http://hz.nwbrower.top/gtgohyshwq.html

================================================================================
来源：http://hz.316326.xyz/gtnavivdbn.html

[O01] 启动一个线程
来源：http://hz.jqgfzy.top/gtuminodus.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.kuanghao11.cn/gtlfdsfvsl.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.daria6918.cn/gtbowvhzkw.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.tanke756.top/gtazamuctf.html

TS:   // 同 JS
来源：http://hz.shzxlz.cn/gtrcmqvodp.html

Java: new Thread(() -> f()).start()
来源：http://hz.dianchejie.cn/gtjoqoauun.html

Go:   go f()
来源：http://hz.tian-w.cn/gtnlsvagra.html

Ruby: Thread.new { f }
来源：http://hz.nwbrower.top/gtxgfmnmyv.html

C#:   Task.Run(() => F());
来源：http://hz.jinyuanbaomall.cn/gtggufblce.html

[O02] 使用线程池
来源：http://hz.nanxinkj.top/gtvmnxohhl.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.cucudq.cn/gtshdljoja.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.dianchejie.cn/gtcuyjelrs.html

JS:   // worker_threads 线程池
来源：http://hz.cqqwz.cn/gtautyoudd.html

TS:   // worker_threads 线程池
来源：http://hz.yj20258.top/gtjnwgwzky.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.yangfankeji.com/gttirpsgqu.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.hywenlv.cn/gtdnhucrux.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.xingfuxueyuan.xyz/gthlmwubov.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.gotoacloud.top/gtnnuknyvb.html

[O03] 加锁保护共享数据
来源：http://hz.yj20258888.top/gthgrpehkr.html

Py:   with lock: shared += 1
来源：http://hz.shanyushiyangtech.top/gtyjcunjdl.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.cheryme.top/gtknmyohhe.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.pycfn.com/gtroquvfwv.html

TS:   // 同 JS
来源：http://hz.cucudq.cn/gtubeflypq.html

Java: synchronized (this) { shared++; }
来源：http://hz.c1oappe.top/gtcsaqesrh.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.yj202588.top/gtqohwnebq.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.shuidangran.top/gtudggmagj.html

C#:   lock (gate) { shared++; }
来源：http://hz.yj20258.top/gtvsyvbggc.html

[O04] 定义异步函数并等待
来源：http://hz.daxiang520.top/gtmavcivcp.html

Py:   async def f():⏎    await g()
来源：http://hz.9152youxi.cn/gtpfxhskur.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.iojbl.cn/gtjtrfyxpk.html

JS:   async function f() { await g(); }
来源：http://hz.zhijiandao.cn/gtnqxvucbu.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.nanxuanxn.top/gtbmnfszyb.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.gzhubu.top/gtbyjqodis.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.gaohongyu789.top/gtttzoqsol.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.hnxiangtu.top/gtnbqgtovx.html

C#:   async Task F() { await G(); }
来源：http://hz.jinyuanbaomall.cn/gtpcqrjjwu.html

[O05] 并发执行并等待全部完成
来源：http://hz.daria6918.cn/gtcgiidayf.html

Py:   asyncio.gather(*tasks)
来源：http://hz.ppjwa.cn/gteyoofcrs.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.jinghuilouyu.cn/gtgddaoogo.html

JS:   await Promise.all(tasks)
来源：http://hz.pycfn.com/gtyzcykqex.html

TS:   await Promise.all(tasks)
来源：http://hz.andypj.xyz/gtfafhweto.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.birdmap.top/gtntwaqbir.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.ybcxt.top/gtseqkfyhu.html

Ruby: threads.map(&:join)
来源：http://hz.chenzaomai.com/gtjrdnkrmg.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.zhengqikj.top/gtabytixbl.html

[O06] 使用进程池
来源：http://hz.chenjidiqi.icu/gtnooosyer.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.fzhhl.top/gtuqudopsz.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.guannengcc.top/gtrekgnzfa.html

JS:   // child_process / cluster 模块
来源：http://hz.ydjk.org.cn/gtezeokdep.html

TS:   // child_process / cluster 模块
来源：http://hz.yonumen.top/gtlogryrph.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.dashuyun.cn/gtooyjvsng.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.9152youxi.cn/gtxflqadwh.html

Ruby: // fork 块
来源：http://hz.wangshuangyany.cn/gtlsjsotwo.html

C#:   Parallel.For
来源：http://hz.iojbl.cn/gtvljiiqte.html

================================================================================
来源：http://hz.zhongyouzk.top/gtcgsfsrdw.html

P. 常用工具函数
来源：http://hz.andypj.xyz/gtzdwfkznt.html

================================================================================
来源：http://hz.chenzaomai.com/gtxwviqowd.html

[P01] 生成 UUID
来源：http://hz.tanke756.top/gtxwuhzxhi.html

Py:   str(uuid.uuid4())
来源：http://hz.xuanzx.com/gtselijnlw.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.redwolf501.top/gtpdsbptyl.html

JS:   crypto.randomUUID()
来源：http://hz.cqqwz.cn/gtqhrjlveg.html

TS:   crypto.randomUUID()
来源：http://hz.guowangkeji.top/gtpekdkdrt.html

Java: UUID.randomUUID().toString()
来源：http://hz.hysaishi.cn/gtdkxueqmb.html

Go:   // 用 github.com/google/uuid
来源：http://hz.yuanzhike.top/gtpzpsvlis.html

Ruby: SecureRandom.uuid
来源：http://hz.sufxvd.cn/gtqbxwfhwh.html


<!-- 参考信息 -->