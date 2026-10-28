代发 wailian999

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.quarkkingdee.top/gtjtebbckv.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.jqgfzy.top/gtvmxkkpfa.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.chenjidiqi.icu/gtlbugtsgi.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.dashuyun.cn/gtzrlylgac.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.zhoulong.xyz/gtekuxtezp.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.zhijiandao.cn/gteaunohjq.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.zhiwuduotai.top/gteavhshrv.html

Py:   pickle.dumps(obj)
来源：http://hz.shangyingyoupin.top/gtsnohylja.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.mhx1999.top/gtwnyggzsi.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.zhiwuduotai.top/gtymedchyf.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.xinyue.icu/gttsvebdto.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.cdnleiting.top/gtdaaovmld.html

Go:   encoding/gob
来源：http://hz.yvedp.cn/gtcealsrvn.html

Ruby: Marshal.dump(obj)
来源：http://hz.guowangkeji.top/gtuvxcyfbr.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.tianlin.xyz/gtqalaeopr.html

================================================================================
来源：http://hz.svipenyu.cn/gtzkigxgos.html

L. 网络请求
来源：http://hz.jinyuanbaomall.cn/gttyhnipnp.html

================================================================================
来源：http://hz.jqgufenzy.top/gtcgnduwqq.html

[L01] 发送 GET 请求
来源：http://hz.tanke756.top/gttdcqnmqn.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.snrcjt.cn/gtrdkxrmtv.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.mhx1999.top/gtwuezcmni.html

JS:   await fetch(url)
来源：http://hz.hysaishi.cn/gteqqkyxko.html

TS:   await fetch(url)
来源：http://hz.cheryme.top/gtaxmswszw.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.shuidangran.top/gtufjndhfh.html

Go:   resp, err := http.Get(url)
来源：http://hz.jqgfzy.top/gthmyqfpzq.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.yangfankeji.com/gtksfmbeyz.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.ppjwa.cn/gtfchvpkyp.html

[L02] 发送 POST JSON
来源：http://hz.yj20258.top/gtztpwbcoj.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.0kj1m.cn/gtmetgajcl.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.c1oappe.top/gtvtjfvbmi.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.pengpengdd.cyou/gttwnphspa.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.feifeiyinyue.top/gteytywwfv.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.ivvv.top/gtavvksfrh.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.zhengqikj.top/gthvlsepmw.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.yongpay.top/gtzazvtuyp.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.shangyingyoupin.top/gtwgtkjezi.html

[L03] 设置自定义请求头
来源：http://hz.jqgufenzy.top/gtznldtzyy.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.hongshengwenyu.top/gtduddqmcr.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.birdmap.top/gtyabdbkuv.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.tianlin.xyz/gtolfhufub.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.shangyingyoupin.top/gtbapwttqp.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.nanxinkj.top/gtyrsnsujk.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.jinqigufen.top/gtuuqejdyu.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.zdqjudy.top/gtvwvmwpgn.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.jlsjyb.cn/gtajbknexw.html

[L04] 设置超时
来源：http://hz.jqgfzy.top/gtdbxtyoua.html

Py:   requests.get(url, timeout=5)
来源：http://hz.cheryme.top/gtlyczikvx.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.kuanghao11.cn/gtrsjohhan.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.snrcjt.cn/gttpubioqe.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.hnqzz.top/gtwhvmrsld.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.jqgfzy.top/gtxaflfggq.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.yanxiufei.cn/gtvydgwlps.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.tanke756.top/gtisskcezr.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.xylfe.cn/gtssmgwvks.html

[L05] 上传文件（multipart）
来源：http://hz.cucudq.cn/gtzcwytqil.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.ybcxt.top/gtaziuxclm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.pengpengdd.cyou/gteqadncht.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.xinyue.icu/gtsmtdghnq.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.yonumen.top/gtfwvohdti.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.zhixingplan.top/gtmhspflqq.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.nwbrower.top/gtzwibngwj.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.shzxlz.cn/gtcobywhmr.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.jiagoushi.top/gtsoodxnoo.html

[L06] 解析响应为 JSON
来源：http://hz.hywenlv.cn/gthzfgizif.html

Py:   resp.json()
来源：http://hz.fengsongda.top/gtszldtkxo.html

PHP:  json_decode($body, true);
来源：http://hz.kuanghao11.cn/gtwohfbynb.html

JS:   await resp.json()
来源：http://hz.dianchejie.cn/gtncbtnvuk.html

TS:   await resp.json()
来源：http://hz.xziqi.cn/gtiikbfggf.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.zhaomingkeji.xyz/gtotqagpjo.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.ppjwa.cn/gtkqkzpnmf.html

Ruby: JSON.parse(resp.body)
来源：http://hz.hnqzz.top/gtunbshafy.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.zhixingplan.top/gthsadbkkl.html

[L07] 处理 HTTP 状态码
来源：http://hz.yj202588.top/gtcypugehp.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.zhaomingkeji.xyz/gtjudyuecm.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.sufxvd.cn/gtixmqbtly.html

JS:   resp.ok;  resp.status
来源：http://hz.guannengcc.top/gtunfxurzp.html

TS:   resp.ok;  resp.status
来源：http://hz.cqqwz.cn/gtuppvlami.html

Java: resp.statusCode()
来源：http://hz.feifeiyinyue.top/gtgngpdjel.html

Go:   resp.StatusCode
来源：http://hz.gzhubu.top/gthethzwgo.html

Ruby: resp.code.to_i
来源：http://hz.ybcxt.top/gtsenulawp.html

C#:   (int)resp.StatusCode
来源：http://hz.daria6918.cn/gtoobdsncb.html

[L08] 并发请求多个地址
来源：http://hz.xinyue.icu/gtpxlfgeiy.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.zhengqikj.top/gtxsldpekb.html

PHP:  curl_multi_init() 系列
来源：http://hz.ybcxt.top/gtctmpuvlc.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yangfankeji.com/gtitmenyos.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.tian-w.cn/gtltktwasb.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.bjfxy.top/gtyjzaufwn.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.birdmap.top/gtdmcpldmn.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.tian-w.cn/gthgpzddny.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.tianlin.xyz/gttjcifief.html

================================================================================
来源：http://hz.havefunace.top/gtjjqojywb.html

M. 命令行 / 进程 / 环境
来源：http://hz.smart0.xyz/gthyjzuzlz.html

================================================================================
来源：http://hz.sxryk.cn/gtzijkjxjp.html

[M01] 读取命令行参数
来源：http://hz.gotoacloud.top/gtqhkpnmqj.html

Py:   sys.argv[1:]
来源：http://hz.shuidangran.top/gtpwszxwdr.html

PHP:  $argv;  $argc;
来源：http://hz.havefunace.top/gthddrqsaw.html

JS:   process.argv.slice(2)
来源：http://hz.cheryme.top/gthweitqyw.html

TS:   process.argv.slice(2)
来源：http://hz.hammf.cn/gtvohsuxfj.html

Java: args 数组（main 方法参数）
来源：http://hz.wangdashe.top/gtdbsorsko.html

Go:   os.Args[1:]
来源：http://hz.aibaodan.cn/gtvwrwafmr.html

Ruby: ARGV
来源：http://hz.iojbl.cn/gtmxpnlotz.html

C#:   args 数组（Main 方法参数）
来源：http://hz.yj202588.top/gtxwpijadf.html

[M02] 读取环境变量
来源：http://hz.zhijiandao.cn/gtgunjisfi.html

Py:   os.environ.get("HOME")
来源：http://hz.zycfv.cn/gtulgpsuhy.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.fengsongda.top/gtequqzbpf.html

JS:   process.env.HOME
来源：http://hz.jyoumei.cn/gtpqjmosyn.html

TS:   process.env.HOME
来源：http://hz.snrcjt.cn/gtvtguqslm.html

Java: System.getenv("HOME")
来源：http://hz.bjfxy.top/gtjzxykwnq.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.fengsongda.top/gtrwvobxkm.html

Ruby: ENV["HOME"]
来源：http://hz.jqgufenzy.top/gtympjeygb.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.hnxiangtu.top/gtvxapwnmf.html

[M03] 执行外部命令
来源：http://hz.gotoacloud.top/gtsjhgyaiw.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.hammf.cn/gtqduuumhe.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.jinyuanbaomall.cn/gtkszammtm.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.ydjk.org.cn/gtafrsspfa.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.jianghu66.top/gtyzvbmvab.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.jinqigfzy.top/gtzsembwmw.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.tianlin.xyz/gtzlybfsrr.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.yonumen.top/gtqtzliycw.html

C#:   Process.Start("ls", "-l");
来源：http://hz.nwbrower.top/gtsghaulsm.html

[M04] 获取当前工作目录
来源：http://hz.c1oappe.top/gthkpwsblq.html

Py:   os.getcwd()
来源：http://hz.feifeiyinyue.top/gtxyqosdwu.html

PHP:  getcwd();
来源：http://hz.hnxiangtu.top/gtwftbemyr.html

JS:   process.cwd()
来源：http://hz.hongshengwenyu.top/gtouzgucge.html

TS:   process.cwd()
来源：http://hz.c1oappe.top/gtdbbquxaw.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.yvedp.cn/gtosgmrhnw.html

Go:   os.Getwd()
来源：http://hz.zhoulong.xyz/gtsjdaewbu.html

Ruby: Dir.pwd
来源：http://hz.sysykeji.top/gtjoopdsdx.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.jqgufenzy.top/gtrzgoloim.html

[M05] 设置退出码
来源：http://hz.0kj1m.cn/gtvsrsmpib.html

Py:   sys.exit(1)
来源：http://hz.c1oappe.top/gtqxgnjddl.html

PHP:  exit(1);
来源：http://hz.zhixingplan.top/gtdepbrubo.html

JS:   process.exit(1)
来源：http://hz.nanxuanxn.top/gtmnrmdsqw.html

TS:   process.exit(1)
来源：http://hz.pycfn.com/gteutwzwdu.html

Java: System.exit(1)
来源：http://hz.zycfv.cn/gtbmbzuxfd.html

Go:   os.Exit(1)
来源：http://hz.fengsongda.top/gtnjhjzmwz.html

Ruby: exit 1
来源：http://hz.pycfn.com/gtgbxlhiki.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.shanyushiyangtech.top/gttbpyplpc.html

[M06] 向标准错误输出
来源：http://hz.dashuyun.cn/gtzokslquh.html

Py:   print("err", file=sys.stderr)
来源：http://hz.iojbl.cn/gtuzkzdxra.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.snrcjt.cn/gthjbptkpi.html

JS:   console.error("err")
来源：http://hz.tanke756.top/gtgdzfajpn.html

TS:   console.error("err")
来源：http://hz.yj20258.top/gttfilwnru.html

Java: System.err.println("err")
来源：http://hz.shuidangran.top/gtbutfpvai.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.sufxvd.cn/gthrcojgxb.html

Ruby: warn "err"
来源：http://hz.sweek.top/gtnxmyudkm.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.guannengcc.top/gtdowgmfyr.html

[M07] 判断是否为主入口
来源：http://hz.hfpthk.cn/gtqioypnhg.html

Py:   if __name__ == "__main__":
来源：http://hz.ywan-chungtsiang.top/gtqjhntham.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.hfpthk.cn/gtutdwjxhg.html

JS:   require.main === module
来源：http://hz.guannengcc.top/gtifbbciap.html

TS:   require.main === module
来源：http://hz.shanyushiyangkeji.top/gtqthaxluq.html

Java: public static void main(String[] args)
来源：http://hz.jqgfzy.top/gtbktnkuwf.html

Go:   func main()
来源：http://hz.jinqigfzy.top/gtlfokcmvr.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.jiagoushi.top/gtegyxnopk.html

C#:   static void Main(string[] args)
来源：http://hz.jinqigfzy.top/gtdptkllqk.html

[M08] 获取系统与运行时信息
来源：http://hz.chenjidiqi.icu/gtcnxwxnuu.html

Py:   platform.system();  platform.python_version()
来源：http://hz.jinqigfzy.top/gtpoensrlh.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.zhiwuduotai.top/gtxxllbclv.html

JS:   process.platform;  process.version
来源：http://hz.zhixingplan.top/gtecuervos.html

TS:   process.platform;  process.version
来源：http://hz.gzhubu.top/gtpvhedxnl.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.zhengqikj.top/gtemwyaoic.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.0kj1m.cn/gtjdnjxvzq.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.jlsjyb.cn/gtbfwnkkqr.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.yangfankeji.com/gtdjjknsdf.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtcyhjrzne.html

N. 数据结构与算法
来源：http://hz.daxiang520.top/gttmkgimbe.html

================================================================================
来源：http://hz.cashguo.top/gtclngfxyo.html

[N01] 二分查找（有序数组）
来源：http://hz.vqdsnc.cn/gtscxkaqte.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.haohaochexian.top/gtjocuqmqo.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.nanxinkj.top/gtqzorrxak.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zhaomingkeji.xyz/gtamvdtwix.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yonumen.top/gtrvdkkxzu.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.shzxlz.cn/gtougogzjg.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.sweek.top/gtonygcquc.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.hfpthk.cn/gtvozmszuk.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.havefunace.top/gthcvbzsqp.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.tanke756.top/gtggbdbmkg.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.ydzc1.top/gtygybhhny.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.hnqzz.top/gtxrhgkdfi.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.cashguo.top/gtvprpcipi.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.meibo888.top/gtbomlrqyy.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.shanyushiyangkeji.top/gtxcksszqg.html

Go:   slices.Sort(arr)
来源：http://hz.yonumen.top/gtvdywrcdy.html

Ruby: arr.sort
来源：http://hz.guowangkeji.top/gtwchftphg.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.gotoacloud.top/gtcnuqmjeu.html

[N03] 快速排序（分治示例）
来源：http://hz.iojbl.cn/gtavsaegbr.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.snrcjt.cn/gtvygmdplg.html

PHP:  // 递归实现，或用 usort
来源：http://hz.xylfe.cn/gtvhirtlyf.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jinyuanbaomall.cn/gtbwhiolxs.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.316326.xyz/gtczsjonef.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.shanyushiyangkeji.top/gtttzqszdg.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.yuanzhike.top/gtvocrwrgf.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.tianlin.xyz/gtormtivds.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.nwbrower.top/gtyxaxaxlf.html

[N04] 斐波那契数列
来源：http://hz.xuanzx.com/gtpxdlqmkx.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.jiagoushi.top/gtntdfjvnj.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.cheryme.top/gtvanezzhu.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.pycfn.com/gtitpatiuo.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.tanke756.top/gtcfirlzzy.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.9152youxi.cn/gtsfuvkxsl.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.52xcode.cn/gtcnplvoib.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.yj20258.top/gthbxjjtba.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.fzhhl.top/gtzayafaru.html

[N05] 最大公约数
来源：http://hz.fzhhl.top/gtdpnkcsnk.html

Py:   math.gcd(a, b)
来源：http://hz.cucudq.cn/gtctyckdrw.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.nanxinkj.top/gthhhrveyv.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.quarkkingdee.top/gtmxlgtctn.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.shanyushiyangkeji.top/gthxbhpafe.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.havefunace.top/gtozrfastg.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.fengsongda.top/gtrbmnacmm.html

Ruby: a.gcd(b)
来源：http://hz.zhaomingkeji.xyz/gtoixtrggn.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.jianghu66.top/gtbepjxboc.html

[N06] 判断回文字符串
来源：http://hz.9152youxi.cn/gtgnmbqdhz.html

Py:   s == s[::-1]
来源：http://hz.yonumen.top/gtdzomzxlp.html

PHP:  $s === strrev($s);
来源：http://hz.nanxuanxn.top/gtxryzubkm.html

JS:   s === [...s].reverse().join("")
来源：http://hz.zhoulong.xyz/gtcttlwdvt.html

TS:   s === [...s].reverse().join("")
来源：http://hz.xuetiantiany.cn/gtcbarmkep.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.sysykeji.top/gtnmxkeflk.html

Go:   // 双指针从两端比较
来源：http://hz.0kj1m.cn/gtodaokpgt.html

Ruby: s == s.reverse
来源：http://hz.gogol.net.cn/gtuboqyimj.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.hnqzz.top/gtilcvcjpk.html

[N07] 两数之和（返回下标）
来源：http://hz.zhoulong.xyz/gtydjflsyi.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.pengpengdd.cyou/gtbwnpmhuk.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.meibo888.top/gtweoqoifh.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.zycfv.cn/gtetosttji.html

TS:   // 手写 Map<string, number>
来源：http://hz.yonumen.top/gtjxtbijbv.html

Java: // 手写 HashMap
来源：http://hz.9152youxi.cn/gtrnvnjatm.html

Go:   // 手写 map[int]int
来源：http://hz.bjfxy.top/gtdyqbntpr.html

Ruby: // 手写 Hash
来源：http://hz.nanxuanxn.top/gtbqnupxps.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.nwbrower.top/gtxpmfnkza.html

[N08] 生成全排列
来源：http://hz.gaohongyu789.top/gtvnaicijj.html

Py:   itertools.permutations(arr)
来源：http://hz.sweek.top/gtgsizfonh.html

PHP:  // 手写递归交换
来源：http://hz.sufxvd.cn/gtuchmmymr.html

JS:   // 手写回溯递归
来源：http://hz.nanxinkj.top/gtjpghtmld.html

TS:   // 手写回溯递归
来源：http://hz.tian-w.cn/gtlaspwidx.html

Java: // 手写回溯递归
来源：http://hz.jqgufenzy.top/gtyktxirgd.html

Go:   // 手写回溯递归
来源：http://hz.316326.xyz/gtnrohuexm.html

Ruby: arr.permutation.to_a
来源：http://hz.0kj1m.cn/gtjcfzkras.html

C#:   // 手写回溯递归
来源：http://hz.pengpengdd.cyou/gtajpmuwzn.html

[N09] 栈与队列
来源：http://hz.bjfxy.top/gtqkupwhqo.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.chenzaomai.com/gtexeegoet.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.yueranfly.top/gtvleiobyw.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.smart0.xyz/gttrsoodux.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.yuanzhike.top/gtyixruntb.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.xuetiantiany.cn/gtkudkwfsk.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.ivvv.top/gtdekvtejc.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.yueranfly.top/gtzaejiqfe.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.hammf.cn/gtoswewwvv.html

[N10] 链表节点定义
来源：http://hz.yanxiufei.cn/gtjcmbokdo.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.guowangkeji.top/gttcehihst.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.xziqi.cn/gtrzjeizca.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.ywan-chungtsiang.top/gtymezcwka.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.nanxuanxn.top/gtktpwixkn.html

Java: class Node { int v; Node next; }
来源：http://hz.xinyue.icu/gthrzmmstf.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.guowangkeji.top/gtnpegicms.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.xingfuxueyuan.xyz/gtakfmugvt.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.jinyuanbaomall.cn/gtzzprdxdf.html

[N11] 二叉树中序遍历
来源：http://hz.yj202588.top/gtmdyjvuzp.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.ydjk.org.cn/gtyhedwynt.html

PHP:  // 手写递归函数
来源：http://hz.xinyue.icu/gtutsymuyq.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.dashuyun.cn/gtfcrvuttg.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.redwolf501.top/gtimgxiokm.html

Java: // 手写递归
来源：http://hz.fzhhl.top/gtfvgxyfgq.html

Go:   // 手写递归
来源：http://hz.zhijiandao.cn/gtwiheaahm.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.nwbrower.top/gtghnitzda.html

C#:   // 手写递归
来源：http://hz.jinghuilouyu.cn/gtfwedihcz.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.pycfn.com/gtiswcjfka.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.jiagoushi.top/gthyawgjsb.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.gaohongyu789.top/gteqvjkbpy.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.vqdsnc.cn/gtpxamerpr.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.zhoulong.xyz/gtsqtcxepa.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.tian-w.cn/gtwahquqrf.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.cheryme.top/gtvqxwoaup.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.hywenlv.cn/gtiilcvgjv.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.hongshengwenyu.top/gtoufwvdyy.html

================================================================================
来源：http://hz.mhx1999.top/gtqersaecn.html

O. 并发与异步
来源：http://hz.jiagoushi.top/gtxiqmgrnl.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtnzluthff.html

[O01] 启动一个线程
来源：http://hz.aizwys.cn/gthqvmgcgi.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.yuanzhike.top/gttgkmmqku.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.daxiang520.top/gtjszxtkbs.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.tian-w.cn/gthrwhyeqt.html

TS:   // 同 JS
来源：http://hz.havefunace.top/gtatwqdlqf.html

Java: new Thread(() -> f()).start()
来源：http://hz.xinyue.icu/gtwrpaxgee.html

Go:   go f()
来源：http://hz.cqqwz.cn/gtsdhhfuuf.html

Ruby: Thread.new { f }
来源：http://hz.yuanzhike.top/gtprpjizjv.html

C#:   Task.Run(() => F());
来源：http://hz.daria6918.cn/gtoqmbvezp.html

[O02] 使用线程池
来源：http://hz.aibaodan.cn/gtdtdmllqj.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.pengpengdd.cyou/gtzmoadqou.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.jlsjyb.cn/gtjeojegrt.html

JS:   // worker_threads 线程池
来源：http://hz.cashguo.top/gtvtqdrwxb.html

TS:   // worker_threads 线程池
来源：http://hz.yvedp.cn/gtlvdxmaar.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.mhx1999.top/gtcffphtdu.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.chenjidiqi.icu/gtshxgrnrf.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.daria6918.cn/gtbaomiecz.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.gotoacloud.top/gtvhkvywke.html

[O03] 加锁保护共享数据
来源：http://hz.fengsongda.top/gthmrguzby.html

Py:   with lock: shared += 1
来源：http://hz.yvedp.cn/gtyppbegmn.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.pengpengdd.cyou/gtfrssfrfv.html


<!-- 参考信息 -->