代发 wailian999

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.tanke756.top/gtgakcpvpc.html

[K07] 进制转换
来源：http://hz.dianchejie.cn/gtbrxvpejw.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.hywenlv.cn/gtabjrykbu.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.ppjwa.cn/gtppsuumaz.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.birdmap.top/gtvytvakzj.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.jyoumei.cn/gtlytppbat.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.jyoumei.cn/gtcbyjymon.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.ppjwa.cn/gtfelgpjny.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.ppjwa.cn/gtzvhxouze.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.ydzc1.top/gtehosmlxt.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.ywan-chungtsiang.top/gtlhqarcgx.html

Py:   pickle.dumps(obj)
来源：http://hz.yanxiufei.cn/gtbztepmdz.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.zhaomingkeji.xyz/gtkwjkdhlg.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.ppjwa.cn/gtncrcknfi.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.yonumen.top/gtncgkvgse.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.havefunace.top/gtwdgeeehj.html

Go:   encoding/gob
来源：http://hz.zhixingplan.top/gtfrxzoupu.html

Ruby: Marshal.dump(obj)
来源：http://hz.ppjwa.cn/gtdhkslauk.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.nanxuanxn.top/gtmmqahnyk.html

================================================================================
来源：http://hz.yonumen.top/gtjtrmbcre.html

L. 网络请求
来源：http://hz.ywan-chungtsiang.top/gtlktnvtzc.html

================================================================================
来源：http://hz.cashguo.top/gtwiylossx.html

[L01] 发送 GET 请求
来源：http://hz.nanxuanxn.top/gtebddhhpe.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.vqdsnc.cn/gtdigffkzf.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.yonumen.top/gtopxdkuqk.html

JS:   await fetch(url)
来源：http://hz.andypj.xyz/gtuaajgvhn.html

TS:   await fetch(url)
来源：http://hz.316326.xyz/gtqnncmzqx.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.ybcxt.top/gtfwutudbw.html

Go:   resp, err := http.Get(url)
来源：http://hz.vqdsnc.cn/gtqenkdfnh.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.snrcjt.cn/gtprjouzpd.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.xylfe.cn/gtmyxubfnv.html

[L02] 发送 POST JSON
来源：http://hz.yanxiufei.cn/gtxviqgftn.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.sufxvd.cn/gtaooarhbd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.sxryk.cn/gtyglillgr.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhaomingkeji.xyz/gthidmuyta.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.havefunace.top/gtjlwypwbt.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.yonumen.top/gtlxolmopc.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.yvedp.cn/gtouofgfam.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.jinqigufen.top/gtfsjwtqfk.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.hnqzz.top/gtkmlwymym.html

[L03] 设置自定义请求头
来源：http://hz.xuetiantiany.cn/gtxmdlmndz.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.nwbrower.top/gtdltrltqc.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.sweek.top/gtnjdomchn.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yj20258888.top/gtnpbjdocp.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.redwolf501.top/gtcdrgcrtf.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.jinqigfzy.top/gtcgdkarqz.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.guowangkeji.top/gtnjjynlqm.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.chenlongwang.top/gtrmdrlyrc.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.jianghu66.top/gtszudytrk.html

[L04] 设置超时
来源：http://hz.yonumen.top/gtwffvqlmg.html

Py:   requests.get(url, timeout=5)
来源：http://hz.yongpay.top/gtbqtaivmg.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.yangfankeji.com/gtjjxaqxmc.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yonumen.top/gtzdgrhffv.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.ivvv.top/gtgjstzdqw.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.ybcxt.top/gtorjpmtqb.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.zhengqikj.top/gtlgvrntcm.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.316326.xyz/gtrfjpcytw.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.hysaishi.cn/gtggzhrmsp.html

[L05] 上传文件（multipart）
来源：http://hz.jinqigfzy.top/gtqwmngnnk.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.quarkkingdee.top/gtbixnbegy.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.guannengcc.top/gtphflspan.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.gogol.net.cn/gtdfqbrfnd.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.hysaishi.cn/gtwmdiibre.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.jyoumei.cn/gtkajvnbnq.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.zhiwuduotai.top/gtnaahcmme.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.guowangkeji.top/gtdeujuvan.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.andypj.xyz/gtzecrwzik.html

[L06] 解析响应为 JSON
来源：http://hz.yuxming.cn/gtqcqkoqvm.html

Py:   resp.json()
来源：http://hz.yvedp.cn/gtqtmwvera.html

PHP:  json_decode($body, true);
来源：http://hz.yj202588.top/gtynyltmxv.html

JS:   await resp.json()
来源：http://hz.mhx1999.top/gtgwegtuvt.html

TS:   await resp.json()
来源：http://hz.jianghu66.top/gtclnhnrln.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.tanke756.top/gtjprcrwfn.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.xingfuxueyuan.xyz/gtipikxssi.html

Ruby: JSON.parse(resp.body)
来源：http://hz.svipenyu.cn/gtlgvpkboh.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.shzxlz.cn/gttkihvdga.html

[L07] 处理 HTTP 状态码
来源：http://hz.pengpengdd.cyou/gtfhifrmvk.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.tian-w.cn/gtxeouwcrz.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.fzhhl.top/gtjanvnnrs.html

JS:   resp.ok;  resp.status
来源：http://hz.yangfankeji.com/gtunocppxt.html

TS:   resp.ok;  resp.status
来源：http://hz.9152youxi.cn/gtwbawxepj.html

Java: resp.statusCode()
来源：http://hz.shzxlz.cn/gtikswpvnw.html

Go:   resp.StatusCode
来源：http://hz.meibo888.top/gtqltamnih.html

Ruby: resp.code.to_i
来源：http://hz.xuanzx.com/gtlthkewcd.html

C#:   (int)resp.StatusCode
来源：http://hz.fzhhl.top/gtsfdycsew.html

[L08] 并发请求多个地址
来源：http://hz.vqdsnc.cn/gtipmsiynq.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.andypj.xyz/gtujopkzmx.html

PHP:  curl_multi_init() 系列
来源：http://hz.zhixingplan.top/gtontuihri.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.xuetiantiany.cn/gtcvwrygpb.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yj20258.top/gtbeqgkfoi.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.havefunace.top/gtefrzzrlr.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.gzhubu.top/gtfyropdwx.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.meibo888.top/gtcqmsvyqm.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.jinqigfzy.top/gtdcycmwqp.html

================================================================================
来源：http://hz.jlsjyb.cn/gtrjggldjb.html

M. 命令行 / 进程 / 环境
来源：http://hz.hywenlv.cn/gtzojjocdn.html

================================================================================
来源：http://hz.svipenyu.cn/gtxkmrxmll.html

[M01] 读取命令行参数
来源：http://hz.haohaochexian.top/gtgmslkmgz.html

Py:   sys.argv[1:]
来源：http://hz.hfpthk.cn/gtneuylknq.html

PHP:  $argv;  $argc;
来源：http://hz.redwolf501.top/gtutmkxooj.html

JS:   process.argv.slice(2)
来源：http://hz.jlsjyb.cn/gtxnvidzbu.html

TS:   process.argv.slice(2)
来源：http://hz.snrcjt.cn/gtkmiurcdx.html

Java: args 数组（main 方法参数）
来源：http://hz.jinqigufen.top/gtlxceshgi.html

Go:   os.Args[1:]
来源：http://hz.zhaomingkeji.xyz/gtdzdnkian.html

Ruby: ARGV
来源：http://hz.birdmap.top/gtsrozljml.html

C#:   args 数组（Main 方法参数）
来源：http://hz.hysaishi.cn/gtqaoplpet.html

[M02] 读取环境变量
来源：http://hz.vqdsnc.cn/gtxfxaurop.html

Py:   os.environ.get("HOME")
来源：http://hz.tian-w.cn/gtkqvvhxnt.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.zhiwuduotai.top/gttyheielm.html

JS:   process.env.HOME
来源：http://hz.zhijiandao.cn/gtfnaioahu.html

TS:   process.env.HOME
来源：http://hz.tanke756.top/gtsshcagqz.html

Java: System.getenv("HOME")
来源：http://hz.aizwys.cn/gtdqpwryrt.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.yongpay.top/gtfbqxthpy.html

Ruby: ENV["HOME"]
来源：http://hz.52xcode.cn/gtbbuifeuj.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.andypj.xyz/gtqhaavavf.html

[M03] 执行外部命令
来源：http://hz.yangfankeji.com/gtjdaebwgn.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.quarkkingdee.top/gtjvsoqouu.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.jqgufenzy.top/gthaznwxns.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.jianghu66.top/gtcjetkzap.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.0kj1m.cn/gtooxycrah.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.havefunace.top/gtyehvhuqx.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.yongpay.top/gtudbezfds.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.jlsjyb.cn/gtiizbgwsr.html

C#:   Process.Start("ls", "-l");
来源：http://hz.zhixingplan.top/gtmbbxzdho.html

[M04] 获取当前工作目录
来源：http://hz.sysykeji.top/gtpnyotrtq.html

Py:   os.getcwd()
来源：http://hz.bjfxy.top/gtymvansot.html

PHP:  getcwd();
来源：http://hz.0kj1m.cn/gtjgijneek.html

JS:   process.cwd()
来源：http://hz.hywenlv.cn/gtormmkplz.html

TS:   process.cwd()
来源：http://hz.jinqigfzy.top/gtnhsoldjy.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.tianlin.xyz/gtknabmzyq.html

Go:   os.Getwd()
来源：http://hz.hysaishi.cn/gtxmmrygjn.html

Ruby: Dir.pwd
来源：http://hz.xuanzx.com/gtcjowujhu.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.yongpay.top/gtuwbnytas.html

[M05] 设置退出码
来源：http://hz.shanyushiyangkeji.top/gtyjojlcyj.html

Py:   sys.exit(1)
来源：http://hz.yongpay.top/gtuapiyulc.html

PHP:  exit(1);
来源：http://hz.jqgufenzy.top/gtzimiuekq.html

JS:   process.exit(1)
来源：http://hz.wangdashe.top/gtygslativ.html

TS:   process.exit(1)
来源：http://hz.yvedp.cn/gtzlyfygsz.html

Java: System.exit(1)
来源：http://hz.jianghu66.top/gtkcsetzxi.html

Go:   os.Exit(1)
来源：http://hz.hammf.cn/gtrazcyxdb.html

Ruby: exit 1
来源：http://hz.yj20258.top/gtlnpxdfsd.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.aizwys.cn/gtwrcoxwcl.html

[M06] 向标准错误输出
来源：http://hz.nanxuanxn.top/gtlfjbrvff.html

Py:   print("err", file=sys.stderr)
来源：http://hz.yuanzhike.top/gtnejaisou.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.svipenyu.cn/gthjywtzbu.html

JS:   console.error("err")
来源：http://hz.xylfe.cn/gtukdwwyev.html

TS:   console.error("err")
来源：http://hz.hnqzz.top/gttjpmhvkq.html

Java: System.err.println("err")
来源：http://hz.snrcjt.cn/gtklkeoawb.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.hywenlv.cn/gthysxbrqo.html

Ruby: warn "err"
来源：http://hz.jqgufenzy.top/gtzmspnljq.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.zhengqikj.top/gttnpbfrab.html

[M07] 判断是否为主入口
来源：http://hz.yangfankeji.com/gtrecrtgvx.html

Py:   if __name__ == "__main__":
来源：http://hz.tian-w.cn/gttxavnzte.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.aizwys.cn/gtsmwueuvb.html

JS:   require.main === module
来源：http://hz.hfpthk.cn/gtydeijifw.html

TS:   require.main === module
来源：http://hz.zhaomingkeji.xyz/gtmxuvioku.html

Java: public static void main(String[] args)
来源：http://hz.ydjk.org.cn/gtqgukeaht.html

Go:   func main()
来源：http://hz.chenjidiqi.icu/gtygcnwtdb.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.tanke756.top/gtqvbkianr.html

C#:   static void Main(string[] args)
来源：http://hz.yueranfly.top/gtbczugerf.html

[M08] 获取系统与运行时信息
来源：http://hz.yangfankeji.com/gtqpoqjefq.html

Py:   platform.system();  platform.python_version()
来源：http://hz.hongshengwenyu.top/gtmueatlsq.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.sufxvd.cn/gtdyvacopj.html

JS:   process.platform;  process.version
来源：http://hz.wangshuangyany.cn/gtmnmlnqcx.html

TS:   process.platform;  process.version
来源：http://hz.wangdashe.top/gtbkwubeng.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.vqdsnc.cn/gtsndmjqnp.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.yonumen.top/gtjgqzeyyu.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.jqgfzy.top/gtjskkhoht.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.cheryme.top/gtlobbohsa.html

================================================================================
来源：http://hz.gzhubu.top/gteuoepjbn.html

N. 数据结构与算法
来源：http://hz.bjfxy.top/gtcdovpxfe.html

================================================================================
来源：http://hz.yangfankeji.com/gtrszgcsqy.html

[N01] 二分查找（有序数组）
来源：http://hz.hnxiangtu.top/gtzwovjksb.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.jiagoushi.top/gtmglmgzwp.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.fzhhl.top/gtbigvoyko.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yonumen.top/gtnsdkamwz.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yj20258.top/gtjdrvzeqs.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.yuxming.cn/gtawccgmko.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.chenjidiqi.icu/gtykmbcfrv.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.svipenyu.cn/gtvuomiawm.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.ywan-chungtsiang.top/gtweqqhkaz.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.yuanzhike.top/gtiqjebrtr.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.xylfe.cn/gtdycfypvo.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.yj202588.top/gtcrwohpni.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.redwolf501.top/gtxjmclzyr.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.gaohongyu789.top/gthflikkxw.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.xuanzx.com/gtqpqrpgih.html

Go:   slices.Sort(arr)
来源：http://hz.c1oappe.top/gtoialxxqh.html

Ruby: arr.sort
来源：http://hz.zdqjudy.top/gtapgwpdmy.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.wangdashe.top/gtwbffdzuk.html

[N03] 快速排序（分治示例）
来源：http://hz.9152youxi.cn/gtiecjdvow.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.xylfe.cn/gtwtaketuq.html

PHP:  // 递归实现，或用 usort
来源：http://hz.pycfn.com/gtnkmdnakh.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zhixingplan.top/gtuvgspcrb.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.gzhubu.top/gtfcfouuhd.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.hywenlv.cn/gtwcsmjanh.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.mhx1999.top/gtwcaycnzj.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.sweek.top/gtfgiigorq.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.ybcxt.top/gtwuffckcg.html

[N04] 斐波那契数列
来源：http://hz.iojbl.cn/gtzrbdyjsq.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.316326.xyz/gtrtfvcadl.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.jyoumei.cn/gtaojgxhkc.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.sxryk.cn/gtbkuivtsv.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.gaohongyu789.top/gtejhqpimf.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.pengpengdd.cyou/gttgdlkexo.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.yongpay.top/gtmfxekvqx.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.guowangkeji.top/gttrumnhzm.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.jiagoushi.top/gtvcovcobl.html

[N05] 最大公约数
来源：http://hz.andypj.xyz/gtniumjeng.html

Py:   math.gcd(a, b)
来源：http://hz.0kj1m.cn/gterakosfl.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.meibo888.top/gtibljahrs.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.0kj1m.cn/gtrfpomrfm.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.shanyushiyangkeji.top/gthntaamjf.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.yuanzhike.top/gtdxubbvmk.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.zycfv.cn/gtzcsmyubg.html

Ruby: a.gcd(b)
来源：http://hz.ehwqpu.com/gtfxcvxumz.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.yj20258888.top/gtjtqyvxby.html

[N06] 判断回文字符串
来源：http://hz.sysykeji.top/gtduhgxxsf.html

Py:   s == s[::-1]
来源：http://hz.shangyingyoupin.top/gtozifbzbf.html

PHP:  $s === strrev($s);
来源：http://hz.cashguo.top/gteianalad.html

JS:   s === [...s].reverse().join("")
来源：http://hz.c1oappe.top/gtulduatnq.html

TS:   s === [...s].reverse().join("")
来源：http://hz.iojbl.cn/gtkwqmajil.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.zhixingplan.top/gticlmqxhw.html

Go:   // 双指针从两端比较
来源：http://hz.cdnleiting.top/gtbhyditko.html

Ruby: s == s.reverse
来源：http://hz.xingfuxueyuan.xyz/gtbsrzbjmk.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.ivvv.top/gtidjnqily.html

[N07] 两数之和（返回下标）
来源：http://hz.zdqjudy.top/gtzpadgkxp.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.xinyue.icu/gtrugqnhvs.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.hysaishi.cn/gtiidxrhqi.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.snrcjt.cn/gtezsypgll.html

TS:   // 手写 Map<string, number>
来源：http://hz.shangyingyoupin.top/gtdgcttjxv.html

Java: // 手写 HashMap
来源：http://hz.fengsongda.top/gtseweskyw.html

Go:   // 手写 map[int]int
来源：http://hz.wangshuangyany.cn/gtuyqnjnlj.html

Ruby: // 手写 Hash
来源：http://hz.ivvv.top/gtnwqgnfbn.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.sufxvd.cn/gtzlvrlhxh.html

[N08] 生成全排列
来源：http://hz.wangdashe.top/gtcrkhrrtv.html

Py:   itertools.permutations(arr)
来源：http://hz.fzhhl.top/gtdobpzecc.html

PHP:  // 手写递归交换
来源：http://hz.xziqi.cn/gtopleudvl.html

JS:   // 手写回溯递归
来源：http://hz.smart0.xyz/gtzsztzeqh.html

TS:   // 手写回溯递归
来源：http://hz.sxryk.cn/gtnikhvhhs.html

Java: // 手写回溯递归
来源：http://hz.mhx1999.top/gttgnmbkwt.html

Go:   // 手写回溯递归
来源：http://hz.zhengqikj.top/gtnckgzuyx.html

Ruby: arr.permutation.to_a
来源：http://hz.guannengcc.top/gtmtebeqpq.html

C#:   // 手写回溯递归
来源：http://hz.quarkkingdee.top/gtejwajdrl.html

[N09] 栈与队列
来源：http://hz.xylfe.cn/gtanunumoe.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.zhongyouzk.top/gtydaubiqm.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.yvedp.cn/gtgoctmkpd.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.yongpay.top/gtpeusfcgu.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.shangyingyoupin.top/gtchxaqcyl.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.jiagoushi.top/gtwkvpxptp.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.yj20258.top/gtcxqaejvx.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.jlsjyb.cn/gtttahbynf.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.yj20258888.top/gtydvnaicg.html

[N10] 链表节点定义
来源：http://hz.jinqigfzy.top/gtzepjmpkj.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.ywan-chungtsiang.top/gtdbpsjxjo.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.chenzaomai.com/gtpjalrznr.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.xziqi.cn/gtntyrpkgq.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.redwolf501.top/gtrbbzowry.html

Java: class Node { int v; Node next; }
来源：http://hz.zhoulong.xyz/gtzszcbqvt.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.tanke756.top/gtwipprrno.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.sufxvd.cn/gtlkydpujz.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.dashuyun.cn/gtxiatszfu.html

[N11] 二叉树中序遍历
来源：http://hz.yj202588.top/gtqzqhjdrg.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.jqgfzy.top/gtdfvijycr.html

PHP:  // 手写递归函数
来源：http://hz.xingfuxueyuan.xyz/gtjbywogcx.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.andypj.xyz/gtamjihvbk.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.xylfe.cn/gtqxtvkyoo.html

Java: // 手写递归
来源：http://hz.daria6918.cn/gtvkveytza.html

Go:   // 手写递归
来源：http://hz.gogol.net.cn/gtswxifvfe.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.svipenyu.cn/gtspsjiyat.html

C#:   // 手写递归
来源：http://hz.nanxuanxn.top/gtwfcfeshx.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.yuxming.cn/gtxvigitvv.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.chenlongwang.top/gtyubrbgzl.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.chenlongwang.top/gtpyzsnvhq.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yangfankeji.com/gthmobyeqg.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.hnqzz.top/gtcuqrxrlh.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yangfankeji.com/gtzjmrsdxv.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.c1oappe.top/gthgzmyjmg.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.aizwys.cn/gtnsamarfp.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yj202588.top/gtkuwwszxh.html

================================================================================
来源：http://hz.gzhubu.top/gtezlqtzdv.html

O. 并发与异步
来源：http://hz.jianghu66.top/gtuzgeiitt.html

================================================================================
来源：http://hz.mhx1999.top/gtffvpfkgq.html

[O01] 启动一个线程
来源：http://hz.shzxlz.cn/gtqbbizcna.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.kuanghao11.cn/gtbtfamfyv.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.shanyushiyangtech.top/gthnlwjjvt.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.xylfe.cn/gtshknwtwu.html

TS:   // 同 JS
来源：http://hz.ydjk.org.cn/gtinmzskkk.html

Java: new Thread(() -> f()).start()
来源：http://hz.jiagoushi.top/gtiqjwrwrz.html

Go:   go f()
来源：http://hz.dashuyun.cn/gthokujbmy.html

Ruby: Thread.new { f }
来源：http://hz.haohaochexian.top/gteihjayer.html

C#:   Task.Run(() => F());
来源：http://hz.zhoulong.xyz/gtayuzfuwc.html

[O02] 使用线程池
来源：http://hz.dashuyun.cn/gthysvfjaj.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.shangyingyoupin.top/gtmllqxyzj.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.0kj1m.cn/gtszrobrlc.html

JS:   // worker_threads 线程池
来源：http://hz.yuanzhike.top/gtfcuuvelh.html

TS:   // worker_threads 线程池
来源：http://hz.havefunace.top/gtzgtsrzyy.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.gaohongyu789.top/gtjztduiqw.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.xingfuxueyuan.xyz/gtqxvtkemd.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.guowangkeji.top/gtlzpzziob.html


<!-- 参考信息 -->