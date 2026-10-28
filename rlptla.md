代发 wailian999

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.bjfxy.top/gtuqoclrxm.html

[K07] 进制转换
来源：http://hz.hywenlv.cn/gtvkbbfmvq.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.xuanzx.com/gtuduuaebv.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.zycfv.cn/gtaumattus.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.meibo888.top/gtjxwxxxpu.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.hysaishi.cn/gtjwxeeown.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.shuidangran.top/gtxttgbvsu.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.nwbrower.top/gtsrfhzjsl.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.jqgfzy.top/gtarxfjhbo.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.andypj.xyz/gtmohxspyi.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.pycfn.com/gtgbaxecal.html

Py:   pickle.dumps(obj)
来源：http://hz.guowangkeji.top/gtklzhippb.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.daria6918.cn/gtpqkpslxi.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.guannengcc.top/gtdpfwgzhy.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.xuetiantiany.cn/gtcdtvvzkm.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.52xcode.cn/gtlyaxwfgm.html

Go:   encoding/gob
来源：http://hz.wangshuangyany.cn/gtabztnztp.html

Ruby: Marshal.dump(obj)
来源：http://hz.xziqi.cn/gteybmcdgd.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.kuanghao11.cn/gteboanamt.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtugqovnxo.html

L. 网络请求
来源：http://hz.ydzc1.top/gtkcjqygor.html

================================================================================
来源：http://hz.hysaishi.cn/gtlwimzzxz.html

[L01] 发送 GET 请求
来源：http://hz.wangdashe.top/gttvolywhk.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.ydzc1.top/gtdcywgvaw.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.daxiang520.top/gttpyezvsu.html

JS:   await fetch(url)
来源：http://hz.nanxuanxn.top/gtpuelbgsm.html

TS:   await fetch(url)
来源：http://hz.bjfxy.top/gtwxvlrtgl.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.yuxming.cn/gtibxhxyrt.html

Go:   resp, err := http.Get(url)
来源：http://hz.jyoumei.cn/gtjtbxgtei.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.zhaomingkeji.xyz/gtrcejziaf.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.hywenlv.cn/gtbkqducfa.html

[L02] 发送 POST JSON
来源：http://hz.sysykeji.top/gtgcabwusw.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.haohaochexian.top/gtemwwrsrr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.hysaishi.cn/gttsmtzxyw.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yangfankeji.com/gtdkvrdjwr.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jqgfzy.top/gthmgwsnly.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.fzhhl.top/gtmnjlycht.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.daxiang520.top/gtxsudjwte.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.gotoacloud.top/gtkylekeph.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.daria6918.cn/gtdmxllwsw.html

[L03] 设置自定义请求头
来源：http://hz.bjfxy.top/gtgsdihcoz.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.xinyue.icu/gtsygrbqpo.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.yj202588.top/gthzilsnya.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.xylfe.cn/gtidqnaava.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.shangyingyoupin.top/gtasdgubzf.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.aibaodan.cn/gtnhurgtro.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.vqdsnc.cn/gtnjxylfiw.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.xziqi.cn/gtmfipckzd.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.fengsongda.top/gtqvmfmixd.html

[L04] 设置超时
来源：http://hz.guowangkeji.top/gtvczsjrpb.html

Py:   requests.get(url, timeout=5)
来源：http://hz.shanyushiyangkeji.top/gtznwcdbru.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.havefunace.top/gtikbuxjtp.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.xinyue.icu/gtzumterzh.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zhixingplan.top/gtkiwvmkhs.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.xylfe.cn/gtpdvvaxhk.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.xinyue.icu/gttiozgfmp.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.chenzaomai.com/gttajrzjcl.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.yueranfly.top/gtjywbezxo.html

[L05] 上传文件（multipart）
来源：http://hz.quarkkingdee.top/gtlxqbrckf.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.yanxiufei.cn/gttjntehdj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.yj20258.top/gtzwtquuhx.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.hnxiangtu.top/gtsejynuxk.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.kuanghao11.cn/gtaoaoeztf.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.ybcxt.top/gtzqxwoawy.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.ybcxt.top/gtpiwzagzf.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.0kj1m.cn/gttxaxonbc.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.zhaomingkeji.xyz/gtwhjkptje.html

[L06] 解析响应为 JSON
来源：http://hz.vqdsnc.cn/gtayawvwpt.html

Py:   resp.json()
来源：http://hz.zhixingplan.top/gtafyfwrke.html

PHP:  json_decode($body, true);
来源：http://hz.guowangkeji.top/gtkopzvnwi.html

JS:   await resp.json()
来源：http://hz.cashguo.top/gtetmwssgg.html

TS:   await resp.json()
来源：http://hz.jyoumei.cn/gtidsykotk.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.cqqwz.cn/gtdqhynrpn.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.0kj1m.cn/gtndgzagyq.html

Ruby: JSON.parse(resp.body)
来源：http://hz.jianghu66.top/gtozciqoea.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.yj20258.top/gtrnultidw.html

[L07] 处理 HTTP 状态码
来源：http://hz.jlsjyb.cn/gteiehgemz.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.snrcjt.cn/gtvgmulubw.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.jianghu66.top/gtmstoojnj.html

JS:   resp.ok;  resp.status
来源：http://hz.yuanzhike.top/gtemyjqxpw.html

TS:   resp.ok;  resp.status
来源：http://hz.birdmap.top/gtwxgymopr.html

Java: resp.statusCode()
来源：http://hz.zhixingplan.top/gtxyihyntn.html

Go:   resp.StatusCode
来源：http://hz.quarkkingdee.top/gtyltmtbxn.html

Ruby: resp.code.to_i
来源：http://hz.gogol.net.cn/gtvmfeqjof.html

C#:   (int)resp.StatusCode
来源：http://hz.hfpthk.cn/gtpgwnudiu.html

[L08] 并发请求多个地址
来源：http://hz.aizwys.cn/gtrbmgjwbg.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.ybcxt.top/gtwssnkkpt.html

PHP:  curl_multi_init() 系列
来源：http://hz.ydzc1.top/gthgofcvpi.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.hnxiangtu.top/gtqbgkdtlg.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.fzhhl.top/gtkzaksnei.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.jqgufenzy.top/gtynxcmiym.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.xinyue.icu/gtaupmrknu.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.jinyuanbaomall.cn/gtlnolktnn.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.tianlin.xyz/gtgjqvlqbj.html

================================================================================
来源：http://hz.gogol.net.cn/gtylmizkpy.html

M. 命令行 / 进程 / 环境
来源：http://hz.xziqi.cn/gtdunujhdn.html

================================================================================
来源：http://hz.quarkkingdee.top/gtplzengqe.html

[M01] 读取命令行参数
来源：http://hz.yangfankeji.com/gtpssxgleu.html

Py:   sys.argv[1:]
来源：http://hz.yuanzhike.top/gtgjkjrmlf.html

PHP:  $argv;  $argc;
来源：http://hz.xuetiantiany.cn/gtocbgikii.html

JS:   process.argv.slice(2)
来源：http://hz.hongshengwenyu.top/gtoezbwoyh.html

TS:   process.argv.slice(2)
来源：http://hz.ivvv.top/gtyxtrefjm.html

Java: args 数组（main 方法参数）
来源：http://hz.shanyushiyangtech.top/gtvndilvjj.html

Go:   os.Args[1:]
来源：http://hz.yangfankeji.com/gtbacubbud.html

Ruby: ARGV
来源：http://hz.jlsjyb.cn/gtbfdrjfwr.html

C#:   args 数组（Main 方法参数）
来源：http://hz.yangfankeji.com/gtdcazkeyp.html

[M02] 读取环境变量
来源：http://hz.svipenyu.cn/gtwvrclecy.html

Py:   os.environ.get("HOME")
来源：http://hz.quarkkingdee.top/gtjjgijajw.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.chenzaomai.com/gttjboxuzf.html

JS:   process.env.HOME
来源：http://hz.snrcjt.cn/gtebcldiqx.html

TS:   process.env.HOME
来源：http://hz.yangfankeji.com/gtokvbywly.html

Java: System.getenv("HOME")
来源：http://hz.vqdsnc.cn/gtfzicosdn.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.hammf.cn/gtwhhnndyh.html

Ruby: ENV["HOME"]
来源：http://hz.meibo888.top/gtcocxztuh.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.yvedp.cn/gtekxeaekh.html

[M03] 执行外部命令
来源：http://hz.fzhhl.top/gtyteymdlr.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.chenjidiqi.icu/gtokhfyyxg.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.ydzc1.top/gtprnlwzpp.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.yonumen.top/gtohqvrnza.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.zhoulong.xyz/gtdhsmskjs.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.haohaochexian.top/gtqnrxmyjn.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.wangdashe.top/gtkuanpeid.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.xingfuxueyuan.xyz/gtmsyftnzy.html

C#:   Process.Start("ls", "-l");
来源：http://hz.gaohongyu789.top/gttbtznbxj.html

[M04] 获取当前工作目录
来源：http://hz.xuanzx.com/gtrpfibxws.html

Py:   os.getcwd()
来源：http://hz.andypj.xyz/gtdgxgfdol.html

PHP:  getcwd();
来源：http://hz.hnxiangtu.top/gtoupmwadt.html

JS:   process.cwd()
来源：http://hz.tianlin.xyz/gtacyoxvyx.html

TS:   process.cwd()
来源：http://hz.wangshuangyany.cn/gtcxzoqocq.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.wangshuangyany.cn/gtoglndofi.html

Go:   os.Getwd()
来源：http://hz.ydjk.org.cn/gtiktbaong.html

Ruby: Dir.pwd
来源：http://hz.bjfxy.top/gtjhjvjyjz.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.chenlongwang.top/gtfzlrkxpc.html

[M05] 设置退出码
来源：http://hz.aibaodan.cn/gtrxokyywh.html

Py:   sys.exit(1)
来源：http://hz.xuetiantiany.cn/gtapambsmy.html

PHP:  exit(1);
来源：http://hz.wangdashe.top/gtsskeoccz.html

JS:   process.exit(1)
来源：http://hz.xuetiantiany.cn/gtrarutahx.html

TS:   process.exit(1)
来源：http://hz.yj20258888.top/gtabuicdpj.html

Java: System.exit(1)
来源：http://hz.hfpthk.cn/gtgzojsous.html

Go:   os.Exit(1)
来源：http://hz.ydzc1.top/gtcwmarsic.html

Ruby: exit 1
来源：http://hz.sufxvd.cn/gtnfsdmziq.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.yj20258888.top/gtiasfsyrn.html

[M06] 向标准错误输出
来源：http://hz.mhx1999.top/gtkztimtta.html

Py:   print("err", file=sys.stderr)
来源：http://hz.jqgfzy.top/gtauzsnkwd.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.shanyushiyangtech.top/gtapcyvaia.html

JS:   console.error("err")
来源：http://hz.smart0.xyz/gttqrnraqc.html

TS:   console.error("err")
来源：http://hz.yj20258888.top/gtgqqrlekr.html

Java: System.err.println("err")
来源：http://hz.yvedp.cn/gtrcospsds.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.vqdsnc.cn/gtohmqchsb.html

Ruby: warn "err"
来源：http://hz.shanyushiyangkeji.top/gtqdqbfhci.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.haohaochexian.top/gtcqdwbjbj.html

[M07] 判断是否为主入口
来源：http://hz.ppjwa.cn/gtlplpjois.html

Py:   if __name__ == "__main__":
来源：http://hz.tianlin.xyz/gtvlvmqayc.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.iojbl.cn/gtwtbnyvrw.html

JS:   require.main === module
来源：http://hz.shuidangran.top/gtqnehgaen.html

TS:   require.main === module
来源：http://hz.yuanzhike.top/gtavpouvmg.html

Java: public static void main(String[] args)
来源：http://hz.pycfn.com/gttikpjvze.html

Go:   func main()
来源：http://hz.kuanghao11.cn/gtstkorcmj.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.yanxiufei.cn/gthwkrjihw.html

C#:   static void Main(string[] args)
来源：http://hz.quarkkingdee.top/gthpwqgsgu.html

[M08] 获取系统与运行时信息
来源：http://hz.yangfankeji.com/gtzqojuqqq.html

Py:   platform.system();  platform.python_version()
来源：http://hz.yonumen.top/gtbvreezaa.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.yueranfly.top/gtwzimvqgl.html

JS:   process.platform;  process.version
来源：http://hz.smart0.xyz/gtnyxpgxsc.html

TS:   process.platform;  process.version
来源：http://hz.xziqi.cn/gtiiszroqq.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.yonumen.top/gtfukeeljk.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.jqgufenzy.top/gtydjsozup.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.zhiwuduotai.top/gtdppcfkyc.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.feifeiyinyue.top/gtnhwdojrg.html

================================================================================
来源：http://hz.xinyue.icu/gtebbqnvty.html

N. 数据结构与算法
来源：http://hz.aizwys.cn/gtpmgfsgjy.html

================================================================================
来源：http://hz.hysaishi.cn/gtummpbrvo.html

[N01] 二分查找（有序数组）
来源：http://hz.cheryme.top/gttdvffeem.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.ywan-chungtsiang.top/gtzhlcgvud.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.yvedp.cn/gtfkcgnctg.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.hnqzz.top/gtbglmsykw.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.52xcode.cn/gtqqkfcnjt.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.meibo888.top/gttfapauvo.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.wangshuangyany.cn/gtzttpevds.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.jinqigfzy.top/gtcivaeubm.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.yangfankeji.com/gtmhblhdyb.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.gotoacloud.top/gtjifclcji.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.cheryme.top/gtyqwonpgf.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.jlsjyb.cn/gtwsxlebbm.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.cqqwz.cn/gtkdaiixof.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jlsjyb.cn/gtjuxtldtm.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.hywenlv.cn/gtovybuury.html

Go:   slices.Sort(arr)
来源：http://hz.hnxiangtu.top/gtutfzkyfz.html

Ruby: arr.sort
来源：http://hz.ywan-chungtsiang.top/gtlabyjvba.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.xinyue.icu/gtyyzxcqle.html

[N03] 快速排序（分治示例）
来源：http://hz.52xcode.cn/gtrwxntvvo.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.cheryme.top/gtwlkoqcpp.html

PHP:  // 递归实现，或用 usort
来源：http://hz.havefunace.top/gtzeykdghn.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.guannengcc.top/gtrstsugxh.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.bjfxy.top/gtpcurvaan.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.snrcjt.cn/gtfawdnzkl.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.jianghu66.top/gtpbbyvtlz.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.zhaomingkeji.xyz/gtxmraernb.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.redwolf501.top/gtpfvcuapj.html

[N04] 斐波那契数列
来源：http://hz.sweek.top/gtekrbzvxv.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.hammf.cn/gtmxokmvuw.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.iojbl.cn/gtrysgjcvt.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.ywan-chungtsiang.top/gtsurpecgq.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.ydjk.org.cn/gtpgopcapx.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.ywan-chungtsiang.top/gtqtiioyul.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.xylfe.cn/gtjqifwoov.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.ydzc1.top/gtwwkyjhus.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.fzhhl.top/gtohbavezp.html

[N05] 最大公约数
来源：http://hz.cucudq.cn/gtccteqbrm.html

Py:   math.gcd(a, b)
来源：http://hz.gzhubu.top/gtliihtkif.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.zhengqikj.top/gtzclxqkua.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.quarkkingdee.top/gtvdludoun.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.shanyushiyangtech.top/gtyeeziboy.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.xingfuxueyuan.xyz/gttalsqtpq.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.zhixingplan.top/gtaglrhehg.html

Ruby: a.gcd(b)
来源：http://hz.meibo888.top/gtcptzybyd.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.feifeiyinyue.top/gtdnpgawcv.html

[N06] 判断回文字符串
来源：http://hz.svipenyu.cn/gtiryvzjsy.html

Py:   s == s[::-1]
来源：http://hz.sxryk.cn/gtbomlphxg.html

PHP:  $s === strrev($s);
来源：http://hz.hfpthk.cn/gtzqfrvsmh.html

JS:   s === [...s].reverse().join("")
来源：http://hz.yj20258.top/gthodqcovv.html

TS:   s === [...s].reverse().join("")
来源：http://hz.hammf.cn/gtwkwwgzdk.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.redwolf501.top/gtuhvuqfhq.html

Go:   // 双指针从两端比较
来源：http://hz.havefunace.top/gtpsbdornr.html

Ruby: s == s.reverse
来源：http://hz.andypj.xyz/gtayvzoidh.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.tian-w.cn/gtrwapoljl.html

[N07] 两数之和（返回下标）
来源：http://hz.zdqjudy.top/gtfcjpvayx.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.ydzc1.top/gthglskncl.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.meibo888.top/gtrdppetdl.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.daxiang520.top/gtajgjawce.html

TS:   // 手写 Map<string, number>
来源：http://hz.wangshuangyany.cn/gtmdrnpelv.html

Java: // 手写 HashMap
来源：http://hz.yongpay.top/gtiihsevog.html

Go:   // 手写 map[int]int
来源：http://hz.ybcxt.top/gtomelsjro.html

Ruby: // 手写 Hash
来源：http://hz.nanxuanxn.top/gtjqrxjmoz.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.ywan-chungtsiang.top/gtlmbbzjri.html

[N08] 生成全排列
来源：http://hz.gotoacloud.top/gtdhukahrl.html

Py:   itertools.permutations(arr)
来源：http://hz.svipenyu.cn/gtenecnsur.html

PHP:  // 手写递归交换
来源：http://hz.zhiwuduotai.top/gtozgddgeg.html

JS:   // 手写回溯递归
来源：http://hz.sufxvd.cn/gtomihlqnb.html

TS:   // 手写回溯递归
来源：http://hz.sufxvd.cn/gtkcgkxfvk.html

Java: // 手写回溯递归
来源：http://hz.yj20258888.top/gtdnuvorse.html

Go:   // 手写回溯递归
来源：http://hz.316326.xyz/gtxibqoxon.html

Ruby: arr.permutation.to_a
来源：http://hz.ehwqpu.com/gtphrcjvae.html

C#:   // 手写回溯递归
来源：http://hz.kuanghao11.cn/gtypbhuszo.html

[N09] 栈与队列
来源：http://hz.zhengqikj.top/gtpzgextrf.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.redwolf501.top/gtbnzzuwvl.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.yj202588.top/gtpvhvbgcz.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.jianghu66.top/gtwxglgojx.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.aibaodan.cn/gtlvkkefqi.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.bjfxy.top/gtybxxwkym.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.zhengqikj.top/gtsrhyspua.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.zhiwuduotai.top/gtpytvmvno.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.yonumen.top/gtjyzlyqtb.html

[N10] 链表节点定义
来源：http://hz.ywan-chungtsiang.top/gtnecrrvwf.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.tanke756.top/gtvwbyhggw.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.havefunace.top/gtgkgypydd.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.c1oappe.top/gtwvshlzqk.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.jinqigfzy.top/gtzxhaaths.html

Java: class Node { int v; Node next; }
来源：http://hz.ehwqpu.com/gtppcvlhoh.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.tianlin.xyz/gtnhoixdlk.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.yangfankeji.com/gtbhdadscj.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.zhongyouzk.top/gtubwxbmsm.html

[N11] 二叉树中序遍历
来源：http://hz.sweek.top/gtzxntxmfq.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.tianlin.xyz/gtturapcls.html

PHP:  // 手写递归函数
来源：http://hz.birdmap.top/gturxawpma.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.chenlongwang.top/gtegogcgmb.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yvedp.cn/gtvoakogik.html

Java: // 手写递归
来源：http://hz.dashuyun.cn/gtkhlkyigh.html

Go:   // 手写递归
来源：http://hz.shanyushiyangtech.top/gtigtkjcwx.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.hnqzz.top/gtrqfcgzdc.html

C#:   // 手写递归
来源：http://hz.hywenlv.cn/gtcmdjhnmu.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.jinyuanbaomall.cn/gtekxwjscl.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.hfpthk.cn/gtdypbhuzo.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.shanyushiyangkeji.top/gtytaprigp.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.daxiang520.top/gtexfemmkq.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.ppjwa.cn/gtejbcgijr.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.zhoulong.xyz/gthxuzhbzr.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.zhongyouzk.top/gtxumxuojt.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.xuanzx.com/gtvukbtkph.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.gzhubu.top/gtuekamitn.html

================================================================================
来源：http://hz.hammf.cn/gtohbxkxfk.html

O. 并发与异步
来源：http://hz.zhongyouzk.top/gtntjapupx.html

================================================================================
来源：http://hz.cheryme.top/gtwdvyynoj.html

[O01] 启动一个线程
来源：http://hz.tanke756.top/gtmtazbmdo.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.hywenlv.cn/gttpsdrvki.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.iojbl.cn/gthimjmmhg.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.gotoacloud.top/gtpnhytjrn.html

TS:   // 同 JS
来源：http://hz.shanyushiyangkeji.top/gtfhaydvja.html

Java: new Thread(() -> f()).start()
来源：http://hz.tian-w.cn/gtwcnwyubw.html

Go:   go f()
来源：http://hz.sweek.top/gtahtlrxef.html

Ruby: Thread.new { f }
来源：http://hz.xylfe.cn/gtoqfytyaf.html

C#:   Task.Run(() => F());
来源：http://hz.zhoulong.xyz/gtdlgnprsw.html

[O02] 使用线程池
来源：http://hz.zhijiandao.cn/gtkjqjmrpb.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.cheryme.top/gtoumdecfk.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.bjfxy.top/gtjamvsqoz.html

JS:   // worker_threads 线程池
来源：http://hz.xziqi.cn/gthqvkwizw.html

TS:   // worker_threads 线程池
来源：http://hz.yuanzhike.top/gtbgxjzsxa.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.cashguo.top/gtrovnmiet.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.hywenlv.cn/gtwwefrjih.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.nanxuanxn.top/gtbvjpoumm.html


<!-- 参考信息 -->