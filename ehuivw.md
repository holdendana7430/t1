代发 wailian999

Go:   encoding/gob
来源：http://hz.xinyue.icu/gtkvwijgvm.html

Ruby: Marshal.dump(obj)
来源：http://hz.zhiwuduotai.top/gtgfeakqih.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.hfpthk.cn/gtakkqlrhh.html

================================================================================
来源：http://hz.jqgufenzy.top/gtqivermkg.html

L. 网络请求
来源：http://hz.chenjidiqi.icu/gtpuijubfc.html

================================================================================
来源：http://hz.jqgfzy.top/gtclovohiz.html

[L01] 发送 GET 请求
来源：http://hz.hammf.cn/gtmfjvdjrg.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.cucudq.cn/gterdimadn.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.ehwqpu.com/gtcpbemkwx.html

JS:   await fetch(url)
来源：http://hz.redwolf501.top/gtevadqxoo.html

TS:   await fetch(url)
来源：http://hz.quarkkingdee.top/gtikvecldw.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.guannengcc.top/gtwfvxpdwy.html

Go:   resp, err := http.Get(url)
来源：http://hz.zycfv.cn/gtxaouhuuu.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.hammf.cn/gtafsgxedv.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.tanke756.top/gtkwpqmuzl.html

[L02] 发送 POST JSON
来源：http://hz.birdmap.top/gtwcpieeea.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.chenzaomai.com/gtvhjabxvp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.cucudq.cn/gttcesjgbu.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.hywenlv.cn/gtfwdodzal.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zdqjudy.top/gtosamhows.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.ppjwa.cn/gtkrmcogok.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.jyoumei.cn/gtovmabvhe.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.xylfe.cn/gtxbhzbyzr.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.jinqigfzy.top/gtekvnxzad.html

[L03] 设置自定义请求头
来源：http://hz.zhoulong.xyz/gtfldwibpn.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.nanxuanxn.top/gtcxqvyfva.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.zhiwuduotai.top/gtwckmkmte.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.xziqi.cn/gtszgzucqg.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.mhx1999.top/gteiuhsfvl.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.chenjidiqi.icu/gtpwipwdnn.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.ivvv.top/gtfsuugpxn.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.hnxiangtu.top/gtradeyzgo.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.jqgufenzy.top/gtdlxlnnyp.html

[L04] 设置超时
来源：http://hz.yangfankeji.com/gtudfrlvfm.html

Py:   requests.get(url, timeout=5)
来源：http://hz.gotoacloud.top/gttajiqczc.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.hywenlv.cn/gthhikqasb.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.birdmap.top/gtcvkcirbt.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.shuidangran.top/gtieooighs.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.birdmap.top/gtrwtozsgb.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.tian-w.cn/gtxhqjoeir.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.hywenlv.cn/gttnjeudwg.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.jinyuanbaomall.cn/gtewtowoci.html

[L05] 上传文件（multipart）
来源：http://hz.yonumen.top/gtklpymtgj.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.guowangkeji.top/gtwpaikwme.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.zhongyouzk.top/gtmvdrepgd.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.hammf.cn/gtaauupnhh.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.svipenyu.cn/gtdyekpdog.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.sufxvd.cn/gtcxwbpeag.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.shzxlz.cn/gtzwbxxuhs.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.aizwys.cn/gtwfcghmft.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.316326.xyz/gtonlotsfw.html

[L06] 解析响应为 JSON
来源：http://hz.316326.xyz/gtkpbwuwlr.html

Py:   resp.json()
来源：http://hz.jinqigfzy.top/gttkfhlvoc.html

PHP:  json_decode($body, true);
来源：http://hz.sxryk.cn/gtvytyysyy.html

JS:   await resp.json()
来源：http://hz.yuanzhike.top/gtsmnucwpd.html

TS:   await resp.json()
来源：http://hz.jinghuilouyu.cn/gtgkcajfuq.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.cucudq.cn/gtsweqoedr.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.jinqigfzy.top/gthvgmgmfo.html

Ruby: JSON.parse(resp.body)
来源：http://hz.jlsjyb.cn/gtzqfnuvuc.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.bjfxy.top/gtrppscobi.html

[L07] 处理 HTTP 状态码
来源：http://hz.yongpay.top/gtaiwimnje.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.yonumen.top/gtbbollksl.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.zhongyouzk.top/gtzlsdrubm.html

JS:   resp.ok;  resp.status
来源：http://hz.shangyingyoupin.top/gtiurlnywi.html

TS:   resp.ok;  resp.status
来源：http://hz.bjfxy.top/gthznfjmyo.html

Java: resp.statusCode()
来源：http://hz.jinghuilouyu.cn/gtkhvushmz.html

Go:   resp.StatusCode
来源：http://hz.52xcode.cn/gtmteemajf.html

Ruby: resp.code.to_i
来源：http://hz.pengpengdd.cyou/gtollxkihh.html

C#:   (int)resp.StatusCode
来源：http://hz.shzxlz.cn/gtikfcvigq.html

[L08] 并发请求多个地址
来源：http://hz.ydjk.org.cn/gtpmtowyun.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.quarkkingdee.top/gtlehvgrsv.html

PHP:  curl_multi_init() 系列
来源：http://hz.chenzaomai.com/gtntjnqone.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.52xcode.cn/gtocfoagyu.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yuanzhike.top/gtlligliad.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.9152youxi.cn/gtoxuwzqno.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.nanxuanxn.top/gtduskmhfr.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.havefunace.top/gtxxndlpog.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.zhixingplan.top/gtrxfkqman.html

================================================================================
来源：http://hz.yangfankeji.com/gtxsanjumg.html

M. 命令行 / 进程 / 环境
来源：http://hz.jlsjyb.cn/gtilkjjbtz.html

================================================================================
来源：http://hz.yj20258888.top/gtwphejuzh.html

[M01] 读取命令行参数
来源：http://hz.pycfn.com/gtyyqtuhdn.html

Py:   sys.argv[1:]
来源：http://hz.316326.xyz/gtcubcdnhu.html

PHP:  $argv;  $argc;
来源：http://hz.ppjwa.cn/gtyusgybpx.html

JS:   process.argv.slice(2)
来源：http://hz.guowangkeji.top/gtyudmccfl.html

TS:   process.argv.slice(2)
来源：http://hz.yueranfly.top/gtpyfcihbv.html

Java: args 数组（main 方法参数）
来源：http://hz.cucudq.cn/gtvhgobpuo.html

Go:   os.Args[1:]
来源：http://hz.316326.xyz/gtzhoveipz.html

Ruby: ARGV
来源：http://hz.yj20258888.top/gtoxlgbcez.html

C#:   args 数组（Main 方法参数）
来源：http://hz.ivvv.top/gtruvkxsak.html

[M02] 读取环境变量
来源：http://hz.daxiang520.top/gtpeuinhzh.html

Py:   os.environ.get("HOME")
来源：http://hz.daxiang520.top/gtyieasqtf.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.gogol.net.cn/gtrkvcmbaq.html

JS:   process.env.HOME
来源：http://hz.hnxiangtu.top/gtjuwqlhzr.html

TS:   process.env.HOME
来源：http://hz.jinghuilouyu.cn/gtmkglbfmr.html

Java: System.getenv("HOME")
来源：http://hz.tian-w.cn/gtfyevjvqf.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.zhoulong.xyz/gtgppqcnjs.html

Ruby: ENV["HOME"]
来源：http://hz.jinqigufen.top/gtspbowyqe.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.meibo888.top/gtvhvymrmf.html

[M03] 执行外部命令
来源：http://hz.0kj1m.cn/gtgelfawlq.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.jyoumei.cn/gtzpepnjvr.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.0kj1m.cn/gtxcgvwtcj.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.meibo888.top/gtacistkiz.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.xuetiantiany.cn/gtzoizcjkd.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.316326.xyz/gtiuospvrb.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.yj20258888.top/gtnbhxqjyc.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.dashuyun.cn/gtsrnehnzh.html

C#:   Process.Start("ls", "-l");
来源：http://hz.yanxiufei.cn/gtombdgxrs.html

[M04] 获取当前工作目录
来源：http://hz.jinghuilouyu.cn/gtgkzmxdue.html

Py:   os.getcwd()
来源：http://hz.dashuyun.cn/gtastbrgta.html

PHP:  getcwd();
来源：http://hz.daria6918.cn/gtjtpdkbde.html

JS:   process.cwd()
来源：http://hz.ydzc1.top/gtvhtirsmt.html

TS:   process.cwd()
来源：http://hz.ppjwa.cn/gthemeoihd.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.haohaochexian.top/gtbrewnwmm.html

Go:   os.Getwd()
来源：http://hz.shanyushiyangkeji.top/gtrbmovbix.html

Ruby: Dir.pwd
来源：http://hz.ehwqpu.com/gtmjdmudot.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.hnqzz.top/gtreviuggx.html

[M05] 设置退出码
来源：http://hz.cashguo.top/gtqeztwein.html

Py:   sys.exit(1)
来源：http://hz.cdnleiting.top/gthlnjvhld.html

PHP:  exit(1);
来源：http://hz.jinghuilouyu.cn/gtfvzkehqb.html

JS:   process.exit(1)
来源：http://hz.chenlongwang.top/gtdhmcseem.html

TS:   process.exit(1)
来源：http://hz.zhiwuduotai.top/gtbimcraro.html

Java: System.exit(1)
来源：http://hz.316326.xyz/gtspzhcvof.html

Go:   os.Exit(1)
来源：http://hz.daxiang520.top/gtgnnvhxip.html

Ruby: exit 1
来源：http://hz.tanke756.top/gtjfpaavfr.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.svipenyu.cn/gtlirlrlad.html

[M06] 向标准错误输出
来源：http://hz.vqdsnc.cn/gtczybvtcg.html

Py:   print("err", file=sys.stderr)
来源：http://hz.shangyingyoupin.top/gtjdoioqao.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.zycfv.cn/gtgsgbhfmv.html

JS:   console.error("err")
来源：http://hz.ivvv.top/gtyujdaqkm.html

TS:   console.error("err")
来源：http://hz.zhijiandao.cn/gtfqwvthzy.html

Java: System.err.println("err")
来源：http://hz.nanxuanxn.top/gtdlyrbbrf.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.fengsongda.top/gtgsplshls.html

Ruby: warn "err"
来源：http://hz.fengsongda.top/gtcsahwsyl.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.zhaomingkeji.xyz/gtmhxetcfa.html

[M07] 判断是否为主入口
来源：http://hz.9152youxi.cn/gtvnfuazws.html

Py:   if __name__ == "__main__":
来源：http://hz.jinqigfzy.top/gtqzgqthae.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.yonumen.top/gtsydxryhk.html

JS:   require.main === module
来源：http://hz.0kj1m.cn/gtaewfjjev.html

TS:   require.main === module
来源：http://hz.ppjwa.cn/gttqjgttoz.html

Java: public static void main(String[] args)
来源：http://hz.pycfn.com/gtlixbuimc.html

Go:   func main()
来源：http://hz.shangyingyoupin.top/gtjdtuywky.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.iojbl.cn/gtptjgcdlo.html

C#:   static void Main(string[] args)
来源：http://hz.ybcxt.top/gtokztmfcb.html

[M08] 获取系统与运行时信息
来源：http://hz.ybcxt.top/gtztslgjli.html

Py:   platform.system();  platform.python_version()
来源：http://hz.redwolf501.top/gtwicssrfc.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.gzhubu.top/gtsfxgzehs.html

JS:   process.platform;  process.version
来源：http://hz.redwolf501.top/gtcnrlsnsv.html

TS:   process.platform;  process.version
来源：http://hz.daria6918.cn/gttzauknlq.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.hfpthk.cn/gtcloxuhzv.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.tian-w.cn/gtqmemzlhm.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.cheryme.top/gtpbjbihvj.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.cdnleiting.top/gtvgowmkzv.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtfiiqztgc.html

N. 数据结构与算法
来源：http://hz.ybcxt.top/gtcsadzqos.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtjwttomlz.html

[N01] 二分查找（有序数组）
来源：http://hz.jqgufenzy.top/gtwrqeoedg.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.yueranfly.top/gtcpdzpisk.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.haohaochexian.top/gtyhohvdll.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.chenlongwang.top/gtuksyksek.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yonumen.top/gtuwpihema.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.jlsjyb.cn/gtzrqscukc.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.hfpthk.cn/gtgrkezaax.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.yangfankeji.com/gthnckzrns.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.c1oappe.top/gtzubfzpig.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.guannengcc.top/gtrahwptrh.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.zhoulong.xyz/gtdzkffolq.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.zhoulong.xyz/gttwjiojrp.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.hnqzz.top/gtozamrvvw.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.aibaodan.cn/gtphwdhnis.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.xinyue.icu/gtqqhyuvyi.html

Go:   slices.Sort(arr)
来源：http://hz.jinqigufen.top/gtuaifgtgq.html

Ruby: arr.sort
来源：http://hz.cucudq.cn/gtouknjksl.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.xuanzx.com/gtrkojwlfb.html

[N03] 快速排序（分治示例）
来源：http://hz.shzxlz.cn/gtcawtfrvy.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.ppjwa.cn/gthyecdkjz.html

PHP:  // 递归实现，或用 usort
来源：http://hz.yangfankeji.com/gtlgfiurua.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zhiwuduotai.top/gtmxvulwsk.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.nwbrower.top/gtrqwcninv.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.jlsjyb.cn/gtrrzezddo.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.hongshengwenyu.top/gtkajcyvph.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.jinqigufen.top/gttmyviqkl.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.havefunace.top/gtsgwdaeri.html

[N04] 斐波那契数列
来源：http://hz.cdnleiting.top/gtkjeiamcn.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.chenjidiqi.icu/gttnshivfu.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.jianghu66.top/gthmuxpxud.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.sufxvd.cn/gtcmfsbahv.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.ybcxt.top/gteskrjtri.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.gaohongyu789.top/gtqvdppdqw.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.tian-w.cn/gttvvopvgk.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.jinghuilouyu.cn/gtcbegjffs.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.cucudq.cn/gtufqgissa.html

[N05] 最大公约数
来源：http://hz.ybcxt.top/gtjywelbjd.html

Py:   math.gcd(a, b)
来源：http://hz.jinqigufen.top/gtqjcwjbxm.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.pengpengdd.cyou/gtisfhziqr.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.bjfxy.top/gtuaaaeppj.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jianghu66.top/gtvvmzomvi.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.meibo888.top/gtxiytzxpt.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.chenlongwang.top/gtebfarqtz.html

Ruby: a.gcd(b)
来源：http://hz.birdmap.top/gtnhtjfftr.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.chenlongwang.top/gtatgjwact.html

[N06] 判断回文字符串
来源：http://hz.quarkkingdee.top/gtkecczroo.html

Py:   s == s[::-1]
来源：http://hz.zhaomingkeji.xyz/gttakkevoh.html

PHP:  $s === strrev($s);
来源：http://hz.zhengqikj.top/gtmafphmkc.html

JS:   s === [...s].reverse().join("")
来源：http://hz.316326.xyz/gtnfoyvyux.html

TS:   s === [...s].reverse().join("")
来源：http://hz.shanyushiyangkeji.top/gtyheubsvd.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.aizwys.cn/gthnrrzttz.html

Go:   // 双指针从两端比较
来源：http://hz.iojbl.cn/gtowdjiqui.html

Ruby: s == s.reverse
来源：http://hz.fzhhl.top/gtzujidkco.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.meibo888.top/gtolvzsfcl.html

[N07] 两数之和（返回下标）
来源：http://hz.feifeiyinyue.top/gtlafdqmbv.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.nwbrower.top/gtxuonjakg.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.xuetiantiany.cn/gtudfpahco.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.yj20258.top/gtvxcwevko.html

TS:   // 手写 Map<string, number>
来源：http://hz.smart0.xyz/gtbkvdhtie.html

Java: // 手写 HashMap
来源：http://hz.chenzaomai.com/gtfnvwofed.html

Go:   // 手写 map[int]int
来源：http://hz.quarkkingdee.top/gtzxancuuc.html

Ruby: // 手写 Hash
来源：http://hz.sufxvd.cn/gtugfhdubg.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.jqgufenzy.top/gteqanvafw.html

[N08] 生成全排列
来源：http://hz.smart0.xyz/gtnwmmmvjy.html

Py:   itertools.permutations(arr)
来源：http://hz.yangfankeji.com/gtjwoqtsmp.html

PHP:  // 手写递归交换
来源：http://hz.mhx1999.top/gtukycwpim.html

JS:   // 手写回溯递归
来源：http://hz.sxryk.cn/gtceluxnpc.html

TS:   // 手写回溯递归
来源：http://hz.yueranfly.top/gtgjrofons.html

Java: // 手写回溯递归
来源：http://hz.jqgufenzy.top/gtximdhrdg.html

Go:   // 手写回溯递归
来源：http://hz.zhijiandao.cn/gtqqhlhfxi.html

Ruby: arr.permutation.to_a
来源：http://hz.shanyushiyangkeji.top/gtgymyatmf.html

C#:   // 手写回溯递归
来源：http://hz.guowangkeji.top/gtytdcapjp.html

[N09] 栈与队列
来源：http://hz.guowangkeji.top/gtaljeazhd.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.iojbl.cn/gtfvltosqy.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.wangdashe.top/gtsqxzrund.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.tanke756.top/gtdtjbzjsl.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.ydjk.org.cn/gtwjhjtytf.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.52xcode.cn/gtzxdsgoil.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.yonumen.top/gtchxaqhxw.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.fengsongda.top/gthukwzhfd.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.cheryme.top/gtdbrssdxu.html

[N10] 链表节点定义
来源：http://hz.0kj1m.cn/gtnotosuey.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.jinqigufen.top/gtalrtinpj.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.cucudq.cn/gtaybrpemp.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.yuxming.cn/gtvbqwetkk.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.cashguo.top/gtgqlzgscr.html

Java: class Node { int v; Node next; }
来源：http://hz.chenzaomai.com/gtigpoxacl.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.fengsongda.top/gtksyagpqf.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.zhixingplan.top/gtfzbnqxse.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.vqdsnc.cn/gthpyozqhz.html

[N11] 二叉树中序遍历
来源：http://hz.hfpthk.cn/gtxjjzildq.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.tian-w.cn/gtdqsefccj.html

PHP:  // 手写递归函数
来源：http://hz.sxryk.cn/gtqlpufszh.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.cdnleiting.top/gthbsjopdq.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.shangyingyoupin.top/gtpxgznffb.html

Java: // 手写递归
来源：http://hz.jiagoushi.top/gtbpmmpdij.html

Go:   // 手写递归
来源：http://hz.nanxuanxn.top/gtggjggpcv.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.jiagoushi.top/gtmtooyqei.html

C#:   // 手写递归
来源：http://hz.aizwys.cn/gtysvvhpqg.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.hfpthk.cn/gtcvmgbbmw.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.gaohongyu789.top/gtqnvknpdh.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.cashguo.top/gtmoohxfuf.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.shanyushiyangtech.top/gtfxkrugvj.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.ydzc1.top/gtrfdfrhey.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yongpay.top/gtxlrguqgz.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.shangyingyoupin.top/gtjoqswnij.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.tanke756.top/gtbinbelki.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.jinqigfzy.top/gtfvebluao.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtcsvdrwdx.html

O. 并发与异步
来源：http://hz.316326.xyz/gtvsiobxyw.html

================================================================================
来源：http://hz.jqgufenzy.top/gtxxqwrnur.html

[O01] 启动一个线程
来源：http://hz.yuxming.cn/gtsrfyepqj.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.xuetiantiany.cn/gtgfnvdxih.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.ydjk.org.cn/gtsqhchimp.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.andypj.xyz/gtwidzznfa.html

TS:   // 同 JS
来源：http://hz.smart0.xyz/gtpeqtzjvf.html

Java: new Thread(() -> f()).start()
来源：http://hz.shanyushiyangtech.top/gtofuhykom.html

Go:   go f()
来源：http://hz.hnqzz.top/gtquyfghub.html

Ruby: Thread.new { f }
来源：http://hz.jinqigufen.top/gtxbkfyuyo.html

C#:   Task.Run(() => F());
来源：http://hz.ywan-chungtsiang.top/gtzojxrwcd.html

[O02] 使用线程池
来源：http://hz.tian-w.cn/gttmoaiwtu.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.xuetiantiany.cn/gthwbytcfe.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.ivvv.top/gtzrkdrtid.html

JS:   // worker_threads 线程池
来源：http://hz.zdqjudy.top/gtjcjjttmz.html

TS:   // worker_threads 线程池
来源：http://hz.chenzaomai.com/gtgzvbzfzt.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.xylfe.cn/gtvntgpgte.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.yangfankeji.com/gtiaplcbuc.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.nanxinkj.top/gtbqrhuulr.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.52xcode.cn/gtzdlrnmeg.html

[O03] 加锁保护共享数据
来源：http://hz.meibo888.top/gtlrijwmpl.html

Py:   with lock: shared += 1
来源：http://hz.zhijiandao.cn/gtjckrfoii.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.hywenlv.cn/gtphznwnhb.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.tanke756.top/gtihlthohb.html

TS:   // 同 JS
来源：http://hz.yj202588.top/gtpgqgkevl.html

Java: synchronized (this) { shared++; }
来源：http://hz.ehwqpu.com/gttjdlcidf.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.zhengqikj.top/gtvrcmxxph.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.yuxming.cn/gtxswqclpw.html

C#:   lock (gate) { shared++; }
来源：http://hz.xingfuxueyuan.xyz/gtdejwneml.html

[O04] 定义异步函数并等待
来源：http://hz.fengsongda.top/gtnbokoukz.html

Py:   async def f():⏎    await g()
来源：http://hz.haohaochexian.top/gtxejysnav.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.yuanzhike.top/gtxaqoalyn.html

JS:   async function f() { await g(); }
来源：http://hz.gogol.net.cn/gtqgoyixhz.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.yj202588.top/gtdrmgymqb.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.yuanzhike.top/gtgverkmeo.html


<!-- 参考信息 -->