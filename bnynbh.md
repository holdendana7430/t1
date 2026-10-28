代发 wailian999

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.dianchejie.cn/gtcuxhdncq.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.nwbrower.top/gticpstphp.html

[L05] 上传文件（multipart）
来源：http://hz.nwbrower.top/gtkhcakbca.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.nanxuanxn.top/gthhbuolkd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.guowangkeji.top/gtwmxrtwei.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.jianghu66.top/gtrzhdilul.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.jinyuanbaomall.cn/gtyocpjqfr.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.sysykeji.top/gtuohdpsql.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.c1oappe.top/gtczpaiizh.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.vqdsnc.cn/gtkedgcpyx.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.xuetiantiany.cn/gtiisrlcbg.html

[L06] 解析响应为 JSON
来源：http://hz.hnxiangtu.top/gtwgxglrxt.html

Py:   resp.json()
来源：http://hz.havefunace.top/gtmojoppkr.html

PHP:  json_decode($body, true);
来源：http://hz.daxiang520.top/gtnlgtoyla.html

JS:   await resp.json()
来源：http://hz.shangyingyoupin.top/gtpccduyjg.html

TS:   await resp.json()
来源：http://hz.iojbl.cn/gtqzzaebkk.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.haohaochexian.top/gtcumglobt.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.feifeiyinyue.top/gtokivxpoj.html

Ruby: JSON.parse(resp.body)
来源：http://hz.yj20258.top/gtizxvjyte.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.nanxuanxn.top/gtgvydlsja.html

[L07] 处理 HTTP 状态码
来源：http://hz.hfpthk.cn/gtjmxilmwd.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.yj20258.top/gtecjidjwe.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.dashuyun.cn/gtjmfxxrua.html

JS:   resp.ok;  resp.status
来源：http://hz.shuidangran.top/gtjpqcxvre.html

TS:   resp.ok;  resp.status
来源：http://hz.ybcxt.top/gthqehnatq.html

Java: resp.statusCode()
来源：http://hz.gzhubu.top/gtitzoxngx.html

Go:   resp.StatusCode
来源：http://hz.yj20258888.top/gtszkmttdx.html

Ruby: resp.code.to_i
来源：http://hz.0kj1m.cn/gtihjspfsl.html

C#:   (int)resp.StatusCode
来源：http://hz.52xcode.cn/gttrmivzun.html

[L08] 并发请求多个地址
来源：http://hz.gotoacloud.top/gtqorvboyi.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.zhixingplan.top/gtppfrmmpc.html

PHP:  curl_multi_init() 系列
来源：http://hz.yj202588.top/gtheosraha.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.ywan-chungtsiang.top/gtngtiaasj.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhaomingkeji.xyz/gtqxzyhvhv.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.xziqi.cn/gtyeqwxkuj.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.xylfe.cn/gtrabbqrdk.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.zhongyouzk.top/gtvwkavpza.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.jyoumei.cn/gtcnongpen.html

================================================================================
来源：http://hz.meibo888.top/gtcnyrgiob.html

M. 命令行 / 进程 / 环境
来源：http://hz.guannengcc.top/gtfhhjqlzj.html

================================================================================
来源：http://hz.gzhubu.top/gtcijulqpv.html

[M01] 读取命令行参数
来源：http://hz.ywan-chungtsiang.top/gtpjxvegxo.html

Py:   sys.argv[1:]
来源：http://hz.tianlin.xyz/gtavlppyls.html

PHP:  $argv;  $argc;
来源：http://hz.sxryk.cn/gttprwxifv.html

JS:   process.argv.slice(2)
来源：http://hz.nwbrower.top/gttyqtvidl.html

TS:   process.argv.slice(2)
来源：http://hz.zhijiandao.cn/gtllpazbgt.html

Java: args 数组（main 方法参数）
来源：http://hz.shzxlz.cn/gtrfrbazjo.html

Go:   os.Args[1:]
来源：http://hz.zhongyouzk.top/gtfzoqbdnk.html

Ruby: ARGV
来源：http://hz.zdqjudy.top/gtvxblbjnt.html

C#:   args 数组（Main 方法参数）
来源：http://hz.quarkkingdee.top/gteazreycq.html

[M02] 读取环境变量
来源：http://hz.ywan-chungtsiang.top/gtknqzbcju.html

Py:   os.environ.get("HOME")
来源：http://hz.birdmap.top/gtevnrvezz.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.nwbrower.top/gtnsuxibaq.html

JS:   process.env.HOME
来源：http://hz.jinghuilouyu.cn/gtetyasqdo.html

TS:   process.env.HOME
来源：http://hz.bjfxy.top/gtorvtymgi.html

Java: System.getenv("HOME")
来源：http://hz.gotoacloud.top/gtsqwkyfzn.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.haohaochexian.top/gtpvsijtut.html

Ruby: ENV["HOME"]
来源：http://hz.guowangkeji.top/gthcqfukce.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.shanyushiyangkeji.top/gtjbdoctlz.html

[M03] 执行外部命令
来源：http://hz.xuetiantiany.cn/gtzrybjrle.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.yvedp.cn/gtshfpxjvw.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.gzhubu.top/gtrkbnmyft.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.chenjidiqi.icu/gtslyhawre.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.shuidangran.top/gtapbteofc.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.yanxiufei.cn/gtrfqthvvo.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.hongshengwenyu.top/gtvwzgllmu.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.vqdsnc.cn/gtjwtlmayw.html

C#:   Process.Start("ls", "-l");
来源：http://hz.hysaishi.cn/gthvmhannt.html

[M04] 获取当前工作目录
来源：http://hz.vqdsnc.cn/gtyzrolsuu.html

Py:   os.getcwd()
来源：http://hz.hysaishi.cn/gtyotgiyti.html

PHP:  getcwd();
来源：http://hz.yongpay.top/gtxzrwhxqd.html

JS:   process.cwd()
来源：http://hz.havefunace.top/gtaxoennbl.html

TS:   process.cwd()
来源：http://hz.shanyushiyangkeji.top/gtpujcowxo.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.xuanzx.com/gtyxpspmgy.html

Go:   os.Getwd()
来源：http://hz.yuxming.cn/gttbmqycqk.html

Ruby: Dir.pwd
来源：http://hz.xuanzx.com/gtedawikzl.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.gzhubu.top/gtnuabchjb.html

[M05] 设置退出码
来源：http://hz.c1oappe.top/gtqvddjsos.html

Py:   sys.exit(1)
来源：http://hz.haohaochexian.top/gttvpexyeq.html

PHP:  exit(1);
来源：http://hz.hysaishi.cn/gtzbfyhlhd.html

JS:   process.exit(1)
来源：http://hz.ywan-chungtsiang.top/gtecvfkjxd.html

TS:   process.exit(1)
来源：http://hz.hysaishi.cn/gttciheool.html

Java: System.exit(1)
来源：http://hz.jinqigfzy.top/gtbcrpiizl.html

Go:   os.Exit(1)
来源：http://hz.jinqigufen.top/gtcxwkkdde.html

Ruby: exit 1
来源：http://hz.c1oappe.top/gtfdxqejou.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.chenlongwang.top/gtplxyfkid.html

[M06] 向标准错误输出
来源：http://hz.dashuyun.cn/gtskgfndey.html

Py:   print("err", file=sys.stderr)
来源：http://hz.meibo888.top/gtaapzfgre.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.mhx1999.top/gtgerpwsgb.html

JS:   console.error("err")
来源：http://hz.ybcxt.top/gttqtitasi.html

TS:   console.error("err")
来源：http://hz.zhengqikj.top/gtbrdlzlyb.html

Java: System.err.println("err")
来源：http://hz.andypj.xyz/gtiasuwale.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.cheryme.top/gtxsfgfbhq.html

Ruby: warn "err"
来源：http://hz.cashguo.top/gtggyruhcd.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.shzxlz.cn/gtikjslmrp.html

[M07] 判断是否为主入口
来源：http://hz.yvedp.cn/gtxpyhwhsz.html

Py:   if __name__ == "__main__":
来源：http://hz.hywenlv.cn/gtgljwccvm.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.shanyushiyangtech.top/gtdumsqhwp.html

JS:   require.main === module
来源：http://hz.chenzaomai.com/gtdphfcamf.html

TS:   require.main === module
来源：http://hz.tanke756.top/gtfmgeonmr.html

Java: public static void main(String[] args)
来源：http://hz.gaohongyu789.top/gtljflburr.html

Go:   func main()
来源：http://hz.kuanghao11.cn/gtcvfgufdp.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.daxiang520.top/gtjpgvzlmv.html

C#:   static void Main(string[] args)
来源：http://hz.fengsongda.top/gtkxoloyql.html

[M08] 获取系统与运行时信息
来源：http://hz.xinyue.icu/gtrptnehon.html

Py:   platform.system();  platform.python_version()
来源：http://hz.ppjwa.cn/gtfolwqmwd.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.dashuyun.cn/gtoymrepuh.html

JS:   process.platform;  process.version
来源：http://hz.pycfn.com/gtpogoxwfd.html

TS:   process.platform;  process.version
来源：http://hz.316326.xyz/gtasscvrcp.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.aibaodan.cn/gtdnegyzqa.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.xylfe.cn/gtxjomanvr.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.meibo888.top/gtprvnjgwd.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.yj202588.top/gtmqretsxq.html

================================================================================
来源：http://hz.jinqigfzy.top/gtokleseeh.html

N. 数据结构与算法
来源：http://hz.kuanghao11.cn/gtgqtboneo.html

================================================================================
来源：http://hz.hywenlv.cn/gtbjcljspz.html

[N01] 二分查找（有序数组）
来源：http://hz.hongshengwenyu.top/gtqykbsrat.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.shanyushiyangtech.top/gtyxkplucy.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.gotoacloud.top/gtvxyvtsgf.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jiagoushi.top/gtveeqbkcv.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.nanxuanxn.top/gtsifambhu.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.vqdsnc.cn/gtijvnhgem.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.hammf.cn/gthpmyyrec.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.svipenyu.cn/gtmuumnvde.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.nwbrower.top/gtggdxywbc.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.sufxvd.cn/gtytjrifhd.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.wangdashe.top/gtxhvpnnbl.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.gotoacloud.top/gtjrqupfgz.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yuxming.cn/gtogbmbtag.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.tian-w.cn/gtdjciweaz.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.haohaochexian.top/gtkwkbwvpy.html

Go:   slices.Sort(arr)
来源：http://hz.redwolf501.top/gtufaombbq.html

Ruby: arr.sort
来源：http://hz.daxiang520.top/gtgvnledrx.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.vqdsnc.cn/gtcozcwlmt.html

[N03] 快速排序（分治示例）
来源：http://hz.fzhhl.top/gtnvpbmuck.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.yuxming.cn/gtteczukco.html

PHP:  // 递归实现，或用 usort
来源：http://hz.shzxlz.cn/gtfoaohbxw.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.xinyue.icu/gtaudiltat.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zhiwuduotai.top/gtsytbueeq.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.chenlongwang.top/gtdfffnvlm.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.jiagoushi.top/gtejikwhgh.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.sweek.top/gtufmupszi.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.feifeiyinyue.top/gtukfemnld.html

[N04] 斐波那契数列
来源：http://hz.zdqjudy.top/gtjerqdhuq.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.zhengqikj.top/gtftsuqdhk.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.smart0.xyz/gtwdebqjmi.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.tian-w.cn/gthsugobbh.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jinghuilouyu.cn/gttmsgzajz.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.jinyuanbaomall.cn/gtufkossha.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.svipenyu.cn/gtsljppvth.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.havefunace.top/gtsnjahjpl.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.yangfankeji.com/gtkquxdxkg.html

[N05] 最大公约数
来源：http://hz.ybcxt.top/gtsghzssgr.html

Py:   math.gcd(a, b)
来源：http://hz.yuxming.cn/gtypkqoasn.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.aizwys.cn/gtmmkxysrz.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.zhijiandao.cn/gthgwllufj.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.xuetiantiany.cn/gtikmaercy.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.ydzc1.top/gtdgjijezv.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.zhongyouzk.top/gtaqxsbjpr.html

Ruby: a.gcd(b)
来源：http://hz.nanxinkj.top/gtxwoumvcg.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.zhoulong.xyz/gtgfulndmt.html

[N06] 判断回文字符串
来源：http://hz.kuanghao11.cn/gtnkktvgds.html

Py:   s == s[::-1]
来源：http://hz.52xcode.cn/gtosudvfol.html

PHP:  $s === strrev($s);
来源：http://hz.dashuyun.cn/gtkdhukxxd.html

JS:   s === [...s].reverse().join("")
来源：http://hz.jlsjyb.cn/gtklluogrp.html

TS:   s === [...s].reverse().join("")
来源：http://hz.hnqzz.top/gttppmcwzi.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.dianchejie.cn/gtgvjdbdxx.html

Go:   // 双指针从两端比较
来源：http://hz.zhengqikj.top/gtwfwrekze.html

Ruby: s == s.reverse
来源：http://hz.ppjwa.cn/gtyhaxpooo.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.hongshengwenyu.top/gtyuemiixw.html

[N07] 两数之和（返回下标）
来源：http://hz.ehwqpu.com/gtztnimdwq.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.xuetiantiany.cn/gtmuxhmwzj.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.birdmap.top/gtjeldltzh.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.sufxvd.cn/gtujhirnew.html

TS:   // 手写 Map<string, number>
来源：http://hz.chenlongwang.top/gtbgyddcyl.html

Java: // 手写 HashMap
来源：http://hz.redwolf501.top/gtbxpkkigc.html

Go:   // 手写 map[int]int
来源：http://hz.ehwqpu.com/gtjkfwwxbf.html

Ruby: // 手写 Hash
来源：http://hz.xuanzx.com/gtlnntkszb.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.yvedp.cn/gtmbwpnjly.html

[N08] 生成全排列
来源：http://hz.vqdsnc.cn/gtyandhhtz.html

Py:   itertools.permutations(arr)
来源：http://hz.hfpthk.cn/gtxtsesirn.html

PHP:  // 手写递归交换
来源：http://hz.jinqigfzy.top/gtumfiyorh.html

JS:   // 手写回溯递归
来源：http://hz.9152youxi.cn/gtwwkfzdnl.html

TS:   // 手写回溯递归
来源：http://hz.vqdsnc.cn/gtofwlfxhq.html

Java: // 手写回溯递归
来源：http://hz.jinqigufen.top/gtnqpalaue.html

Go:   // 手写回溯递归
来源：http://hz.ywan-chungtsiang.top/gtbxrbfooq.html

Ruby: arr.permutation.to_a
来源：http://hz.aibaodan.cn/gtlwsozphr.html

C#:   // 手写回溯递归
来源：http://hz.pengpengdd.cyou/gtueduavld.html

[N09] 栈与队列
来源：http://hz.havefunace.top/gtjxxorxre.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.hongshengwenyu.top/gtwtziojhc.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.aibaodan.cn/gtejlwlipw.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.yonumen.top/gtheabrbob.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.yuanzhike.top/gtrekxkkbl.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.cqqwz.cn/gtptytkhhq.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.yuanzhike.top/gtdjfigewk.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.shanyushiyangtech.top/gtzsfluqwr.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.quarkkingdee.top/gtpeijwxxc.html

[N10] 链表节点定义
来源：http://hz.yueranfly.top/gtduwfuvft.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.birdmap.top/gtbrcjtlbs.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.meibo888.top/gtekjitplx.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.ywan-chungtsiang.top/gtboktmtok.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.dianchejie.cn/gtdfahhlok.html

Java: class Node { int v; Node next; }
来源：http://hz.birdmap.top/gtfrjxbnaa.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.jqgufenzy.top/gtbzvngrpr.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.meibo888.top/gtlzwhwvdt.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.zhixingplan.top/gtcbahlpyf.html

[N11] 二叉树中序遍历
来源：http://hz.zycfv.cn/gtygxmhwlm.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.9152youxi.cn/gtncpaonjt.html

PHP:  // 手写递归函数
来源：http://hz.yj20258888.top/gtattkcour.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.svipenyu.cn/gtbsulhygz.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yvedp.cn/gtbduijghs.html

Java: // 手写递归
来源：http://hz.shanyushiyangkeji.top/gtxcyaydmf.html

Go:   // 手写递归
来源：http://hz.gotoacloud.top/gtxvxheooq.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.wangdashe.top/gtgiaywznw.html

C#:   // 手写递归
来源：http://hz.xingfuxueyuan.xyz/gtjhptivvy.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.bjfxy.top/gtpjtvxakz.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.gotoacloud.top/gtkoqsenyq.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.jianghu66.top/gtgnefjkku.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.shzxlz.cn/gtxnsfjluq.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.tianlin.xyz/gtfqabzljf.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.jiagoushi.top/gtzfkvirda.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.ppjwa.cn/gtiprocbkw.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.yonumen.top/gttipesqaf.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.cashguo.top/gtwtleohfr.html

================================================================================
来源：http://hz.316326.xyz/gtminxepda.html

O. 并发与异步
来源：http://hz.ydzc1.top/gtctwzqqsu.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtwtumydgr.html

[O01] 启动一个线程
来源：http://hz.xingfuxueyuan.xyz/gtyvhypkzh.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.daria6918.cn/gtcnvhdggy.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.xylfe.cn/gtejzqpxot.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.tianlin.xyz/gtoyzqdizl.html

TS:   // 同 JS
来源：http://hz.gaohongyu789.top/gtokihymvr.html

Java: new Thread(() -> f()).start()
来源：http://hz.aizwys.cn/gtphndsxnr.html

Go:   go f()
来源：http://hz.jiagoushi.top/gtgjttyonn.html

Ruby: Thread.new { f }
来源：http://hz.tianlin.xyz/gtsmspcaaa.html

C#:   Task.Run(() => F());
来源：http://hz.jqgfzy.top/gtzhzaflhx.html

[O02] 使用线程池
来源：http://hz.yuxming.cn/gteoinsqfp.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.xingfuxueyuan.xyz/gtzgdatadw.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.mhx1999.top/gtwjgukrlg.html

JS:   // worker_threads 线程池
来源：http://hz.tanke756.top/gtkknczjmn.html

TS:   // worker_threads 线程池
来源：http://hz.wangshuangyany.cn/gttwinqdki.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.gzhubu.top/gtlvyateyq.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.cqqwz.cn/gtcrpbhptj.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.tanke756.top/gtmkugdhwt.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.316326.xyz/gtfarakzgy.html

[O03] 加锁保护共享数据
来源：http://hz.xylfe.cn/gtszxkusse.html

Py:   with lock: shared += 1
来源：http://hz.sxryk.cn/gtzpgtuhei.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.zhijiandao.cn/gtoztxtzfr.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.9152youxi.cn/gtiamudqme.html

TS:   // 同 JS
来源：http://hz.jinghuilouyu.cn/gthgjllwmz.html

Java: synchronized (this) { shared++; }
来源：http://hz.andypj.xyz/gtwqqetbaf.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.jinyuanbaomall.cn/gtbgvfjqin.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.ppjwa.cn/gtsqjwiaff.html

C#:   lock (gate) { shared++; }
来源：http://hz.hongshengwenyu.top/gtcaqmphie.html

[O04] 定义异步函数并等待
来源：http://hz.pycfn.com/gthyxkrtgx.html

Py:   async def f():⏎    await g()
来源：http://hz.zdqjudy.top/gtqkfnhugv.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.wangshuangyany.cn/gtrutflhio.html

JS:   async function f() { await g(); }
来源：http://hz.zhaomingkeji.xyz/gttyzmnsal.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.redwolf501.top/gtsddwrzhl.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.ivvv.top/gtrvldsicj.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.jianghu66.top/gtvzosrviq.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.sysykeji.top/gtsfmvhydv.html

C#:   async Task F() { await G(); }
来源：http://hz.shuidangran.top/gtxatngtoh.html

[O05] 并发执行并等待全部完成
来源：http://hz.wangdashe.top/gtbrzspseu.html

Py:   asyncio.gather(*tasks)
来源：http://hz.yuxming.cn/gtbjfomaui.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.zhongyouzk.top/gtjbzrzjdo.html

JS:   await Promise.all(tasks)
来源：http://hz.yvedp.cn/gtjvhudkga.html

TS:   await Promise.all(tasks)
来源：http://hz.yuanzhike.top/gtobfrxgkt.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.bjfxy.top/gtchjrfjtm.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.xingfuxueyuan.xyz/gtdxhygvjt.html

Ruby: threads.map(&:join)
来源：http://hz.jinqigfzy.top/gtcsavgnzr.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.xinyue.icu/gtpfgrusvv.html

[O06] 使用进程池
来源：http://hz.xuetiantiany.cn/gtyblbkwop.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.yj202588.top/gtbbgnhget.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.jinyuanbaomall.cn/gtjhqssmzi.html

JS:   // child_process / cluster 模块
来源：http://hz.9152youxi.cn/gtablrkwyg.html

TS:   // child_process / cluster 模块
来源：http://hz.sufxvd.cn/gtoojqksby.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.hysaishi.cn/gtrtnbjwam.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.hywenlv.cn/gtsgpqrzkn.html

Ruby: // fork 块
来源：http://hz.c1oappe.top/gtqqkckivf.html

C#:   Parallel.For
来源：http://hz.xziqi.cn/gtsvhskmfr.html

================================================================================
来源：http://hz.jqgufenzy.top/gtzhtulybu.html

P. 常用工具函数
来源：http://hz.yangfankeji.com/gtzkswrbcs.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtwplplhak.html

[P01] 生成 UUID
来源：http://hz.cqqwz.cn/gtewjuvtes.html

Py:   str(uuid.uuid4())
来源：http://hz.jiagoushi.top/gtytzbhenk.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.gzhubu.top/gtwuaidafm.html

JS:   crypto.randomUUID()
来源：http://hz.cucudq.cn/gtjlclnrfb.html

TS:   crypto.randomUUID()
来源：http://hz.aibaodan.cn/gtpiiziwnr.html

Java: UUID.randomUUID().toString()
来源：http://hz.316326.xyz/gtjnbidfxf.html

Go:   // 用 github.com/google/uuid
来源：http://hz.jiagoushi.top/gtplppckvc.html

Ruby: SecureRandom.uuid
来源：http://hz.316326.xyz/gtgqguztez.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.zdqjudy.top/gtazseclvk.html

[P02] MD5 / SHA256 摘要
来源：http://hz.andypj.xyz/gtqfgirmce.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.smart0.xyz/gttcsznaeb.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.wangdashe.top/gtkdedzlum.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hz.sysykeji.top/gtjhyuvmxy.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hz.tianlin.xyz/gtqhutfhjz.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hz.iojbl.cn/gtfmjuqwdd.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hz.svipenyu.cn/gtyrhhptrj.html


<!-- 参考信息 -->