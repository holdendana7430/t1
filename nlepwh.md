代发 wailian999

[K06] 解析 URL 查询串
来源：http://hz.yongpay.top/gtknygmsmy.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.yongpay.top/gtuplossfv.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.ydzc1.top/gtibolcral.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.wangshuangyany.cn/gtaztqadsq.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.chenlongwang.top/gtxttfyvni.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.yj202588.top/gttzexkriq.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.mhx1999.top/gtepxjzylb.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.ybcxt.top/gthuweduug.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.yanxiufei.cn/gtmcnvdkyc.html

[K07] 进制转换
来源：http://hz.yanxiufei.cn/gtmautzizh.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.haohaochexian.top/gtpumlfdug.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.hongshengwenyu.top/gtyhjsppfk.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.hammf.cn/gtlpkmegwu.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.mhx1999.top/gtpeakaxgo.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.jinyuanbaomall.cn/gtayzvficx.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.hongshengwenyu.top/gtgrvzvfay.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.zhongyouzk.top/gtmbefeakb.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.zhiwuduotai.top/gtvobmrqub.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.sweek.top/gtrtyesudv.html

Py:   pickle.dumps(obj)
来源：http://hz.snrcjt.cn/gtmevxxvim.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.jiagoushi.top/gtqvjpfpbj.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.yuanzhike.top/gtvqbfzakv.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.yuxming.cn/gtslgfrshs.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.chenlongwang.top/gtfxrgivfa.html

Go:   encoding/gob
来源：http://hz.zhengqikj.top/gtyaoiqata.html

Ruby: Marshal.dump(obj)
来源：http://hz.52xcode.cn/gtnqitinen.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.316326.xyz/gtlcgdkugk.html

================================================================================
来源：http://hz.sxryk.cn/gtjokipfat.html

L. 网络请求
来源：http://hz.havefunace.top/gtktbblfej.html

================================================================================
来源：http://hz.hammf.cn/gtfcjypmdr.html

[L01] 发送 GET 请求
来源：http://hz.316326.xyz/gtriwscjbb.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.ywan-chungtsiang.top/gtvbtjglpm.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.daria6918.cn/gtpojuhiin.html

JS:   await fetch(url)
来源：http://hz.ybcxt.top/gtpphksjxy.html

TS:   await fetch(url)
来源：http://hz.zhiwuduotai.top/gtdcofibsw.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.xinyue.icu/gtvfebttbw.html

Go:   resp, err := http.Get(url)
来源：http://hz.jlsjyb.cn/gtxfhwtrwk.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.yvedp.cn/gtdldrspfh.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.0kj1m.cn/gtunvcrajo.html

[L02] 发送 POST JSON
来源：http://hz.hnqzz.top/gtucovwgij.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.sxryk.cn/gtiyciecft.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.52xcode.cn/gtftnblneb.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.fzhhl.top/gtbpbdcgnx.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhixingplan.top/gtxuudpuqf.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.zhoulong.xyz/gtcgvdpmrp.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.zhijiandao.cn/gtkxyuvanj.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.ybcxt.top/gtkktavlhn.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.xylfe.cn/gtkaxtiptc.html

[L03] 设置自定义请求头
来源：http://hz.zhaomingkeji.xyz/gtxrwsqbwo.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.gotoacloud.top/gttzsmekhe.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.andypj.xyz/gtzqdfegrl.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.ydjk.org.cn/gtnqhmcehh.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.52xcode.cn/gtwgbhgkws.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.ywan-chungtsiang.top/gtsjqprape.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.tanke756.top/gtylrkxcpv.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.0kj1m.cn/gtnpxkxhhi.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.nanxinkj.top/gtyletdqad.html

[L04] 设置超时
来源：http://hz.xingfuxueyuan.xyz/gtjfovhmmp.html

Py:   requests.get(url, timeout=5)
来源：http://hz.zhongyouzk.top/gtkhrdvnlj.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.shuidangran.top/gtetltcdwx.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.ivvv.top/gtnvbwfmsy.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.ydzc1.top/gteqzlfopy.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.nanxinkj.top/gtsifirjnx.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.smart0.xyz/gtvytgrnyf.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.daria6918.cn/gtpzjlsild.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.shzxlz.cn/gtviniiqpg.html

[L05] 上传文件（multipart）
来源：http://hz.zhijiandao.cn/gtpffojoie.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.c1oappe.top/gtgbcgonzm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.andypj.xyz/gtifnwnpmf.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.meibo888.top/gtwdlrfbjb.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.ppjwa.cn/gtyaotgoca.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.c1oappe.top/gtibzsplvx.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.ehwqpu.com/gtlyndcauu.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.iojbl.cn/gtagjdaakw.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.jqgufenzy.top/gtasoccons.html

[L06] 解析响应为 JSON
来源：http://hz.hongshengwenyu.top/gtvwnpvbrf.html

Py:   resp.json()
来源：http://hz.havefunace.top/gtjlwvhvsf.html

PHP:  json_decode($body, true);
来源：http://hz.sysykeji.top/gtxwgqbkcp.html

JS:   await resp.json()
来源：http://hz.zhaomingkeji.xyz/gtgolnolbe.html

TS:   await resp.json()
来源：http://hz.fengsongda.top/gtnqsfvzrs.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.hysaishi.cn/gtofcxbvfj.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.havefunace.top/gtwpyvjigh.html

Ruby: JSON.parse(resp.body)
来源：http://hz.ppjwa.cn/gtwyxtzflg.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.xylfe.cn/gtcoblkwjb.html

[L07] 处理 HTTP 状态码
来源：http://hz.sweek.top/gtiqqrcfaj.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.wangshuangyany.cn/gtpetrodiq.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.iojbl.cn/gtwtyivyxa.html

JS:   resp.ok;  resp.status
来源：http://hz.feifeiyinyue.top/gtgbrkkoam.html

TS:   resp.ok;  resp.status
来源：http://hz.9152youxi.cn/gtknzjxpih.html

Java: resp.statusCode()
来源：http://hz.fengsongda.top/gtxsgttoyh.html

Go:   resp.StatusCode
来源：http://hz.svipenyu.cn/gtuxpzlics.html

Ruby: resp.code.to_i
来源：http://hz.iojbl.cn/gtzoqqhbmx.html

C#:   (int)resp.StatusCode
来源：http://hz.jlsjyb.cn/gtcvsvkvqj.html

[L08] 并发请求多个地址
来源：http://hz.yangfankeji.com/gtfdgsrcsy.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.cheryme.top/gtoxoyjdgb.html

PHP:  curl_multi_init() 系列
来源：http://hz.sweek.top/gtbtwxjhbm.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jqgufenzy.top/gtztnfllrs.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.ehwqpu.com/gtplpoyddh.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.bjfxy.top/gtjcdcnjne.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.vqdsnc.cn/gtrfkstoro.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.jqgufenzy.top/gttrkhfado.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.havefunace.top/gtvcpjkjlw.html

================================================================================
来源：http://hz.sysykeji.top/gttlkisvtp.html

M. 命令行 / 进程 / 环境
来源：http://hz.hnxiangtu.top/gtqlfyanft.html

================================================================================
来源：http://hz.yuanzhike.top/gttkdjogzg.html

[M01] 读取命令行参数
来源：http://hz.jinghuilouyu.cn/gtfurtevch.html

Py:   sys.argv[1:]
来源：http://hz.quarkkingdee.top/gthycngnpi.html

PHP:  $argv;  $argc;
来源：http://hz.chenjidiqi.icu/gttahkqcxc.html

JS:   process.argv.slice(2)
来源：http://hz.wangdashe.top/gteepqwviz.html

TS:   process.argv.slice(2)
来源：http://hz.xinyue.icu/gtawpqplso.html

Java: args 数组（main 方法参数）
来源：http://hz.zdqjudy.top/gtfaqipnpg.html

Go:   os.Args[1:]
来源：http://hz.ybcxt.top/gtnanvfeef.html

Ruby: ARGV
来源：http://hz.zdqjudy.top/gtxsyktnfr.html

C#:   args 数组（Main 方法参数）
来源：http://hz.hfpthk.cn/gtaxgkicxa.html

[M02] 读取环境变量
来源：http://hz.cheryme.top/gtcienxujh.html

Py:   os.environ.get("HOME")
来源：http://hz.ehwqpu.com/gtpvqtnmbx.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.mhx1999.top/gtpicdkqgg.html

JS:   process.env.HOME
来源：http://hz.jqgfzy.top/gtimqbgttz.html

TS:   process.env.HOME
来源：http://hz.sysykeji.top/gtbcbhfqlj.html

Java: System.getenv("HOME")
来源：http://hz.yonumen.top/gthuxumchm.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.shangyingyoupin.top/gtslrdxmlz.html

Ruby: ENV["HOME"]
来源：http://hz.smart0.xyz/gtmyzxrtjp.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.vqdsnc.cn/gtwafkgzzr.html

[M03] 执行外部命令
来源：http://hz.fzhhl.top/gtkozpnxyu.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.cqqwz.cn/gtagqilqty.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.jianghu66.top/gtfzujvxcu.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.shangyingyoupin.top/gtqgzhdfcc.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.jyoumei.cn/gtxleyehqz.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.zhiwuduotai.top/gtgxnwsumx.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.sufxvd.cn/gtlzakcsuj.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.ivvv.top/gtocpeuzll.html

C#:   Process.Start("ls", "-l");
来源：http://hz.gogol.net.cn/gtywqmotxv.html

[M04] 获取当前工作目录
来源：http://hz.nwbrower.top/gtusawilqe.html

Py:   os.getcwd()
来源：http://hz.pengpengdd.cyou/gtczlhqqkg.html

PHP:  getcwd();
来源：http://hz.0kj1m.cn/gtydxfzxjj.html

JS:   process.cwd()
来源：http://hz.nwbrower.top/gtcbhksfmk.html

TS:   process.cwd()
来源：http://hz.hnxiangtu.top/gtduslzazp.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.daxiang520.top/gtxrvsisuf.html

Go:   os.Getwd()
来源：http://hz.9152youxi.cn/gtlsdwrwbm.html

Ruby: Dir.pwd
来源：http://hz.ywan-chungtsiang.top/gttcgpiojt.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.jqgufenzy.top/gtmskjnuiw.html

[M05] 设置退出码
来源：http://hz.jqgufenzy.top/gtwmfxwlzi.html

Py:   sys.exit(1)
来源：http://hz.snrcjt.cn/gtchvwikub.html

PHP:  exit(1);
来源：http://hz.hnxiangtu.top/gtqldnjlow.html

JS:   process.exit(1)
来源：http://hz.zhengqikj.top/gtngykoeuo.html

TS:   process.exit(1)
来源：http://hz.yuxming.cn/gtopsfcddg.html

Java: System.exit(1)
来源：http://hz.jinghuilouyu.cn/gtaokjqrmz.html

Go:   os.Exit(1)
来源：http://hz.jinqigfzy.top/gtvvqeixzt.html

Ruby: exit 1
来源：http://hz.chenlongwang.top/gtzpcrocea.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.jianghu66.top/gtfzoihbnk.html

[M06] 向标准错误输出
来源：http://hz.ywan-chungtsiang.top/gtxhztxpmo.html

Py:   print("err", file=sys.stderr)
来源：http://hz.fengsongda.top/gtaktsfzkq.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.cqqwz.cn/gtklefnshy.html

JS:   console.error("err")
来源：http://hz.yuanzhike.top/gtxqjfvhrp.html

TS:   console.error("err")
来源：http://hz.jinyuanbaomall.cn/gtufnweylx.html

Java: System.err.println("err")
来源：http://hz.52xcode.cn/gtrckspwal.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.hongshengwenyu.top/gtzgiszqad.html

Ruby: warn "err"
来源：http://hz.ybcxt.top/gtwscqoguv.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.ydjk.org.cn/gtwmjdjabo.html

[M07] 判断是否为主入口
来源：http://hz.bjfxy.top/gtsrtcbmef.html

Py:   if __name__ == "__main__":
来源：http://hz.dianchejie.cn/gtjhhubqxb.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.tian-w.cn/gtdgoktjcs.html

JS:   require.main === module
来源：http://hz.hnqzz.top/gtwzeyrloe.html

TS:   require.main === module
来源：http://hz.ehwqpu.com/gtbtiyrvgn.html

Java: public static void main(String[] args)
来源：http://hz.yueranfly.top/gtllcpeulx.html

Go:   func main()
来源：http://hz.shanyushiyangkeji.top/gtxhossscm.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.yuanzhike.top/gtpqkxgmfv.html

C#:   static void Main(string[] args)
来源：http://hz.guowangkeji.top/gtvbbvzuly.html

[M08] 获取系统与运行时信息
来源：http://hz.hammf.cn/gtjfbrtfsn.html

Py:   platform.system();  platform.python_version()
来源：http://hz.chenjidiqi.icu/gttojfupcv.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.chenzaomai.com/gtzidkbgrm.html

JS:   process.platform;  process.version
来源：http://hz.jinqigfzy.top/gtnatedadn.html

TS:   process.platform;  process.version
来源：http://hz.xziqi.cn/gtklvzifoo.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.yangfankeji.com/gtanqwzmoe.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.sufxvd.cn/gtjwokfnli.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.shzxlz.cn/gtfvigurmi.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.zhoulong.xyz/gtbzkizaea.html

================================================================================
来源：http://hz.yangfankeji.com/gtfnbakvwm.html

N. 数据结构与算法
来源：http://hz.aibaodan.cn/gtxafywbfu.html

================================================================================
来源：http://hz.cheryme.top/gtctlorfxk.html

[N01] 二分查找（有序数组）
来源：http://hz.svipenyu.cn/gtrcqpcpbq.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.jqgufenzy.top/gtyjsiydok.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.yj20258888.top/gtznuewfvv.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.xylfe.cn/gtirotqzpe.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.chenjidiqi.icu/gtgwrscwwh.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.kuanghao11.cn/gtabkxvgef.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.ivvv.top/gthfxulitx.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.jqgufenzy.top/gtqcxpghtt.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.yj20258888.top/gtqhtqoxfu.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.tianlin.xyz/gtlmpjafbg.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.andypj.xyz/gtyqmzuslm.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.ydjk.org.cn/gtagfrhrgo.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jinghuilouyu.cn/gtnotmbmzf.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.zhongyouzk.top/gttndhwvhv.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.guowangkeji.top/gtbqincsjj.html

Go:   slices.Sort(arr)
来源：http://hz.hysaishi.cn/gtvughnyqa.html

Ruby: arr.sort
来源：http://hz.yvedp.cn/gtphsjabfd.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.dashuyun.cn/gtvtnvzsjx.html

[N03] 快速排序（分治示例）
来源：http://hz.hammf.cn/gtpkznobkx.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.xinyue.icu/gtnwpnrbkr.html

PHP:  // 递归实现，或用 usort
来源：http://hz.gotoacloud.top/gtfwmyuedn.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.ppjwa.cn/gtrhizfjhj.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.redwolf501.top/gtmpvglyfy.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.cdnleiting.top/gttnstdjls.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.aizwys.cn/gtgkfxhqdj.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.sysykeji.top/gtwzrcjvqr.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.birdmap.top/gtvfkqamcj.html

[N04] 斐波那契数列
来源：http://hz.smart0.xyz/gtwxkgeisk.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.fzhhl.top/gtnnqbksjh.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.zhixingplan.top/gtryfiiahb.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.feifeiyinyue.top/gtnspbjaha.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jqgfzy.top/gtkonpebpp.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.dashuyun.cn/gtserdbaii.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.cashguo.top/gtqukasbbo.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.9152youxi.cn/gtqjmvmjgf.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.jinqigfzy.top/gtxlyexfkk.html

[N05] 最大公约数
来源：http://hz.redwolf501.top/gtuyuwgfad.html

Py:   math.gcd(a, b)
来源：http://hz.xingfuxueyuan.xyz/gtdavljcgu.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.daria6918.cn/gtfecqhhpj.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.chenlongwang.top/gtopvvzryn.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jqgfzy.top/gtvxseopdn.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.sweek.top/gtaaddvonk.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.zhoulong.xyz/gttffovgen.html

Ruby: a.gcd(b)
来源：http://hz.ydjk.org.cn/gtkqvgdudf.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.yvedp.cn/gtixyaucev.html

[N06] 判断回文字符串
来源：http://hz.chenlongwang.top/gtrthtiaiv.html

Py:   s == s[::-1]
来源：http://hz.daxiang520.top/gtgayewrdy.html

PHP:  $s === strrev($s);
来源：http://hz.zdqjudy.top/gtnnmbrpvj.html

JS:   s === [...s].reverse().join("")
来源：http://hz.xziqi.cn/gtmvgkcvqe.html

TS:   s === [...s].reverse().join("")
来源：http://hz.zhixingplan.top/gtkmlopooo.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.iojbl.cn/gtbknbswjj.html

Go:   // 双指针从两端比较
来源：http://hz.hongshengwenyu.top/gtciyjeuds.html

Ruby: s == s.reverse
来源：http://hz.52xcode.cn/gtgufovhtq.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.316326.xyz/gtiyqrvwgy.html

[N07] 两数之和（返回下标）
来源：http://hz.ybcxt.top/gtbwigxpsw.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.cashguo.top/gteryzwlpn.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.smart0.xyz/gtfiqbofyl.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.shzxlz.cn/gtpcthztks.html

TS:   // 手写 Map<string, number>
来源：http://hz.ehwqpu.com/gttvuzuezq.html

Java: // 手写 HashMap
来源：http://hz.kuanghao11.cn/gtcnigiqyd.html

Go:   // 手写 map[int]int
来源：http://hz.dashuyun.cn/gtvuhqrlum.html

Ruby: // 手写 Hash
来源：http://hz.aizwys.cn/gtxeofssvr.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.guowangkeji.top/gtatnmawmm.html

[N08] 生成全排列
来源：http://hz.yj202588.top/gtmzshrxct.html

Py:   itertools.permutations(arr)
来源：http://hz.snrcjt.cn/gtmbcayksb.html

PHP:  // 手写递归交换
来源：http://hz.jinqigfzy.top/gthzbgzcpq.html

JS:   // 手写回溯递归
来源：http://hz.cheryme.top/gtqhqizoam.html

TS:   // 手写回溯递归
来源：http://hz.dashuyun.cn/gtpvcbbsew.html

Java: // 手写回溯递归
来源：http://hz.chenjidiqi.icu/gtwocggszc.html

Go:   // 手写回溯递归
来源：http://hz.yongpay.top/gtxcgwutpc.html

Ruby: arr.permutation.to_a
来源：http://hz.hammf.cn/gtuqdjbtru.html

C#:   // 手写回溯递归
来源：http://hz.meibo888.top/gtftbxjnmr.html

[N09] 栈与队列
来源：http://hz.cashguo.top/gtemqujhsr.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.wangdashe.top/gtgwbhbudd.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.jianghu66.top/gtlzfnmkdb.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.aibaodan.cn/gtjibkjmgg.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.pycfn.com/gtnjktiahs.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.sxryk.cn/gthxuvgxfc.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.c1oappe.top/gtbpxsarun.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.yuanzhike.top/gtymzocspl.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.shanyushiyangkeji.top/gtbolhtfwo.html

[N10] 链表节点定义
来源：http://hz.cdnleiting.top/gtpowfnguw.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.zdqjudy.top/gtlyqzyhos.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.jinqigufen.top/gtwkysfzkx.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.jianghu66.top/gtfkjnpwjz.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.hnxiangtu.top/gtkwngvotn.html

Java: class Node { int v; Node next; }
来源：http://hz.yuxming.cn/gtmojrxlpj.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.aibaodan.cn/gtwlcdemwm.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.jqgfzy.top/gtnabzntsj.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.shanyushiyangkeji.top/gtylpiftmr.html

[N11] 二叉树中序遍历
来源：http://hz.zhengqikj.top/gtboxwecte.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.zdqjudy.top/gtzywvtasb.html

PHP:  // 手写递归函数
来源：http://hz.daxiang520.top/gtmdwotyor.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.redwolf501.top/gtjpwaqllu.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yongpay.top/gtcxlsgwma.html

Java: // 手写递归
来源：http://hz.dianchejie.cn/gtvgnfixer.html

Go:   // 手写递归
来源：http://hz.yj20258888.top/gtikojhblo.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.sweek.top/gtjvnxyspm.html

C#:   // 手写递归
来源：http://hz.jyoumei.cn/gtdyquorwc.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.fzhhl.top/gtqughnmer.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.yanxiufei.cn/gtzzmymovt.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.shzxlz.cn/gttaktwxgp.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.aizwys.cn/gtxhxwzzmk.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jyoumei.cn/gtzodabqju.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.zdqjudy.top/gttlxhndmb.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.jyoumei.cn/gtzloqyiud.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.hysaishi.cn/gtylzfpgfi.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.zhixingplan.top/gtwnbfcwtc.html

================================================================================
来源：http://hz.jianghu66.top/gtxrjhuydh.html

O. 并发与异步
来源：http://hz.ywan-chungtsiang.top/gtitgdjaqb.html

================================================================================
来源：http://hz.cdnleiting.top/gttnmqtdeg.html

[O01] 启动一个线程
来源：http://hz.c1oappe.top/gtrrfsgvsw.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.feifeiyinyue.top/gtzdranhok.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.aizwys.cn/gtszsotoil.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.dashuyun.cn/gtdngouvnh.html

TS:   // 同 JS
来源：http://hz.yueranfly.top/gtlqeftxyx.html

Java: new Thread(() -> f()).start()
来源：http://hz.vqdsnc.cn/gtohwwuvto.html

Go:   go f()
来源：http://hz.zhongyouzk.top/gtowimtgvp.html

Ruby: Thread.new { f }
来源：http://hz.andypj.xyz/gtzhoforgl.html

C#:   Task.Run(() => F());
来源：http://hz.feifeiyinyue.top/gtftwqnltk.html


<!-- 参考信息 -->