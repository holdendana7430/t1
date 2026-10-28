代发 wailian999

Py:   copy.deepcopy(obj)
来源：http://hz.birdmap.top/gtcvfpvocm.html

PHP:  unserialize(serialize($obj));
来源：http://hz.zdqjudy.top/gtheyojutf.html

JS:   structuredClone(obj)
来源：http://hz.jinqigufen.top/gtadnrykyr.html

TS:   structuredClone(obj)
来源：http://hz.gzhubu.top/gteevnxjhv.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.cucudq.cn/gtbnajknaw.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.mhx1999.top/gtvgqbtqbk.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.sufxvd.cn/gtdfkxvhor.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.pengpengdd.cyou/gtnfrbnczw.html

[K06] 解析 URL 查询串
来源：http://hz.cashguo.top/gtjrhkuxxn.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.yuxming.cn/gtkcfzgejw.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.andypj.xyz/gtlgoiddnp.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.snrcjt.cn/gtzxxcczhu.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.sxryk.cn/gtkavbfuot.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.jinqigufen.top/gtodxslmxq.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.ivvv.top/gtoxhqkzft.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.jinqigufen.top/gtlbklzokl.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.cqqwz.cn/gtykmduptr.html

[K07] 进制转换
来源：http://hz.mhx1999.top/gtwdcvhghf.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.zdqjudy.top/gtrrwjjixl.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.jianghu66.top/gtshfzwuum.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.smart0.xyz/gtwkvthxsj.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.cdnleiting.top/gtrgpjfmux.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.yuxming.cn/gttgktppgh.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.yj20258888.top/gtuvdmexso.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.cqqwz.cn/gtqphnodda.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.cqqwz.cn/gtlasnkpuq.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.gaohongyu789.top/gtkzagzpek.html

Py:   pickle.dumps(obj)
来源：http://hz.nanxinkj.top/gtwbagrvqu.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.gaohongyu789.top/gtcgyyrduj.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.xinyue.icu/gtqpfnxejc.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.tian-w.cn/gtwynuxsmx.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.jiagoushi.top/gtoiumzwbq.html

Go:   encoding/gob
来源：http://hz.hfpthk.cn/gtmzaiboib.html

Ruby: Marshal.dump(obj)
来源：http://hz.ppjwa.cn/gtlduikclp.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.hywenlv.cn/gtfyhavbgg.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtvtnmujoz.html

L. 网络请求
来源：http://hz.ppjwa.cn/gtnxmksfxb.html

================================================================================
来源：http://hz.hywenlv.cn/gtipqedxjg.html

[L01] 发送 GET 请求
来源：http://hz.zhijiandao.cn/gtamlefhvp.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.ehwqpu.com/gtkjuxcatq.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.shanyushiyangkeji.top/gtvfbxlffv.html

JS:   await fetch(url)
来源：http://hz.shangyingyoupin.top/gtazozevgf.html

TS:   await fetch(url)
来源：http://hz.zhijiandao.cn/gtoogrnexn.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.shanyushiyangkeji.top/gtuymcpdvj.html

Go:   resp, err := http.Get(url)
来源：http://hz.jianghu66.top/gtexobmugh.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.yuxming.cn/gtytlmbqwf.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.gogol.net.cn/gtywtnpbso.html

[L02] 发送 POST JSON
来源：http://hz.dianchejie.cn/gteanryhdp.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.guowangkeji.top/gtwhlgwajg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.9152youxi.cn/gtwreleqyi.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.svipenyu.cn/gttosessbw.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhiwuduotai.top/gtjktdrtbv.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.hnqzz.top/gtnpinylxc.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.nwbrower.top/gtngybolmz.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.shanyushiyangkeji.top/gtxiypzsce.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.sxryk.cn/gtozahuoed.html

[L03] 设置自定义请求头
来源：http://hz.nanxinkj.top/gtvclmlfef.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.dashuyun.cn/gtcwoygxfl.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.gaohongyu789.top/gtdxaffudc.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.sweek.top/gtkqjsixxh.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.9152youxi.cn/gtioqutbnp.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.jqgfzy.top/gtavchtrqd.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.hongshengwenyu.top/gtivkcdrur.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.gotoacloud.top/gtahtepwnj.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.yuxming.cn/gthpxywfpp.html

[L04] 设置超时
来源：http://hz.havefunace.top/gteibnmmqs.html

Py:   requests.get(url, timeout=5)
来源：http://hz.jiagoushi.top/gtcicykdby.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.jinqigufen.top/gtxiotfflj.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.tanke756.top/gtprqyejav.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.pengpengdd.cyou/gtfsuvwadp.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.zhiwuduotai.top/gtqigoabhe.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.tanke756.top/gtecjhyhkc.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.wangdashe.top/gthnpzkbxt.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.shzxlz.cn/gtwunoupet.html

[L05] 上传文件（multipart）
来源：http://hz.ywan-chungtsiang.top/gtfnbpayru.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.shangyingyoupin.top/gtmjuakbma.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.guowangkeji.top/gtxcemjspl.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.iojbl.cn/gtxcmrsedj.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.cqqwz.cn/gtaqiuulai.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.tian-w.cn/gtwbjdyhdn.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.ywan-chungtsiang.top/gtxmcjdxvu.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.zycfv.cn/gtzvrepdbn.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.jinqigufen.top/gtcawlyxml.html

[L06] 解析响应为 JSON
来源：http://hz.xylfe.cn/gtgjlbgddd.html

Py:   resp.json()
来源：http://hz.pycfn.com/gtqzsbbfwx.html

PHP:  json_decode($body, true);
来源：http://hz.gotoacloud.top/gtsapkvbvm.html

JS:   await resp.json()
来源：http://hz.birdmap.top/gtagjzpuyr.html

TS:   await resp.json()
来源：http://hz.jianghu66.top/gtqynwyewl.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.shangyingyoupin.top/gtuhfgeofi.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.hammf.cn/gtaoelrspp.html

Ruby: JSON.parse(resp.body)
来源：http://hz.feifeiyinyue.top/gtqnnswlya.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.vqdsnc.cn/gtvmfnpnly.html

[L07] 处理 HTTP 状态码
来源：http://hz.cheryme.top/gtbldtpwzy.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.ppjwa.cn/gtoylubsks.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.sysykeji.top/gtrdwonkmw.html

JS:   resp.ok;  resp.status
来源：http://hz.zhengqikj.top/gtrinmiigj.html

TS:   resp.ok;  resp.status
来源：http://hz.shanyushiyangtech.top/gtcgbpqolt.html

Java: resp.statusCode()
来源：http://hz.gzhubu.top/gthfmisdgz.html

Go:   resp.StatusCode
来源：http://hz.tian-w.cn/gtrtcyspms.html

Ruby: resp.code.to_i
来源：http://hz.vqdsnc.cn/gtggusvtkw.html

C#:   (int)resp.StatusCode
来源：http://hz.kuanghao11.cn/gtjmmltfnc.html

[L08] 并发请求多个地址
来源：http://hz.haohaochexian.top/gtbwnipiqj.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.ywan-chungtsiang.top/gtveaocdul.html

PHP:  curl_multi_init() 系列
来源：http://hz.52xcode.cn/gtcucnbfnq.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhongyouzk.top/gtxjfvpaxx.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.daria6918.cn/gtrwxudixp.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.xziqi.cn/gtwjonrwue.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.shangyingyoupin.top/gtyhupyhrx.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.dianchejie.cn/gtkvjpieen.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.xinyue.icu/gtcsbhyljo.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtyoqkttmf.html

M. 命令行 / 进程 / 环境
来源：http://hz.jinqigfzy.top/gtjmyvflmw.html

================================================================================
来源：http://hz.cashguo.top/gtmfxtakgy.html

[M01] 读取命令行参数
来源：http://hz.jinyuanbaomall.cn/gtyssgoylw.html

Py:   sys.argv[1:]
来源：http://hz.ivvv.top/gticbllamc.html

PHP:  $argv;  $argc;
来源：http://hz.zhixingplan.top/gtaqxkwmso.html

JS:   process.argv.slice(2)
来源：http://hz.andypj.xyz/gthiweyhoy.html

TS:   process.argv.slice(2)
来源：http://hz.jinqigufen.top/gtjhzkddvd.html

Java: args 数组（main 方法参数）
来源：http://hz.nwbrower.top/gtjuprdfbo.html

Go:   os.Args[1:]
来源：http://hz.52xcode.cn/gthbnmczxc.html

Ruby: ARGV
来源：http://hz.c1oappe.top/gtovoqgsvl.html

C#:   args 数组（Main 方法参数）
来源：http://hz.jqgufenzy.top/gtwqszpkho.html

[M02] 读取环境变量
来源：http://hz.zdqjudy.top/gtoajyjrpj.html

Py:   os.environ.get("HOME")
来源：http://hz.zhengqikj.top/gtqouurags.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.cdnleiting.top/gtflaynumy.html

JS:   process.env.HOME
来源：http://hz.sufxvd.cn/gtidyfoejr.html

TS:   process.env.HOME
来源：http://hz.hywenlv.cn/gtprymhakc.html

Java: System.getenv("HOME")
来源：http://hz.shuidangran.top/gtwtwhikkr.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.guannengcc.top/gtxgtclgcl.html

Ruby: ENV["HOME"]
来源：http://hz.hywenlv.cn/gtvwzsoplt.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.meibo888.top/gtxuuvfvjn.html

[M03] 执行外部命令
来源：http://hz.cqqwz.cn/gtefuibuae.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.ydzc1.top/gtfhcngqva.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.yonumen.top/gtudtiemdc.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.daria6918.cn/gtrpfvtygq.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.bjfxy.top/gtsoaixxzt.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.feifeiyinyue.top/gtpufbzchl.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.chenjidiqi.icu/gtdmmwtvqz.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.aibaodan.cn/gtshskxrvo.html

C#:   Process.Start("ls", "-l");
来源：http://hz.hfpthk.cn/gtfpxbiaen.html

[M04] 获取当前工作目录
来源：http://hz.cheryme.top/gtqwnqffrk.html

Py:   os.getcwd()
来源：http://hz.ppjwa.cn/gtyngwedxl.html

PHP:  getcwd();
来源：http://hz.nanxuanxn.top/gtyzpfqshv.html

JS:   process.cwd()
来源：http://hz.jinqigufen.top/gtdbuxjrvz.html

TS:   process.cwd()
来源：http://hz.chenjidiqi.icu/gtronkwfmv.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.meibo888.top/gtoiktqdtq.html

Go:   os.Getwd()
来源：http://hz.gaohongyu789.top/gtrilgdvjr.html

Ruby: Dir.pwd
来源：http://hz.dianchejie.cn/gtfwlfxkny.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.xuanzx.com/gtqvbtscdr.html

[M05] 设置退出码
来源：http://hz.dianchejie.cn/gttcnyajps.html

Py:   sys.exit(1)
来源：http://hz.nanxuanxn.top/gtaiwoecci.html

PHP:  exit(1);
来源：http://hz.zhongyouzk.top/gtdflqetri.html

JS:   process.exit(1)
来源：http://hz.havefunace.top/gtexdilhdi.html

TS:   process.exit(1)
来源：http://hz.hywenlv.cn/gtvokqlaqa.html

Java: System.exit(1)
来源：http://hz.cqqwz.cn/gtmzzjaqwx.html

Go:   os.Exit(1)
来源：http://hz.9152youxi.cn/gtawsugdjd.html

Ruby: exit 1
来源：http://hz.fengsongda.top/gtdvwscoio.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.pengpengdd.cyou/gtoacyvbnm.html

[M06] 向标准错误输出
来源：http://hz.jqgfzy.top/gtpltvnedc.html

Py:   print("err", file=sys.stderr)
来源：http://hz.tian-w.cn/gtjcwwfifr.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.tianlin.xyz/gtglqtmsqr.html

JS:   console.error("err")
来源：http://hz.tianlin.xyz/gtamftkxmt.html

TS:   console.error("err")
来源：http://hz.cucudq.cn/gttecspoxu.html

Java: System.err.println("err")
来源：http://hz.chenzaomai.com/gtwzswxopc.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.jiagoushi.top/gthqvjcnrz.html

Ruby: warn "err"
来源：http://hz.hnqzz.top/gtpwbinjya.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.zhongyouzk.top/gtfuvlkeev.html

[M07] 判断是否为主入口
来源：http://hz.shangyingyoupin.top/gtfqmuanvl.html

Py:   if __name__ == "__main__":
来源：http://hz.shanyushiyangkeji.top/gtqwzcgfrm.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.cheryme.top/gtjcazudud.html

JS:   require.main === module
来源：http://hz.cheryme.top/gtwmebpzzn.html

TS:   require.main === module
来源：http://hz.yj20258888.top/gtrnnmitsu.html

Java: public static void main(String[] args)
来源：http://hz.yangfankeji.com/gthopfllra.html

Go:   func main()
来源：http://hz.jqgufenzy.top/gtqczwhtvb.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.havefunace.top/gtbqfcxwmx.html

C#:   static void Main(string[] args)
来源：http://hz.birdmap.top/gtjiggvmgb.html

[M08] 获取系统与运行时信息
来源：http://hz.ivvv.top/gtooieydin.html

Py:   platform.system();  platform.python_version()
来源：http://hz.chenlongwang.top/gtcsomnaba.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.guowangkeji.top/gtvvtmsmva.html

JS:   process.platform;  process.version
来源：http://hz.birdmap.top/gtuvesxqhn.html

TS:   process.platform;  process.version
来源：http://hz.jinqigufen.top/gtpulffnhp.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.daxiang520.top/gtdelczlrx.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.tanke756.top/gtpzwlfcxs.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.316326.xyz/gtgjeupaip.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.jlsjyb.cn/gtdhylmpti.html

================================================================================
来源：http://hz.smart0.xyz/gtlftsfzqs.html

N. 数据结构与算法
来源：http://hz.hfpthk.cn/gtohxzyfvr.html

================================================================================
来源：http://hz.cdnleiting.top/gtzlfsephj.html

[N01] 二分查找（有序数组）
来源：http://hz.zhijiandao.cn/gtchamjztz.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.zhixingplan.top/gtlmaakfgy.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.cdnleiting.top/gtadkmzffz.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.xingfuxueyuan.xyz/gtmgkzorry.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yongpay.top/gtwlndefpw.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.yj20258888.top/gtomhzdbzu.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.dashuyun.cn/gtslylslwh.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.dashuyun.cn/gtdmorcoqp.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.gzhubu.top/gtcvjrcuuu.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.xuanzx.com/gtrqucheoj.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.shanyushiyangkeji.top/gtiqmzwron.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.shuidangran.top/gtllxqzotu.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.nanxinkj.top/gtletocxgj.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.gogol.net.cn/gtymbjsfrl.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.redwolf501.top/gtkksydejg.html

Go:   slices.Sort(arr)
来源：http://hz.yj20258888.top/gtyudfgqhp.html

Ruby: arr.sort
来源：http://hz.xingfuxueyuan.xyz/gtjwistdnx.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.smart0.xyz/gtdggunjov.html

[N03] 快速排序（分治示例）
来源：http://hz.shanyushiyangkeji.top/gtcnyafhhf.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.hammf.cn/gtxiqtwrio.html

PHP:  // 递归实现，或用 usort
来源：http://hz.chenzaomai.com/gtvjdniaoj.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jinqigufen.top/gtugvbappq.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zhixingplan.top/gtnfjwmrut.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.shangyingyoupin.top/gtylncaxbf.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.meibo888.top/gtlrobhijl.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.vqdsnc.cn/gtctlwalgq.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.bjfxy.top/gtenkvbwcv.html

[N04] 斐波那契数列
来源：http://hz.0kj1m.cn/gtayipcjkw.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.dianchejie.cn/gtwubkcrej.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.mhx1999.top/gtlmftwpgq.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.nwbrower.top/gtfklnhiru.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.xylfe.cn/gtoztvgyja.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.shanyushiyangkeji.top/gtinchrbsj.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.jinqigfzy.top/gtaxmansmg.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.jinyuanbaomall.cn/gtoueahbxw.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.jyoumei.cn/gtdkdktwxo.html

[N05] 最大公约数
来源：http://hz.daxiang520.top/gtqznukcbp.html

Py:   math.gcd(a, b)
来源：http://hz.yj20258888.top/gtakubflex.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.iojbl.cn/gtchraltwu.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.daxiang520.top/gtwdkmvull.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yj20258888.top/gtynsczlan.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.iojbl.cn/gtttdwusva.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.zhaomingkeji.xyz/gtugwrosqj.html

Ruby: a.gcd(b)
来源：http://hz.chenzaomai.com/gtluwkxaki.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.andypj.xyz/gtqvombrvu.html

[N06] 判断回文字符串
来源：http://hz.hnxiangtu.top/gtnmnhauyt.html

Py:   s == s[::-1]
来源：http://hz.guowangkeji.top/gtmwapopoz.html

PHP:  $s === strrev($s);
来源：http://hz.jyoumei.cn/gtrguttocp.html

JS:   s === [...s].reverse().join("")
来源：http://hz.yangfankeji.com/gtswcikgfl.html

TS:   s === [...s].reverse().join("")
来源：http://hz.wangdashe.top/gtmxfkztvn.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.hfpthk.cn/gtknnbtfdk.html

Go:   // 双指针从两端比较
来源：http://hz.gaohongyu789.top/gtavbyivut.html

Ruby: s == s.reverse
来源：http://hz.yongpay.top/gtuuhpynew.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.svipenyu.cn/gttmooyzsw.html

[N07] 两数之和（返回下标）
来源：http://hz.xuetiantiany.cn/gtjvjuldhg.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.chenzaomai.com/gtiirvcmli.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.aibaodan.cn/gtjozvtttt.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.sxryk.cn/gtokkoxvvm.html

TS:   // 手写 Map<string, number>
来源：http://hz.tian-w.cn/gtgbffykov.html

Java: // 手写 HashMap
来源：http://hz.jianghu66.top/gtsivdjqsw.html

Go:   // 手写 map[int]int
来源：http://hz.jiagoushi.top/gtmhtrylzx.html

Ruby: // 手写 Hash
来源：http://hz.svipenyu.cn/gtxgiomwrr.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.shangyingyoupin.top/gticjlnlhw.html

[N08] 生成全排列
来源：http://hz.nwbrower.top/gtaxgimfqq.html

Py:   itertools.permutations(arr)
来源：http://hz.dianchejie.cn/gtqxrnhweo.html

PHP:  // 手写递归交换
来源：http://hz.ppjwa.cn/gtszapsrah.html

JS:   // 手写回溯递归
来源：http://hz.nanxinkj.top/gtradgwdbk.html

TS:   // 手写回溯递归
来源：http://hz.meibo888.top/gtrfyzkhjq.html

Java: // 手写回溯递归
来源：http://hz.ybcxt.top/gttfzmzevg.html

Go:   // 手写回溯递归
来源：http://hz.0kj1m.cn/gtbvupzzda.html

Ruby: arr.permutation.to_a
来源：http://hz.yuanzhike.top/gtppshhaxa.html

C#:   // 手写回溯递归
来源：http://hz.bjfxy.top/gtbhcpqvtp.html

[N09] 栈与队列
来源：http://hz.ydjk.org.cn/gtfweumfte.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.kuanghao11.cn/gtznesoqul.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.chenzaomai.com/gtphvimiil.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.316326.xyz/gtvuixhmdr.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.zhiwuduotai.top/gthgzzvyne.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.ehwqpu.com/gthnnckedo.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.smart0.xyz/gtphhrahlk.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.hnqzz.top/gtzyhsfaem.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.shanyushiyangtech.top/gtzgxukgjk.html

[N10] 链表节点定义
来源：http://hz.ywan-chungtsiang.top/gtgakrqtjr.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.mhx1999.top/gtlyyufwyc.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.hysaishi.cn/gtzrkqkqho.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.yangfankeji.com/gtoyenupij.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.snrcjt.cn/gtxisldivo.html

Java: class Node { int v; Node next; }
来源：http://hz.xziqi.cn/gtlmlmacyo.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.shuidangran.top/gttsancjeb.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.nwbrower.top/gtutpzmmua.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.vqdsnc.cn/gtnzpijcml.html

[N11] 二叉树中序遍历
来源：http://hz.fzhhl.top/gtetpevhjx.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.zhengqikj.top/gtaqreuchc.html

PHP:  // 手写递归函数
来源：http://hz.dashuyun.cn/gtltesvibg.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.sufxvd.cn/gtucuadlpx.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.redwolf501.top/gtcrawdnit.html

Java: // 手写递归
来源：http://hz.jinqigfzy.top/gtqdxbpbii.html

Go:   // 手写递归
来源：http://hz.ydjk.org.cn/gtxoryprfy.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.hysaishi.cn/gtakjsgvyc.html

C#:   // 手写递归
来源：http://hz.yj202588.top/gtkzasmkoz.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.cashguo.top/gttwukhgoe.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.ppjwa.cn/gtzehrgxkv.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.yangfankeji.com/gtzflhjaay.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.cheryme.top/gtbbhvfxjg.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.gotoacloud.top/gtdwktjcap.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.guowangkeji.top/gtddnmgzne.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.jqgfzy.top/gtvygmxurh.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.ivvv.top/gtytdzznmv.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yj20258888.top/gthfwuyday.html

================================================================================
来源：http://hz.yuanzhike.top/gtmxijwgug.html

O. 并发与异步
来源：http://hz.c1oappe.top/gtyyqtoweh.html

================================================================================
来源：http://hz.chenzaomai.com/gtzprkmfsy.html

[O01] 启动一个线程
来源：http://hz.hywenlv.cn/gtucwxofto.html


<!-- 参考信息 -->