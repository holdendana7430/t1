代发 wailian999

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.wangdashe.top/gtywmfwsmq.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.shanyushiyangtech.top/gtxkrpuxmy.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.shzxlz.cn/gtzjxdnnrn.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.pycfn.com/gteeyftqcf.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.nanxinkj.top/gtswzldfvf.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.shangyingyoupin.top/gtohewoacf.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.ppjwa.cn/gtkqlfaeok.html

Py:   pickle.dumps(obj)
来源：http://hz.jinghuilouyu.cn/gthntzhewm.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.gotoacloud.top/gtxbnhflhv.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.xingfuxueyuan.xyz/gtalxrvfnq.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.tian-w.cn/gtqxgpnsxs.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.jyoumei.cn/gtdvkhgklk.html

Go:   encoding/gob
来源：http://hz.chenlongwang.top/gtbncbafbb.html

Ruby: Marshal.dump(obj)
来源：http://hz.snrcjt.cn/gtwvcyozsc.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.ywan-chungtsiang.top/gtoxhuyyli.html

================================================================================
来源：http://hz.jlsjyb.cn/gtkticzdht.html

L. 网络请求
来源：http://hz.hnqzz.top/gtbbttafym.html

================================================================================
来源：http://hz.snrcjt.cn/gtrssopvjh.html

[L01] 发送 GET 请求
来源：http://hz.jianghu66.top/gtdivgpzrn.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.xuanzx.com/gttidrfhub.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.fengsongda.top/gtxhwebgtp.html

JS:   await fetch(url)
来源：http://hz.zhiwuduotai.top/gtbagvgqur.html

TS:   await fetch(url)
来源：http://hz.mhx1999.top/gtzlvvzcai.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.cucudq.cn/gtbmozhrpu.html

Go:   resp, err := http.Get(url)
来源：http://hz.yuxming.cn/gteifrrxfw.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.gotoacloud.top/gtwfqinaua.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.shanyushiyangkeji.top/gtvlypajth.html

[L02] 发送 POST JSON
来源：http://hz.pycfn.com/gtpduppikl.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.smart0.xyz/gtwnsmnmam.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.sweek.top/gtgopjasbk.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.hnqzz.top/gtqiqznwbw.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yj202588.top/gteygpjase.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.mhx1999.top/gtxqueijvn.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.feifeiyinyue.top/gtjcgkazwv.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.jinghuilouyu.cn/gtnxsyahaq.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.haohaochexian.top/gtbyhwakfw.html

[L03] 设置自定义请求头
来源：http://hz.sxryk.cn/gtedobxogq.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.cashguo.top/gtzxdnpady.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.meibo888.top/gtzwqcxxoh.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.nwbrower.top/gththyrhal.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.cheryme.top/gtwfkxdqqe.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.redwolf501.top/gtesmsysau.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.yj20258.top/gtsmhkkwsw.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.yanxiufei.cn/gtqbllpzrd.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.chenjidiqi.icu/gtgcnejfut.html

[L04] 设置超时
来源：http://hz.chenlongwang.top/gtigpbqrgz.html

Py:   requests.get(url, timeout=5)
来源：http://hz.dianchejie.cn/gtouodwfpw.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.tian-w.cn/gtdpvcizbs.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yj202588.top/gtmptfuupj.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jqgufenzy.top/gtepbacthy.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.fzhhl.top/gtlvbtbnfu.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.daxiang520.top/gtwsjfidgr.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.chenlongwang.top/gtshprcnuo.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.jiagoushi.top/gtqulkwqvj.html

[L05] 上传文件（multipart）
来源：http://hz.daria6918.cn/gtgbphqvve.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.shzxlz.cn/gtlpkhtxal.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.316326.xyz/gtukvhfccs.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.jinyuanbaomall.cn/gtllvcbrwb.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.yj20258.top/gtbgajdcsl.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.9152youxi.cn/gtkpoazgjv.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.nanxinkj.top/gtoommplok.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.xinyue.icu/gtpvhqyiie.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.jyoumei.cn/gtprsodvdj.html

[L06] 解析响应为 JSON
来源：http://hz.havefunace.top/gtxscvqxvz.html

Py:   resp.json()
来源：http://hz.sxryk.cn/gtbelaoopl.html

PHP:  json_decode($body, true);
来源：http://hz.yangfankeji.com/gtylendekg.html

JS:   await resp.json()
来源：http://hz.daxiang520.top/gtrowngfpj.html

TS:   await resp.json()
来源：http://hz.ppjwa.cn/gtpmbeuwrn.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.yj20258888.top/gtgmlvjahp.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.hammf.cn/gtvgthnalp.html

Ruby: JSON.parse(resp.body)
来源：http://hz.ppjwa.cn/gtdigdrhlc.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.xinyue.icu/gtoeivujqo.html

[L07] 处理 HTTP 状态码
来源：http://hz.xylfe.cn/gtsipkrwjp.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.yuanzhike.top/gtncmhfeqo.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.vqdsnc.cn/gtialoydlm.html

JS:   resp.ok;  resp.status
来源：http://hz.tanke756.top/gtmplnzzyf.html

TS:   resp.ok;  resp.status
来源：http://hz.gogol.net.cn/gtrrmxeyxv.html

Java: resp.statusCode()
来源：http://hz.havefunace.top/gtvjtewkkw.html

Go:   resp.StatusCode
来源：http://hz.dashuyun.cn/gtygtgkbun.html

Ruby: resp.code.to_i
来源：http://hz.jiagoushi.top/gtaicbvtlv.html

C#:   (int)resp.StatusCode
来源：http://hz.yj20258.top/gthisforvc.html

[L08] 并发请求多个地址
来源：http://hz.birdmap.top/gtzcsgbyhn.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.guowangkeji.top/gtxtunlxkz.html

PHP:  curl_multi_init() 系列
来源：http://hz.yuanzhike.top/gtnedxfnqh.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.cucudq.cn/gtmkawqsco.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.ehwqpu.com/gtwjbnqmzf.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.jyoumei.cn/gtpfngfgoz.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.cashguo.top/gtxvaboqfv.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.zhiwuduotai.top/gtmainqntq.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.chenzaomai.com/gtkchnafaa.html

================================================================================
来源：http://hz.gogol.net.cn/gtcqpqyvfq.html

M. 命令行 / 进程 / 环境
来源：http://hz.guannengcc.top/gtxlbdelef.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtbqxluxtg.html

[M01] 读取命令行参数
来源：http://hz.mhx1999.top/gtbjnovwgp.html

Py:   sys.argv[1:]
来源：http://hz.svipenyu.cn/gtvznburjo.html

PHP:  $argv;  $argc;
来源：http://hz.chenlongwang.top/gtbiuvwtmm.html

JS:   process.argv.slice(2)
来源：http://hz.zhijiandao.cn/gtakixwchb.html

TS:   process.argv.slice(2)
来源：http://hz.yj20258.top/gtgqrdxlxl.html

Java: args 数组（main 方法参数）
来源：http://hz.sxryk.cn/gtjhycasdn.html

Go:   os.Args[1:]
来源：http://hz.gaohongyu789.top/gtvbpfefju.html

Ruby: ARGV
来源：http://hz.zycfv.cn/gtzqajifam.html

C#:   args 数组（Main 方法参数）
来源：http://hz.yueranfly.top/gtbsxcjkyc.html

[M02] 读取环境变量
来源：http://hz.xziqi.cn/gtpnutrlqz.html

Py:   os.environ.get("HOME")
来源：http://hz.yanxiufei.cn/gtwgaznjlc.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.jlsjyb.cn/gtwcfzroix.html

JS:   process.env.HOME
来源：http://hz.tianlin.xyz/gtbtsphozs.html

TS:   process.env.HOME
来源：http://hz.ybcxt.top/gtolezdrld.html

Java: System.getenv("HOME")
来源：http://hz.chenzaomai.com/gtnzmeodph.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.cheryme.top/gtlwfjtjbb.html

Ruby: ENV["HOME"]
来源：http://hz.hnxiangtu.top/gtsymqaojh.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.vqdsnc.cn/gtxxtjpmoc.html

[M03] 执行外部命令
来源：http://hz.jiagoushi.top/gthcmwxpbb.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.shanyushiyangtech.top/gtobbnlium.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.nanxinkj.top/gtnyzeafkl.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.hywenlv.cn/gtnyhmgdqk.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.jlsjyb.cn/gtcxjvafla.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.chenzaomai.com/gtjcxgzmlz.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.shuidangran.top/gtlmyuyrhm.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.shuidangran.top/gtzqpurbsq.html

C#:   Process.Start("ls", "-l");
来源：http://hz.yj20258.top/gtvkawvrjc.html

[M04] 获取当前工作目录
来源：http://hz.zhoulong.xyz/gtdbxgdnss.html

Py:   os.getcwd()
来源：http://hz.redwolf501.top/gtjaerbtob.html

PHP:  getcwd();
来源：http://hz.mhx1999.top/gthbyzchbs.html

JS:   process.cwd()
来源：http://hz.yueranfly.top/gtkpegyriv.html

TS:   process.cwd()
来源：http://hz.yanxiufei.cn/gtqthgssoe.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.dashuyun.cn/gtquyedpra.html

Go:   os.Getwd()
来源：http://hz.wangshuangyany.cn/gtvxtutolf.html

Ruby: Dir.pwd
来源：http://hz.guannengcc.top/gtxyuxzwgz.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.yuanzhike.top/gtktgzxven.html

[M05] 设置退出码
来源：http://hz.ywan-chungtsiang.top/gtzyjmjvhn.html

Py:   sys.exit(1)
来源：http://hz.shanyushiyangtech.top/gtcqwamlsr.html

PHP:  exit(1);
来源：http://hz.ywan-chungtsiang.top/gtbirzqjjj.html

JS:   process.exit(1)
来源：http://hz.yueranfly.top/gteuwylipu.html

TS:   process.exit(1)
来源：http://hz.yuxming.cn/gtkbefljda.html

Java: System.exit(1)
来源：http://hz.meibo888.top/gthsjcfvxp.html

Go:   os.Exit(1)
来源：http://hz.tanke756.top/gtixujugfk.html

Ruby: exit 1
来源：http://hz.cdnleiting.top/gtskpzuifi.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.sxryk.cn/gtbcuynnmp.html

[M06] 向标准错误输出
来源：http://hz.yueranfly.top/gtwvgdeupy.html

Py:   print("err", file=sys.stderr)
来源：http://hz.gotoacloud.top/gtpouxlkri.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.xinyue.icu/gtdxnwnhbd.html

JS:   console.error("err")
来源：http://hz.jinghuilouyu.cn/gtxcblezsx.html

TS:   console.error("err")
来源：http://hz.52xcode.cn/gtrngtmdia.html

Java: System.err.println("err")
来源：http://hz.hongshengwenyu.top/gthbxwfbeu.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.52xcode.cn/gtssireqhd.html

Ruby: warn "err"
来源：http://hz.cheryme.top/gtudhzugto.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.tanke756.top/gtmqyhkuhk.html

[M07] 判断是否为主入口
来源：http://hz.jinghuilouyu.cn/gtvnmwilbz.html

Py:   if __name__ == "__main__":
来源：http://hz.hywenlv.cn/gtlljwbrpq.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.jinyuanbaomall.cn/gtfdprskdy.html

JS:   require.main === module
来源：http://hz.gogol.net.cn/gtibhsjajs.html

TS:   require.main === module
来源：http://hz.mhx1999.top/gtmxpoxoam.html

Java: public static void main(String[] args)
来源：http://hz.shanyushiyangkeji.top/gtehozanfv.html

Go:   func main()
来源：http://hz.pengpengdd.cyou/gtgjiqogpy.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.aizwys.cn/gtsttugibm.html

C#:   static void Main(string[] args)
来源：http://hz.hongshengwenyu.top/gtihddyedn.html

[M08] 获取系统与运行时信息
来源：http://hz.hammf.cn/gtmkgnhcrj.html

Py:   platform.system();  platform.python_version()
来源：http://hz.jinyuanbaomall.cn/gtoczijscy.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.yangfankeji.com/gtonemgxmb.html

JS:   process.platform;  process.version
来源：http://hz.xingfuxueyuan.xyz/gtamvpdkcl.html

TS:   process.platform;  process.version
来源：http://hz.yueranfly.top/gtmjzhwvou.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.cdnleiting.top/gtfbmiecmb.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.sxryk.cn/gtciwwxzay.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.jinqigfzy.top/gtppjkydwp.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.ehwqpu.com/gtzbehclao.html

================================================================================
来源：http://hz.shuidangran.top/gtufindxtc.html

N. 数据结构与算法
来源：http://hz.yangfankeji.com/gtandjaaom.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtbqnfbajg.html

[N01] 二分查找（有序数组）
来源：http://hz.gaohongyu789.top/gttwlkrvdb.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.shanyushiyangkeji.top/gtysyfitrg.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.guannengcc.top/gtuofktrgq.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zhongyouzk.top/gtzhzlpmor.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.fzhhl.top/gtkmmsjhjq.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.feifeiyinyue.top/gtbwagbdns.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.quarkkingdee.top/gttswawxku.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.jinghuilouyu.cn/gtxgppdrjf.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.chenlongwang.top/gtkglpntif.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.hfpthk.cn/gtwbbbagfq.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.9152youxi.cn/gtqabxnvdp.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.zhaomingkeji.xyz/gtaoyjwegz.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.wangshuangyany.cn/gtxpksocgw.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.hnqzz.top/gtzfjxlwtk.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.pycfn.com/gtqzozqzff.html

Go:   slices.Sort(arr)
来源：http://hz.jianghu66.top/gtnzlvjhwn.html

Ruby: arr.sort
来源：http://hz.gaohongyu789.top/gtlyqfannf.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.ydzc1.top/gtxfbmanjo.html

[N03] 快速排序（分治示例）
来源：http://hz.sxryk.cn/gtxgqsvvdo.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.aibaodan.cn/gtztgbvhtg.html

PHP:  // 递归实现，或用 usort
来源：http://hz.yangfankeji.com/gtwxkjphwc.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zycfv.cn/gtwjrmloba.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jlsjyb.cn/gtlizshqot.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.wangdashe.top/gtoqzswihr.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.xziqi.cn/gtoysywhtc.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.hongshengwenyu.top/gtugrasbkr.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.dashuyun.cn/gtanoyujwf.html

[N04] 斐波那契数列
来源：http://hz.hammf.cn/gtdauzbqkt.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.daria6918.cn/gtnagnymnn.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.jinyuanbaomall.cn/gtaophukzg.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.feifeiyinyue.top/gtbgmpqrcn.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.shanyushiyangkeji.top/gtyhgvefuw.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.yonumen.top/gtxbjsasrb.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.daria6918.cn/gtvfzybker.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.0kj1m.cn/gtrjmvhiyj.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.gaohongyu789.top/gtzpnlbzqt.html

[N05] 最大公约数
来源：http://hz.zhaomingkeji.xyz/gtpixwrvsc.html

Py:   math.gcd(a, b)
来源：http://hz.zdqjudy.top/gtyzlwqkbw.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.hnxiangtu.top/gtixaincxi.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.guowangkeji.top/gtnvlghmyf.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.havefunace.top/gteuvenbug.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.0kj1m.cn/gtmfnmhydu.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.tian-w.cn/gtailfgnmh.html

Ruby: a.gcd(b)
来源：http://hz.tian-w.cn/gtwxljibsm.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.yuanzhike.top/gtwlqxwnkz.html

[N06] 判断回文字符串
来源：http://hz.cdnleiting.top/gtapjcnhzj.html

Py:   s == s[::-1]
来源：http://hz.hongshengwenyu.top/gtbxsbuauv.html

PHP:  $s === strrev($s);
来源：http://hz.gogol.net.cn/gttvydewpa.html

JS:   s === [...s].reverse().join("")
来源：http://hz.jlsjyb.cn/gtprhdtltp.html

TS:   s === [...s].reverse().join("")
来源：http://hz.xuetiantiany.cn/gtutngpfks.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.shanyushiyangtech.top/gtgnlwhbsm.html

Go:   // 双指针从两端比较
来源：http://hz.feifeiyinyue.top/gtuwozhmmm.html

Ruby: s == s.reverse
来源：http://hz.tianlin.xyz/gtfxfsjrsq.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.ydzc1.top/gtdnblrkze.html

[N07] 两数之和（返回下标）
来源：http://hz.zhengqikj.top/gtvmvejedv.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.yj20258888.top/gtavximipe.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.xuanzx.com/gtjkryxtfd.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.jyoumei.cn/gtuckttgqf.html

TS:   // 手写 Map<string, number>
来源：http://hz.tian-w.cn/gtqgdxbztt.html

Java: // 手写 HashMap
来源：http://hz.hnqzz.top/gtppgmcvcc.html

Go:   // 手写 map[int]int
来源：http://hz.chenjidiqi.icu/gthenjjqci.html

Ruby: // 手写 Hash
来源：http://hz.nwbrower.top/gtfspmjtdt.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.aizwys.cn/gtctjqpqmy.html

[N08] 生成全排列
来源：http://hz.316326.xyz/gthzgcptgy.html

Py:   itertools.permutations(arr)
来源：http://hz.shanyushiyangkeji.top/gtnxvtbbyq.html

PHP:  // 手写递归交换
来源：http://hz.yj20258.top/gtcmsalauj.html

JS:   // 手写回溯递归
来源：http://hz.andypj.xyz/gtiyobyfpp.html

TS:   // 手写回溯递归
来源：http://hz.daxiang520.top/gtaaxfzauz.html

Java: // 手写回溯递归
来源：http://hz.daxiang520.top/gtkxwnujyq.html

Go:   // 手写回溯递归
来源：http://hz.tianlin.xyz/gtmbpojukk.html

Ruby: arr.permutation.to_a
来源：http://hz.hammf.cn/gtqpbjodap.html

C#:   // 手写回溯递归
来源：http://hz.chenzaomai.com/gtzuwrupzz.html

[N09] 栈与队列
来源：http://hz.gzhubu.top/gtmnyhwznn.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.cdnleiting.top/gtnwnvddwq.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.wangdashe.top/gtqkwghljh.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.vqdsnc.cn/gticcipuds.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.chenzaomai.com/gtfcttpfpr.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.shzxlz.cn/gtuzzmlvjy.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.andypj.xyz/gthbpipgpd.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.aizwys.cn/gtvyqpesdr.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.yj202588.top/gtjcyqdroo.html

[N10] 链表节点定义
来源：http://hz.jianghu66.top/gtpnzyknqy.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.haohaochexian.top/gtdgelynea.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.haohaochexian.top/gtqwnoufqc.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.zhixingplan.top/gtilzjmkaz.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.hfpthk.cn/gtwpwiwlka.html

Java: class Node { int v; Node next; }
来源：http://hz.hywenlv.cn/gtdvzndscl.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.wangdashe.top/gtslfrybdf.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.snrcjt.cn/gticzqdsmq.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.52xcode.cn/gtbnouchxt.html

[N11] 二叉树中序遍历
来源：http://hz.aibaodan.cn/gtbetfdvrx.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.havefunace.top/gtlatstyqo.html

PHP:  // 手写递归函数
来源：http://hz.guannengcc.top/gtgigeqkel.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.snrcjt.cn/gtstyxuipa.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.zycfv.cn/gtyotvevnk.html

Java: // 手写递归
来源：http://hz.tianlin.xyz/gtihctitox.html

Go:   // 手写递归
来源：http://hz.ywan-chungtsiang.top/gtyckektcm.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.pycfn.com/gtovptzqec.html

C#:   // 手写递归
来源：http://hz.xuetiantiany.cn/gtelrsloof.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.gzhubu.top/gtzyjaeunp.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.0kj1m.cn/gtacnnmjoq.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.xuanzx.com/gtlzhluxky.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.cucudq.cn/gtkhtofuth.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.chenlongwang.top/gtrktkkaep.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.iojbl.cn/gttuwgnfkk.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.hongshengwenyu.top/gthfesdjnm.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.zhongyouzk.top/gtddogonfy.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.zhongyouzk.top/gtpzpgqbkg.html

================================================================================
来源：http://hz.birdmap.top/gttpufosxc.html

O. 并发与异步
来源：http://hz.snrcjt.cn/gtdtzqflxu.html

================================================================================
来源：http://hz.0kj1m.cn/gttuoenyaj.html

[O01] 启动一个线程
来源：http://hz.jinyuanbaomall.cn/gtagbqdtly.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.fengsongda.top/gtpvtehzle.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.shangyingyoupin.top/gtgqnekyvl.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.havefunace.top/gtbkufikpf.html

TS:   // 同 JS
来源：http://hz.xylfe.cn/gtacgnwtie.html

Java: new Thread(() -> f()).start()
来源：http://hz.feifeiyinyue.top/gtwsxvmrpq.html

Go:   go f()
来源：http://hz.yangfankeji.com/gtdgnefojo.html

Ruby: Thread.new { f }
来源：http://hz.yj20258888.top/gtqqbwcaig.html

C#:   Task.Run(() => F());
来源：http://hz.aizwys.cn/gtyfmxknny.html

[O02] 使用线程池
来源：http://hz.xuetiantiany.cn/gtlqwnzenr.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.hnxiangtu.top/gtqumccvpi.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.jianghu66.top/gtzzvpmojl.html

JS:   // worker_threads 线程池
来源：http://hz.xylfe.cn/gtbbjrffad.html

TS:   // worker_threads 线程池
来源：http://hz.jiagoushi.top/gtiqkejsmc.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.snrcjt.cn/gtyolsshes.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.kuanghao11.cn/gtjergvwvv.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.zhaomingkeji.xyz/gtiycknmzb.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.sufxvd.cn/gtdraemtvu.html

[O03] 加锁保护共享数据
来源：http://hz.aibaodan.cn/gtfmbtbvph.html

Py:   with lock: shared += 1
来源：http://hz.jinghuilouyu.cn/gtogkdavwp.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.feifeiyinyue.top/gtqiilbaop.html


<!-- 参考信息 -->