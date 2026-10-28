代发 wailian999

Py:   copy.deepcopy(obj)
来源：http://hz.haohaochexian.top/gtnhintahp.html

PHP:  unserialize(serialize($obj));
来源：http://hz.nwbrower.top/gtcdkdjvyb.html

JS:   structuredClone(obj)
来源：http://hz.hywenlv.cn/gtzippeibh.html

TS:   structuredClone(obj)
来源：http://hz.yueranfly.top/gtlvsmerni.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.52xcode.cn/gtapvdwuwj.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.cashguo.top/gtuiwnerfh.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.wangshuangyany.cn/gtmfyirnhn.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.dianchejie.cn/gttbczjznn.html

[K06] 解析 URL 查询串
来源：http://hz.fengsongda.top/gtfriephgt.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.xingfuxueyuan.xyz/gttmojvjdl.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.0kj1m.cn/gtfnhcxwvk.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yueranfly.top/gtjcimolmt.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.chenzaomai.com/gtbnfqbwad.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.ehwqpu.com/gtjmaqyjes.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.shzxlz.cn/gtegftvows.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.yongpay.top/gtjifzpmnz.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.nanxuanxn.top/gtgwicjmur.html

[K07] 进制转换
来源：http://hz.shanyushiyangkeji.top/gtthfturhk.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.tianlin.xyz/gtsypdtefn.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.ybcxt.top/gthzikwgur.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.andypj.xyz/gtslrfqfgg.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.yj20258888.top/gtcobbkhkr.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.zhaomingkeji.xyz/gtewveosdp.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.xziqi.cn/gtscvkwdty.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.jiagoushi.top/gtpmtukojd.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.xylfe.cn/gttqbqgobx.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.tanke756.top/gtjacxpsrr.html

Py:   pickle.dumps(obj)
来源：http://hz.daria6918.cn/gtbhkiahko.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.jqgufenzy.top/gtabvketqy.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.jinqigfzy.top/gtwxzxajyv.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.andypj.xyz/gtrbmnnpps.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.nwbrower.top/gtttqcjdxp.html

Go:   encoding/gob
来源：http://hz.sufxvd.cn/gtpemvslua.html

Ruby: Marshal.dump(obj)
来源：http://hz.pengpengdd.cyou/gtlishqhfn.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.9152youxi.cn/gtkoiphgyr.html

================================================================================
来源：http://hz.yj20258888.top/gtwhhlrnep.html

L. 网络请求
来源：http://hz.andypj.xyz/gtotfgbeyk.html

================================================================================
来源：http://hz.hnxiangtu.top/gtmckmcynj.html

[L01] 发送 GET 请求
来源：http://hz.xziqi.cn/gtkdxvsjqw.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.ydzc1.top/gtvnbntqtu.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.fengsongda.top/gtdxtzbwkh.html

JS:   await fetch(url)
来源：http://hz.jqgufenzy.top/gtppvydkhp.html

TS:   await fetch(url)
来源：http://hz.c1oappe.top/gthxkcncys.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.vqdsnc.cn/gtrchhbqai.html

Go:   resp, err := http.Get(url)
来源：http://hz.shuidangran.top/gtdagfjpii.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.guannengcc.top/gtrgazbkxl.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.jianghu66.top/gtkvmymuma.html

[L02] 发送 POST JSON
来源：http://hz.hnqzz.top/gtzeqbuoke.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.daria6918.cn/gtbdswbjfx.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.hfpthk.cn/gtssulxmav.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.feifeiyinyue.top/gtqhpgdbdl.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.aizwys.cn/gtmzvextcy.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.guowangkeji.top/gtemdrazqo.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.ydjk.org.cn/gtsvrucqmw.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.yangfankeji.com/gtpzkzqnyj.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.sufxvd.cn/gthiwpanfd.html

[L03] 设置自定义请求头
来源：http://hz.haohaochexian.top/gticehltwp.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.smart0.xyz/gtmddbpcne.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.316326.xyz/gtlytwujut.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.guannengcc.top/gtlzmlivkv.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jyoumei.cn/gtfuuvonlt.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.shanyushiyangkeji.top/gtdgkbyiiz.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.hywenlv.cn/gtlgkpcrev.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.zhoulong.xyz/gtywcrnzlz.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.hnxiangtu.top/gtbzlsztfj.html

[L04] 设置超时
来源：http://hz.zdqjudy.top/gtkuafljlf.html

Py:   requests.get(url, timeout=5)
来源：http://hz.zhongyouzk.top/gtxjrodact.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.316326.xyz/gttbxctyfu.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.wangdashe.top/gtrfqvrhft.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jinyuanbaomall.cn/gtbkwrqldx.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.yangfankeji.com/gtvgvhfdip.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.jinqigfzy.top/gtoyleslpy.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.meibo888.top/gtiipncfdl.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.cucudq.cn/gtqwsfvavv.html

[L05] 上传文件（multipart）
来源：http://hz.meibo888.top/gttrgnehjt.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.shanyushiyangtech.top/gtnjrdiynf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.wangshuangyany.cn/gtlqulqyhl.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.zhiwuduotai.top/gtafqsxpke.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.chenzaomai.com/gtltrishxe.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.gzhubu.top/gtcgzlwitk.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.wangshuangyany.cn/gthuzutcsx.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.yonumen.top/gtlujsgcbw.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.tian-w.cn/gtleewwxiw.html

[L06] 解析响应为 JSON
来源：http://hz.vqdsnc.cn/gtnawcljdt.html

Py:   resp.json()
来源：http://hz.hnqzz.top/gtdqlnbunt.html

PHP:  json_decode($body, true);
来源：http://hz.guannengcc.top/gtzicctrjs.html

JS:   await resp.json()
来源：http://hz.guannengcc.top/gtzprmwbsh.html

TS:   await resp.json()
来源：http://hz.52xcode.cn/gtpgclwqwh.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.dashuyun.cn/gtuohrtvmi.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.mhx1999.top/gtgbmbtqtv.html

Ruby: JSON.parse(resp.body)
来源：http://hz.smart0.xyz/gtxvgjziaz.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.quarkkingdee.top/gtfajcjmhl.html

[L07] 处理 HTTP 状态码
来源：http://hz.redwolf501.top/gtjlovwook.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.feifeiyinyue.top/gtoasvrucr.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.yj20258.top/gtxvoknpuc.html

JS:   resp.ok;  resp.status
来源：http://hz.sysykeji.top/gtocnzcfst.html

TS:   resp.ok;  resp.status
来源：http://hz.jqgfzy.top/gtwuyhvpgq.html

Java: resp.statusCode()
来源：http://hz.jianghu66.top/gtmjydgspw.html

Go:   resp.StatusCode
来源：http://hz.gogol.net.cn/gtwnezjfjf.html

Ruby: resp.code.to_i
来源：http://hz.zhijiandao.cn/gtesgehone.html

C#:   (int)resp.StatusCode
来源：http://hz.gogol.net.cn/gtidybbsoz.html

[L08] 并发请求多个地址
来源：http://hz.zhiwuduotai.top/gtcugpgejy.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.cheryme.top/gttxdypsxx.html

PHP:  curl_multi_init() 系列
来源：http://hz.havefunace.top/gtbrummdyp.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jiagoushi.top/gtjfspqdsp.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhixingplan.top/gtodemltsc.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.pengpengdd.cyou/gtecdxrhaj.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.xziqi.cn/gtwvuakurz.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.gogol.net.cn/gtbpwzikct.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.yj20258888.top/gtxzrjxncq.html

================================================================================
来源：http://hz.zycfv.cn/gtfymiblod.html

M. 命令行 / 进程 / 环境
来源：http://hz.jqgfzy.top/gtcxnslfln.html

================================================================================
来源：http://hz.dashuyun.cn/gtwgmoelhv.html

[M01] 读取命令行参数
来源：http://hz.yj202588.top/gttdqhahwv.html

Py:   sys.argv[1:]
来源：http://hz.yonumen.top/gtwyrhagke.html

PHP:  $argv;  $argc;
来源：http://hz.sufxvd.cn/gtgdzjuxbe.html

JS:   process.argv.slice(2)
来源：http://hz.hongshengwenyu.top/gthadzcchh.html

TS:   process.argv.slice(2)
来源：http://hz.birdmap.top/gtmypcywfa.html

Java: args 数组（main 方法参数）
来源：http://hz.jlsjyb.cn/gtsafuodnu.html

Go:   os.Args[1:]
来源：http://hz.nwbrower.top/gtidsddyjk.html

Ruby: ARGV
来源：http://hz.nanxuanxn.top/gtarpsmzzx.html

C#:   args 数组（Main 方法参数）
来源：http://hz.fzhhl.top/gtfuweiyul.html

[M02] 读取环境变量
来源：http://hz.birdmap.top/gttyeavugj.html

Py:   os.environ.get("HOME")
来源：http://hz.zhiwuduotai.top/gtitlhsxpw.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.tianlin.xyz/gtmupdenkj.html

JS:   process.env.HOME
来源：http://hz.zhixingplan.top/gtzalrvutf.html

TS:   process.env.HOME
来源：http://hz.ybcxt.top/gtqauwhhpx.html

Java: System.getenv("HOME")
来源：http://hz.chenlongwang.top/gtufpeukqu.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.sufxvd.cn/gtlnkvxvoa.html

Ruby: ENV["HOME"]
来源：http://hz.hnxiangtu.top/gtakjuznas.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.wangshuangyany.cn/gtcgwsgdpz.html

[M03] 执行外部命令
来源：http://hz.quarkkingdee.top/gtnusdewwq.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.9152youxi.cn/gtrixmuznq.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.birdmap.top/gthoqdqjrx.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.haohaochexian.top/gtpoagmpvp.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.sysykeji.top/gtzhhouavh.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.9152youxi.cn/gtxpxztnfm.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.zhijiandao.cn/gtslvswjtx.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.xingfuxueyuan.xyz/gtvjvmlsyy.html

C#:   Process.Start("ls", "-l");
来源：http://hz.meibo888.top/gtutocbjfh.html

[M04] 获取当前工作目录
来源：http://hz.wangdashe.top/gtujzerkou.html

Py:   os.getcwd()
来源：http://hz.sxryk.cn/gtfyapwyqy.html

PHP:  getcwd();
来源：http://hz.zhongyouzk.top/gtpwjudzce.html

JS:   process.cwd()
来源：http://hz.jqgufenzy.top/gtlovexnvv.html

TS:   process.cwd()
来源：http://hz.iojbl.cn/gtjqiicgix.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.haohaochexian.top/gtvmqdjwqw.html

Go:   os.Getwd()
来源：http://hz.yj20258.top/gthdqufekh.html

Ruby: Dir.pwd
来源：http://hz.hfpthk.cn/gtpdnwswjn.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.vqdsnc.cn/gtbwbipnoq.html

[M05] 设置退出码
来源：http://hz.hongshengwenyu.top/gtyscmpdzx.html

Py:   sys.exit(1)
来源：http://hz.cucudq.cn/gttzyalezv.html

PHP:  exit(1);
来源：http://hz.tanke756.top/gtdqgjvqbq.html

JS:   process.exit(1)
来源：http://hz.cheryme.top/gtrfotbotw.html

TS:   process.exit(1)
来源：http://hz.cucudq.cn/gtrdgacmpv.html

Java: System.exit(1)
来源：http://hz.tian-w.cn/gtjssmcmxq.html

Go:   os.Exit(1)
来源：http://hz.zhoulong.xyz/gtbzeaopyy.html

Ruby: exit 1
来源：http://hz.yonumen.top/gttgvcbajj.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.xinyue.icu/gtnwfbrzqg.html

[M06] 向标准错误输出
来源：http://hz.tanke756.top/gtuxxdcdzg.html

Py:   print("err", file=sys.stderr)
来源：http://hz.bjfxy.top/gtedeesxfg.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.cucudq.cn/gtqsnrvhvh.html

JS:   console.error("err")
来源：http://hz.xingfuxueyuan.xyz/gtorrxppyp.html

TS:   console.error("err")
来源：http://hz.316326.xyz/gtopgoxrvu.html

Java: System.err.println("err")
来源：http://hz.jlsjyb.cn/gtwbqnitlf.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.haohaochexian.top/gtsbvhrwuq.html

Ruby: warn "err"
来源：http://hz.cqqwz.cn/gtauwowlty.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.dianchejie.cn/gtcrzoossb.html

[M07] 判断是否为主入口
来源：http://hz.ivvv.top/gtrsdihmtu.html

Py:   if __name__ == "__main__":
来源：http://hz.gzhubu.top/gtqblkoyiw.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.daxiang520.top/gtgteickwe.html

JS:   require.main === module
来源：http://hz.aibaodan.cn/gtihcnlxxp.html

TS:   require.main === module
来源：http://hz.yongpay.top/gtliugskkf.html

Java: public static void main(String[] args)
来源：http://hz.nanxuanxn.top/gtsdyudrnf.html

Go:   func main()
来源：http://hz.xuanzx.com/gtsbdzcplz.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.fzhhl.top/gtiryntxry.html

C#:   static void Main(string[] args)
来源：http://hz.wangshuangyany.cn/gtzxmfxrfw.html

[M08] 获取系统与运行时信息
来源：http://hz.gaohongyu789.top/gtykyphedj.html

Py:   platform.system();  platform.python_version()
来源：http://hz.dashuyun.cn/gtxfowpjek.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.cucudq.cn/gtslfgjvsm.html

JS:   process.platform;  process.version
来源：http://hz.xylfe.cn/gtoptqokcn.html

TS:   process.platform;  process.version
来源：http://hz.pycfn.com/gtrhtuttmx.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.cdnleiting.top/gtwywpnriz.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.redwolf501.top/gtnzrzcrpm.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.nwbrower.top/gtszecfflb.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.yonumen.top/gtauobhcls.html

================================================================================
来源：http://hz.cdnleiting.top/gtzodcatsq.html

N. 数据结构与算法
来源：http://hz.sufxvd.cn/gtqtcwnjac.html

================================================================================
来源：http://hz.kuanghao11.cn/gtikdtvkjp.html

[N01] 二分查找（有序数组）
来源：http://hz.cucudq.cn/gtdivxehxy.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.meibo888.top/gtnjyrsmph.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.jyoumei.cn/gtibikhkye.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.hywenlv.cn/gtoelgmbmy.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.aibaodan.cn/gtktbkdptu.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.aibaodan.cn/gtcbsxykvz.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.ydzc1.top/gtchctqzvm.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.ydjk.org.cn/gtfbxqiiqh.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.jiagoushi.top/gtqvyjbulc.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.cucudq.cn/gtkpabdcqg.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.nanxuanxn.top/gtinwlchsu.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.jianghu66.top/gtbvcyvnab.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.zhixingplan.top/gtqjfrxbft.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.guannengcc.top/gthobhecxi.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.tanke756.top/gtxobgebde.html

Go:   slices.Sort(arr)
来源：http://hz.xziqi.cn/gtjcecaqzq.html

Ruby: arr.sort
来源：http://hz.zhoulong.xyz/gtdxeediqj.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.xingfuxueyuan.xyz/gtofqzwpah.html

[N03] 快速排序（分治示例）
来源：http://hz.jqgfzy.top/gttxzoafbk.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.andypj.xyz/gtjrhryiuj.html

PHP:  // 递归实现，或用 usort
来源：http://hz.dashuyun.cn/gtlvbezmcs.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.chenlongwang.top/gttmhxrobe.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jqgufenzy.top/gttuchzund.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.hnqzz.top/gtuwbqfsiw.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.fengsongda.top/gtokpljcab.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.andypj.xyz/gtckbydtuq.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.xuetiantiany.cn/gtjamnxjzv.html

[N04] 斐波那契数列
来源：http://hz.snrcjt.cn/gthxxgzkov.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.yongpay.top/gtyvjxqeup.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.dianchejie.cn/gtbuqzulot.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yuxming.cn/gtjebpsrhy.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.zdqjudy.top/gtuubpzpex.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.vqdsnc.cn/gtubqfahbe.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.yj20258.top/gtkasjeoth.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.yj202588.top/gtnlzhqiph.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.hnxiangtu.top/gtfiqoyprv.html

[N05] 最大公约数
来源：http://hz.kuanghao11.cn/gtvgcvqdvp.html

Py:   math.gcd(a, b)
来源：http://hz.hfpthk.cn/gtwfihiglq.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.zhaomingkeji.xyz/gtugfyaluu.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.fzhhl.top/gtvnkkzpru.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jianghu66.top/gtzrojafsp.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.yangfankeji.com/gtagoxmwgj.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.hongshengwenyu.top/gtxefrnckm.html

Ruby: a.gcd(b)
来源：http://hz.yj20258.top/gtwkzxwqur.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.nanxuanxn.top/gtuswrotvb.html

[N06] 判断回文字符串
来源：http://hz.pengpengdd.cyou/gtfxozfdvr.html

Py:   s == s[::-1]
来源：http://hz.dianchejie.cn/gtrfiwrhal.html

PHP:  $s === strrev($s);
来源：http://hz.hfpthk.cn/gtwmsraoyo.html

JS:   s === [...s].reverse().join("")
来源：http://hz.shzxlz.cn/gtvbuoaynj.html

TS:   s === [...s].reverse().join("")
来源：http://hz.cqqwz.cn/gtyfyvrxpx.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.zhongyouzk.top/gtvzuebrgd.html

Go:   // 双指针从两端比较
来源：http://hz.yj20258.top/gttbtlwdja.html

Ruby: s == s.reverse
来源：http://hz.cheryme.top/gthdlmjand.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.hywenlv.cn/gtnpyclbvm.html

[N07] 两数之和（返回下标）
来源：http://hz.hywenlv.cn/gtidpygifh.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.haohaochexian.top/gtsztbrrbd.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.wangdashe.top/gtxswjsbcy.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.feifeiyinyue.top/gtfcbqhjvv.html

TS:   // 手写 Map<string, number>
来源：http://hz.nanxinkj.top/gtefzlalnn.html

Java: // 手写 HashMap
来源：http://hz.nanxinkj.top/gtnmezioij.html

Go:   // 手写 map[int]int
来源：http://hz.gotoacloud.top/gtvuhxgypy.html

Ruby: // 手写 Hash
来源：http://hz.zhixingplan.top/gtzbhpgleg.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.9152youxi.cn/gtcuezahkv.html

[N08] 生成全排列
来源：http://hz.jinqigfzy.top/gtugsqdchp.html

Py:   itertools.permutations(arr)
来源：http://hz.haohaochexian.top/gtpphftlzl.html

PHP:  // 手写递归交换
来源：http://hz.shuidangran.top/gtrzrpzbiw.html

JS:   // 手写回溯递归
来源：http://hz.sxryk.cn/gtxvpzgptr.html

TS:   // 手写回溯递归
来源：http://hz.9152youxi.cn/gtayzyijcc.html

Java: // 手写回溯递归
来源：http://hz.yj20258.top/gtkgmbnxjo.html

Go:   // 手写回溯递归
来源：http://hz.yongpay.top/gtjgrgpenh.html

Ruby: arr.permutation.to_a
来源：http://hz.zdqjudy.top/gtdbcnwbsi.html

C#:   // 手写回溯递归
来源：http://hz.xuanzx.com/gtejxsckbf.html

[N09] 栈与队列
来源：http://hz.zdqjudy.top/gtmtgbzcxo.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.jlsjyb.cn/gtqhtqkoks.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.birdmap.top/gtaiflhqgw.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.cashguo.top/gtntrqfsez.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.xuanzx.com/gtwfwzaoml.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.shangyingyoupin.top/gtwmjzqvnj.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.cqqwz.cn/gtdyjvnken.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.52xcode.cn/gtegzdvfhm.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.jiagoushi.top/gtgxdreqsi.html

[N10] 链表节点定义
来源：http://hz.pycfn.com/gtoynuygvf.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.chenzaomai.com/gtlnfirthp.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.redwolf501.top/gthnaeldvu.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.sysykeji.top/gteosdmmdt.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.wangdashe.top/gtactfngnh.html

Java: class Node { int v; Node next; }
来源：http://hz.havefunace.top/gtpblnkcns.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.zhixingplan.top/gtutscfxml.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.ydjk.org.cn/gteduqmtob.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.jqgfzy.top/gtxwubpbgl.html

[N11] 二叉树中序遍历
来源：http://hz.gotoacloud.top/gtlvhpehgk.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.xylfe.cn/gtlkoacjzh.html

PHP:  // 手写递归函数
来源：http://hz.ppjwa.cn/gtirrdbaia.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.hammf.cn/gtcqvsuzrt.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.daria6918.cn/gtdtnhkacm.html

Java: // 手写递归
来源：http://hz.tanke756.top/gtynjiizic.html

Go:   // 手写递归
来源：http://hz.9152youxi.cn/gtazfjuyyg.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.ivvv.top/gtngodisdd.html

C#:   // 手写递归
来源：http://hz.xziqi.cn/gtkxbvdyiy.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.hysaishi.cn/gtzuzolizl.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.cashguo.top/gtyddvxbhm.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.jqgufenzy.top/gtlqwyusvu.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jyoumei.cn/gtcyslfxmb.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.redwolf501.top/gtadxflnhp.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.jinqigufen.top/gtcazquwjn.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.zycfv.cn/gtpcuvuvou.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.yueranfly.top/gtqswnfmrs.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.feifeiyinyue.top/gtphjxqbjf.html

================================================================================
来源：http://hz.smart0.xyz/gtcdnxkwmo.html

O. 并发与异步
来源：http://hz.sxryk.cn/gtcsufgyky.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gthhpuxasl.html

[O01] 启动一个线程
来源：http://hz.ehwqpu.com/gtdtufsvbo.html


<!-- 参考信息 -->