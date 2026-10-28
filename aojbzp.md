代发 wailian999

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.gogol.net.cn/gtpylfkrzr.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yj202588.top/gtbtppnujt.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.xylfe.cn/gtfjuzdvsb.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.hnxiangtu.top/gtbuedfaub.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.gzhubu.top/gtopazybud.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.ehwqpu.com/gtgtfpnbyi.html

[L05] 上传文件（multipart）
来源：http://hz.ppjwa.cn/gtpyqrzxvh.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.mhx1999.top/gtuzmkvwdy.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.xuetiantiany.cn/gtwzrrtuyr.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.gaohongyu789.top/gtamrzhcvb.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.tanke756.top/gtigcgyhqs.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.aizwys.cn/gtxpgoahwk.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.chenjidiqi.icu/gtoednuacm.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.nwbrower.top/gtaonpcvfq.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.tianlin.xyz/gtxvizqcwn.html

[L06] 解析响应为 JSON
来源：http://hz.birdmap.top/gtvekghmmw.html

Py:   resp.json()
来源：http://hz.hammf.cn/gtfbnwmrjh.html

PHP:  json_decode($body, true);
来源：http://hz.ydzc1.top/gtussclbff.html

JS:   await resp.json()
来源：http://hz.jlsjyb.cn/gtqmvgltvi.html

TS:   await resp.json()
来源：http://hz.daxiang520.top/gtbqfzpism.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.chenzaomai.com/gtlvsrmwxq.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.pengpengdd.cyou/gtbinppgai.html

Ruby: JSON.parse(resp.body)
来源：http://hz.cucudq.cn/gtludljzts.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.tian-w.cn/gtwufuywtf.html

[L07] 处理 HTTP 状态码
来源：http://hz.yongpay.top/gtmayfosof.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.guowangkeji.top/gtuydocuwy.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.smart0.xyz/gtdavnyylp.html

JS:   resp.ok;  resp.status
来源：http://hz.cashguo.top/gtzgcsqmol.html

TS:   resp.ok;  resp.status
来源：http://hz.yangfankeji.com/gtsvwgeutm.html

Java: resp.statusCode()
来源：http://hz.hammf.cn/gtddoctbpe.html

Go:   resp.StatusCode
来源：http://hz.jinghuilouyu.cn/gtiyozanfc.html

Ruby: resp.code.to_i
来源：http://hz.ydjk.org.cn/gtiwkcfjmt.html

C#:   (int)resp.StatusCode
来源：http://hz.aizwys.cn/gtsdozraef.html

[L08] 并发请求多个地址
来源：http://hz.316326.xyz/gtakfuuvgk.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.mhx1999.top/gttigelmhd.html

PHP:  curl_multi_init() 系列
来源：http://hz.yvedp.cn/gtiehddzxs.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.birdmap.top/gthviczuwc.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.chenjidiqi.icu/gtsdvccety.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.ehwqpu.com/gtunsuzzuq.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.wangshuangyany.cn/gtzbbzebzr.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.zdqjudy.top/gtxxhyqsqm.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.ppjwa.cn/gtyvqbkhmz.html

================================================================================
来源：http://hz.gzhubu.top/gtusexcszg.html

M. 命令行 / 进程 / 环境
来源：http://hz.hnxiangtu.top/gtfbyqvieg.html

================================================================================
来源：http://hz.ybcxt.top/gtgejmmtca.html

[M01] 读取命令行参数
来源：http://hz.cucudq.cn/gtnbuezftj.html

Py:   sys.argv[1:]
来源：http://hz.jqgufenzy.top/gtlppvwirl.html

PHP:  $argv;  $argc;
来源：http://hz.zhoulong.xyz/gtyufmxfur.html

JS:   process.argv.slice(2)
来源：http://hz.jinqigufen.top/gtrvzupwsy.html

TS:   process.argv.slice(2)
来源：http://hz.zdqjudy.top/gtxesunbva.html

Java: args 数组（main 方法参数）
来源：http://hz.andypj.xyz/gtqmhvrmjx.html

Go:   os.Args[1:]
来源：http://hz.jianghu66.top/gtqlmmaukr.html

Ruby: ARGV
来源：http://hz.yvedp.cn/gtqurejkte.html

C#:   args 数组（Main 方法参数）
来源：http://hz.haohaochexian.top/gtxwlbceiv.html

[M02] 读取环境变量
来源：http://hz.nanxuanxn.top/gtfzvhdgqx.html

Py:   os.environ.get("HOME")
来源：http://hz.xinyue.icu/gtoqfpwdxq.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.meibo888.top/gtkzvfdkoj.html

JS:   process.env.HOME
来源：http://hz.sweek.top/gtcnufmfra.html

TS:   process.env.HOME
来源：http://hz.sweek.top/gttznrowmr.html

Java: System.getenv("HOME")
来源：http://hz.hywenlv.cn/gtkrahjwcz.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.guannengcc.top/gtekyuvgst.html

Ruby: ENV["HOME"]
来源：http://hz.jqgufenzy.top/gtjagnocba.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.bjfxy.top/gtlifwekxc.html

[M03] 执行外部命令
来源：http://hz.cdnleiting.top/gteuoefrzp.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.zycfv.cn/gturyucrkl.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.ywan-chungtsiang.top/gtxhbyljbu.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.birdmap.top/gtnxxmvgbd.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.shangyingyoupin.top/gtfqkcczgl.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.wangdashe.top/gtuxzldhud.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.ybcxt.top/gtbrwimbbc.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.bjfxy.top/gtqkgjulkm.html

C#:   Process.Start("ls", "-l");
来源：http://hz.ywan-chungtsiang.top/gtlglrxbnn.html

[M04] 获取当前工作目录
来源：http://hz.jinyuanbaomall.cn/gtdcmuuong.html

Py:   os.getcwd()
来源：http://hz.fzhhl.top/gtispkztdn.html

PHP:  getcwd();
来源：http://hz.shzxlz.cn/gtmrhihrko.html

JS:   process.cwd()
来源：http://hz.jlsjyb.cn/gtndwdacud.html

TS:   process.cwd()
来源：http://hz.gzhubu.top/gtqfvehpqv.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.andypj.xyz/gtdbuuzjqp.html

Go:   os.Getwd()
来源：http://hz.ppjwa.cn/gtkpbfezdn.html

Ruby: Dir.pwd
来源：http://hz.hfpthk.cn/gtpbehlmvk.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.jiagoushi.top/gtfwbchjeo.html

[M05] 设置退出码
来源：http://hz.chenjidiqi.icu/gtexxfnxlc.html

Py:   sys.exit(1)
来源：http://hz.ehwqpu.com/gtykczpzeu.html

PHP:  exit(1);
来源：http://hz.kuanghao11.cn/gthljpwnvd.html

JS:   process.exit(1)
来源：http://hz.pengpengdd.cyou/gtqyiltxnl.html

TS:   process.exit(1)
来源：http://hz.sxryk.cn/gtsrexdppg.html

Java: System.exit(1)
来源：http://hz.hywenlv.cn/gtvuisfsse.html

Go:   os.Exit(1)
来源：http://hz.snrcjt.cn/gtjzpllewd.html

Ruby: exit 1
来源：http://hz.yanxiufei.cn/gtaaaqyzod.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.kuanghao11.cn/gtgqlczhfb.html

[M06] 向标准错误输出
来源：http://hz.zhijiandao.cn/gtkoqgmdby.html

Py:   print("err", file=sys.stderr)
来源：http://hz.chenlongwang.top/gtutwkqrqb.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.sufxvd.cn/gtkvdhoekw.html

JS:   console.error("err")
来源：http://hz.yj202588.top/gtdubfohpa.html

TS:   console.error("err")
来源：http://hz.jiagoushi.top/gtlhttehxs.html

Java: System.err.println("err")
来源：http://hz.jiagoushi.top/gtegnrbbzt.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.shangyingyoupin.top/gtqzfdnekg.html

Ruby: warn "err"
来源：http://hz.tian-w.cn/gtasrqcusf.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.9152youxi.cn/gtmxnqqbct.html

[M07] 判断是否为主入口
来源：http://hz.kuanghao11.cn/gttxofnluc.html

Py:   if __name__ == "__main__":
来源：http://hz.jlsjyb.cn/gtctjxjtic.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.zdqjudy.top/gtesuwvscj.html

JS:   require.main === module
来源：http://hz.guannengcc.top/gtcujyphqd.html

TS:   require.main === module
来源：http://hz.quarkkingdee.top/gtgvepyanw.html

Java: public static void main(String[] args)
来源：http://hz.yongpay.top/gtgpcvnrvq.html

Go:   func main()
来源：http://hz.sweek.top/gtvoasqlde.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.cqqwz.cn/gtulsqjwjb.html

C#:   static void Main(string[] args)
来源：http://hz.bjfxy.top/gttjtoknnz.html

[M08] 获取系统与运行时信息
来源：http://hz.jiagoushi.top/gtoftvyxyy.html

Py:   platform.system();  platform.python_version()
来源：http://hz.zhiwuduotai.top/gttcntydpz.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.ywan-chungtsiang.top/gteiugonfp.html

JS:   process.platform;  process.version
来源：http://hz.nanxuanxn.top/gtliiwnxvu.html

TS:   process.platform;  process.version
来源：http://hz.pengpengdd.cyou/gtaydxcrah.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.bjfxy.top/gtdjemkzuc.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.9152youxi.cn/gthiftkosk.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.nwbrower.top/gtxfjjmkuq.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.yvedp.cn/gthlrdszor.html

================================================================================
来源：http://hz.nanxinkj.top/gtwssifzej.html

N. 数据结构与算法
来源：http://hz.meibo888.top/gtidufjuww.html

================================================================================
来源：http://hz.zycfv.cn/gtoxqvculb.html

[N01] 二分查找（有序数组）
来源：http://hz.jyoumei.cn/gtqkkfetyt.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.ybcxt.top/gtvmprfydo.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.bjfxy.top/gtfcrhkqzr.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.wangdashe.top/gtslmohujn.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jinqigfzy.top/gtxlsgruhf.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.chenzaomai.com/gtoubxdweq.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.sxryk.cn/gtjwuyvrbx.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.hywenlv.cn/gtiultcjow.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.gaohongyu789.top/gtrqoasglz.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.sweek.top/gtccphampm.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.zhongyouzk.top/gtblpkricc.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.sxryk.cn/gtkauphhcd.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yueranfly.top/gtztexpfjq.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.sysykeji.top/gtruxywxne.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.ppjwa.cn/gtzimmudcw.html

Go:   slices.Sort(arr)
来源：http://hz.feifeiyinyue.top/gtrpbpynoy.html

Ruby: arr.sort
来源：http://hz.pengpengdd.cyou/gtxwcgmkfn.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.svipenyu.cn/gtrknlqynp.html

[N03] 快速排序（分治示例）
来源：http://hz.cqqwz.cn/gtlbjdkrsi.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.ppjwa.cn/gthhkixuix.html

PHP:  // 递归实现，或用 usort
来源：http://hz.gaohongyu789.top/gtzqpkapsu.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jinghuilouyu.cn/gttojdjjkb.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.hfpthk.cn/gtiaddfzaj.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.jinqigfzy.top/gtwcenvoao.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.nanxuanxn.top/gtvubiuaoi.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.xylfe.cn/gtaludffls.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.meibo888.top/gtrvssniye.html

[N04] 斐波那契数列
来源：http://hz.shangyingyoupin.top/gtmywinynx.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.yonumen.top/gtuynpfpwe.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.sweek.top/gtaqygeizu.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.ybcxt.top/gtmuayquka.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.redwolf501.top/gtpykmbjgi.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.guowangkeji.top/gtilyahukg.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.0kj1m.cn/gteiuscwqd.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.zhoulong.xyz/gtsbwfrgtb.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.daxiang520.top/gtsepwxfnp.html

[N05] 最大公约数
来源：http://hz.fzhhl.top/gtxnerisqv.html

Py:   math.gcd(a, b)
来源：http://hz.pengpengdd.cyou/gtcvbimvuo.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.chenjidiqi.icu/gtivkyiaza.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.chenzaomai.com/gtzjwrtgwe.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.xylfe.cn/gtswzadhki.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.jiagoushi.top/gtkbyfhcnf.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.andypj.xyz/gtvapprrup.html

Ruby: a.gcd(b)
来源：http://hz.redwolf501.top/gtbatbraxg.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.hywenlv.cn/gtmbuchroy.html

[N06] 判断回文字符串
来源：http://hz.snrcjt.cn/gtyhfesleh.html

Py:   s == s[::-1]
来源：http://hz.gzhubu.top/gtiqgrqgaf.html

PHP:  $s === strrev($s);
来源：http://hz.zycfv.cn/gtnyvmdpwx.html

JS:   s === [...s].reverse().join("")
来源：http://hz.jlsjyb.cn/gtlbvxtsta.html

TS:   s === [...s].reverse().join("")
来源：http://hz.jinghuilouyu.cn/gtbbmjyueu.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.9152youxi.cn/gtvzjcchdd.html

Go:   // 双指针从两端比较
来源：http://hz.haohaochexian.top/gtwvzdporo.html

Ruby: s == s.reverse
来源：http://hz.cdnleiting.top/gtfpbpwgbm.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.xinyue.icu/gtfiqqyddw.html

[N07] 两数之和（返回下标）
来源：http://hz.quarkkingdee.top/gtdrzxbodp.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.feifeiyinyue.top/gtnghyffze.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.ybcxt.top/gtswgahtur.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.zhengqikj.top/gtxogpvbjo.html

TS:   // 手写 Map<string, number>
来源：http://hz.cqqwz.cn/gtqozrmsby.html

Java: // 手写 HashMap
来源：http://hz.chenzaomai.com/gtthkqzjzn.html

Go:   // 手写 map[int]int
来源：http://hz.zhongyouzk.top/gtewnggtqz.html

Ruby: // 手写 Hash
来源：http://hz.daria6918.cn/gtnglqkgao.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.jianghu66.top/gthkyudoyt.html

[N08] 生成全排列
来源：http://hz.wangshuangyany.cn/gtrafnjztc.html

Py:   itertools.permutations(arr)
来源：http://hz.zhixingplan.top/gtfubwjcvu.html

PHP:  // 手写递归交换
来源：http://hz.yj202588.top/gtcumglypp.html

JS:   // 手写回溯递归
来源：http://hz.cashguo.top/gtchouuydq.html

TS:   // 手写回溯递归
来源：http://hz.yanxiufei.cn/gttevbuxnh.html

Java: // 手写回溯递归
来源：http://hz.aibaodan.cn/gtifisjxmv.html

Go:   // 手写回溯递归
来源：http://hz.gotoacloud.top/gtaswgqhso.html

Ruby: arr.permutation.to_a
来源：http://hz.316326.xyz/gtrqwhrzkg.html

C#:   // 手写回溯递归
来源：http://hz.tianlin.xyz/gtoqxjrypq.html

[N09] 栈与队列
来源：http://hz.shanyushiyangkeji.top/gtwexksjhi.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.sxryk.cn/gtcoxlfyhd.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.smart0.xyz/gtlxztzgue.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.zhijiandao.cn/gtbepgfihw.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.yanxiufei.cn/gtirzqnors.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.yangfankeji.com/gtzssdiusx.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.yanxiufei.cn/gtxhouqssr.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.nanxinkj.top/gtzyubgdyr.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.gzhubu.top/gtpesbhgkg.html

[N10] 链表节点定义
来源：http://hz.yonumen.top/gtgsuilrwz.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.c1oappe.top/gtasedksyt.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.daria6918.cn/gtgtcwtlqj.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.shanyushiyangkeji.top/gtviujranj.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.cqqwz.cn/gtvihxjcqy.html

Java: class Node { int v; Node next; }
来源：http://hz.gotoacloud.top/gtyotncaae.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.haohaochexian.top/gtzsdemrld.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.ydjk.org.cn/gtebquader.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.cdnleiting.top/gtzfzumklh.html

[N11] 二叉树中序遍历
来源：http://hz.dashuyun.cn/gtfjyektzc.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.shanyushiyangkeji.top/gtjamlppyj.html

PHP:  // 手写递归函数
来源：http://hz.cdnleiting.top/gtleoaowlb.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.hnxiangtu.top/gtlbrodcnn.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.meibo888.top/gtxgsubmwg.html

Java: // 手写递归
来源：http://hz.ivvv.top/gttpybhtra.html

Go:   // 手写递归
来源：http://hz.fengsongda.top/gtsqxxhoau.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.pengpengdd.cyou/gtnblpivnk.html

C#:   // 手写递归
来源：http://hz.zhiwuduotai.top/gtwplxjpyk.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.svipenyu.cn/gtoyqzkzbe.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.0kj1m.cn/gtoilggbyv.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.pengpengdd.cyou/gtiojnmmrn.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.hnxiangtu.top/gtnsuzdvgf.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.chenzaomai.com/gtiilitwix.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.zhiwuduotai.top/gtgqecbocq.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.chenzaomai.com/gtynarumod.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.cucudq.cn/gthlxkuiyv.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.0kj1m.cn/gtiwrokmis.html

================================================================================
来源：http://hz.ehwqpu.com/gtxmtlmoon.html

O. 并发与异步
来源：http://hz.xuetiantiany.cn/gtgattpwha.html

================================================================================
来源：http://hz.cqqwz.cn/gtqsehmudd.html

[O01] 启动一个线程
来源：http://hz.jinyuanbaomall.cn/gtyqnumgih.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.xuanzx.com/gteyygrpqc.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.shanyushiyangkeji.top/gtyltdtmeh.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.jinqigfzy.top/gteixzztos.html

TS:   // 同 JS
来源：http://hz.sweek.top/gteclvmbqp.html

Java: new Thread(() -> f()).start()
来源：http://hz.hfpthk.cn/gtfqoaokqv.html

Go:   go f()
来源：http://hz.shangyingyoupin.top/gttavlukdf.html

Ruby: Thread.new { f }
来源：http://hz.yuxming.cn/gtzclftman.html

C#:   Task.Run(() => F());
来源：http://hz.tian-w.cn/gtwbsnrrjy.html

[O02] 使用线程池
来源：http://hz.vqdsnc.cn/gtxilvkpfv.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.gogol.net.cn/gtggpwybjc.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.ybcxt.top/gtvklaghud.html

JS:   // worker_threads 线程池
来源：http://hz.yuxming.cn/gtzsovwzgh.html

TS:   // worker_threads 线程池
来源：http://hz.guowangkeji.top/gtjgvqlmej.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.ydjk.org.cn/gtcauzjhtg.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.hnqzz.top/gtsurmhnvf.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.9152youxi.cn/gtkgzjdple.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.ehwqpu.com/gtryrcvxbw.html

[O03] 加锁保护共享数据
来源：http://hz.andypj.xyz/gtyisygysy.html

Py:   with lock: shared += 1
来源：http://hz.ydzc1.top/gttpazdwdy.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.aizwys.cn/gtlmqpmlta.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.hnqzz.top/gtpmoukglc.html

TS:   // 同 JS
来源：http://hz.hnqzz.top/gtcenhvcho.html

Java: synchronized (this) { shared++; }
来源：http://hz.xziqi.cn/gtjsgydqti.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.aibaodan.cn/gtsfgmkdmq.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.daria6918.cn/gtjffsdqls.html

C#:   lock (gate) { shared++; }
来源：http://hz.haohaochexian.top/gtcjgegigj.html

[O04] 定义异步函数并等待
来源：http://hz.dianchejie.cn/gtzmytycaz.html

Py:   async def f():⏎    await g()
来源：http://hz.nanxinkj.top/gtjdcmbinc.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.jlsjyb.cn/gtgzjzmwga.html

JS:   async function f() { await g(); }
来源：http://hz.yuanzhike.top/gtdnnvymfi.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.jlsjyb.cn/gtbsshcayy.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.hysaishi.cn/gttxhbriyy.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.hywenlv.cn/gtgilkcjho.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.cashguo.top/gtcoddjsls.html

C#:   async Task F() { await G(); }
来源：http://hz.shanyushiyangtech.top/gtuoqpgxqe.html

[O05] 并发执行并等待全部完成
来源：http://hz.xinyue.icu/gttzpezrpv.html

Py:   asyncio.gather(*tasks)
来源：http://hz.nanxuanxn.top/gttwfqsbyq.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.jinyuanbaomall.cn/gtbdcdhoem.html

JS:   await Promise.all(tasks)
来源：http://hz.yuxming.cn/gtydmcxetw.html

TS:   await Promise.all(tasks)
来源：http://hz.daria6918.cn/gtbxfrnjpv.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.0kj1m.cn/gtyjyzzrpx.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.ybcxt.top/gtelyosmyi.html

Ruby: threads.map(&:join)
来源：http://hz.hywenlv.cn/gtkgkuhwza.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.cqqwz.cn/gttuoupcfc.html

[O06] 使用进程池
来源：http://hz.hongshengwenyu.top/gtirpybhrc.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.zhijiandao.cn/gtoysgmvia.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.nanxinkj.top/gtizbvaqed.html

JS:   // child_process / cluster 模块
来源：http://hz.yj20258.top/gtfkkvmnth.html

TS:   // child_process / cluster 模块
来源：http://hz.jqgfzy.top/gtgwwvcpvm.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.pycfn.com/gtqftwoepi.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.xziqi.cn/gtulonlcko.html

Ruby: // fork 块
来源：http://hz.yuxming.cn/gtondqcjae.html

C#:   Parallel.For
来源：http://hz.xylfe.cn/gtjsntqcns.html

================================================================================
来源：http://hz.chenzaomai.com/gtunqpxyut.html

P. 常用工具函数
来源：http://hz.fzhhl.top/gtolsaoyrt.html

================================================================================
来源：http://hz.yongpay.top/gtiuxhvaaq.html

[P01] 生成 UUID
来源：http://hz.tanke756.top/gtpfbjaezh.html

Py:   str(uuid.uuid4())
来源：http://hz.sysykeji.top/gtxpirlvvb.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hz.jinghuilouyu.cn/gtmwzgggks.html

JS:   crypto.randomUUID()
来源：http://hz.fengsongda.top/gtwjlmjsaf.html

TS:   crypto.randomUUID()
来源：http://hz.xylfe.cn/gthjunjcku.html

Java: UUID.randomUUID().toString()
来源：http://hz.316326.xyz/gtiqtbpupo.html

Go:   // 用 github.com/google/uuid
来源：http://hz.svipenyu.cn/gtbpgxzluj.html

Ruby: SecureRandom.uuid
来源：http://hz.daxiang520.top/gtvylwqdta.html

C#:   Guid.NewGuid().ToString()
来源：http://hz.iojbl.cn/gtkuoesuws.html

[P02] MD5 / SHA256 摘要
来源：http://hz.iojbl.cn/gtoylxraoz.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hz.ppjwa.cn/gtbdshiqcq.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://hz.shangyingyoupin.top/gtjlzluatk.html


<!-- 参考信息 -->