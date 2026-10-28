代发 wailian999

Py:   copy.deepcopy(obj)
来源：http://hz.yangfankeji.com/gtscqerlpw.html

PHP:  unserialize(serialize($obj));
来源：http://hz.ydjk.org.cn/gtoqtcbyxe.html

JS:   structuredClone(obj)
来源：http://hz.zhongyouzk.top/gtyeyboecs.html

TS:   structuredClone(obj)
来源：http://hz.316326.xyz/gttdzyqqex.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.iojbl.cn/gtfcjozxny.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.guowangkeji.top/gtigfdticy.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.meibo888.top/gtfevacghk.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.yuxming.cn/gtlaqcilmc.html

[K06] 解析 URL 查询串
来源：http://hz.cashguo.top/gtezjxsjqi.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.gaohongyu789.top/gtmusxzsjb.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.cucudq.cn/gtirkllvio.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jiagoushi.top/gtdpfbncoz.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jiagoushi.top/gtqjiwvyhf.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.wangdashe.top/gtubdydjbq.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.redwolf501.top/gtfoauiibi.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.iojbl.cn/gtejymlqho.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.aibaodan.cn/gtjeojtwue.html

[K07] 进制转换
来源：http://hz.hammf.cn/gtnbahxsez.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.dianchejie.cn/gtnyxkapyd.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.c1oappe.top/gtydouwgrf.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.52xcode.cn/gtbqqioyml.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.hammf.cn/gtvysvdjqp.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.svipenyu.cn/gtyzxyksgd.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.redwolf501.top/gtorrrqcbv.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.xingfuxueyuan.xyz/gthpimnqzw.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.zhaomingkeji.xyz/gtfedowjkg.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.shanyushiyangtech.top/gtorvgwjuv.html

Py:   pickle.dumps(obj)
来源：http://hz.havefunace.top/gtxsmvycrn.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.guannengcc.top/gtlicoohvj.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.shanyushiyangkeji.top/gtttonaxcy.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.yueranfly.top/gtvcnupfal.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.hnxiangtu.top/gtuonigpqo.html

Go:   encoding/gob
来源：http://hz.quarkkingdee.top/gtftfzemvw.html

Ruby: Marshal.dump(obj)
来源：http://hz.nanxuanxn.top/gtencuznzs.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.birdmap.top/gtnuswashl.html

================================================================================
来源：http://hz.nanxinkj.top/gtzesxxyuu.html

L. 网络请求
来源：http://hz.tianlin.xyz/gtmknzvjpx.html

================================================================================
来源：http://hz.kuanghao11.cn/gtbyyzymnr.html

[L01] 发送 GET 请求
来源：http://hz.hfpthk.cn/gtxprbpegr.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.cucudq.cn/gtbwwnycwn.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.xingfuxueyuan.xyz/gtxujqyglx.html

JS:   await fetch(url)
来源：http://hz.meibo888.top/gtjihpaute.html

TS:   await fetch(url)
来源：http://hz.gzhubu.top/gtmhdkjjzx.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.hongshengwenyu.top/gthjdwrmfa.html

Go:   resp, err := http.Get(url)
来源：http://hz.cqqwz.cn/gtvwknqzdo.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.c1oappe.top/gtnszxwyum.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.haohaochexian.top/gtwqdnsxcm.html

[L02] 发送 POST JSON
来源：http://hz.vqdsnc.cn/gtyzvkrveq.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.jinqigufen.top/gtelaslkjz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.yangfankeji.com/gtswdzgqvh.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.aizwys.cn/gtvsijaaev.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.gotoacloud.top/gtbmhhkpew.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.gaohongyu789.top/gtytgjoiia.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.316326.xyz/gtfryzjebm.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.shangyingyoupin.top/gtauvhkvyt.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.hysaishi.cn/gtwdgipycj.html

[L03] 设置自定义请求头
来源：http://hz.52xcode.cn/gtqsvmnlat.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.guannengcc.top/gtjxmxmavd.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.ivvv.top/gteiqgxrxh.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.ehwqpu.com/gtrhpbhcaa.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.wangshuangyany.cn/gtxedbwoyv.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.ivvv.top/gtffnuwhzs.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.yonumen.top/gtpahlnavi.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.bjfxy.top/gtthamtatq.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.bjfxy.top/gtqnfogdqt.html

[L04] 设置超时
来源：http://hz.jlsjyb.cn/gtmrzkqbmj.html

Py:   requests.get(url, timeout=5)
来源：http://hz.jinyuanbaomall.cn/gtwocgnsiq.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.jinqigfzy.top/gtwlqwuvmv.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zhaomingkeji.xyz/gtisasixgt.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.feifeiyinyue.top/gtlfqmxxvc.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.daria6918.cn/gtsgemfiiz.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.gaohongyu789.top/gthwgsfuuo.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.yj20258888.top/gtsphorwnj.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.guowangkeji.top/gtrageaznk.html

[L05] 上传文件（multipart）
来源：http://hz.52xcode.cn/gtocyhyqzx.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.zdqjudy.top/gtcjhumwfa.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.gaohongyu789.top/gtemokmorl.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.yueranfly.top/gtowifbtfu.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.nwbrower.top/gtxrxloyhi.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.hnqzz.top/gtfeopddgp.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.tian-w.cn/gtwqvnbkhn.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.hfpthk.cn/gtmffqvdiq.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.tian-w.cn/gtwuvjgtsf.html

[L06] 解析响应为 JSON
来源：http://hz.yj20258.top/gtlojakius.html

Py:   resp.json()
来源：http://hz.sweek.top/gtegovpfck.html

PHP:  json_decode($body, true);
来源：http://hz.tianlin.xyz/gtbhusbvvc.html

JS:   await resp.json()
来源：http://hz.wangshuangyany.cn/gttrnjwdmr.html

TS:   await resp.json()
来源：http://hz.fengsongda.top/gtyumxpvmd.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.0kj1m.cn/gtfkfnvbeb.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.chenzaomai.com/gtwdhanltf.html

Ruby: JSON.parse(resp.body)
来源：http://hz.birdmap.top/gtxaievpqm.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.iojbl.cn/gtzgiicrui.html

[L07] 处理 HTTP 状态码
来源：http://hz.andypj.xyz/gtwqmjoznc.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.chenzaomai.com/gtxorxxjyi.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.sufxvd.cn/gtwffezfim.html

JS:   resp.ok;  resp.status
来源：http://hz.jinyuanbaomall.cn/gtsedzrezq.html

TS:   resp.ok;  resp.status
来源：http://hz.xinyue.icu/gtcyuvqyyk.html

Java: resp.statusCode()
来源：http://hz.aizwys.cn/gtwpbwecxg.html

Go:   resp.StatusCode
来源：http://hz.ppjwa.cn/gtkehakxpu.html

Ruby: resp.code.to_i
来源：http://hz.dianchejie.cn/gtqhtrkerc.html

C#:   (int)resp.StatusCode
来源：http://hz.gzhubu.top/gtmmarxfsj.html

[L08] 并发请求多个地址
来源：http://hz.birdmap.top/gtwljxsfnh.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.0kj1m.cn/gtirabkuun.html

PHP:  curl_multi_init() 系列
来源：http://hz.wangdashe.top/gtpzuqgtdh.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.svipenyu.cn/gtwrcnbkhm.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.hongshengwenyu.top/gtkrolbkck.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.c1oappe.top/gtavipstwe.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.zhongyouzk.top/gtcdzdfrrt.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.hnqzz.top/gtgbipdtym.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.hongshengwenyu.top/gtsnfksvzs.html

================================================================================
来源：http://hz.ybcxt.top/gtsnhfttbi.html

M. 命令行 / 进程 / 环境
来源：http://hz.jinqigufen.top/gtjkvixqwy.html

================================================================================
来源：http://hz.havefunace.top/gtfwxycvwj.html

[M01] 读取命令行参数
来源：http://hz.chenjidiqi.icu/gtcpiiswwc.html

Py:   sys.argv[1:]
来源：http://hz.pengpengdd.cyou/gtdoymmlil.html

PHP:  $argv;  $argc;
来源：http://hz.andypj.xyz/gtiljykvyz.html

JS:   process.argv.slice(2)
来源：http://hz.zhiwuduotai.top/gteuewrgjn.html

TS:   process.argv.slice(2)
来源：http://hz.andypj.xyz/gtiglhmlmy.html

Java: args 数组（main 方法参数）
来源：http://hz.haohaochexian.top/gtvnwedgxa.html

Go:   os.Args[1:]
来源：http://hz.pycfn.com/gtouiacpox.html

Ruby: ARGV
来源：http://hz.fengsongda.top/gtmebrjlkn.html

C#:   args 数组（Main 方法参数）
来源：http://hz.chenzaomai.com/gtjrkbznhi.html

[M02] 读取环境变量
来源：http://hz.ybcxt.top/gtazfgurzs.html

Py:   os.environ.get("HOME")
来源：http://hz.snrcjt.cn/gtncrdurto.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.cheryme.top/gtxtbqqnqq.html

JS:   process.env.HOME
来源：http://hz.0kj1m.cn/gthbdogtoc.html

TS:   process.env.HOME
来源：http://hz.yvedp.cn/gtljgllcrv.html

Java: System.getenv("HOME")
来源：http://hz.xylfe.cn/gtidfysrtp.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.tanke756.top/gtflcfigph.html

Ruby: ENV["HOME"]
来源：http://hz.zhoulong.xyz/gtdujqdhey.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.hnqzz.top/gtngfoxyue.html

[M03] 执行外部命令
来源：http://hz.iojbl.cn/gtieixbvaq.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.fengsongda.top/gteeutsshc.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.cashguo.top/gtbzogoxtw.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.guowangkeji.top/gtdkrwmkzg.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.havefunace.top/gtwydzszru.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.daxiang520.top/gtsyobivvu.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.chenjidiqi.icu/gtciwptger.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.ybcxt.top/gtguyvwnhg.html

C#:   Process.Start("ls", "-l");
来源：http://hz.yueranfly.top/gtpgfvrdcb.html

[M04] 获取当前工作目录
来源：http://hz.xziqi.cn/gtrcnurddq.html

Py:   os.getcwd()
来源：http://hz.birdmap.top/gtphevmevx.html

PHP:  getcwd();
来源：http://hz.jqgufenzy.top/gtozdqqkzt.html

JS:   process.cwd()
来源：http://hz.zycfv.cn/gtxdiqicsu.html

TS:   process.cwd()
来源：http://hz.xziqi.cn/gtdkhhibzx.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.hongshengwenyu.top/gtabofbdax.html

Go:   os.Getwd()
来源：http://hz.hysaishi.cn/gtrdnzhurz.html

Ruby: Dir.pwd
来源：http://hz.iojbl.cn/gtttcqvhyw.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.zhaomingkeji.xyz/gtmfqghvqz.html

[M05] 设置退出码
来源：http://hz.sxryk.cn/gtfvygtjpm.html

Py:   sys.exit(1)
来源：http://hz.hfpthk.cn/gtsniyrkll.html

PHP:  exit(1);
来源：http://hz.chenzaomai.com/gtnbggycsa.html

JS:   process.exit(1)
来源：http://hz.jiagoushi.top/gtxdrgceoz.html

TS:   process.exit(1)
来源：http://hz.zhongyouzk.top/gtudacdxol.html

Java: System.exit(1)
来源：http://hz.dianchejie.cn/gtwyuziebd.html

Go:   os.Exit(1)
来源：http://hz.yuanzhike.top/gtvplnubqi.html

Ruby: exit 1
来源：http://hz.shanyushiyangkeji.top/gtfvszabms.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.yongpay.top/gtknqkqvqh.html

[M06] 向标准错误输出
来源：http://hz.dianchejie.cn/gtxbjllajc.html

Py:   print("err", file=sys.stderr)
来源：http://hz.hywenlv.cn/gtigwigiff.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.zhoulong.xyz/gtodrtoejh.html

JS:   console.error("err")
来源：http://hz.snrcjt.cn/gtfflkagjj.html

TS:   console.error("err")
来源：http://hz.aizwys.cn/gtvkebyall.html

Java: System.err.println("err")
来源：http://hz.zhaomingkeji.xyz/gtkcfwrsur.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.zhengqikj.top/gthyjzbcdo.html

Ruby: warn "err"
来源：http://hz.tanke756.top/gtqtdlhrur.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.snrcjt.cn/gtqyshrdnp.html

[M07] 判断是否为主入口
来源：http://hz.chenlongwang.top/gtexrnjjtq.html

Py:   if __name__ == "__main__":
来源：http://hz.cheryme.top/gthdqptrkq.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.cheryme.top/gtiqxfbklv.html

JS:   require.main === module
来源：http://hz.wangdashe.top/gtwbvrjkmz.html

TS:   require.main === module
来源：http://hz.yuanzhike.top/gtivwwvrbl.html

Java: public static void main(String[] args)
来源：http://hz.chenlongwang.top/gthduhkuta.html

Go:   func main()
来源：http://hz.chenlongwang.top/gtrxtfsquq.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.fzhhl.top/gtlfqdubpb.html

C#:   static void Main(string[] args)
来源：http://hz.wangdashe.top/gtvsqycbuv.html

[M08] 获取系统与运行时信息
来源：http://hz.iojbl.cn/gtloljqwov.html

Py:   platform.system();  platform.python_version()
来源：http://hz.bjfxy.top/gtfatmbieh.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.ehwqpu.com/gtmrksbdtu.html

JS:   process.platform;  process.version
来源：http://hz.aibaodan.cn/gtwpbmpdcc.html

TS:   process.platform;  process.version
来源：http://hz.shangyingyoupin.top/gtwlkaoeva.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.zhoulong.xyz/gtbctbygcj.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.shanyushiyangkeji.top/gtblqrhgbg.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.zhoulong.xyz/gtfkagbana.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.hywenlv.cn/gtcfaileci.html

================================================================================
来源：http://hz.yuxming.cn/gtblayrfqx.html

N. 数据结构与算法
来源：http://hz.jinyuanbaomall.cn/gtkcywwqcn.html

================================================================================
来源：http://hz.chenzaomai.com/gtlexvdsnf.html

[N01] 二分查找（有序数组）
来源：http://hz.jiagoushi.top/gtevzcutay.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.chenjidiqi.icu/gtisvvxyoa.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.aizwys.cn/gtbrxfpvly.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.smart0.xyz/gtfejevwit.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zhoulong.xyz/gtxuhydlet.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.xuanzx.com/gtjuhpfdvr.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.jiagoushi.top/gtsnwicquu.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.ywan-chungtsiang.top/gtilpkrrng.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.jinghuilouyu.cn/gteagvbhlc.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.guannengcc.top/gtacldemxy.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.cdnleiting.top/gtytzwufja.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.daxiang520.top/gthhtkimrc.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.vqdsnc.cn/gtvjqmacaq.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.xinyue.icu/gtthybrxoy.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.guannengcc.top/gtckvccsiw.html

Go:   slices.Sort(arr)
来源：http://hz.vqdsnc.cn/gtftebrhdc.html

Ruby: arr.sort
来源：http://hz.ehwqpu.com/gtjpgrbgrj.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.nanxuanxn.top/gtwztepean.html

[N03] 快速排序（分治示例）
来源：http://hz.ywan-chungtsiang.top/gtsdkgenqi.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.ywan-chungtsiang.top/gtkodqytip.html

PHP:  // 递归实现，或用 usort
来源：http://hz.cucudq.cn/gtnczyltbh.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.daxiang520.top/gtgxxrjkzp.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.feifeiyinyue.top/gthhjulznf.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.zhijiandao.cn/gthrorucvk.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.aibaodan.cn/gttwkiqtgm.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.snrcjt.cn/gtkjgucwvk.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.yvedp.cn/gtibohshht.html

[N04] 斐波那契数列
来源：http://hz.vqdsnc.cn/gtmhwziplk.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.cheryme.top/gtwrxbigbt.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.ivvv.top/gtmzhzcdff.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.andypj.xyz/gtushlhryv.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.daxiang520.top/gtuftzjmpr.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.svipenyu.cn/gtovvvjzpr.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.jinghuilouyu.cn/gtqnzdsrkm.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.shzxlz.cn/gtgectfhet.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.gaohongyu789.top/gttufpukpf.html

[N05] 最大公约数
来源：http://hz.0kj1m.cn/gtzftdjudp.html

Py:   math.gcd(a, b)
来源：http://hz.yj20258888.top/gtkmtnzeui.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.redwolf501.top/gtquoujoza.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.hammf.cn/gtmruzkazk.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.zhengqikj.top/gtvyrwcvmv.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.pycfn.com/gtlondvkni.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.pengpengdd.cyou/gtkuclhnpv.html

Ruby: a.gcd(b)
来源：http://hz.xylfe.cn/gtvxzjvfnu.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.jlsjyb.cn/gtxqpgbral.html

[N06] 判断回文字符串
来源：http://hz.wangdashe.top/gtdmtfsrur.html

Py:   s == s[::-1]
来源：http://hz.wangshuangyany.cn/gtgbvspipl.html

PHP:  $s === strrev($s);
来源：http://hz.jinghuilouyu.cn/gtprhuuvpp.html

JS:   s === [...s].reverse().join("")
来源：http://hz.gogol.net.cn/gtyambausv.html

TS:   s === [...s].reverse().join("")
来源：http://hz.zhengqikj.top/gtbcelmuko.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.daxiang520.top/gtxvgucujw.html

Go:   // 双指针从两端比较
来源：http://hz.kuanghao11.cn/gttoetyoex.html

Ruby: s == s.reverse
来源：http://hz.zdqjudy.top/gtoeowtuom.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.hywenlv.cn/gtkrhxlqpt.html

[N07] 两数之和（返回下标）
来源：http://hz.jqgfzy.top/gtkwzxuovh.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.snrcjt.cn/gtmuxqtdvk.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.sxryk.cn/gtvwinelah.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.jyoumei.cn/gtzebvsqod.html

TS:   // 手写 Map<string, number>
来源：http://hz.dashuyun.cn/gtupzrqvga.html

Java: // 手写 HashMap
来源：http://hz.jqgufenzy.top/gtmhrjehcl.html

Go:   // 手写 map[int]int
来源：http://hz.9152youxi.cn/gtafuclzqs.html

Ruby: // 手写 Hash
来源：http://hz.zhengqikj.top/gtbfemgjml.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.aizwys.cn/gtuvfdqnxn.html

[N08] 生成全排列
来源：http://hz.sysykeji.top/gtajvyxuuu.html

Py:   itertools.permutations(arr)
来源：http://hz.shanyushiyangkeji.top/gtdycsscpy.html

PHP:  // 手写递归交换
来源：http://hz.shangyingyoupin.top/gtezjcrfyo.html

JS:   // 手写回溯递归
来源：http://hz.jianghu66.top/gtnnbfoxyi.html

TS:   // 手写回溯递归
来源：http://hz.gaohongyu789.top/gtwoujxueh.html

Java: // 手写回溯递归
来源：http://hz.cdnleiting.top/gtybjsmzuo.html

Go:   // 手写回溯递归
来源：http://hz.feifeiyinyue.top/gtamokcdom.html

Ruby: arr.permutation.to_a
来源：http://hz.yangfankeji.com/gtybdogtld.html

C#:   // 手写回溯递归
来源：http://hz.yangfankeji.com/gtgbanlyjf.html

[N09] 栈与队列
来源：http://hz.yj20258888.top/gtiavrtvcf.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.wangshuangyany.cn/gtnsfxynjy.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.shanyushiyangtech.top/gtinhcwosb.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.hammf.cn/gtmzulsjag.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.pycfn.com/gtfmkpnulj.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.yangfankeji.com/gtzxfxamok.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.hywenlv.cn/gtgyugqriy.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.tanke756.top/gtblirsttd.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.zycfv.cn/gtcytyvldd.html

[N10] 链表节点定义
来源：http://hz.jinyuanbaomall.cn/gttfttmhkd.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.guannengcc.top/gtkhwwlkfe.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.zhixingplan.top/gtacmgjevo.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.vqdsnc.cn/gthsrlmduj.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.hysaishi.cn/gtxgzqfnqx.html

Java: class Node { int v; Node next; }
来源：http://hz.feifeiyinyue.top/gtrtyelxbz.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.zhoulong.xyz/gtikwtamtj.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.nanxuanxn.top/gtmrhpvtkf.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.birdmap.top/gtrcijlxjb.html

[N11] 二叉树中序遍历
来源：http://hz.316326.xyz/gtabxotqbp.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.gzhubu.top/gthkwxefqt.html

PHP:  // 手写递归函数
来源：http://hz.jinqigufen.top/gtqfgggedn.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.guowangkeji.top/gtzirkzzcz.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.snrcjt.cn/gtiejwzgja.html

Java: // 手写递归
来源：http://hz.yj20258.top/gtnfupumoz.html

Go:   // 手写递归
来源：http://hz.tanke756.top/gtyqrmovhj.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.wangshuangyany.cn/gtdyfvhkkc.html

C#:   // 手写递归
来源：http://hz.quarkkingdee.top/gtljyqmqda.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.guannengcc.top/gtegfygpls.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.hysaishi.cn/gtwfldnejm.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.xingfuxueyuan.xyz/gtvuclhywo.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.zhongyouzk.top/gtmozilksq.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yuanzhike.top/gtfujthsec.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.jinqigufen.top/gtwgpqitza.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.zhaomingkeji.xyz/gtkkwiickn.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.jqgufenzy.top/gtjnvkfczf.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.hnxiangtu.top/gtyqgzsush.html

================================================================================
来源：http://hz.jlsjyb.cn/gtkwztrehp.html

O. 并发与异步
来源：http://hz.sxryk.cn/gtersppuvl.html

================================================================================
来源：http://hz.aibaodan.cn/gtlqsoqpzk.html

[O01] 启动一个线程
来源：http://hz.gogol.net.cn/gtstiaczsj.html


<!-- 参考信息 -->