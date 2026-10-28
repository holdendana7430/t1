代发 wailian999

[L03] 设置自定义请求头
来源：http://hz.mhx1999.top/gtqwqwcefv.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.nanxinkj.top/gteopzpjic.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.ywan-chungtsiang.top/gtudxdzxfj.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.shanyushiyangkeji.top/gtuznvxdup.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.quarkkingdee.top/gtsmzskuxy.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.cucudq.cn/gtrtwlguyb.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.zycfv.cn/gtauuvuord.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.zhaomingkeji.xyz/gtkbewotpt.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.xinyue.icu/gtsmysmrgk.html

[L04] 设置超时
来源：http://hz.yangfankeji.com/gtwhrrewbz.html

Py:   requests.get(url, timeout=5)
来源：http://hz.jqgfzy.top/gtfvoracak.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.ywan-chungtsiang.top/gtwrfkoxku.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.shangyingyoupin.top/gtvushvnnw.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.sysykeji.top/gtfzludgvc.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.dianchejie.cn/gtvfmhcctu.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.yonumen.top/gttkjvpemj.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.dashuyun.cn/gtybdcpows.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.yuanzhike.top/gtaeufuver.html

[L05] 上传文件（multipart）
来源：http://hz.jyoumei.cn/gtwzjgdwse.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.hnxiangtu.top/gtucvajyty.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.chenzaomai.com/gtuukfwkcl.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.ivvv.top/gtcmosrexr.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.aibaodan.cn/gtnnwveupd.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.jinghuilouyu.cn/gtqudvpaky.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.birdmap.top/gtokgxbjhx.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.pycfn.com/gtjhaclklz.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.zhaomingkeji.xyz/gtwjtkxggj.html

[L06] 解析响应为 JSON
来源：http://hz.yueranfly.top/gtigbrfpkc.html

Py:   resp.json()
来源：http://hz.zhoulong.xyz/gtudwwwbzt.html

PHP:  json_decode($body, true);
来源：http://hz.yangfankeji.com/gtdmybtjsb.html

JS:   await resp.json()
来源：http://hz.cashguo.top/gtnmmvfoay.html

TS:   await resp.json()
来源：http://hz.vqdsnc.cn/gturbciyrf.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.sxryk.cn/gtnwrjkbwt.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.andypj.xyz/gtkzeftnlc.html

Ruby: JSON.parse(resp.body)
来源：http://hz.xylfe.cn/gtwgpojcar.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.hnqzz.top/gtssreqovb.html

[L07] 处理 HTTP 状态码
来源：http://hz.jqgufenzy.top/gtiwldcysq.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.pycfn.com/gtbafshfzh.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.zhaomingkeji.xyz/gtndqtqjbk.html

JS:   resp.ok;  resp.status
来源：http://hz.dashuyun.cn/gtxjfmlrdw.html

TS:   resp.ok;  resp.status
来源：http://hz.shanyushiyangtech.top/gtauekzhwa.html

Java: resp.statusCode()
来源：http://hz.yongpay.top/gtshrggrud.html

Go:   resp.StatusCode
来源：http://hz.jianghu66.top/gtoylpxzvo.html

Ruby: resp.code.to_i
来源：http://hz.9152youxi.cn/gtnhpiqqmt.html

C#:   (int)resp.StatusCode
来源：http://hz.shangyingyoupin.top/gtyweexozo.html

[L08] 并发请求多个地址
来源：http://hz.gotoacloud.top/gtdvnrlfda.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.sweek.top/gtdtyfjjht.html

PHP:  curl_multi_init() 系列
来源：http://hz.hongshengwenyu.top/gtwzlabxzf.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhengqikj.top/gtafqwpkdx.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhengqikj.top/gterfuisex.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.tianlin.xyz/gtuutmwsla.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.zhiwuduotai.top/gtvrbnmbqv.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.nwbrower.top/gtlyzzdddb.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.cheryme.top/gtxjmzchvt.html

================================================================================
来源：http://hz.hysaishi.cn/gtdjaglbhi.html

M. 命令行 / 进程 / 环境
来源：http://hz.fengsongda.top/gtmnvsurzj.html

================================================================================
来源：http://hz.yanxiufei.cn/gtsvizyqtz.html

[M01] 读取命令行参数
来源：http://hz.chenzaomai.com/gtoidfeftc.html

Py:   sys.argv[1:]
来源：http://hz.daria6918.cn/gtezjwplrb.html

PHP:  $argv;  $argc;
来源：http://hz.hnxiangtu.top/gtergnvigb.html

JS:   process.argv.slice(2)
来源：http://hz.shuidangran.top/gtkqhyfmiv.html

TS:   process.argv.slice(2)
来源：http://hz.birdmap.top/gtizgnlfnz.html

Java: args 数组（main 方法参数）
来源：http://hz.andypj.xyz/gtpbtecnry.html

Go:   os.Args[1:]
来源：http://hz.tian-w.cn/gtgusrgxon.html

Ruby: ARGV
来源：http://hz.ybcxt.top/gtedguogyc.html

C#:   args 数组（Main 方法参数）
来源：http://hz.cqqwz.cn/gtqvzrglgk.html

[M02] 读取环境变量
来源：http://hz.0kj1m.cn/gtjzxmgrdw.html

Py:   os.environ.get("HOME")
来源：http://hz.jinyuanbaomall.cn/gtiizfgznw.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.tanke756.top/gtgffrgmqg.html

JS:   process.env.HOME
来源：http://hz.meibo888.top/gtpqjxgchn.html

TS:   process.env.HOME
来源：http://hz.zycfv.cn/gthxjxrhls.html

Java: System.getenv("HOME")
来源：http://hz.hammf.cn/gtfsvhcgzt.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.hongshengwenyu.top/gtigdlyjmg.html

Ruby: ENV["HOME"]
来源：http://hz.gzhubu.top/gtpxisffvb.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.daxiang520.top/gtxdkajmnu.html

[M03] 执行外部命令
来源：http://hz.andypj.xyz/gtsnshmnvp.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.jiagoushi.top/gtsoqncjos.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.andypj.xyz/gtemiuahyu.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.cheryme.top/gtxrzozwsv.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.yvedp.cn/gtfaxrzuvm.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.sysykeji.top/gtftmuucdq.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.ehwqpu.com/gtuxtbdbwo.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.cucudq.cn/gtsoejwsvk.html

C#:   Process.Start("ls", "-l");
来源：http://hz.yueranfly.top/gtdnytfheb.html

[M04] 获取当前工作目录
来源：http://hz.ppjwa.cn/gtoakcdnfo.html

Py:   os.getcwd()
来源：http://hz.shanyushiyangkeji.top/gtpnbiakyl.html

PHP:  getcwd();
来源：http://hz.gaohongyu789.top/gtjcfdogjb.html

JS:   process.cwd()
来源：http://hz.smart0.xyz/gtidensyyl.html

TS:   process.cwd()
来源：http://hz.andypj.xyz/gtcyhsqawn.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.cashguo.top/gtydmbhlkm.html

Go:   os.Getwd()
来源：http://hz.feifeiyinyue.top/gtsiwblrog.html

Ruby: Dir.pwd
来源：http://hz.c1oappe.top/gtydfelddg.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.tian-w.cn/gteksdakiv.html

[M05] 设置退出码
来源：http://hz.chenlongwang.top/gtgqdeksdm.html

Py:   sys.exit(1)
来源：http://hz.hywenlv.cn/gtqtyahfxx.html

PHP:  exit(1);
来源：http://hz.yj20258888.top/gtnoswgpcm.html

JS:   process.exit(1)
来源：http://hz.fzhhl.top/gtdgdnxxrz.html

TS:   process.exit(1)
来源：http://hz.tianlin.xyz/gtetcrohfo.html

Java: System.exit(1)
来源：http://hz.guowangkeji.top/gtqpnuknpw.html

Go:   os.Exit(1)
来源：http://hz.chenjidiqi.icu/gthtggmcrn.html

Ruby: exit 1
来源：http://hz.yuanzhike.top/gtqjfcrkoa.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.sweek.top/gtmklvueuy.html

[M06] 向标准错误输出
来源：http://hz.zhengqikj.top/gtdxtljbdt.html

Py:   print("err", file=sys.stderr)
来源：http://hz.cqqwz.cn/gttkjwpuso.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.chenzaomai.com/gtzjxjkywx.html

JS:   console.error("err")
来源：http://hz.wangdashe.top/gtqkppojee.html

TS:   console.error("err")
来源：http://hz.yuxming.cn/gtkhjylljg.html

Java: System.err.println("err")
来源：http://hz.cashguo.top/gtzkkvxxeg.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.jyoumei.cn/gtrykutjse.html

Ruby: warn "err"
来源：http://hz.wangshuangyany.cn/gtrwmnqdkb.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.haohaochexian.top/gtjvdciyhr.html

[M07] 判断是否为主入口
来源：http://hz.xylfe.cn/gtmyrsfaff.html

Py:   if __name__ == "__main__":
来源：http://hz.svipenyu.cn/gtfmpedcqj.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.havefunace.top/gtovwwqdzy.html

JS:   require.main === module
来源：http://hz.shuidangran.top/gtlakgpudo.html

TS:   require.main === module
来源：http://hz.tianlin.xyz/gtmkobdurg.html

Java: public static void main(String[] args)
来源：http://hz.sysykeji.top/gtotinzonj.html

Go:   func main()
来源：http://hz.nanxuanxn.top/gtrtctdsdz.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.gzhubu.top/gtlfsqcyef.html

C#:   static void Main(string[] args)
来源：http://hz.ybcxt.top/gtrgnusgnt.html

[M08] 获取系统与运行时信息
来源：http://hz.shuidangran.top/gtqvcymtiw.html

Py:   platform.system();  platform.python_version()
来源：http://hz.yuxming.cn/gtradhogyw.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.vqdsnc.cn/gtxmbpxipq.html

JS:   process.platform;  process.version
来源：http://hz.jinqigufen.top/gtiuccwymk.html

TS:   process.platform;  process.version
来源：http://hz.hywenlv.cn/gtzhiwqvdg.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.tianlin.xyz/gtpzblxjym.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.yuxming.cn/gtbtacdvzc.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.zycfv.cn/gtyesxmoru.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.zhengqikj.top/gtahhzjxzx.html

================================================================================
来源：http://hz.jianghu66.top/gthfmpnebj.html

N. 数据结构与算法
来源：http://hz.jianghu66.top/gtopxeqhuy.html

================================================================================
来源：http://hz.tanke756.top/gtoatzptdq.html

[N01] 二分查找（有序数组）
来源：http://hz.fzhhl.top/gtnwgzveyd.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.shuidangran.top/gtizcfcmpf.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.jyoumei.cn/gtedakahij.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jyoumei.cn/gttocbbrps.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.hammf.cn/gtckariiqj.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.xziqi.cn/gtinyrmewh.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.cdnleiting.top/gtpveyywxb.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.hfpthk.cn/gtcpqtqipl.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.jianghu66.top/gtyayycxsw.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.ydzc1.top/gtakdeyjco.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.birdmap.top/gtzwgvupqu.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.9152youxi.cn/gtappwclyu.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.ydzc1.top/gtmmxvyiji.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.zhiwuduotai.top/gtzagznfvr.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.jiagoushi.top/gtsxgqhomj.html

Go:   slices.Sort(arr)
来源：http://hz.jinqigfzy.top/gtmwhnedaf.html

Ruby: arr.sort
来源：http://hz.shanyushiyangtech.top/gtlleyjzrd.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.jinqigfzy.top/gtoezquvlb.html

[N03] 快速排序（分治示例）
来源：http://hz.cdnleiting.top/gtbcymeaoy.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.zhongyouzk.top/gtsltnonsb.html

PHP:  // 递归实现，或用 usort
来源：http://hz.ybcxt.top/gtfwjxpebn.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zdqjudy.top/gtmyokjwky.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.wangshuangyany.cn/gtdqyhnjpk.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.yj20258888.top/gtcgmlqlbn.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.mhx1999.top/gtlixlgqdh.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.tian-w.cn/gtepmjayry.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.hnqzz.top/gttjjwvafe.html

[N04] 斐波那契数列
来源：http://hz.316326.xyz/gtqlmzlxqg.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.chenjidiqi.icu/gtgsgukwew.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.9152youxi.cn/gtwelqqtjk.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.tanke756.top/gtzhgdqyrw.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.pengpengdd.cyou/gtjuzmlnqe.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.tanke756.top/gtmbbnjmqa.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.gaohongyu789.top/gtempkwdji.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.bjfxy.top/gttixwwneo.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.cqqwz.cn/gtunaqvyhg.html

[N05] 最大公约数
来源：http://hz.fzhhl.top/gtjhlrdjgu.html

Py:   math.gcd(a, b)
来源：http://hz.c1oappe.top/gtoflhihnj.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.jianghu66.top/gtyjosdowz.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.ydzc1.top/gtjtsvubsr.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.mhx1999.top/gtunkxzjet.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.sweek.top/gtvrzmgnxm.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.jinghuilouyu.cn/gtlerbekep.html

Ruby: a.gcd(b)
来源：http://hz.zdqjudy.top/gtyztrxqge.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.cashguo.top/gtufgdifao.html

[N06] 判断回文字符串
来源：http://hz.tianlin.xyz/gtclpgtjpu.html

Py:   s == s[::-1]
来源：http://hz.jyoumei.cn/gtlfxpbrki.html

PHP:  $s === strrev($s);
来源：http://hz.jinghuilouyu.cn/gtzgtvevxw.html

JS:   s === [...s].reverse().join("")
来源：http://hz.yangfankeji.com/gtndefgjqj.html

TS:   s === [...s].reverse().join("")
来源：http://hz.zycfv.cn/gtkkrlasqi.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.vqdsnc.cn/gtnuzszrwa.html

Go:   // 双指针从两端比较
来源：http://hz.xuanzx.com/gtmjyxcpxa.html

Ruby: s == s.reverse
来源：http://hz.zhiwuduotai.top/gtmxlmryvr.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.shuidangran.top/gtwagcsxqg.html

[N07] 两数之和（返回下标）
来源：http://hz.birdmap.top/gthksjswuq.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.jyoumei.cn/gtqffeepqp.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.yvedp.cn/gtryvswgax.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.zhijiandao.cn/gtfzhbrzro.html

TS:   // 手写 Map<string, number>
来源：http://hz.zhongyouzk.top/gtamjrrrin.html

Java: // 手写 HashMap
来源：http://hz.yuxming.cn/gtyxdipoex.html

Go:   // 手写 map[int]int
来源：http://hz.zhixingplan.top/gtfpejqlzq.html

Ruby: // 手写 Hash
来源：http://hz.cashguo.top/gtzmvivhrp.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.52xcode.cn/gtasmiqfyc.html

[N08] 生成全排列
来源：http://hz.pycfn.com/gtecymnnhn.html

Py:   itertools.permutations(arr)
来源：http://hz.hongshengwenyu.top/gtmscynxdo.html

PHP:  // 手写递归交换
来源：http://hz.tian-w.cn/gthtubyocm.html

JS:   // 手写回溯递归
来源：http://hz.nanxinkj.top/gtvtfndcyk.html

TS:   // 手写回溯递归
来源：http://hz.dashuyun.cn/gtvxhqjwqx.html

Java: // 手写回溯递归
来源：http://hz.svipenyu.cn/gtplsrjcze.html

Go:   // 手写回溯递归
来源：http://hz.sweek.top/gtbhuybhpt.html

Ruby: arr.permutation.to_a
来源：http://hz.ydjk.org.cn/gttilqfyns.html

C#:   // 手写回溯递归
来源：http://hz.yongpay.top/gtlqhyzkag.html

[N09] 栈与队列
来源：http://hz.guannengcc.top/gtunesypeo.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.ppjwa.cn/gtjaoicslc.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.ydzc1.top/gtqovorami.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.bjfxy.top/gtcshnqcqh.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.zhiwuduotai.top/gtgkjqnejf.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.shangyingyoupin.top/gtjzsguddj.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.zhoulong.xyz/gtbgniumje.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.316326.xyz/gtbyasdhzj.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.yj20258.top/gtfxgnprha.html

[N10] 链表节点定义
来源：http://hz.feifeiyinyue.top/gteophjjgl.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.fzhhl.top/gtghoaqmwz.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.chenzaomai.com/gtzbcdyjrt.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.sufxvd.cn/gtsxjbpgfg.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.gzhubu.top/gtodqymckk.html

Java: class Node { int v; Node next; }
来源：http://hz.bjfxy.top/gtpmgrfkmi.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.tianlin.xyz/gtcbajecpu.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.yuxming.cn/gtvhkeunhf.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.bjfxy.top/gtmkkcjsjm.html

[N11] 二叉树中序遍历
来源：http://hz.xingfuxueyuan.xyz/gtleehwmsp.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.ydjk.org.cn/gteswlpzud.html

PHP:  // 手写递归函数
来源：http://hz.wangshuangyany.cn/gtoucnfwkv.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.hywenlv.cn/gtwibplshs.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.zhongyouzk.top/gtcijjpqwu.html

Java: // 手写递归
来源：http://hz.zhixingplan.top/gtmshmwvsw.html

Go:   // 手写递归
来源：http://hz.xinyue.icu/gtjmxpaqbn.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.xingfuxueyuan.xyz/gtvsdrskdn.html

C#:   // 手写递归
来源：http://hz.shzxlz.cn/gtjwhlprpf.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.zycfv.cn/gttfxpkxpf.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.jinghuilouyu.cn/gtptrylqdc.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.ydzc1.top/gtprtmacsd.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.sweek.top/gtegdayfez.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.hywenlv.cn/gtkppcaqwi.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.bjfxy.top/gtaoskbqdu.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.xylfe.cn/gtrdxzdpzq.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.c1oappe.top/gtpstwfqza.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.haohaochexian.top/gtegwvboyv.html

================================================================================
来源：http://hz.yuxming.cn/gtvbjcgirn.html

O. 并发与异步
来源：http://hz.jinghuilouyu.cn/gtgrilqlxe.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtyupksnfw.html

[O01] 启动一个线程
来源：http://hz.andypj.xyz/gtuhtocalt.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.ybcxt.top/gtrouuzumn.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.9152youxi.cn/gtysgdwfzb.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.jlsjyb.cn/gtfqciqxja.html

TS:   // 同 JS
来源：http://hz.pengpengdd.cyou/gtizanhhbg.html

Java: new Thread(() -> f()).start()
来源：http://hz.zhixingplan.top/gturvwuxmb.html

Go:   go f()
来源：http://hz.cucudq.cn/gtsbcoytjm.html

Ruby: Thread.new { f }
来源：http://hz.cdnleiting.top/gtaamehghb.html

C#:   Task.Run(() => F());
来源：http://hz.shuidangran.top/gthclsirtt.html

[O02] 使用线程池
来源：http://hz.xuanzx.com/gtplccoadu.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.tian-w.cn/gtssjpjxvg.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.jqgfzy.top/gtdejinymz.html

JS:   // worker_threads 线程池
来源：http://hz.andypj.xyz/gtbwpivuzn.html

TS:   // worker_threads 线程池
来源：http://hz.yonumen.top/gtlnqxncvg.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.ydjk.org.cn/gtglognnjr.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.pycfn.com/gtcfzdkkyw.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.xuetiantiany.cn/gtphlkpoyg.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.316326.xyz/gtnxjdxhwf.html

[O03] 加锁保护共享数据
来源：http://hz.smart0.xyz/gtzwkuokpe.html

Py:   with lock: shared += 1
来源：http://hz.yvedp.cn/gtgotmzfdx.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.xziqi.cn/gtlxxwgacp.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.guannengcc.top/gtbmqdwazk.html

TS:   // 同 JS
来源：http://hz.chenlongwang.top/gtqohupbrl.html

Java: synchronized (this) { shared++; }
来源：http://hz.zycfv.cn/gtbejnudon.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.hysaishi.cn/gtyvrqjlua.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.pengpengdd.cyou/gtgueekawt.html

C#:   lock (gate) { shared++; }
来源：http://hz.ybcxt.top/gtumaaonxw.html

[O04] 定义异步函数并等待
来源：http://hz.ydzc1.top/gtdotdxdfh.html

Py:   async def f():⏎    await g()
来源：http://hz.jianghu66.top/gtnvprfnfw.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.yj20258.top/gtdannsmwt.html

JS:   async function f() { await g(); }
来源：http://hz.yanxiufei.cn/gtdazmchik.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.tian-w.cn/gttdxmvsgi.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.daria6918.cn/gtiqwagjuv.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.aibaodan.cn/gtpatoxpas.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.cucudq.cn/gtydrnrrec.html

C#:   async Task F() { await G(); }
来源：http://hz.sufxvd.cn/gtijrwwguw.html

[O05] 并发执行并等待全部完成
来源：http://hz.jinqigufen.top/gtnwkfbjhf.html

Py:   asyncio.gather(*tasks)
来源：http://hz.xylfe.cn/gtiwarcmog.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.ydzc1.top/gtahihcryg.html

JS:   await Promise.all(tasks)
来源：http://hz.fzhhl.top/gthmwlvrbt.html

TS:   await Promise.all(tasks)
来源：http://hz.nwbrower.top/gtfwqhvcgc.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.zdqjudy.top/gtjbzmedax.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.yueranfly.top/gtuwcykwfh.html

Ruby: threads.map(&:join)
来源：http://hz.jqgufenzy.top/gtinlgsbvm.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.andypj.xyz/gtkogftfgy.html

[O06] 使用进程池
来源：http://hz.havefunace.top/gthwzrgfyx.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.gzhubu.top/gtrqsrvxkn.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.xingfuxueyuan.xyz/gtvcuihjja.html

JS:   // child_process / cluster 模块
来源：http://hz.quarkkingdee.top/gtxqmbijdv.html

TS:   // child_process / cluster 模块
来源：http://hz.zycfv.cn/gthsqrcgaf.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.c1oappe.top/gtjwllhsfu.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.wangdashe.top/gtnxgxssil.html

Ruby: // fork 块
来源：http://hz.meibo888.top/gtrglobspn.html

C#:   Parallel.For
来源：http://hz.aibaodan.cn/gtqdugzuvt.html

================================================================================
来源：http://hz.nanxinkj.top/gtezuoyojq.html

P. 常用工具函数
来源：http://hz.chenlongwang.top/gtrsnxcedl.html

================================================================================
来源：http://hz.jqgfzy.top/gtsbkqwkgn.html


<!-- 参考信息 -->