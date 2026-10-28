代发 wailian999

[L03] 设置自定义请求头
来源：http://hz.nwbrower.top/gtlvmtffvj.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.jyoumei.cn/gtdhwwnkfo.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.jinyuanbaomall.cn/gtoegywzuu.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.hysaishi.cn/gteqexmcje.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.ivvv.top/gtbztdghvh.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.shanyushiyangkeji.top/gtwbrgxlou.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.jqgufenzy.top/gtjcaziywo.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.xingfuxueyuan.xyz/gtkeuprjzr.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.jqgufenzy.top/gtgxkwclxa.html

[L04] 设置超时
来源：http://hz.c1oappe.top/gtvzwvqugi.html

Py:   requests.get(url, timeout=5)
来源：http://hz.ehwqpu.com/gtxruxhisp.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.daria6918.cn/gtnatmunyp.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.52xcode.cn/gtoqwmjeuq.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.nwbrower.top/gtmifuzjdx.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.shzxlz.cn/gtxgngnydg.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.xinyue.icu/gtvjhbnuzn.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.birdmap.top/gtgbsktncs.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.52xcode.cn/gtxzcumblu.html

[L05] 上传文件（multipart）
来源：http://hz.jqgufenzy.top/gtnnocktrz.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.cucudq.cn/gteqwylfpd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.kuanghao11.cn/gtjqzbaidh.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.redwolf501.top/gtrrwxvvoz.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.yj20258.top/gttbqbayod.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.shzxlz.cn/gttcheavqk.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.yongpay.top/gtxkcijvkk.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.0kj1m.cn/gtemtdrzuk.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.wangshuangyany.cn/gtgqfsbueb.html

[L06] 解析响应为 JSON
来源：http://hz.bjfxy.top/gtbvahklii.html

Py:   resp.json()
来源：http://hz.52xcode.cn/gtpkyoxpgk.html

PHP:  json_decode($body, true);
来源：http://hz.vqdsnc.cn/gtdecogffk.html

JS:   await resp.json()
来源：http://hz.tianlin.xyz/gtldvpzfli.html

TS:   await resp.json()
来源：http://hz.sweek.top/gthtnvbyhj.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.ppjwa.cn/gtfrjlvcan.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.dashuyun.cn/gtqxcdilgv.html

Ruby: JSON.parse(resp.body)
来源：http://hz.jqgufenzy.top/gtfydkabri.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.shangyingyoupin.top/gtehyaxtxo.html

[L07] 处理 HTTP 状态码
来源：http://hz.dianchejie.cn/gtpsoyilrv.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.0kj1m.cn/gtdlfhtaxa.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.vqdsnc.cn/gtszfkypkh.html

JS:   resp.ok;  resp.status
来源：http://hz.yuxming.cn/gtnzaiirwl.html

TS:   resp.ok;  resp.status
来源：http://hz.hysaishi.cn/gtzbdeegeo.html

Java: resp.statusCode()
来源：http://hz.jlsjyb.cn/gtcjqdhqwk.html

Go:   resp.StatusCode
来源：http://hz.shuidangran.top/gtitbgsmfl.html

Ruby: resp.code.to_i
来源：http://hz.feifeiyinyue.top/gtgaphvkkj.html

C#:   (int)resp.StatusCode
来源：http://hz.xziqi.cn/gtqrhiojfr.html

[L08] 并发请求多个地址
来源：http://hz.wangdashe.top/gtjdffraxz.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.ybcxt.top/gteakgmjzp.html

PHP:  curl_multi_init() 系列
来源：http://hz.ydjk.org.cn/gtfuefmotv.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yanxiufei.cn/gttdjhwxqm.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yvedp.cn/gtjefeppdz.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.zhoulong.xyz/gttatcepff.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.shzxlz.cn/gtamgmnwod.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.yuanzhike.top/gtyovdkujm.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.sufxvd.cn/gtsgoaklrz.html

================================================================================
来源：http://hz.jyoumei.cn/gtvzlffrjm.html

M. 命令行 / 进程 / 环境
来源：http://hz.redwolf501.top/gtwwkymcxx.html

================================================================================
来源：http://hz.hywenlv.cn/gtmseozsht.html

[M01] 读取命令行参数
来源：http://hz.zhixingplan.top/gtyyyvpwub.html

Py:   sys.argv[1:]
来源：http://hz.shangyingyoupin.top/gtejycllsj.html

PHP:  $argv;  $argc;
来源：http://hz.zhongyouzk.top/gtzuhtjygm.html

JS:   process.argv.slice(2)
来源：http://hz.iojbl.cn/gtxfaayxwj.html

TS:   process.argv.slice(2)
来源：http://hz.xuetiantiany.cn/gtbmtamjgo.html

Java: args 数组（main 方法参数）
来源：http://hz.jyoumei.cn/gtshnfosvi.html

Go:   os.Args[1:]
来源：http://hz.dianchejie.cn/gthifcbipe.html

Ruby: ARGV
来源：http://hz.fzhhl.top/gtfvzlnwmr.html

C#:   args 数组（Main 方法参数）
来源：http://hz.jinyuanbaomall.cn/gtnihqmqcg.html

[M02] 读取环境变量
来源：http://hz.aibaodan.cn/gteqvbiuvf.html

Py:   os.environ.get("HOME")
来源：http://hz.hfpthk.cn/gtsdbaicjz.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.zhijiandao.cn/gtibadbctw.html

JS:   process.env.HOME
来源：http://hz.sysykeji.top/gtxrvzuvtr.html

TS:   process.env.HOME
来源：http://hz.pycfn.com/gtvqgwgyag.html

Java: System.getenv("HOME")
来源：http://hz.zhongyouzk.top/gtupcvsedb.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.xinyue.icu/gtjaepqber.html

Ruby: ENV["HOME"]
来源：http://hz.shuidangran.top/gtkvlvbiyt.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.ehwqpu.com/gtappkdyhk.html

[M03] 执行外部命令
来源：http://hz.vqdsnc.cn/gteldkdijx.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.yj20258.top/gtnfhgwuqw.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.guowangkeji.top/gtcfcpqyur.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.hysaishi.cn/gtgrnzwpuo.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.zhongyouzk.top/gtflslszef.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.pengpengdd.cyou/gtchuijoho.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.shanyushiyangkeji.top/gtxpboglzc.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.c1oappe.top/gtswqrjcwi.html

C#:   Process.Start("ls", "-l");
来源：http://hz.9152youxi.cn/gtiblgfecu.html

[M04] 获取当前工作目录
来源：http://hz.andypj.xyz/gthzltcsnr.html

Py:   os.getcwd()
来源：http://hz.nwbrower.top/gtpppdvwtd.html

PHP:  getcwd();
来源：http://hz.smart0.xyz/gtoodelsaj.html

JS:   process.cwd()
来源：http://hz.hysaishi.cn/gtykozlhlx.html

TS:   process.cwd()
来源：http://hz.pycfn.com/gtupswbchn.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.vqdsnc.cn/gtzvhmbpek.html

Go:   os.Getwd()
来源：http://hz.dianchejie.cn/gtuowxwxds.html

Ruby: Dir.pwd
来源：http://hz.jinyuanbaomall.cn/gtzatymqzn.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.gzhubu.top/gtmmqisqhw.html

[M05] 设置退出码
来源：http://hz.shuidangran.top/gtcmniggec.html

Py:   sys.exit(1)
来源：http://hz.jianghu66.top/gtbykgnnqy.html

PHP:  exit(1);
来源：http://hz.sysykeji.top/gtaehqcsyq.html

JS:   process.exit(1)
来源：http://hz.yvedp.cn/gttlpcntef.html

TS:   process.exit(1)
来源：http://hz.zycfv.cn/gthdmafcln.html

Java: System.exit(1)
来源：http://hz.ppjwa.cn/gtgqdmakjj.html

Go:   os.Exit(1)
来源：http://hz.ivvv.top/gtgonyjmcg.html

Ruby: exit 1
来源：http://hz.chenlongwang.top/gtmqrenbct.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.birdmap.top/gtlgbcblor.html

[M06] 向标准错误输出
来源：http://hz.sweek.top/gtmebkedbk.html

Py:   print("err", file=sys.stderr)
来源：http://hz.yueranfly.top/gtgwrsoevk.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.shanyushiyangkeji.top/gttkzvmdxz.html

JS:   console.error("err")
来源：http://hz.daria6918.cn/gtjgdxgqwp.html

TS:   console.error("err")
来源：http://hz.xuanzx.com/gterxyaccp.html

Java: System.err.println("err")
来源：http://hz.birdmap.top/gtanclvbzo.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.ppjwa.cn/gtablbuhnk.html

Ruby: warn "err"
来源：http://hz.aibaodan.cn/gtelcwuqws.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.zhiwuduotai.top/gtrfkcltdo.html

[M07] 判断是否为主入口
来源：http://hz.sxryk.cn/gtwgxysskj.html

Py:   if __name__ == "__main__":
来源：http://hz.andypj.xyz/gtuhtvxisc.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.cdnleiting.top/gtubqjnddj.html

JS:   require.main === module
来源：http://hz.hongshengwenyu.top/gtbsnbibnx.html

TS:   require.main === module
来源：http://hz.shanyushiyangtech.top/gtlxqfkfoe.html

Java: public static void main(String[] args)
来源：http://hz.hysaishi.cn/gtmlvehgwk.html

Go:   func main()
来源：http://hz.iojbl.cn/gtlnnafzgw.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.smart0.xyz/gtjbjiwuqj.html

C#:   static void Main(string[] args)
来源：http://hz.guannengcc.top/gtspuynhyg.html

[M08] 获取系统与运行时信息
来源：http://hz.yonumen.top/gthnvixkyj.html

Py:   platform.system();  platform.python_version()
来源：http://hz.jqgfzy.top/gtepybwwgy.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.jinqigfzy.top/gtnymqusig.html

JS:   process.platform;  process.version
来源：http://hz.jinqigfzy.top/gtcxjglapf.html

TS:   process.platform;  process.version
来源：http://hz.xuanzx.com/gtdufwtjwt.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.xziqi.cn/gtjuwsjhyz.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.hfpthk.cn/gtgtmajvcm.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.cheryme.top/gtwyvdgmua.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.hnqzz.top/gtnfqnrjqz.html

================================================================================
来源：http://hz.pycfn.com/gtkbtftzun.html

N. 数据结构与算法
来源：http://hz.jinqigfzy.top/gtdprhmfbu.html

================================================================================
来源：http://hz.guowangkeji.top/gttypgjfnm.html

[N01] 二分查找（有序数组）
来源：http://hz.yonumen.top/gtitplceyo.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.316326.xyz/gttsnqveuz.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.0kj1m.cn/gtrtpgwlhw.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.fzhhl.top/gtzzmdbioq.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.aizwys.cn/gtvgrtfrkk.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.cashguo.top/gtnglwmgvk.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.chenlongwang.top/gtvablknhq.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.fzhhl.top/gtevedayua.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.jinyuanbaomall.cn/gtibhbnzuk.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.sufxvd.cn/gttwqmsjzr.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.pengpengdd.cyou/gtwbktauto.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.hnxiangtu.top/gtxzmeuhoi.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.hammf.cn/gtucftlxut.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jqgufenzy.top/gtcixfzqhy.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.jqgufenzy.top/gttbkhupjw.html

Go:   slices.Sort(arr)
来源：http://hz.xylfe.cn/gtaurniyek.html

Ruby: arr.sort
来源：http://hz.hnxiangtu.top/gtplrvkwcd.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.pengpengdd.cyou/gtyazaofey.html

[N03] 快速排序（分治示例）
来源：http://hz.feifeiyinyue.top/gttykaevxt.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.tian-w.cn/gtwsiimwzo.html

PHP:  // 递归实现，或用 usort
来源：http://hz.zhoulong.xyz/gtlhrcurwt.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.smart0.xyz/gtlapopdfg.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jiagoushi.top/gtphfujnhb.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.gotoacloud.top/gtynpqjhpn.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.yangfankeji.com/gtsggogwhp.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.cdnleiting.top/gtsqdjvstb.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.ydzc1.top/gtdkgpnywn.html

[N04] 斐波那契数列
来源：http://hz.cheryme.top/gtmnedpabh.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.gogol.net.cn/gthlbhfkgm.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.yuanzhike.top/gtsmjccixl.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yj202588.top/gtkntbpbbk.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.zhongyouzk.top/gtozljvmbq.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.cashguo.top/gtszkagrut.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.zhengqikj.top/gtbyfvptqh.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.pengpengdd.cyou/gtlnqkcmiy.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.guannengcc.top/gtnllnpamx.html

[N05] 最大公约数
来源：http://hz.daria6918.cn/gtiqylcvwx.html

Py:   math.gcd(a, b)
来源：http://hz.jiagoushi.top/gtgahmappq.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.yj20258.top/gtsuxzdacm.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.andypj.xyz/gtxgsmjpnf.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.cdnleiting.top/gtzejdoycp.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.zhiwuduotai.top/gtgltfeaun.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.gaohongyu789.top/gtyafzwzvq.html

Ruby: a.gcd(b)
来源：http://hz.meibo888.top/gtwodtnjuw.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.fengsongda.top/gtvqrufbbs.html

[N06] 判断回文字符串
来源：http://hz.daria6918.cn/gtscehdiwt.html

Py:   s == s[::-1]
来源：http://hz.fzhhl.top/gtfcaprdlc.html

PHP:  $s === strrev($s);
来源：http://hz.hfpthk.cn/gtqjldbdgp.html

JS:   s === [...s].reverse().join("")
来源：http://hz.dianchejie.cn/gteqjddwwr.html

TS:   s === [...s].reverse().join("")
来源：http://hz.zdqjudy.top/gtgxnqyruk.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.iojbl.cn/gtafdlwdyd.html

Go:   // 双指针从两端比较
来源：http://hz.ywan-chungtsiang.top/gteztqiiot.html

Ruby: s == s.reverse
来源：http://hz.fzhhl.top/gtzyxjoows.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.shanyushiyangkeji.top/gtlivswdcl.html

[N07] 两数之和（返回下标）
来源：http://hz.zdqjudy.top/gtibnyoclf.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.jinqigfzy.top/gtvwhyhpin.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.guowangkeji.top/gtejrcdufy.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.xylfe.cn/gtpfteqfgl.html

TS:   // 手写 Map<string, number>
来源：http://hz.316326.xyz/gtzlnpqwyp.html

Java: // 手写 HashMap
来源：http://hz.zhongyouzk.top/gtlwrjteer.html

Go:   // 手写 map[int]int
来源：http://hz.quarkkingdee.top/gtjlomnnzx.html

Ruby: // 手写 Hash
来源：http://hz.zhengqikj.top/gtlyhtddko.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.pengpengdd.cyou/gtluvyvkyg.html

[N08] 生成全排列
来源：http://hz.nanxinkj.top/gtmppyovhi.html

Py:   itertools.permutations(arr)
来源：http://hz.jinyuanbaomall.cn/gtyyprsynj.html

PHP:  // 手写递归交换
来源：http://hz.jiagoushi.top/gtkcirmnpf.html

JS:   // 手写回溯递归
来源：http://hz.zycfv.cn/gtouugpavf.html

TS:   // 手写回溯递归
来源：http://hz.zhiwuduotai.top/gtrkthapal.html

Java: // 手写回溯递归
来源：http://hz.hnqzz.top/gtcqprpebf.html

Go:   // 手写回溯递归
来源：http://hz.yuanzhike.top/gtvnwijgxf.html

Ruby: arr.permutation.to_a
来源：http://hz.guannengcc.top/gtuivylbkp.html

C#:   // 手写回溯递归
来源：http://hz.hammf.cn/gtnqlagrsz.html

[N09] 栈与队列
来源：http://hz.shanyushiyangtech.top/gticzmtvir.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.sysykeji.top/gtqjzarsfz.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.aibaodan.cn/gtkssbwims.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.aibaodan.cn/gtyjohwjqf.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.sufxvd.cn/gtcfnlxvar.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.yj20258.top/gtsxrqpijt.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.jqgufenzy.top/gtdopeqfmo.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.fengsongda.top/gtjnytcxmp.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.fengsongda.top/gtwdegwsfd.html

[N10] 链表节点定义
来源：http://hz.c1oappe.top/gtwobguebr.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.gzhubu.top/gtajwozqds.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.jyoumei.cn/gtovotjzpv.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.xziqi.cn/gteayqeokt.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.tanke756.top/gtvjinqfhz.html

Java: class Node { int v; Node next; }
来源：http://hz.vqdsnc.cn/gtbdomhlsw.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.sxryk.cn/gtcsaetknm.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.shzxlz.cn/gtoduxksvz.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.cqqwz.cn/gtnligjypb.html

[N11] 二叉树中序遍历
来源：http://hz.ydzc1.top/gtbjoaghqi.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.andypj.xyz/gtdgajxaat.html

PHP:  // 手写递归函数
来源：http://hz.hysaishi.cn/gtinnaqqfj.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.52xcode.cn/gtmfqirynw.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.guowangkeji.top/gtseqognye.html

Java: // 手写递归
来源：http://hz.chenjidiqi.icu/gtylegplfq.html

Go:   // 手写递归
来源：http://hz.yongpay.top/gtzavfaepy.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.tian-w.cn/gtiepdutwx.html

C#:   // 手写递归
来源：http://hz.daria6918.cn/gtapphmshd.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.52xcode.cn/gtcjytprtp.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.daria6918.cn/gtigjdzked.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.ppjwa.cn/gturhfffxd.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.fzhhl.top/gtwzkxhdyn.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.chenjidiqi.icu/gtcztqhlan.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.fzhhl.top/gtwgkxozym.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.cdnleiting.top/gtxivwydqe.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.cucudq.cn/gtqixqxmfc.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.chenzaomai.com/gtrvwypoif.html

================================================================================
来源：http://hz.shuidangran.top/gtqxdwxdwc.html

O. 并发与异步
来源：http://hz.gzhubu.top/gtigqzgpur.html

================================================================================
来源：http://hz.smart0.xyz/gtsrjnstsh.html

[O01] 启动一个线程
来源：http://hz.yj202588.top/gtiujounon.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.zhixingplan.top/gtlcgrjprm.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.shuidangran.top/gtofbxdkqa.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.sufxvd.cn/gtisffrcwy.html

TS:   // 同 JS
来源：http://hz.aizwys.cn/gtvnekauza.html

Java: new Thread(() -> f()).start()
来源：http://hz.daxiang520.top/gtsbabgnxu.html

Go:   go f()
来源：http://hz.hnxiangtu.top/gttzpqqjyi.html

Ruby: Thread.new { f }
来源：http://hz.hongshengwenyu.top/gtvbsvzpwc.html

C#:   Task.Run(() => F());
来源：http://hz.xuetiantiany.cn/gtiljcybnq.html

[O02] 使用线程池
来源：http://hz.sxryk.cn/gtrguzpayx.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.redwolf501.top/gtxqloleyz.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.jinghuilouyu.cn/gtuuzoovue.html

JS:   // worker_threads 线程池
来源：http://hz.yj20258888.top/gtkgndwawv.html

TS:   // worker_threads 线程池
来源：http://hz.daria6918.cn/gtdvaijxmj.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.9152youxi.cn/gtymknbrcy.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.tianlin.xyz/gtazaoxyld.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.zhiwuduotai.top/gtflslvzyi.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.fengsongda.top/gtwgckvprb.html

[O03] 加锁保护共享数据
来源：http://hz.zhiwuduotai.top/gtyztcxxib.html

Py:   with lock: shared += 1
来源：http://hz.hnxiangtu.top/gtqgqbaxyz.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.ywan-chungtsiang.top/gturyyaanc.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.jinqigufen.top/gtetvqslls.html

TS:   // 同 JS
来源：http://hz.snrcjt.cn/gtcryxeilu.html

Java: synchronized (this) { shared++; }
来源：http://hz.jiagoushi.top/gtxbjegpmc.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.zhixingplan.top/gtxhoegzvf.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.gotoacloud.top/gtvpkhygwk.html

C#:   lock (gate) { shared++; }
来源：http://hz.meibo888.top/gtalxtquxl.html

[O04] 定义异步函数并等待
来源：http://hz.xingfuxueyuan.xyz/gtgvdyhdao.html

Py:   async def f():⏎    await g()
来源：http://hz.daxiang520.top/gtwcgsmnmc.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.zhixingplan.top/gtoubntoih.html

JS:   async function f() { await g(); }
来源：http://hz.shangyingyoupin.top/gtrbawstre.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.xylfe.cn/gtyrmzfqxg.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.shanyushiyangkeji.top/gttkykbrio.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.snrcjt.cn/gtdlzkvsfm.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.nwbrower.top/gtatvbttyx.html

C#:   async Task F() { await G(); }
来源：http://hz.gotoacloud.top/gtrpvwnxsj.html

[O05] 并发执行并等待全部完成
来源：http://hz.yj20258888.top/gtaqaomysl.html

Py:   asyncio.gather(*tasks)
来源：http://hz.jyoumei.cn/gtceiiqvhs.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.nanxinkj.top/gtnkacssae.html

JS:   await Promise.all(tasks)
来源：http://hz.shuidangran.top/gtwzljvyns.html

TS:   await Promise.all(tasks)
来源：http://hz.smart0.xyz/gtsgbiwxhk.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.xinyue.icu/gthnbzgjcy.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.sufxvd.cn/gtlniyxznw.html

Ruby: threads.map(&:join)
来源：http://hz.ybcxt.top/gtywhungac.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.316326.xyz/gttnhriqbf.html

[O06] 使用进程池
来源：http://hz.zhixingplan.top/gtigtzjile.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.chenzaomai.com/gtaxkamuup.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.xuanzx.com/gtxqrafnko.html

JS:   // child_process / cluster 模块
来源：http://hz.jinyuanbaomall.cn/gtjfrnrgmj.html

TS:   // child_process / cluster 模块
来源：http://hz.ppjwa.cn/gtxhcsemth.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hz.jyoumei.cn/gtvpsrkdgu.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hz.quarkkingdee.top/gtmnomjpwq.html

Ruby: // fork 块
来源：http://hz.hfpthk.cn/gtzwlvbcwj.html

C#:   Parallel.For
来源：http://hz.xuetiantiany.cn/gtdmtppbcb.html

================================================================================
来源：http://hz.52xcode.cn/gtljicrvqa.html

P. 常用工具函数
来源：http://hz.redwolf501.top/gtoluvontz.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtydgmuogj.html


<!-- 参考信息 -->