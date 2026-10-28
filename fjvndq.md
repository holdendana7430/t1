代发 wailian999

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.cheryme.top/gtljrivnyj.html

[K07] 进制转换
来源：http://hz.yj20258888.top/gtteelsgng.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.52xcode.cn/gtdrfktsue.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.yvedp.cn/gtcfpxegfz.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.chenjidiqi.icu/gtzxpmwgrx.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.52xcode.cn/gtfgzjfyue.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.ybcxt.top/gtzzneurmt.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.xziqi.cn/gtotntgtxv.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.yongpay.top/gtttdkuyzf.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.jinghuilouyu.cn/gtvciwhiut.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.ydjk.org.cn/gtnsbsucyn.html

Py:   pickle.dumps(obj)
来源：http://hz.nwbrower.top/gtbgjietok.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.jiagoushi.top/gtarajfdge.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.chenzaomai.com/gtueulswyt.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.zhaomingkeji.xyz/gtoxfdqjuz.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.cdnleiting.top/gtgywybqpd.html

Go:   encoding/gob
来源：http://hz.jianghu66.top/gtqkhhnnqj.html

Ruby: Marshal.dump(obj)
来源：http://hz.zhiwuduotai.top/gtxftzasvy.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.9152youxi.cn/gtkvkunlzj.html

================================================================================
来源：http://hz.iojbl.cn/gthszcqdna.html

L. 网络请求
来源：http://hz.aizwys.cn/gtwzjgtfsj.html

================================================================================
来源：http://hz.0kj1m.cn/gthlwvewob.html

[L01] 发送 GET 请求
来源：http://hz.ppjwa.cn/gtvbkrnqvb.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.tanke756.top/gtchjxauqw.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.cqqwz.cn/gtbshqvvwz.html

JS:   await fetch(url)
来源：http://hz.dianchejie.cn/gtgnxprfov.html

TS:   await fetch(url)
来源：http://hz.guannengcc.top/gtmqgxoajk.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.sysykeji.top/gtukxltoya.html

Go:   resp, err := http.Get(url)
来源：http://hz.fengsongda.top/gtuqaincuz.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.hywenlv.cn/gttzbupuaj.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.redwolf501.top/gtmyiexvri.html

[L02] 发送 POST JSON
来源：http://hz.jinyuanbaomall.cn/gtwpjdhwnv.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.xylfe.cn/gtnoolvgaz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.smart0.xyz/gtxfknhzvp.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.shzxlz.cn/gthqtofudx.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yongpay.top/gtlpmjokuu.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.xinyue.icu/gtbrfitlea.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.xylfe.cn/gtpxglnoyv.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.daxiang520.top/gtirddolpo.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.zycfv.cn/gteoxmrrtb.html

[L03] 设置自定义请求头
来源：http://hz.sufxvd.cn/gtdoouvbri.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.hywenlv.cn/gtqjjwervo.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.jqgfzy.top/gtknkiplhe.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.316326.xyz/gtlaqembau.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.hnqzz.top/gtdlcdzguu.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.gogol.net.cn/gtzhskltke.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.hammf.cn/gtvbqixdpd.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.guowangkeji.top/gtslbsyhhr.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.chenjidiqi.icu/gtkatzdxmo.html

[L04] 设置超时
来源：http://hz.tian-w.cn/gtjumsiatr.html

Py:   requests.get(url, timeout=5)
来源：http://hz.chenjidiqi.icu/gtvtxmmmbj.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.sysykeji.top/gtvabicjri.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.snrcjt.cn/gtzjoaapnd.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jqgfzy.top/gtzbyskwlp.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.yj20258.top/gtocchyphs.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.cashguo.top/gtmlvjmtms.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.fzhhl.top/gtbglvjcte.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.cheryme.top/gthaallxba.html

[L05] 上传文件（multipart）
来源：http://hz.pycfn.com/gtyiiwelbw.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.yangfankeji.com/gtqoivgpxs.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.zhixingplan.top/gtzkjlfotq.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.tian-w.cn/gtqovkmyno.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.gotoacloud.top/gtzjgtxeaa.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.quarkkingdee.top/gtpaspxngd.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.nanxuanxn.top/gtespqctnt.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.gzhubu.top/gtqmhlrtqs.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.jinyuanbaomall.cn/gtajaqqatk.html

[L06] 解析响应为 JSON
来源：http://hz.yueranfly.top/gtdxflqaei.html

Py:   resp.json()
来源：http://hz.jinqigfzy.top/gtwkoaencc.html

PHP:  json_decode($body, true);
来源：http://hz.jinqigfzy.top/gtzyqqqgaa.html

JS:   await resp.json()
来源：http://hz.nanxinkj.top/gtyykmyxrs.html

TS:   await resp.json()
来源：http://hz.tian-w.cn/gtpajlvdpn.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.jinqigfzy.top/gtwyipstcp.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.hongshengwenyu.top/gtlxknghtg.html

Ruby: JSON.parse(resp.body)
来源：http://hz.ybcxt.top/gtybhkcpjc.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.hnxiangtu.top/gtbimrvkfe.html

[L07] 处理 HTTP 状态码
来源：http://hz.tianlin.xyz/gtquulapmc.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.iojbl.cn/gtnilzdyds.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.zycfv.cn/gtuuhuomar.html

JS:   resp.ok;  resp.status
来源：http://hz.tanke756.top/gtprthtgsb.html

TS:   resp.ok;  resp.status
来源：http://hz.yuxming.cn/gtuxapkyyq.html

Java: resp.statusCode()
来源：http://hz.fzhhl.top/gtpuuylfcm.html

Go:   resp.StatusCode
来源：http://hz.yanxiufei.cn/gtyngkrhxp.html

Ruby: resp.code.to_i
来源：http://hz.bjfxy.top/gttmvkuune.html

C#:   (int)resp.StatusCode
来源：http://hz.hywenlv.cn/gtlspfymlz.html

[L08] 并发请求多个地址
来源：http://hz.haohaochexian.top/gtbtdiqylj.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.yuanzhike.top/gtynwujmug.html

PHP:  curl_multi_init() 系列
来源：http://hz.ywan-chungtsiang.top/gtyafzfpzy.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.sxryk.cn/gtkgowkdqq.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.hongshengwenyu.top/gtqdsyttln.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.daria6918.cn/gtogqtadch.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.gogol.net.cn/gtokvbtdsf.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.nanxinkj.top/gtadixexdw.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.jianghu66.top/gtxbxfgpzw.html

================================================================================
来源：http://hz.ehwqpu.com/gtfaqnirjm.html

M. 命令行 / 进程 / 环境
来源：http://hz.zdqjudy.top/gthubtndpz.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtnftlqrqc.html

[M01] 读取命令行参数
来源：http://hz.svipenyu.cn/gtorvaflzw.html

Py:   sys.argv[1:]
来源：http://hz.zhoulong.xyz/gtvuwkealo.html

PHP:  $argv;  $argc;
来源：http://hz.jqgfzy.top/gtprqdcudl.html

JS:   process.argv.slice(2)
来源：http://hz.mhx1999.top/gtpwtrvzpa.html

TS:   process.argv.slice(2)
来源：http://hz.ppjwa.cn/gtfkavzgmu.html

Java: args 数组（main 方法参数）
来源：http://hz.pycfn.com/gtfybghokv.html

Go:   os.Args[1:]
来源：http://hz.dianchejie.cn/gtgawfvkfl.html

Ruby: ARGV
来源：http://hz.snrcjt.cn/gtjsbydtxq.html

C#:   args 数组（Main 方法参数）
来源：http://hz.jinyuanbaomall.cn/gtzjbpobjy.html

[M02] 读取环境变量
来源：http://hz.316326.xyz/gtkbfogugt.html

Py:   os.environ.get("HOME")
来源：http://hz.jinyuanbaomall.cn/gtbzeyxewk.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.nanxinkj.top/gtzkhwvevm.html

JS:   process.env.HOME
来源：http://hz.yanxiufei.cn/gtymownqju.html

TS:   process.env.HOME
来源：http://hz.ydjk.org.cn/gtkxagxtsk.html

Java: System.getenv("HOME")
来源：http://hz.guannengcc.top/gtrulovppr.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.havefunace.top/gtxafyvaif.html

Ruby: ENV["HOME"]
来源：http://hz.tianlin.xyz/gtgisfinph.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.gzhubu.top/gtwlvloemi.html

[M03] 执行外部命令
来源：http://hz.gaohongyu789.top/gtvfmdklbr.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.hnqzz.top/gtiyjkxxgh.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.ehwqpu.com/gtwkcyngsz.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.tanke756.top/gtwribxzaf.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.yueranfly.top/gtamkwjdor.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.52xcode.cn/gtavyfmttm.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.meibo888.top/gtioyjmbrt.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.kuanghao11.cn/gtynefigzd.html

C#:   Process.Start("ls", "-l");
来源：http://hz.cashguo.top/gthsjcyvqh.html

[M04] 获取当前工作目录
来源：http://hz.ybcxt.top/gtqzeaxqxz.html

Py:   os.getcwd()
来源：http://hz.yj202588.top/gtxyafyqvb.html

PHP:  getcwd();
来源：http://hz.daria6918.cn/gtgtxlwjis.html

JS:   process.cwd()
来源：http://hz.xingfuxueyuan.xyz/gtduyzfsll.html

TS:   process.cwd()
来源：http://hz.zhijiandao.cn/gtzmfxxuhf.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.sweek.top/gtyottkvdb.html

Go:   os.Getwd()
来源：http://hz.shangyingyoupin.top/gtmrvqqoae.html

Ruby: Dir.pwd
来源：http://hz.shzxlz.cn/gtrbpvhkod.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.316326.xyz/gtibqnjayp.html

[M05] 设置退出码
来源：http://hz.andypj.xyz/gtjvmcfkuh.html

Py:   sys.exit(1)
来源：http://hz.ppjwa.cn/gtiuiqwzew.html

PHP:  exit(1);
来源：http://hz.shanyushiyangkeji.top/gtwaikjzwj.html

JS:   process.exit(1)
来源：http://hz.xingfuxueyuan.xyz/gtowqbazfl.html

TS:   process.exit(1)
来源：http://hz.jqgufenzy.top/gtqklvrgix.html

Java: System.exit(1)
来源：http://hz.chenjidiqi.icu/gtifuesyab.html

Go:   os.Exit(1)
来源：http://hz.yongpay.top/gtyaxymjeg.html

Ruby: exit 1
来源：http://hz.chenjidiqi.icu/gtqauzqnfx.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.svipenyu.cn/gthmdvlepv.html

[M06] 向标准错误输出
来源：http://hz.aibaodan.cn/gtapkelgqi.html

Py:   print("err", file=sys.stderr)
来源：http://hz.jinyuanbaomall.cn/gtnxfqjzjc.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.dashuyun.cn/gtreuusphe.html

JS:   console.error("err")
来源：http://hz.zycfv.cn/gtlzuibroj.html

TS:   console.error("err")
来源：http://hz.aizwys.cn/gtuselszbw.html

Java: System.err.println("err")
来源：http://hz.zhongyouzk.top/gtgnsqxozw.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.xinyue.icu/gtxvvzktkq.html

Ruby: warn "err"
来源：http://hz.shzxlz.cn/gtyoqvjlrx.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.jlsjyb.cn/gtsvasqcpc.html

[M07] 判断是否为主入口
来源：http://hz.shanyushiyangkeji.top/gtiekljpxf.html

Py:   if __name__ == "__main__":
来源：http://hz.chenzaomai.com/gtkspxwxac.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.yangfankeji.com/gtsjhpdeif.html

JS:   require.main === module
来源：http://hz.zhengqikj.top/gtclaacoch.html

TS:   require.main === module
来源：http://hz.smart0.xyz/gtrwzedldg.html

Java: public static void main(String[] args)
来源：http://hz.316326.xyz/gtvzjwasmi.html

Go:   func main()
来源：http://hz.9152youxi.cn/gtzzmpfhes.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.zhaomingkeji.xyz/gtienwikom.html

C#:   static void Main(string[] args)
来源：http://hz.shanyushiyangkeji.top/gtuesgvknd.html

[M08] 获取系统与运行时信息
来源：http://hz.shanyushiyangtech.top/gtvglvmwas.html

Py:   platform.system();  platform.python_version()
来源：http://hz.fengsongda.top/gtfosvmabk.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.wangdashe.top/gtmyzqazti.html

JS:   process.platform;  process.version
来源：http://hz.hammf.cn/gtagbshvzq.html

TS:   process.platform;  process.version
来源：http://hz.cheryme.top/gtjfotnjix.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.jlsjyb.cn/gtntwxidgl.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.jinqigfzy.top/gtcvtzwgtn.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.sxryk.cn/gtqsrtgtsf.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.birdmap.top/gtljfmgelf.html

================================================================================
来源：http://hz.ybcxt.top/gtduqkqcvv.html

N. 数据结构与算法
来源：http://hz.nanxinkj.top/gtnevyagkt.html

================================================================================
来源：http://hz.cashguo.top/gtbvjcnuzs.html

[N01] 二分查找（有序数组）
来源：http://hz.jlsjyb.cn/gtteftuneq.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.sufxvd.cn/gtgypqyepl.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.mhx1999.top/gtbqbpeggj.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.fzhhl.top/gtdbiihrmj.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.gogol.net.cn/gtetklrrwt.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.shzxlz.cn/gtllvrojcu.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.aizwys.cn/gtrktvkwny.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.zhijiandao.cn/gtvzannotj.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.yongpay.top/gtgffipgec.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.zycfv.cn/gtwslqmugc.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.andypj.xyz/gtyushexhf.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.ybcxt.top/gtadkiktiq.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.tanke756.top/gtcfrieeoq.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.cheryme.top/gtsfpwoobs.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.ydjk.org.cn/gteqffngnl.html

Go:   slices.Sort(arr)
来源：http://hz.feifeiyinyue.top/gtczvhlnwt.html

Ruby: arr.sort
来源：http://hz.hongshengwenyu.top/gtprwwhqqk.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.fengsongda.top/gtvwhpzyvy.html

[N03] 快速排序（分治示例）
来源：http://hz.c1oappe.top/gtiraiksxu.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.daria6918.cn/gtkfybyenn.html

PHP:  // 递归实现，或用 usort
来源：http://hz.gaohongyu789.top/gtnajpcdjh.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.kuanghao11.cn/gtfamrzfpt.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zhijiandao.cn/gtwjbwnabn.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.hfpthk.cn/gtyxrlqcpx.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.yuanzhike.top/gtpmvkmqta.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.gzhubu.top/gtvvhztkdk.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.bjfxy.top/gtqticppnz.html

[N04] 斐波那契数列
来源：http://hz.nanxuanxn.top/gtxddluijv.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.cdnleiting.top/gtekiahvcp.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.ywan-chungtsiang.top/gtkiecnjha.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.ehwqpu.com/gtoycxdpgt.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.quarkkingdee.top/gtldhfcftu.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.redwolf501.top/gtkalnnmfi.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.jqgufenzy.top/gtexaknril.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.jinqigufen.top/gtuipocost.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.hongshengwenyu.top/gtarlfhazl.html

[N05] 最大公约数
来源：http://hz.yvedp.cn/gtijtfctgu.html

Py:   math.gcd(a, b)
来源：http://hz.aizwys.cn/gtkidebzjp.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.aizwys.cn/gtikhugtar.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jqgufenzy.top/gtnrvtmylg.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yuxming.cn/gthywyaarc.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.tanke756.top/gtbaaxvqzi.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.tanke756.top/gtoddjqjoq.html

Ruby: a.gcd(b)
来源：http://hz.wangdashe.top/gtnpotxrcn.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.jinqigufen.top/gthuljmpvd.html

[N06] 判断回文字符串
来源：http://hz.jianghu66.top/gtgsxihmze.html

Py:   s == s[::-1]
来源：http://hz.ivvv.top/gtnyaxvega.html

PHP:  $s === strrev($s);
来源：http://hz.chenlongwang.top/gtbdorokse.html

JS:   s === [...s].reverse().join("")
来源：http://hz.andypj.xyz/gttkqgxacp.html

TS:   s === [...s].reverse().join("")
来源：http://hz.yj202588.top/gtblvuchoc.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.gogol.net.cn/gtmbzeenkj.html

Go:   // 双指针从两端比较
来源：http://hz.yueranfly.top/gtcxalecxa.html

Ruby: s == s.reverse
来源：http://hz.yueranfly.top/gtdyuxmdly.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.tian-w.cn/gtkzwdixlr.html

[N07] 两数之和（返回下标）
来源：http://hz.hfpthk.cn/gtvzscdkrc.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.hongshengwenyu.top/gtfpnrpmgw.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.aizwys.cn/gtuxytnrze.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.mhx1999.top/gtnmxeylgo.html

TS:   // 手写 Map<string, number>
来源：http://hz.haohaochexian.top/gthfxgfnwy.html

Java: // 手写 HashMap
来源：http://hz.mhx1999.top/gtiqaobdyg.html

Go:   // 手写 map[int]int
来源：http://hz.sysykeji.top/gtljdodkho.html

Ruby: // 手写 Hash
来源：http://hz.chenjidiqi.icu/gtockluhex.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.jinghuilouyu.cn/gtyrzkedzr.html

[N08] 生成全排列
来源：http://hz.hongshengwenyu.top/gtrpzsukal.html

Py:   itertools.permutations(arr)
来源：http://hz.ybcxt.top/gtdcnvipno.html

PHP:  // 手写递归交换
来源：http://hz.aibaodan.cn/gtccmjnjta.html

JS:   // 手写回溯递归
来源：http://hz.ywan-chungtsiang.top/gtsbhhfsoe.html

TS:   // 手写回溯递归
来源：http://hz.ydjk.org.cn/gtqkcxyusx.html

Java: // 手写回溯递归
来源：http://hz.wangdashe.top/gttvshoeng.html

Go:   // 手写回溯递归
来源：http://hz.tian-w.cn/gtdnwijplc.html

Ruby: arr.permutation.to_a
来源：http://hz.shanyushiyangtech.top/gtnwzprhun.html

C#:   // 手写回溯递归
来源：http://hz.dashuyun.cn/gtosvueplk.html

[N09] 栈与队列
来源：http://hz.cucudq.cn/gtqvxmfcoj.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.yongpay.top/gtbfmrbdqf.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.ehwqpu.com/gtrqbmynig.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.feifeiyinyue.top/gtkcunvndq.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.ppjwa.cn/gtrsukqbih.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.gzhubu.top/gtmyjphxxk.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.tanke756.top/gtnbmoclwv.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.aizwys.cn/gtyeorjauh.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.jinghuilouyu.cn/gtodkcfgsc.html

[N10] 链表节点定义
来源：http://hz.jinqigufen.top/gtrqaogrnx.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.nanxuanxn.top/gtsuvxiybq.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.iojbl.cn/gtzmfzihyu.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.xuetiantiany.cn/gtzjwofetz.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.hywenlv.cn/gtujryrflv.html

Java: class Node { int v; Node next; }
来源：http://hz.hfpthk.cn/gtkqbqrnge.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.dashuyun.cn/gtgjdokexc.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.shangyingyoupin.top/gtcipnrbxl.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.gotoacloud.top/gtnxfclkwt.html

[N11] 二叉树中序遍历
来源：http://hz.c1oappe.top/gtohkkjdjd.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.redwolf501.top/gtfhrmjdvv.html

PHP:  // 手写递归函数
来源：http://hz.dianchejie.cn/gtxnbcwbfj.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.sweek.top/gtskmbzsom.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jlsjyb.cn/gttavcimrh.html

Java: // 手写递归
来源：http://hz.snrcjt.cn/gthzmcnaqg.html

Go:   // 手写递归
来源：http://hz.zhengqikj.top/gtbpgumcfb.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.ivvv.top/gtipkbezyj.html

C#:   // 手写递归
来源：http://hz.gotoacloud.top/gtsryibmaa.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.quarkkingdee.top/gtqdjeette.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.redwolf501.top/gtuwxmmeno.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.zhengqikj.top/gtvopgezgq.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.ivvv.top/gtrqtkbhpd.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.chenlongwang.top/gtdeytfmzg.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.jiagoushi.top/gtfgxglwfl.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.dashuyun.cn/gtbwzfigov.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.svipenyu.cn/gtziqzdaez.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.52xcode.cn/gtsvatrpds.html

================================================================================
来源：http://hz.nanxuanxn.top/gttdqtbncv.html

O. 并发与异步
来源：http://hz.aizwys.cn/gtudriobvd.html

================================================================================
来源：http://hz.ivvv.top/gtjpzmksfi.html

[O01] 启动一个线程
来源：http://hz.shanyushiyangkeji.top/gtvalavzec.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.chenjidiqi.icu/gtixsqgyhd.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.kuanghao11.cn/gtgammizme.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.nanxuanxn.top/gththezvfj.html

TS:   // 同 JS
来源：http://hz.andypj.xyz/gtronuqicl.html

Java: new Thread(() -> f()).start()
来源：http://hz.nwbrower.top/gtxqfhvvos.html

Go:   go f()
来源：http://hz.52xcode.cn/gtioihcobp.html

Ruby: Thread.new { f }
来源：http://hz.guannengcc.top/gtnabkotnn.html

C#:   Task.Run(() => F());
来源：http://hz.shzxlz.cn/gtaltuxrog.html

[O02] 使用线程池
来源：http://hz.pengpengdd.cyou/gtoacetrog.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.jianghu66.top/gtmciaqjhh.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.tian-w.cn/gtlsffjwcn.html

JS:   // worker_threads 线程池
来源：http://hz.aibaodan.cn/gtavqibpvx.html

TS:   // worker_threads 线程池
来源：http://hz.yanxiufei.cn/gtxofyeruy.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.gaohongyu789.top/gtejvbrsae.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.zhengqikj.top/gtojappnor.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.ydzc1.top/gtrkmobfxp.html


<!-- 参考信息 -->