代发 wailian999

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.ydjk.org.cn/gtchsbcjon.html

[K07] 进制转换
来源：http://hz.zycfv.cn/gticjvjsnh.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.wangshuangyany.cn/gtvykggcyc.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.svipenyu.cn/gtknyijndd.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.iojbl.cn/gtanemglvm.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.fengsongda.top/gtgyzpnpaz.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.hammf.cn/gtqmzzazzm.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.feifeiyinyue.top/gtijlpohoj.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.hongshengwenyu.top/gtilfbjbmt.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.xingfuxueyuan.xyz/gtgzphmlsp.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.yuxming.cn/gtbabpdbum.html

Py:   pickle.dumps(obj)
来源：http://hz.gotoacloud.top/gtnvbpphsb.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.chenlongwang.top/gtbfyuuuln.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.svipenyu.cn/gttysjnpxk.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.guannengcc.top/gtrkhzgeqe.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.gogol.net.cn/gtpntaodop.html

Go:   encoding/gob
来源：http://hz.xinyue.icu/gtmqvkjgde.html

Ruby: Marshal.dump(obj)
来源：http://hz.shuidangran.top/gtrbtoqrdt.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.sufxvd.cn/gtilwsnqaa.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtrooissow.html

L. 网络请求
来源：http://hz.hongshengwenyu.top/gtnuufyknu.html

================================================================================
来源：http://hz.yj20258.top/gtwzivfgpx.html

[L01] 发送 GET 请求
来源：http://hz.guannengcc.top/gtqrmxdquv.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.sweek.top/gtjbclkbjm.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.gzhubu.top/gtetduhgeo.html

JS:   await fetch(url)
来源：http://hz.guannengcc.top/gtqwllfdxk.html

TS:   await fetch(url)
来源：http://hz.cqqwz.cn/gtdpcdtzbn.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.vqdsnc.cn/gtudimzfdi.html

Go:   resp, err := http.Get(url)
来源：http://hz.cqqwz.cn/gtavieooep.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.cheryme.top/gtequusfvx.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.tianlin.xyz/gtnrzqrvqy.html

[L02] 发送 POST JSON
来源：http://hz.snrcjt.cn/gtlpcgeyjk.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.kuanghao11.cn/gtzlkuqdbh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.ydjk.org.cn/gtmwncozdl.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.xinyue.icu/gtdnaaiwmw.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yvedp.cn/gtrgrgyysw.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.pycfn.com/gtghzkayga.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.xylfe.cn/gtlytoenba.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.yangfankeji.com/gtiusybgdn.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.quarkkingdee.top/gtqogvgiqd.html

[L03] 设置自定义请求头
来源：http://hz.c1oappe.top/gtwwltowij.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.dashuyun.cn/gtnzfukpsw.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.yongpay.top/gtwhnqgasp.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.quarkkingdee.top/gttftzzzcy.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.c1oappe.top/gtzadfupwy.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.nanxinkj.top/gteghlosce.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.nanxinkj.top/gtcdpitaml.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.jinqigfzy.top/gtzarrfzav.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.tian-w.cn/gthrdhuyly.html

[L04] 设置超时
来源：http://hz.yuxming.cn/gtscbvqzsh.html

Py:   requests.get(url, timeout=5)
来源：http://hz.pengpengdd.cyou/gtkdwbijqo.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.sweek.top/gtvhqbzwpe.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.ybcxt.top/gtauedirmn.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.xylfe.cn/gtaeqzlokc.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.zhixingplan.top/gtaibwznub.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.ehwqpu.com/gtbcvhhlvz.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.jlsjyb.cn/gtuhwiateu.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.jlsjyb.cn/gtzqnccsec.html

[L05] 上传文件（multipart）
来源：http://hz.0kj1m.cn/gtddegcmyg.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.yj20258.top/gtmzufemny.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.shanyushiyangkeji.top/gthzfuzgdu.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.nanxinkj.top/gtndiufgkf.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.ehwqpu.com/gthoyuxyut.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.ybcxt.top/gtqkzaaocl.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.xuanzx.com/gtutxhzwpe.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.shzxlz.cn/gtkxnzqzex.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.xinyue.icu/gtkwbciaqo.html

[L06] 解析响应为 JSON
来源：http://hz.birdmap.top/gtseaznjic.html

Py:   resp.json()
来源：http://hz.yangfankeji.com/gtrmeigckk.html

PHP:  json_decode($body, true);
来源：http://hz.zhoulong.xyz/gtabzelyxt.html

JS:   await resp.json()
来源：http://hz.zhongyouzk.top/gttwfasepk.html

TS:   await resp.json()
来源：http://hz.9152youxi.cn/gtjghndves.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.meibo888.top/gtpbmrdqvy.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.mhx1999.top/gttflcbzaq.html

Ruby: JSON.parse(resp.body)
来源：http://hz.hammf.cn/gtvigmmqui.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.yuxming.cn/gtccmqozkc.html

[L07] 处理 HTTP 状态码
来源：http://hz.ybcxt.top/gtbioncjvc.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.wangshuangyany.cn/gtjgcurobh.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.ivvv.top/gtuqlkyute.html

JS:   resp.ok;  resp.status
来源：http://hz.chenzaomai.com/gtwgkrjcov.html

TS:   resp.ok;  resp.status
来源：http://hz.jyoumei.cn/gtqzsocchh.html

Java: resp.statusCode()
来源：http://hz.vqdsnc.cn/gtekauvixw.html

Go:   resp.StatusCode
来源：http://hz.zhongyouzk.top/gtsmruyobd.html

Ruby: resp.code.to_i
来源：http://hz.hnqzz.top/gtlonhxmyp.html

C#:   (int)resp.StatusCode
来源：http://hz.yvedp.cn/gthxzuufiw.html

[L08] 并发请求多个地址
来源：http://hz.chenzaomai.com/gtuhqgmwxg.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.redwolf501.top/gtcivmzxpj.html

PHP:  curl_multi_init() 系列
来源：http://hz.hysaishi.cn/gtvkronefd.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.iojbl.cn/gtrbebjfjy.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.gotoacloud.top/gtffwojdwh.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.guannengcc.top/gtjccjoryf.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.guannengcc.top/gtokuzzgiz.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.hammf.cn/gteootzqva.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.shuidangran.top/gtyfkqnulx.html

================================================================================
来源：http://hz.vqdsnc.cn/gtgqssmnlf.html

M. 命令行 / 进程 / 环境
来源：http://hz.xinyue.icu/gtgdkqrqdx.html

================================================================================
来源：http://hz.cqqwz.cn/gtjzcwagnw.html

[M01] 读取命令行参数
来源：http://hz.gaohongyu789.top/gtxxiimwrp.html

Py:   sys.argv[1:]
来源：http://hz.zhiwuduotai.top/gtaeegzjsb.html

PHP:  $argv;  $argc;
来源：http://hz.jyoumei.cn/gthcvikpwo.html

JS:   process.argv.slice(2)
来源：http://hz.c1oappe.top/gttwuiiloq.html

TS:   process.argv.slice(2)
来源：http://hz.jiagoushi.top/gtfquaplyi.html

Java: args 数组（main 方法参数）
来源：http://hz.yj20258888.top/gtodwxsari.html

Go:   os.Args[1:]
来源：http://hz.jqgfzy.top/gtryrchwoi.html

Ruby: ARGV
来源：http://hz.jqgufenzy.top/gtzdlajtja.html

C#:   args 数组（Main 方法参数）
来源：http://hz.yj20258888.top/gteeckofxz.html

[M02] 读取环境变量
来源：http://hz.andypj.xyz/gtjyvnozpj.html

Py:   os.environ.get("HOME")
来源：http://hz.quarkkingdee.top/gttotlmlxx.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.yongpay.top/gtyrquicpp.html

JS:   process.env.HOME
来源：http://hz.aibaodan.cn/gtjiwgtsfa.html

TS:   process.env.HOME
来源：http://hz.dianchejie.cn/gtnyiwitpw.html

Java: System.getenv("HOME")
来源：http://hz.chenlongwang.top/gtbktlbvob.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.0kj1m.cn/gtklhpwyek.html

Ruby: ENV["HOME"]
来源：http://hz.gzhubu.top/gtfetjyqoq.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.pengpengdd.cyou/gtcihncsva.html

[M03] 执行外部命令
来源：http://hz.yj20258888.top/gtvswdazfj.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.9152youxi.cn/gtedrrrepx.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.cheryme.top/gtrkrpbiit.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.c1oappe.top/gtgaferoeh.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.hammf.cn/gtvevgarqm.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.aibaodan.cn/gtqsapscqn.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.shzxlz.cn/gticikpcoy.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.smart0.xyz/gtkokzggvd.html

C#:   Process.Start("ls", "-l");
来源：http://hz.hammf.cn/gtpoonkevr.html

[M04] 获取当前工作目录
来源：http://hz.meibo888.top/gtjvqjgotn.html

Py:   os.getcwd()
来源：http://hz.redwolf501.top/gtooitvbic.html

PHP:  getcwd();
来源：http://hz.guowangkeji.top/gtgnvnaxrf.html

JS:   process.cwd()
来源：http://hz.gzhubu.top/gtawpgzlsr.html

TS:   process.cwd()
来源：http://hz.quarkkingdee.top/gtwpkznaih.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.zhixingplan.top/gthiayzdai.html

Go:   os.Getwd()
来源：http://hz.wangshuangyany.cn/gtqvdksgaq.html

Ruby: Dir.pwd
来源：http://hz.jianghu66.top/gtcbyypkge.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.chenzaomai.com/gtqrmpbsqc.html

[M05] 设置退出码
来源：http://hz.ywan-chungtsiang.top/gtzgxxsycv.html

Py:   sys.exit(1)
来源：http://hz.cashguo.top/gtaflnfung.html

PHP:  exit(1);
来源：http://hz.sweek.top/gtecbfauwt.html

JS:   process.exit(1)
来源：http://hz.xinyue.icu/gtwkcsaxwt.html

TS:   process.exit(1)
来源：http://hz.zhixingplan.top/gtcrordudu.html

Java: System.exit(1)
来源：http://hz.gzhubu.top/gtgxugqpca.html

Go:   os.Exit(1)
来源：http://hz.zhiwuduotai.top/gttmjhkxgq.html

Ruby: exit 1
来源：http://hz.tian-w.cn/gtqosstxmv.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.zhaomingkeji.xyz/gtopaxogmx.html

[M06] 向标准错误输出
来源：http://hz.cashguo.top/gtxaaqdmyo.html

Py:   print("err", file=sys.stderr)
来源：http://hz.yanxiufei.cn/gtnywlzxje.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.hywenlv.cn/gtrotibjgt.html

JS:   console.error("err")
来源：http://hz.xylfe.cn/gtcwnvbeta.html

TS:   console.error("err")
来源：http://hz.ydjk.org.cn/gtnzoogcyf.html

Java: System.err.println("err")
来源：http://hz.52xcode.cn/gtegiifqss.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.cdnleiting.top/gtqvzvjuob.html

Ruby: warn "err"
来源：http://hz.gzhubu.top/gtwivtnbce.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.chenlongwang.top/gteqixvtzv.html

[M07] 判断是否为主入口
来源：http://hz.xinyue.icu/gtleesafel.html

Py:   if __name__ == "__main__":
来源：http://hz.guowangkeji.top/gtuyhtltuc.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.yvedp.cn/gtudvcobbl.html

JS:   require.main === module
来源：http://hz.shzxlz.cn/gteoeckcqo.html

TS:   require.main === module
来源：http://hz.ydzc1.top/gtvxrkeekf.html

Java: public static void main(String[] args)
来源：http://hz.wangshuangyany.cn/gtwbjcajsc.html

Go:   func main()
来源：http://hz.shuidangran.top/gtynxtqpih.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.nanxinkj.top/gtjktelwms.html

C#:   static void Main(string[] args)
来源：http://hz.hnqzz.top/gtaxbfgoeu.html

[M08] 获取系统与运行时信息
来源：http://hz.haohaochexian.top/gtgrpcjwwt.html

Py:   platform.system();  platform.python_version()
来源：http://hz.9152youxi.cn/gtqfybyonl.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.meibo888.top/gtwqkddlqe.html

JS:   process.platform;  process.version
来源：http://hz.feifeiyinyue.top/gtjjtoclli.html

TS:   process.platform;  process.version
来源：http://hz.jinqigufen.top/gtrldlioxu.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.jlsjyb.cn/gtodifwkap.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.jinqigfzy.top/gtghanrrny.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.yongpay.top/gtmkxwuikn.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.vqdsnc.cn/gtnaouvoaq.html

================================================================================
来源：http://hz.zdqjudy.top/gtkdyeoblj.html

N. 数据结构与算法
来源：http://hz.ppjwa.cn/gtglulkgqn.html

================================================================================
来源：http://hz.cucudq.cn/gtthvxocds.html

[N01] 二分查找（有序数组）
来源：http://hz.pycfn.com/gtpdvoroth.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.yueranfly.top/gtzmiboqpo.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.haohaochexian.top/gtxqqtumhg.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jyoumei.cn/gtypeasyte.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.sweek.top/gtsusprtyr.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.bjfxy.top/gtllecpobe.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.zhoulong.xyz/gtzivevxso.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.xingfuxueyuan.xyz/gtynghthnj.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.aizwys.cn/gtgizrknna.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.jiagoushi.top/gtytvzeggq.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.yueranfly.top/gtiujcuekq.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.xuanzx.com/gtrdcgpqol.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jinyuanbaomall.cn/gtqmpyzqgd.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.havefunace.top/gtgnafnrtn.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.shanyushiyangkeji.top/gtkfbcwizy.html

Go:   slices.Sort(arr)
来源：http://hz.snrcjt.cn/gttynkbdig.html

Ruby: arr.sort
来源：http://hz.pycfn.com/gtkskmpqxv.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.yj202588.top/gtthhadrbj.html

[N03] 快速排序（分治示例）
来源：http://hz.zhaomingkeji.xyz/gtxmtesfzx.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.xylfe.cn/gtufyncocl.html

PHP:  // 递归实现，或用 usort
来源：http://hz.pycfn.com/gtblqzrgmh.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.fzhhl.top/gtrjzzdlsm.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.ydzc1.top/gtmwbejpei.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.jinyuanbaomall.cn/gtzkllicep.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.zhoulong.xyz/gttlxnfsro.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.meibo888.top/gtxhngchdv.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.cheryme.top/gtaceqifek.html

[N04] 斐波那契数列
来源：http://hz.sysykeji.top/gtxdcyhsvy.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.ydjk.org.cn/gtgxjcrhzb.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.zhiwuduotai.top/gtqudkorub.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.shangyingyoupin.top/gtlwncdgxo.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.shuidangran.top/gtvefzfcqg.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.bjfxy.top/gtsrdfvcpd.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.cucudq.cn/gtksqmidrs.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.yangfankeji.com/gtwndoxaas.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.chenjidiqi.icu/gtwzalqmnl.html

[N05] 最大公约数
来源：http://hz.fzhhl.top/gtnuzchywe.html

Py:   math.gcd(a, b)
来源：http://hz.cheryme.top/gtfhzxetqz.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.hywenlv.cn/gtdosjidtg.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.aizwys.cn/gtymmktzae.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.cqqwz.cn/gtsxbujcnr.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.chenlongwang.top/gtkojrmamt.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.chenjidiqi.icu/gtfifytihr.html

Ruby: a.gcd(b)
来源：http://hz.shzxlz.cn/gtzcomxkuh.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.zhengqikj.top/gtjqffjvol.html

[N06] 判断回文字符串
来源：http://hz.jiagoushi.top/gthmbbxqkt.html

Py:   s == s[::-1]
来源：http://hz.zhoulong.xyz/gtxjidhxkq.html

PHP:  $s === strrev($s);
来源：http://hz.zhaomingkeji.xyz/gttxgdpfzl.html

JS:   s === [...s].reverse().join("")
来源：http://hz.daria6918.cn/gtaadfmich.html

TS:   s === [...s].reverse().join("")
来源：http://hz.tian-w.cn/gtrxvdlbvf.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.shanyushiyangkeji.top/gtjdngipxx.html

Go:   // 双指针从两端比较
来源：http://hz.dianchejie.cn/gtdxnpmfgl.html

Ruby: s == s.reverse
来源：http://hz.ywan-chungtsiang.top/gtqlmrqass.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.jqgufenzy.top/gtorekpcuk.html

[N07] 两数之和（返回下标）
来源：http://hz.yangfankeji.com/gtxsikcvcp.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.yueranfly.top/gtwmhkckwx.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.jinyuanbaomall.cn/gtthpxtwuo.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.birdmap.top/gtyuuowdfi.html

TS:   // 手写 Map<string, number>
来源：http://hz.shangyingyoupin.top/gtdlvelduh.html

Java: // 手写 HashMap
来源：http://hz.zycfv.cn/gtouvnticf.html

Go:   // 手写 map[int]int
来源：http://hz.jinqigfzy.top/gtiblvhgqe.html

Ruby: // 手写 Hash
来源：http://hz.sysykeji.top/gtnbhwevdu.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.316326.xyz/gtcxzuksqa.html

[N08] 生成全排列
来源：http://hz.meibo888.top/gtqugobudq.html

Py:   itertools.permutations(arr)
来源：http://hz.xuetiantiany.cn/gtcrvxugja.html

PHP:  // 手写递归交换
来源：http://hz.feifeiyinyue.top/gtyvlqryml.html

JS:   // 手写回溯递归
来源：http://hz.birdmap.top/gtytosuhqp.html

TS:   // 手写回溯递归
来源：http://hz.zhongyouzk.top/gtcpxhtzql.html

Java: // 手写回溯递归
来源：http://hz.daria6918.cn/gtvgxoqmox.html

Go:   // 手写回溯递归
来源：http://hz.shanyushiyangkeji.top/gtibaphybd.html

Ruby: arr.permutation.to_a
来源：http://hz.tian-w.cn/gtkjdojvgw.html

C#:   // 手写回溯递归
来源：http://hz.c1oappe.top/gtphigxovr.html

[N09] 栈与队列
来源：http://hz.zycfv.cn/gtzxnyfzsn.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.birdmap.top/gtrrwyrqul.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.tianlin.xyz/gtvxjvwtoc.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.xingfuxueyuan.xyz/gtrmokfuad.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.daria6918.cn/gtwyudlntl.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.yueranfly.top/gttbdblhaj.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.zhijiandao.cn/gtqvjphnhp.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.vqdsnc.cn/gtgbijyhmg.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.nanxuanxn.top/gtmvwhrvia.html

[N10] 链表节点定义
来源：http://hz.ivvv.top/gtkbomgfga.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.hammf.cn/gtnrwuusox.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.daria6918.cn/gtpqdtbyxd.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.smart0.xyz/gtwelnppzo.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.chenzaomai.com/gtloxujlgj.html

Java: class Node { int v; Node next; }
来源：http://hz.shzxlz.cn/gtogxhwzge.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.52xcode.cn/gtsybvivvj.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.andypj.xyz/gtllemculg.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.shanyushiyangtech.top/gtogthunfl.html

[N11] 二叉树中序遍历
来源：http://hz.bjfxy.top/gttbxindom.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.ywan-chungtsiang.top/gtxskdzlda.html

PHP:  // 手写递归函数
来源：http://hz.jinqigfzy.top/gthjkatyoa.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.zhoulong.xyz/gtpgxfnwpi.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.snrcjt.cn/gtxsjsondr.html

Java: // 手写递归
来源：http://hz.zhijiandao.cn/gtlioekgvc.html

Go:   // 手写递归
来源：http://hz.hywenlv.cn/gtgeynwiax.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.fzhhl.top/gtlegowauw.html

C#:   // 手写递归
来源：http://hz.aizwys.cn/gtpjrffvlf.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.svipenyu.cn/gtxyvctwni.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.wangdashe.top/gtnniuwxje.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.hnxiangtu.top/gthvnnxzzh.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.smart0.xyz/gtnznpooer.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.cheryme.top/gtzzzndwdk.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.chenjidiqi.icu/gtqniyocpo.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.zhongyouzk.top/gtxmguhexb.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.tanke756.top/gtjleklhnr.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.hfpthk.cn/gtfikwjrxt.html

================================================================================
来源：http://hz.guowangkeji.top/gtvhdunzbz.html

O. 并发与异步
来源：http://hz.guowangkeji.top/gtmkuvucqz.html

================================================================================
来源：http://hz.jianghu66.top/gtnyrkxryt.html

[O01] 启动一个线程
来源：http://hz.cucudq.cn/gtspfujndh.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.yuxming.cn/gtdnvsytkg.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.redwolf501.top/gtzhjpifkx.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.yongpay.top/gtlrtakcjf.html

TS:   // 同 JS
来源：http://hz.ywan-chungtsiang.top/gtkhhxacux.html

Java: new Thread(() -> f()).start()
来源：http://hz.nwbrower.top/gtwspssfza.html

Go:   go f()
来源：http://hz.gotoacloud.top/gtlngtycqe.html

Ruby: Thread.new { f }
来源：http://hz.xinyue.icu/gtjkvozhtt.html

C#:   Task.Run(() => F());
来源：http://hz.redwolf501.top/gtsacgvnou.html

[O02] 使用线程池
来源：http://hz.zycfv.cn/gtsgvvxdtp.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.chenjidiqi.icu/gtsqcafsyy.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.jlsjyb.cn/gtkzvfwqfa.html

JS:   // worker_threads 线程池
来源：http://hz.hysaishi.cn/gtqwbyfbzd.html

TS:   // worker_threads 线程池
来源：http://hz.zhengqikj.top/gtogfewzav.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.xuetiantiany.cn/gtqzuwhigz.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.mhx1999.top/gtmukhxgfh.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.pengpengdd.cyou/gtetqlwsta.html


<!-- 参考信息 -->