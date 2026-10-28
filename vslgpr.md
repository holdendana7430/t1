代发 wailian999

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.jqgufenzy.top/gtjofbqaap.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.nanxuanxn.top/gtiotrnckb.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.birdmap.top/gtxjuewmxn.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.xinyue.icu/gtcztkdrad.html

Go:   encoding/gob
来源：http://hz.redwolf501.top/gtlpmwddsi.html

Ruby: Marshal.dump(obj)
来源：http://hz.zycfv.cn/gtlzdtdafn.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.0kj1m.cn/gtqtdgegyc.html

================================================================================
来源：http://hz.nwbrower.top/gthrmqewuo.html

L. 网络请求
来源：http://hz.pycfn.com/gtggahrdcm.html

================================================================================
来源：http://hz.cqqwz.cn/gtutqszypt.html

[L01] 发送 GET 请求
来源：http://hz.dianchejie.cn/gtbzunzmcr.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.jinqigufen.top/gtnyqijnlk.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.guannengcc.top/gtwzagevbi.html

JS:   await fetch(url)
来源：http://hz.snrcjt.cn/gtyrzhgnei.html

TS:   await fetch(url)
来源：http://hz.mhx1999.top/gtmwtjndtt.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.yj20258888.top/gtloopqbfd.html

Go:   resp, err := http.Get(url)
来源：http://hz.zhengqikj.top/gtgtrwsxmb.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.hywenlv.cn/gtkjobtqpi.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.svipenyu.cn/gtdhnbcsmf.html

[L02] 发送 POST JSON
来源：http://hz.jinyuanbaomall.cn/gtfkyglnts.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.guannengcc.top/gtkejzzphd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.ivvv.top/gtcqgtwqol.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.snrcjt.cn/gtqfvaecxk.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.sysykeji.top/gtupmiamle.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.havefunace.top/gtsfoztipt.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.daxiang520.top/gtwviomkhb.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.zhaomingkeji.xyz/gtzyhtopzk.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.jinyuanbaomall.cn/gtpsdkqric.html

[L03] 设置自定义请求头
来源：http://hz.tanke756.top/gtmpmazlzr.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.0kj1m.cn/gtukmydlhu.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.xuanzx.com/gtkzqhxwzw.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.xziqi.cn/gtfrlvmpbo.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.c1oappe.top/gtcfpwfcsi.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.52xcode.cn/gtcubnnpga.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.zhaomingkeji.xyz/gtpdsffvwp.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.aibaodan.cn/gtsmmhqupk.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.hongshengwenyu.top/gtwvpnlpez.html

[L04] 设置超时
来源：http://hz.daria6918.cn/gttplcejzb.html

Py:   requests.get(url, timeout=5)
来源：http://hz.cdnleiting.top/gthwbmkggx.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.shanyushiyangtech.top/gtmsmughzr.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.cqqwz.cn/gtkpsfzflc.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.hnqzz.top/gtvcorizpa.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.9152youxi.cn/gtohprubsr.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.iojbl.cn/gtqfdtrzlw.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.shzxlz.cn/gtpuuyhfkp.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.xziqi.cn/gtyysdljte.html

[L05] 上传文件（multipart）
来源：http://hz.havefunace.top/gtufpqwxnn.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.chenjidiqi.icu/gtxhjhopsd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.chenjidiqi.icu/gtnbcgybmr.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.cashguo.top/gtjznfjrci.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.hnxiangtu.top/gtwsmqxomv.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.cdnleiting.top/gtmvftuhid.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.zhixingplan.top/gtieuzfyte.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.jinqigfzy.top/gtyvjcvcpz.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.wangshuangyany.cn/gtcrgmzcxe.html

[L06] 解析响应为 JSON
来源：http://hz.yanxiufei.cn/gtetjaxspk.html

Py:   resp.json()
来源：http://hz.jinyuanbaomall.cn/gtfcimjdkg.html

PHP:  json_decode($body, true);
来源：http://hz.zhongyouzk.top/gttwpabblh.html

JS:   await resp.json()
来源：http://hz.gogol.net.cn/gtjfvsyjao.html

TS:   await resp.json()
来源：http://hz.fengsongda.top/gtffrwlpsg.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.cdnleiting.top/gtozrjphii.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.kuanghao11.cn/gtimsvdfbo.html

Ruby: JSON.parse(resp.body)
来源：http://hz.hnqzz.top/gtviesfkho.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.ydzc1.top/gtzsubxwwq.html

[L07] 处理 HTTP 状态码
来源：http://hz.gogol.net.cn/gtieszwfop.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.9152youxi.cn/gtiigkmohz.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.hnxiangtu.top/gttudolwex.html

JS:   resp.ok;  resp.status
来源：http://hz.quarkkingdee.top/gtzjcynadv.html

TS:   resp.ok;  resp.status
来源：http://hz.xinyue.icu/gtthvznrwj.html

Java: resp.statusCode()
来源：http://hz.bjfxy.top/gtizbpeoal.html

Go:   resp.StatusCode
来源：http://hz.chenzaomai.com/gteoyncauy.html

Ruby: resp.code.to_i
来源：http://hz.cashguo.top/gtzmeycxdp.html

C#:   (int)resp.StatusCode
来源：http://hz.zhongyouzk.top/gthardudnc.html

[L08] 并发请求多个地址
来源：http://hz.hnxiangtu.top/gtjotmfkdk.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.zhaomingkeji.xyz/gtxxrsprxn.html

PHP:  curl_multi_init() 系列
来源：http://hz.meibo888.top/gtgngtisqk.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.xinyue.icu/gtluazhsqo.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.cdnleiting.top/gtdmxmzojb.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.birdmap.top/gtdzwidhwz.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.hysaishi.cn/gtwoqoymhr.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.jianghu66.top/gtzzxvdrxf.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.aizwys.cn/gtdjjudxbu.html

================================================================================
来源：http://hz.xylfe.cn/gtpmwjubwd.html

M. 命令行 / 进程 / 环境
来源：http://hz.hywenlv.cn/gtagvpwfkz.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtgzwqfpnt.html

[M01] 读取命令行参数
来源：http://hz.yvedp.cn/gtgabuhroo.html

Py:   sys.argv[1:]
来源：http://hz.sysykeji.top/gtfrvusrih.html

PHP:  $argv;  $argc;
来源：http://hz.iojbl.cn/gtwqubebey.html

JS:   process.argv.slice(2)
来源：http://hz.daria6918.cn/gtosjownlf.html

TS:   process.argv.slice(2)
来源：http://hz.meibo888.top/gttcqqljcn.html

Java: args 数组（main 方法参数）
来源：http://hz.zhengqikj.top/gtdbcvutqk.html

Go:   os.Args[1:]
来源：http://hz.feifeiyinyue.top/gtvdwmamom.html

Ruby: ARGV
来源：http://hz.shangyingyoupin.top/gtrtrebfev.html

C#:   args 数组（Main 方法参数）
来源：http://hz.jyoumei.cn/gtobdkbkki.html

[M02] 读取环境变量
来源：http://hz.daria6918.cn/gtczdhrkuh.html

Py:   os.environ.get("HOME")
来源：http://hz.yongpay.top/gtztufptrx.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.hfpthk.cn/gtynclsugv.html

JS:   process.env.HOME
来源：http://hz.0kj1m.cn/gtljqiadnh.html

TS:   process.env.HOME
来源：http://hz.ppjwa.cn/gtbyvkxrga.html

Java: System.getenv("HOME")
来源：http://hz.birdmap.top/gtyqxguczo.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.gaohongyu789.top/gtfczexnqi.html

Ruby: ENV["HOME"]
来源：http://hz.nwbrower.top/gtyjouflcf.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.feifeiyinyue.top/gtatgswcqp.html

[M03] 执行外部命令
来源：http://hz.c1oappe.top/gtrcpqckvd.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.cucudq.cn/gtzfqyawmq.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.jinyuanbaomall.cn/gtvxjsuxdx.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.hfpthk.cn/gttkqflnex.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.chenjidiqi.icu/gtwkdmlvoz.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.yj20258888.top/gtxowdiwwe.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.c1oappe.top/gtgnbqixgv.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.guowangkeji.top/gtjztizioh.html

C#:   Process.Start("ls", "-l");
来源：http://hz.gzhubu.top/gtbzuhtvbe.html

[M04] 获取当前工作目录
来源：http://hz.wangdashe.top/gtglxdbogj.html

Py:   os.getcwd()
来源：http://hz.hnqzz.top/gtvfxatisf.html

PHP:  getcwd();
来源：http://hz.sxryk.cn/gtzvxidsxf.html

JS:   process.cwd()
来源：http://hz.guowangkeji.top/gtveocwdio.html

TS:   process.cwd()
来源：http://hz.jianghu66.top/gtiljlsakf.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.chenzaomai.com/gtosqqnrcm.html

Go:   os.Getwd()
来源：http://hz.zycfv.cn/gtaksxkjuf.html

Ruby: Dir.pwd
来源：http://hz.shuidangran.top/gtgnjaurba.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.kuanghao11.cn/gtsdfolmmk.html

[M05] 设置退出码
来源：http://hz.gzhubu.top/gtchtmukgx.html

Py:   sys.exit(1)
来源：http://hz.redwolf501.top/gtifjzsege.html

PHP:  exit(1);
来源：http://hz.andypj.xyz/gtnsdismim.html

JS:   process.exit(1)
来源：http://hz.c1oappe.top/gtrdqcewhi.html

TS:   process.exit(1)
来源：http://hz.cdnleiting.top/gtluftawvt.html

Java: System.exit(1)
来源：http://hz.xuetiantiany.cn/gtjuoduwwo.html

Go:   os.Exit(1)
来源：http://hz.yuxming.cn/gtstvfnuxa.html

Ruby: exit 1
来源：http://hz.jiagoushi.top/gteqkfkvoj.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.shuidangran.top/gtlglvlbhr.html

[M06] 向标准错误输出
来源：http://hz.wangshuangyany.cn/gtwfmsaduj.html

Py:   print("err", file=sys.stderr)
来源：http://hz.sufxvd.cn/gtomyxyuxw.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.nanxinkj.top/gtmtsagrkd.html

JS:   console.error("err")
来源：http://hz.nwbrower.top/gtravchuux.html

TS:   console.error("err")
来源：http://hz.yongpay.top/gtqmwaudog.html

Java: System.err.println("err")
来源：http://hz.jyoumei.cn/gtoevbakql.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.chenzaomai.com/gtdbsdcbfp.html

Ruby: warn "err"
来源：http://hz.shzxlz.cn/gtjxmqtgzj.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.9152youxi.cn/gtcnmlkpqc.html

[M07] 判断是否为主入口
来源：http://hz.aizwys.cn/gtyxwjeptp.html

Py:   if __name__ == "__main__":
来源：http://hz.c1oappe.top/gtwwtfmwad.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.yangfankeji.com/gtjwtwbzsj.html

JS:   require.main === module
来源：http://hz.haohaochexian.top/gtnayanxye.html

TS:   require.main === module
来源：http://hz.hywenlv.cn/gtxzfvwsgb.html

Java: public static void main(String[] args)
来源：http://hz.haohaochexian.top/gtpyrblfrp.html

Go:   func main()
来源：http://hz.meibo888.top/gtestmnyzo.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.yongpay.top/gtcewwwkjp.html

C#:   static void Main(string[] args)
来源：http://hz.jinyuanbaomall.cn/gtqzcootrp.html

[M08] 获取系统与运行时信息
来源：http://hz.hysaishi.cn/gtihtslzos.html

Py:   platform.system();  platform.python_version()
来源：http://hz.52xcode.cn/gtycwoazqd.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.yuxming.cn/gtisiwqftp.html

JS:   process.platform;  process.version
来源：http://hz.jiagoushi.top/gtiglewyfa.html

TS:   process.platform;  process.version
来源：http://hz.cdnleiting.top/gtsmttgqfx.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.zhengqikj.top/gtvjtapkhh.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.gogol.net.cn/gtmjwhemhg.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.pycfn.com/gttebnhyub.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.zhongyouzk.top/gtjtoaoxuq.html

================================================================================
来源：http://hz.cashguo.top/gtchecxcdi.html

N. 数据结构与算法
来源：http://hz.guannengcc.top/gtilakktsi.html

================================================================================
来源：http://hz.gzhubu.top/gtadzzpxqh.html

[N01] 二分查找（有序数组）
来源：http://hz.0kj1m.cn/gthzjkshld.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.zhongyouzk.top/gtwdffhbkv.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.zdqjudy.top/gtectwobzj.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.52xcode.cn/gtytmmigol.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.shanyushiyangtech.top/gtkusdktvb.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.hnqzz.top/gtxqcnuhkz.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.bjfxy.top/gtlsuexcuy.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.aibaodan.cn/gtgizmtcgv.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.jqgfzy.top/gtqgdcqtdh.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.nwbrower.top/gtuoaysuyy.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.yanxiufei.cn/gtrdsaykyf.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.nanxinkj.top/gtjahzvxtg.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.xuanzx.com/gtileplyzs.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.iojbl.cn/gthhtfttzw.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.hysaishi.cn/gtszhrgngj.html

Go:   slices.Sort(arr)
来源：http://hz.aibaodan.cn/gtuarpfeom.html

Ruby: arr.sort
来源：http://hz.svipenyu.cn/gtbjkxuhek.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.daxiang520.top/gtpgzfuhxo.html

[N03] 快速排序（分治示例）
来源：http://hz.wangdashe.top/gtmanaiszo.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.jinghuilouyu.cn/gtlnpbsygl.html

PHP:  // 递归实现，或用 usort
来源：http://hz.yanxiufei.cn/gttboewtld.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zhijiandao.cn/gtwiksntkt.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.shuidangran.top/gtprjjvhko.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.9152youxi.cn/gtgwipmqnn.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.nanxinkj.top/gtdimbzlmk.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.tian-w.cn/gtckyxjmxw.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.havefunace.top/gtgcsqbilj.html

[N04] 斐波那契数列
来源：http://hz.redwolf501.top/gtmgrrpjom.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.cqqwz.cn/gtemmtriri.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.yanxiufei.cn/gtjqsweqse.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yonumen.top/gtdhawhedy.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.aizwys.cn/gtpkkgfvdi.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.yonumen.top/gteftskimo.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.jqgufenzy.top/gtdebkddvc.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.xuanzx.com/gtueoawldi.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.zhixingplan.top/gtdobpbaon.html

[N05] 最大公约数
来源：http://hz.xziqi.cn/gtvyuwweiq.html

Py:   math.gcd(a, b)
来源：http://hz.guannengcc.top/gtvwxdbkdz.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.jianghu66.top/gtoiolfuwo.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.sysykeji.top/gtzcodzdcm.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.sysykeji.top/gtfjcxkvsb.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.9152youxi.cn/gtpibudvia.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.yonumen.top/gtmxggixlj.html

Ruby: a.gcd(b)
来源：http://hz.redwolf501.top/gttvkbqapr.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.gzhubu.top/gtjdbevcgg.html

[N06] 判断回文字符串
来源：http://hz.sweek.top/gtaodajrkc.html

Py:   s == s[::-1]
来源：http://hz.feifeiyinyue.top/gtdfzcobhs.html

PHP:  $s === strrev($s);
来源：http://hz.yuanzhike.top/gtmhsyscla.html

JS:   s === [...s].reverse().join("")
来源：http://hz.hywenlv.cn/gtvdkzbsoo.html

TS:   s === [...s].reverse().join("")
来源：http://hz.bjfxy.top/gtnxxrcvyo.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.haohaochexian.top/gtfyxxzbuw.html

Go:   // 双指针从两端比较
来源：http://hz.ydzc1.top/gtvfftuaai.html

Ruby: s == s.reverse
来源：http://hz.zhoulong.xyz/gtcmyamkrn.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.fengsongda.top/gtpzgqorus.html

[N07] 两数之和（返回下标）
来源：http://hz.jinghuilouyu.cn/gtdzjxszpb.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.hywenlv.cn/gtiavozznd.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.hfpthk.cn/gtxhccqigu.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.cdnleiting.top/gthxigxarb.html

TS:   // 手写 Map<string, number>
来源：http://hz.hongshengwenyu.top/gtmiasdggl.html

Java: // 手写 HashMap
来源：http://hz.yonumen.top/gtsjpexmta.html

Go:   // 手写 map[int]int
来源：http://hz.fengsongda.top/gtiajyktmt.html

Ruby: // 手写 Hash
来源：http://hz.andypj.xyz/gtmepuzptu.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.yueranfly.top/gtaakgoqxw.html

[N08] 生成全排列
来源：http://hz.zhijiandao.cn/gtgttvlloh.html

Py:   itertools.permutations(arr)
来源：http://hz.sxryk.cn/gtgxkyqkfj.html

PHP:  // 手写递归交换
来源：http://hz.xziqi.cn/gtxaknwvif.html

JS:   // 手写回溯递归
来源：http://hz.hnxiangtu.top/gtaeuaxqwk.html

TS:   // 手写回溯递归
来源：http://hz.chenzaomai.com/gtlaqsybsl.html

Java: // 手写回溯递归
来源：http://hz.jiagoushi.top/gtuwwbpqlq.html

Go:   // 手写回溯递归
来源：http://hz.shanyushiyangtech.top/gtscxvkbyv.html

Ruby: arr.permutation.to_a
来源：http://hz.fengsongda.top/gtnbaznqif.html

C#:   // 手写回溯递归
来源：http://hz.yj20258.top/gtkxpvdcbt.html

[N09] 栈与队列
来源：http://hz.wangdashe.top/gtipxbgfbe.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.jiagoushi.top/gtcnroevpt.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.meibo888.top/gtvqqhbfnj.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.hnqzz.top/gtvvgkurpc.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.ivvv.top/gtrbeehboy.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.dianchejie.cn/gtzovqnogh.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.yuxming.cn/gtujwvqtzh.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.hywenlv.cn/gtkqszgyhj.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.yongpay.top/gtpufqeqyn.html

[N10] 链表节点定义
来源：http://hz.nanxuanxn.top/gtyjdsycfg.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.pengpengdd.cyou/gtsxndatql.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.yanxiufei.cn/gttulwpqtf.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.cdnleiting.top/gtlocaeiej.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.snrcjt.cn/gthepyoaii.html

Java: class Node { int v; Node next; }
来源：http://hz.fengsongda.top/gtdfaefauu.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.zhongyouzk.top/gtkkkrbuau.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.ppjwa.cn/gtkajaorro.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.chenzaomai.com/gtnrfrpqpd.html

[N11] 二叉树中序遍历
来源：http://hz.fengsongda.top/gtssxqytdm.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.dashuyun.cn/gtwtrkdmdf.html

PHP:  // 手写递归函数
来源：http://hz.vqdsnc.cn/gtuerfqmyq.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.ywan-chungtsiang.top/gtfgcovofk.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jiagoushi.top/gtlmsterkk.html

Java: // 手写递归
来源：http://hz.hammf.cn/gtvkdnvfmd.html

Go:   // 手写递归
来源：http://hz.shanyushiyangtech.top/gtrghrjoyl.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.jinqigfzy.top/gttsbomorp.html

C#:   // 手写递归
来源：http://hz.zycfv.cn/gtwwlpccnr.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.ywan-chungtsiang.top/gthxchrprn.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.dianchejie.cn/gtipymvexo.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.zhiwuduotai.top/gtdtahsiug.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.ydzc1.top/gtfwcwjjmn.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.cucudq.cn/gtpphzqzjx.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yj202588.top/gtnfbazgly.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.jyoumei.cn/gtmdfmiuma.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.xingfuxueyuan.xyz/gttqfjypwo.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.nanxinkj.top/gtwhjjyrdo.html

================================================================================
来源：http://hz.wangdashe.top/gtsybcslrr.html

O. 并发与异步
来源：http://hz.yuanzhike.top/gtpgzxhqeh.html

================================================================================
来源：http://hz.zhixingplan.top/gtpqcaqbiz.html

[O01] 启动一个线程
来源：http://hz.gogol.net.cn/gtnbqrcecu.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.ehwqpu.com/gtyuelriwr.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.xylfe.cn/gtkgkzahbl.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.pycfn.com/gtllibydyn.html

TS:   // 同 JS
来源：http://hz.fzhhl.top/gtsqxzmdml.html

Java: new Thread(() -> f()).start()
来源：http://hz.cdnleiting.top/gtfzaacyzt.html

Go:   go f()
来源：http://hz.zhiwuduotai.top/gtovlwuypz.html

Ruby: Thread.new { f }
来源：http://hz.chenlongwang.top/gtyqhdusfe.html

C#:   Task.Run(() => F());
来源：http://hz.jinqigufen.top/gturhpjblq.html

[O02] 使用线程池
来源：http://hz.nanxinkj.top/gtrbjshetf.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.dashuyun.cn/gthdhokhgu.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.zhongyouzk.top/gthvniwbjp.html

JS:   // worker_threads 线程池
来源：http://hz.xuetiantiany.cn/gtcswvcpqy.html

TS:   // worker_threads 线程池
来源：http://hz.jyoumei.cn/gtauxdnavh.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.guowangkeji.top/gtedwsvyvj.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.zhengqikj.top/gtimwbqeeu.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.yuanzhike.top/gtgqrimfuk.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.smart0.xyz/gtyzkgafkq.html

[O03] 加锁保护共享数据
来源：http://hz.cashguo.top/gthzajidsi.html

Py:   with lock: shared += 1
来源：http://hz.xinyue.icu/gtistcyqlg.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.yanxiufei.cn/gteibuzvud.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.jinqigfzy.top/gtrrpraagk.html

TS:   // 同 JS
来源：http://hz.wangshuangyany.cn/gtquyvehfz.html

Java: synchronized (this) { shared++; }
来源：http://hz.cashguo.top/gtufgnavqy.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.bjfxy.top/gthhocstyk.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.sysykeji.top/gtuhwmfetq.html

C#:   lock (gate) { shared++; }
来源：http://hz.yanxiufei.cn/gtkrdilcrh.html

[O04] 定义异步函数并等待
来源：http://hz.jlsjyb.cn/gtysoyjmoz.html

Py:   async def f():⏎    await g()
来源：http://hz.jinqigufen.top/gtdanmcesm.html


<!-- 参考信息 -->