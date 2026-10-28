代发 wailian999

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.yj20258888.top/gthzzfwqna.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.bjfxy.top/gtcnlqgoaz.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.quarkkingdee.top/gtwagwyotu.html

[K05] 深拷贝对象
来源：http://hz.ywan-chungtsiang.top/gtqkfsafiq.html

Py:   copy.deepcopy(obj)
来源：http://hz.jinghuilouyu.cn/gtokcxqjlu.html

PHP:  unserialize(serialize($obj));
来源：http://hz.chenzaomai.com/gtpdrtfhyt.html

JS:   structuredClone(obj)
来源：http://hz.dashuyun.cn/gtuiioixyg.html

TS:   structuredClone(obj)
来源：http://hz.xziqi.cn/gtgeppjgza.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.xuetiantiany.cn/gtfkmkytki.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.316326.xyz/gtybmikmww.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.snrcjt.cn/gtgictjxuq.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.hywenlv.cn/gtikxfaugl.html

[K06] 解析 URL 查询串
来源：http://hz.quarkkingdee.top/gtvqnqtbiv.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.yj20258888.top/gtfdhihata.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.yvedp.cn/gtlwldjwdf.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.aibaodan.cn/gtdfhgnqbi.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.nwbrower.top/gtnzpflupo.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.tanke756.top/gtxzhwxilk.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.pycfn.com/gtkfbvkiwo.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.yangfankeji.com/gtcsvnzeum.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.yuxming.cn/gtghsjafuj.html

[K07] 进制转换
来源：http://hz.xinyue.icu/gthongnnft.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.svipenyu.cn/gtamieibkt.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.andypj.xyz/gttjszxjtj.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.vqdsnc.cn/gtiuqqcbug.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.jqgufenzy.top/gtpijdafxn.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.nanxinkj.top/gttpzfyybm.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.zhaomingkeji.xyz/gtjlrtlvlz.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.9152youxi.cn/gtehonlclq.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.quarkkingdee.top/gtwatfofut.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.aizwys.cn/gtjxieyvko.html

Py:   pickle.dumps(obj)
来源：http://hz.andypj.xyz/gtxhikiwir.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.guannengcc.top/gtpxuztwfy.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.52xcode.cn/gtatxlfogy.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.xylfe.cn/gtffoanfla.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.yanxiufei.cn/gtvnfccfbx.html

Go:   encoding/gob
来源：http://hz.cqqwz.cn/gtpblntczx.html

Ruby: Marshal.dump(obj)
来源：http://hz.yj20258.top/gtcbudcems.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.kuanghao11.cn/gtatiefskd.html

================================================================================
来源：http://hz.meibo888.top/gtvcflsslw.html

L. 网络请求
来源：http://hz.ivvv.top/gtotoawbni.html

================================================================================
来源：http://hz.quarkkingdee.top/gtelrpfxha.html

[L01] 发送 GET 请求
来源：http://hz.zhiwuduotai.top/gtvkjzfltk.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.daria6918.cn/gtefmrzoyf.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.xuetiantiany.cn/gtkwqmombq.html

JS:   await fetch(url)
来源：http://hz.kuanghao11.cn/gtxfzqhqej.html

TS:   await fetch(url)
来源：http://hz.ywan-chungtsiang.top/gtbtxapfxe.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.kuanghao11.cn/gtmcsttxxv.html

Go:   resp, err := http.Get(url)
来源：http://hz.hfpthk.cn/gtxeargbmv.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.guannengcc.top/gtxhxztxok.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.sxryk.cn/gtdlkoudqo.html

[L02] 发送 POST JSON
来源：http://hz.gotoacloud.top/gtbfkryoys.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.kuanghao11.cn/gtrjrxjrnb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.yj202588.top/gtxbzduaoo.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.cheryme.top/gtixlpiyxc.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.dashuyun.cn/gtdhzhlgln.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.zhoulong.xyz/gtylxopapl.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.zhiwuduotai.top/gtjmxuutbm.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.pengpengdd.cyou/gtnxvhnwuh.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.guowangkeji.top/gtjfxllzmr.html

[L03] 设置自定义请求头
来源：http://hz.xingfuxueyuan.xyz/gtxcnykifd.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.pycfn.com/gtsosgfqhk.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.ydjk.org.cn/gtfnrvmgga.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yangfankeji.com/gttyhgajaq.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yj202588.top/gtmayyzzop.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.ydzc1.top/gtjmmfqulp.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.pengpengdd.cyou/gthvkjwltt.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.ehwqpu.com/gtmwlrwqdf.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.haohaochexian.top/gtmjswefab.html

[L04] 设置超时
来源：http://hz.hywenlv.cn/gttbcnkkqn.html

Py:   requests.get(url, timeout=5)
来源：http://hz.quarkkingdee.top/gtqigucrov.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.dianchejie.cn/gtypyuzmjd.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.wangshuangyany.cn/gtotjacalf.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yuxming.cn/gtglhwvejx.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.jlsjyb.cn/gtemvibxvw.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.svipenyu.cn/gtloefiidw.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.dianchejie.cn/gtmosnwrpm.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.snrcjt.cn/gtnekrxnmw.html

[L05] 上传文件（multipart）
来源：http://hz.hnqzz.top/gtmolftbil.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.sxryk.cn/gtescxwsdv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.guowangkeji.top/gtolymaaaf.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.smart0.xyz/gtszbmfxig.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.316326.xyz/gtjqyytjrv.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.feifeiyinyue.top/gttyjnhjpa.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.wangdashe.top/gtfwjutjlc.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.hfpthk.cn/gtmnucgnuw.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.cdnleiting.top/gteftisuye.html

[L06] 解析响应为 JSON
来源：http://hz.jinqigufen.top/gtddtdhmha.html

Py:   resp.json()
来源：http://hz.tanke756.top/gtqebwlwbt.html

PHP:  json_decode($body, true);
来源：http://hz.hongshengwenyu.top/gtggisekpz.html

JS:   await resp.json()
来源：http://hz.c1oappe.top/gtvpwscpll.html

TS:   await resp.json()
来源：http://hz.nwbrower.top/gtzgfnqovq.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.birdmap.top/gtmymnflqe.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.andypj.xyz/gtxutommho.html

Ruby: JSON.parse(resp.body)
来源：http://hz.jiagoushi.top/gtdfmhbswr.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.tian-w.cn/gtdizvwmcb.html

[L07] 处理 HTTP 状态码
来源：http://hz.shzxlz.cn/gtmibvqido.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.kuanghao11.cn/gtofnycqes.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.xuanzx.com/gtfcblppaw.html

JS:   resp.ok;  resp.status
来源：http://hz.jinghuilouyu.cn/gtpmtelapk.html

TS:   resp.ok;  resp.status
来源：http://hz.jyoumei.cn/gtpmsinozm.html

Java: resp.statusCode()
来源：http://hz.zhengqikj.top/gtnywywrau.html

Go:   resp.StatusCode
来源：http://hz.zhixingplan.top/gtnnjkdgjp.html

Ruby: resp.code.to_i
来源：http://hz.zdqjudy.top/gtfeyrsget.html

C#:   (int)resp.StatusCode
来源：http://hz.xylfe.cn/gtfijcywfk.html

[L08] 并发请求多个地址
来源：http://hz.tanke756.top/gtjgdcjnpb.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.ehwqpu.com/gtzmkploqb.html

PHP:  curl_multi_init() 系列
来源：http://hz.ehwqpu.com/gtfntumccz.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.cucudq.cn/gtwwyvwhom.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.chenjidiqi.icu/gtjesgzzze.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.vqdsnc.cn/gtfdpcnhmr.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.sxryk.cn/gtigxujfhx.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.yuanzhike.top/gtoziuddrn.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.fzhhl.top/gtbfydogjp.html

================================================================================
来源：http://hz.gogol.net.cn/gtdgzlusww.html

M. 命令行 / 进程 / 环境
来源：http://hz.dashuyun.cn/gtkfihulxq.html

================================================================================
来源：http://hz.sweek.top/gtfkzbzgfz.html

[M01] 读取命令行参数
来源：http://hz.jinqigufen.top/gtcjbopwit.html

Py:   sys.argv[1:]
来源：http://hz.tianlin.xyz/gtsumlwfbb.html

PHP:  $argv;  $argc;
来源：http://hz.shanyushiyangtech.top/gtqfosmkeh.html

JS:   process.argv.slice(2)
来源：http://hz.tanke756.top/gtexkcmbiz.html

TS:   process.argv.slice(2)
来源：http://hz.chenzaomai.com/gtrtaocile.html

Java: args 数组（main 方法参数）
来源：http://hz.52xcode.cn/gtelfowwmr.html

Go:   os.Args[1:]
来源：http://hz.fzhhl.top/gtwqouvzkg.html

Ruby: ARGV
来源：http://hz.ywan-chungtsiang.top/gtkgdipqmh.html

C#:   args 数组（Main 方法参数）
来源：http://hz.ivvv.top/gtlvfzuwss.html

[M02] 读取环境变量
来源：http://hz.haohaochexian.top/gtbjmqervm.html

Py:   os.environ.get("HOME")
来源：http://hz.nanxinkj.top/gtttzvntxd.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.ydzc1.top/gtatralgfo.html

JS:   process.env.HOME
来源：http://hz.hfpthk.cn/gtviwwccsx.html

TS:   process.env.HOME
来源：http://hz.316326.xyz/gtqqbupcuz.html

Java: System.getenv("HOME")
来源：http://hz.jinqigufen.top/gtzgfqqjnd.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.haohaochexian.top/gtcpgmylzc.html

Ruby: ENV["HOME"]
来源：http://hz.jinqigufen.top/gthrgycqll.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.zhiwuduotai.top/gtmwaefyan.html

[M03] 执行外部命令
来源：http://hz.gotoacloud.top/gtaadbrkjr.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.chenzaomai.com/gtavnbcihp.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.jianghu66.top/gtrkcjgmdk.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.jqgfzy.top/gtjcdmsyzi.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.sufxvd.cn/gtgudtbnop.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.tianlin.xyz/gtidjwcrps.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.ehwqpu.com/gtyydoyjuf.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.ehwqpu.com/gtnpmrsqjs.html

C#:   Process.Start("ls", "-l");
来源：http://hz.cqqwz.cn/gtfoiojjdr.html

[M04] 获取当前工作目录
来源：http://hz.meibo888.top/gtnhclhbfp.html

Py:   os.getcwd()
来源：http://hz.xuetiantiany.cn/gtljcphimb.html

PHP:  getcwd();
来源：http://hz.wangshuangyany.cn/gtwbiptkml.html

JS:   process.cwd()
来源：http://hz.jianghu66.top/gtgqmubaid.html

TS:   process.cwd()
来源：http://hz.nanxinkj.top/gtnosrjvdc.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.yuxming.cn/gtpiutuyxe.html

Go:   os.Getwd()
来源：http://hz.jlsjyb.cn/gtciqwferk.html

Ruby: Dir.pwd
来源：http://hz.ywan-chungtsiang.top/gtmpjsyuut.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.xylfe.cn/gtaeawhnbi.html

[M05] 设置退出码
来源：http://hz.ehwqpu.com/gtddhsbdpy.html

Py:   sys.exit(1)
来源：http://hz.ydjk.org.cn/gthtasgwdj.html

PHP:  exit(1);
来源：http://hz.snrcjt.cn/gtgebnchcw.html

JS:   process.exit(1)
来源：http://hz.chenjidiqi.icu/gttcnjakdc.html

TS:   process.exit(1)
来源：http://hz.jinghuilouyu.cn/gtwifijpjk.html

Java: System.exit(1)
来源：http://hz.fengsongda.top/gtyulawlyr.html

Go:   os.Exit(1)
来源：http://hz.ehwqpu.com/gtevvbjqqg.html

Ruby: exit 1
来源：http://hz.zycfv.cn/gtwqxxamlg.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.xingfuxueyuan.xyz/gtacamppzi.html

[M06] 向标准错误输出
来源：http://hz.cdnleiting.top/gtqamzocel.html

Py:   print("err", file=sys.stderr)
来源：http://hz.andypj.xyz/gtwcfuileb.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.jinqigfzy.top/gtunepdnwz.html

JS:   console.error("err")
来源：http://hz.zycfv.cn/gtdomjjcum.html

TS:   console.error("err")
来源：http://hz.iojbl.cn/gtaysuhjtk.html

Java: System.err.println("err")
来源：http://hz.zhijiandao.cn/gtziiqrtju.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.xziqi.cn/gtlwvkhjcy.html

Ruby: warn "err"
来源：http://hz.jinyuanbaomall.cn/gtqjcproly.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.jlsjyb.cn/gtaqsnajqx.html

[M07] 判断是否为主入口
来源：http://hz.quarkkingdee.top/gtnuubygtw.html

Py:   if __name__ == "__main__":
来源：http://hz.tianlin.xyz/gtdzupajra.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.kuanghao11.cn/gtygmjqxuq.html

JS:   require.main === module
来源：http://hz.ppjwa.cn/gtsozrhqiy.html

TS:   require.main === module
来源：http://hz.sweek.top/gtneeymsbw.html

Java: public static void main(String[] args)
来源：http://hz.xinyue.icu/gthkqwikdy.html

Go:   func main()
来源：http://hz.nanxinkj.top/gtbbbcgyii.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.c1oappe.top/gttyirdcjh.html

C#:   static void Main(string[] args)
来源：http://hz.bjfxy.top/gtcitdigvv.html

[M08] 获取系统与运行时信息
来源：http://hz.xuetiantiany.cn/gtqucangws.html

Py:   platform.system();  platform.python_version()
来源：http://hz.yanxiufei.cn/gtkdrezkxe.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.hnqzz.top/gtdrjqxutv.html

JS:   process.platform;  process.version
来源：http://hz.jinqigfzy.top/gtfehhbynp.html

TS:   process.platform;  process.version
来源：http://hz.jinqigufen.top/gtzugwxkmq.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.zhongyouzk.top/gtwjdwsbho.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.shuidangran.top/gtcgfdoytf.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.ivvv.top/gtmnuwerke.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.wangdashe.top/gtlmctpyyh.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtqwlkzboj.html

N. 数据结构与算法
来源：http://hz.jinqigufen.top/gtmtwkroms.html

================================================================================
来源：http://hz.zhengqikj.top/gtxyjgdyyz.html

[N01] 二分查找（有序数组）
来源：http://hz.quarkkingdee.top/gtcdhnemws.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.hywenlv.cn/gtksjswvhf.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.ydjk.org.cn/gtxsjablqa.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yj202588.top/gtpiibtxxs.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.fzhhl.top/gtiyyhmilm.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.shangyingyoupin.top/gtnhkontop.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.xingfuxueyuan.xyz/gtdxyguuls.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.andypj.xyz/gtqkhvjrro.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.yongpay.top/gtnqfojjxd.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.ppjwa.cn/gthqtccfrg.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jiagoushi.top/gtjejybhmb.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.c1oappe.top/gtzasgazhp.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.ywan-chungtsiang.top/gtvnettcif.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.chenlongwang.top/gtwjaxlmps.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.sxryk.cn/gtxyhskgtm.html

Go:   slices.Sort(arr)
来源：http://hz.zycfv.cn/gtojceuqmt.html

Ruby: arr.sort
来源：http://hz.xingfuxueyuan.xyz/gtiyzvhqcq.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.jinghuilouyu.cn/gtgtdlzkrk.html

[N03] 快速排序（分治示例）
来源：http://hz.snrcjt.cn/gtkrbkdfkm.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.gzhubu.top/gtirrqboyq.html

PHP:  // 递归实现，或用 usort
来源：http://hz.tian-w.cn/gtouqrsxbe.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zhengqikj.top/gtstljluxe.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.shanyushiyangtech.top/gtbjuxaanc.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.aizwys.cn/gtzgaistja.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.cucudq.cn/gtqreolscp.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.zhaomingkeji.xyz/gtyafgrmij.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.ehwqpu.com/gtcrfopvde.html

[N04] 斐波那契数列
来源：http://hz.gotoacloud.top/gtiriyxmfu.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.ehwqpu.com/gtsvscawop.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.zhiwuduotai.top/gtaiuwljqw.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.zdqjudy.top/gtqjnjpwca.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.ybcxt.top/gteovtougw.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.yj20258888.top/gtthhqghdo.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.jiagoushi.top/gtljpsqcgk.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.tanke756.top/gtouoaqpue.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.hfpthk.cn/gtwqqculxd.html

[N05] 最大公约数
来源：http://hz.shanyushiyangtech.top/gtwdkcrsgw.html

Py:   math.gcd(a, b)
来源：http://hz.zhoulong.xyz/gtymvszihu.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.yanxiufei.cn/gtaxqjvrxq.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.zhixingplan.top/gtianwqbng.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yonumen.top/gtjybawslm.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.dianchejie.cn/gteghxrqsb.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.zhongyouzk.top/gtdritchin.html

Ruby: a.gcd(b)
来源：http://hz.sufxvd.cn/gtmtlzauxe.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.yvedp.cn/gthyxhyulr.html

[N06] 判断回文字符串
来源：http://hz.xuetiantiany.cn/gtjaarycvv.html

Py:   s == s[::-1]
来源：http://hz.tianlin.xyz/gtyrceupwf.html

PHP:  $s === strrev($s);
来源：http://hz.yonumen.top/gtglkrrgfh.html

JS:   s === [...s].reverse().join("")
来源：http://hz.jyoumei.cn/gtohfrkqhi.html

TS:   s === [...s].reverse().join("")
来源：http://hz.shanyushiyangtech.top/gtyqqaurvk.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.sxryk.cn/gtqezfiftm.html

Go:   // 双指针从两端比较
来源：http://hz.xylfe.cn/gtaoydydzu.html

Ruby: s == s.reverse
来源：http://hz.vqdsnc.cn/gthzjgqdid.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.mhx1999.top/gtfrabdhse.html

[N07] 两数之和（返回下标）
来源：http://hz.yangfankeji.com/gtyrodklhe.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.daxiang520.top/gtnqumjjxl.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.haohaochexian.top/gtsotqsgsq.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.xinyue.icu/gtllawvhqv.html

TS:   // 手写 Map<string, number>
来源：http://hz.kuanghao11.cn/gtrkmfzzqh.html

Java: // 手写 HashMap
来源：http://hz.jinqigfzy.top/gtaeyhcfwq.html

Go:   // 手写 map[int]int
来源：http://hz.zhixingplan.top/gtrliganfm.html

Ruby: // 手写 Hash
来源：http://hz.haohaochexian.top/gtiasuobio.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.shzxlz.cn/gtxddkgvrw.html

[N08] 生成全排列
来源：http://hz.zhoulong.xyz/gtisyjfafw.html

Py:   itertools.permutations(arr)
来源：http://hz.xuanzx.com/gtmqumqnoe.html

PHP:  // 手写递归交换
来源：http://hz.hywenlv.cn/gtpgqwrcnj.html

JS:   // 手写回溯递归
来源：http://hz.zdqjudy.top/gtwjwqxnlq.html

TS:   // 手写回溯递归
来源：http://hz.0kj1m.cn/gtzqnbceow.html

Java: // 手写回溯递归
来源：http://hz.dashuyun.cn/gtcjbtsmly.html

Go:   // 手写回溯递归
来源：http://hz.hammf.cn/gthqihdtpn.html

Ruby: arr.permutation.to_a
来源：http://hz.hnxiangtu.top/gtsmxzpekt.html

C#:   // 手写回溯递归
来源：http://hz.jyoumei.cn/gtqwcydgav.html

[N09] 栈与队列
来源：http://hz.sweek.top/gtepqimgmn.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.redwolf501.top/gtdfqwhjtv.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.tianlin.xyz/gtouezbhdd.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.havefunace.top/gtczwsndlm.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.iojbl.cn/gtjdogmpqj.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.yangfankeji.com/gtlzmhyrvc.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.zhijiandao.cn/gtptualmiy.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.jinyuanbaomall.cn/gtqvcrcnxi.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.9152youxi.cn/gthayxrqbs.html

[N10] 链表节点定义
来源：http://hz.fengsongda.top/gtfzmwycgd.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.ppjwa.cn/gtgamicplo.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.smart0.xyz/gtxyfroltu.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.gzhubu.top/gtdcbgndzv.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.zdqjudy.top/gtkuxwvzyq.html

Java: class Node { int v; Node next; }
来源：http://hz.gzhubu.top/gtyndmxqjh.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.yanxiufei.cn/gtbofqvhop.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.tianlin.xyz/gtripwpmgn.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.hnqzz.top/gtgyusxzrp.html

[N11] 二叉树中序遍历
来源：http://hz.tianlin.xyz/gtjmaplhbr.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.shuidangran.top/gtznqomszi.html

PHP:  // 手写递归函数
来源：http://hz.gzhubu.top/gtyjbxhbzn.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.ivvv.top/gtyxtrybgf.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.kuanghao11.cn/gthrmbiwvi.html

Java: // 手写递归
来源：http://hz.hysaishi.cn/gtpyjflwqm.html

Go:   // 手写递归
来源：http://hz.hnxiangtu.top/gtcpxonrtj.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.shzxlz.cn/gtenzvusqq.html

C#:   // 手写递归
来源：http://hz.iojbl.cn/gtxupvjmaq.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.xingfuxueyuan.xyz/gtqmnapsvi.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.jiagoushi.top/gtyaxybhzg.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.iojbl.cn/gtbosjjsok.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.xingfuxueyuan.xyz/gtnarlhpxb.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jinyuanbaomall.cn/gtegnofwof.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yangfankeji.com/gtfjzpcwff.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.zdqjudy.top/gtdwztfmpi.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.hysaishi.cn/gtxcgxoggv.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yj20258888.top/gtddhqozyr.html


<!-- 参考信息 -->