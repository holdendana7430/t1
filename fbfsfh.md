代发 wailian999

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.feifeiyinyue.top/gtcmgwjbzt.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.pengpengdd.cyou/gtxbgonarp.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.aibaodan.cn/gtnakktbuq.html

[K05] 深拷贝对象
来源：http://hz.jinyuanbaomall.cn/gtldoaqltz.html

Py:   copy.deepcopy(obj)
来源：http://hz.hfpthk.cn/gtspjyisyx.html

PHP:  unserialize(serialize($obj));
来源：http://hz.yueranfly.top/gtdteltezu.html

JS:   structuredClone(obj)
来源：http://hz.zhiwuduotai.top/gtcgkjfgol.html

TS:   structuredClone(obj)
来源：http://hz.yj202588.top/gthawrcsii.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.fzhhl.top/gtwejargwz.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.haohaochexian.top/gtrekipgxt.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.ybcxt.top/gtmgfbziez.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.chenjidiqi.icu/gtrbsmqmns.html

[K06] 解析 URL 查询串
来源：http://hz.dashuyun.cn/gtnmsltahw.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.zdqjudy.top/gtdslxqgha.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.xuanzx.com/gtonmmcfpx.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jqgufenzy.top/gtnnhsitla.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.sufxvd.cn/gtlcaqhruf.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.yonumen.top/gtcgknwaso.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.dianchejie.cn/gtaaxanqly.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.chenlongwang.top/gtdfcgpmew.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.shangyingyoupin.top/gthbxzzajk.html

[K07] 进制转换
来源：http://hz.iojbl.cn/gtzydelctc.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.fengsongda.top/gteddwcpcq.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.svipenyu.cn/gtltcytolo.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.hnqzz.top/gtecxdxqlg.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.gogol.net.cn/gtqaroihmr.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.hfpthk.cn/gtjxnaovoe.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.gzhubu.top/gtdlocnqzt.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.cqqwz.cn/gtieqnzcoe.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.tianlin.xyz/gtkevgketj.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.dianchejie.cn/gtsxfftgvu.html

Py:   pickle.dumps(obj)
来源：http://hz.yangfankeji.com/gtemvpxonj.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.quarkkingdee.top/gtazncycvr.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.smart0.xyz/gthavqgtgp.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.meibo888.top/gttrnhcmoy.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.fengsongda.top/gtlnilazxq.html

Go:   encoding/gob
来源：http://hz.birdmap.top/gtnfpqkxpd.html

Ruby: Marshal.dump(obj)
来源：http://hz.svipenyu.cn/gtdgxvlkta.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.52xcode.cn/gtwtpcawaq.html

================================================================================
来源：http://hz.andypj.xyz/gtpqvxexqo.html

L. 网络请求
来源：http://hz.daria6918.cn/gteoaknxct.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtvmyxpozu.html

[L01] 发送 GET 请求
来源：http://hz.jiagoushi.top/gtwkbkqknu.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.ydjk.org.cn/gtyyyrekes.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.cashguo.top/gtmopyfnlw.html

JS:   await fetch(url)
来源：http://hz.ppjwa.cn/gtlxqmktef.html

TS:   await fetch(url)
来源：http://hz.ybcxt.top/gtjwrslhbw.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.zdqjudy.top/gtchbumzwe.html

Go:   resp, err := http.Get(url)
来源：http://hz.gogol.net.cn/gtjwhogtls.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.shanyushiyangkeji.top/gtyutkuvct.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.guowangkeji.top/gtzrdydvwv.html

[L02] 发送 POST JSON
来源：http://hz.yj20258888.top/gtpdybrscd.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.zdqjudy.top/gtwjutsjcc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.cashguo.top/gtngtfvyug.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yueranfly.top/gtpyzxqdhk.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.tanke756.top/gteqthlujh.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.nwbrower.top/gtjmtajpxk.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.pengpengdd.cyou/gtirvbgofg.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.mhx1999.top/gtfnvbxmjc.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.pengpengdd.cyou/gtbmbqrdvr.html

[L03] 设置自定义请求头
来源：http://hz.daria6918.cn/gtterkrpjf.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.kuanghao11.cn/gtevrhvcag.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.jiagoushi.top/gtthtpmkgl.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.xingfuxueyuan.xyz/gtoyjhffxp.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.tanke756.top/gtbmwwtvqr.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.hongshengwenyu.top/gtfvgexign.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.nanxinkj.top/gtuvzirxvu.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.hnqzz.top/gtotcgjcfk.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.andypj.xyz/gtkutitdab.html

[L04] 设置超时
来源：http://hz.zhiwuduotai.top/gteulgvmun.html

Py:   requests.get(url, timeout=5)
来源：http://hz.smart0.xyz/gtxgsgyyyn.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.yj202588.top/gtwubvoxrg.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.c1oappe.top/gtcochpuwu.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.cucudq.cn/gtbwphnkhh.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.cdnleiting.top/gtbpixxiqh.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.hywenlv.cn/gtcuaxvgjf.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.jqgufenzy.top/gtlpfwwunx.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.ppjwa.cn/gtcwrlwbzm.html

[L05] 上传文件（multipart）
来源：http://hz.gaohongyu789.top/gtohnnskvg.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.gogol.net.cn/gtwcguilea.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.tanke756.top/gtmmczcxiu.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.yongpay.top/gtnxzkflym.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.jinyuanbaomall.cn/gtwdisgbvd.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.jinghuilouyu.cn/gtxshrcxwx.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.hnqzz.top/gthedbqfgy.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.bjfxy.top/gtmlfeutek.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.fzhhl.top/gtylywshgf.html

[L06] 解析响应为 JSON
来源：http://hz.shanyushiyangtech.top/gthzbfcfpp.html

Py:   resp.json()
来源：http://hz.yj20258.top/gtnrijxgww.html

PHP:  json_decode($body, true);
来源：http://hz.jqgfzy.top/gtrppvzord.html

JS:   await resp.json()
来源：http://hz.zdqjudy.top/gtljxkrlcx.html

TS:   await resp.json()
来源：http://hz.52xcode.cn/gtxtqlgitj.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.zhixingplan.top/gttqvdvzzp.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.shzxlz.cn/gtdvnytulz.html

Ruby: JSON.parse(resp.body)
来源：http://hz.pycfn.com/gtkwwxjfng.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.tianlin.xyz/gtqzcbluzn.html

[L07] 处理 HTTP 状态码
来源：http://hz.jqgufenzy.top/gtscyoqfvc.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.zycfv.cn/gtkxwdnvli.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.meibo888.top/gtnvztxfkx.html

JS:   resp.ok;  resp.status
来源：http://hz.xylfe.cn/gthvfktpnt.html

TS:   resp.ok;  resp.status
来源：http://hz.0kj1m.cn/gtpgkudncj.html

Java: resp.statusCode()
来源：http://hz.ppjwa.cn/gtrnjoavgo.html

Go:   resp.StatusCode
来源：http://hz.gotoacloud.top/gtklpgavru.html

Ruby: resp.code.to_i
来源：http://hz.yj20258.top/gtiuaxhihh.html

C#:   (int)resp.StatusCode
来源：http://hz.pycfn.com/gtdjgjnbwn.html

[L08] 并发请求多个地址
来源：http://hz.jyoumei.cn/gtveagiwwm.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.zhixingplan.top/gtqrjrzeyg.html

PHP:  curl_multi_init() 系列
来源：http://hz.zhiwuduotai.top/gtxiwtgbuk.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.fengsongda.top/gtvunilrnr.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zdqjudy.top/gteuusrrbh.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.xingfuxueyuan.xyz/gtvsejwowd.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.zhaomingkeji.xyz/gtueioptlm.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.9152youxi.cn/gtjarwowww.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.xinyue.icu/gtqpypxitg.html

================================================================================
来源：http://hz.chenlongwang.top/gttypgpuxu.html

M. 命令行 / 进程 / 环境
来源：http://hz.pycfn.com/gtguhopxmp.html

================================================================================
来源：http://hz.nwbrower.top/gtrhrwrqme.html

[M01] 读取命令行参数
来源：http://hz.guannengcc.top/gtjkvxnmje.html

Py:   sys.argv[1:]
来源：http://hz.dashuyun.cn/gtwbwalpir.html

PHP:  $argv;  $argc;
来源：http://hz.xziqi.cn/gtvmzuuqcw.html

JS:   process.argv.slice(2)
来源：http://hz.hongshengwenyu.top/gthahakyqo.html

TS:   process.argv.slice(2)
来源：http://hz.jinqigufen.top/gtkcwvvukz.html

Java: args 数组（main 方法参数）
来源：http://hz.ehwqpu.com/gtjoixkhdr.html

Go:   os.Args[1:]
来源：http://hz.yangfankeji.com/gtjuzamoxv.html

Ruby: ARGV
来源：http://hz.cdnleiting.top/gtlokjllot.html

C#:   args 数组（Main 方法参数）
来源：http://hz.pycfn.com/gtzkaiinwk.html

[M02] 读取环境变量
来源：http://hz.ybcxt.top/gtbluzpics.html

Py:   os.environ.get("HOME")
来源：http://hz.ybcxt.top/gtwwxzvbzp.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.cucudq.cn/gtkecubhnp.html

JS:   process.env.HOME
来源：http://hz.ivvv.top/gtvgpbpndd.html

TS:   process.env.HOME
来源：http://hz.0kj1m.cn/gtcugkkxme.html

Java: System.getenv("HOME")
来源：http://hz.svipenyu.cn/gtkpudadbj.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.meibo888.top/gtkzgtoqjc.html

Ruby: ENV["HOME"]
来源：http://hz.dashuyun.cn/gtmnifujsp.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.quarkkingdee.top/gtlsufsloq.html

[M03] 执行外部命令
来源：http://hz.shangyingyoupin.top/gtvjndwsth.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.ivvv.top/gtomhjexqm.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.shuidangran.top/gttnivcemx.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.cucudq.cn/gtttoqyiwt.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.xingfuxueyuan.xyz/gtpcrrnrwx.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.tian-w.cn/gteijjqaae.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.ydjk.org.cn/gtevphgckb.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.zhixingplan.top/gtshujyqaa.html

C#:   Process.Start("ls", "-l");
来源：http://hz.zhoulong.xyz/gtkyplbbma.html

[M04] 获取当前工作目录
来源：http://hz.wangshuangyany.cn/gtxcreurgo.html

Py:   os.getcwd()
来源：http://hz.sufxvd.cn/gtbnfovsiv.html

PHP:  getcwd();
来源：http://hz.havefunace.top/gtbsfrzwen.html

JS:   process.cwd()
来源：http://hz.havefunace.top/gtyaceeebk.html

TS:   process.cwd()
来源：http://hz.guowangkeji.top/gtavdnmwik.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.chenjidiqi.icu/gtcjrgjtei.html

Go:   os.Getwd()
来源：http://hz.zhengqikj.top/gtxnvkevpp.html

Ruby: Dir.pwd
来源：http://hz.yj20258888.top/gtwuskogdp.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.smart0.xyz/gtaiquhzrp.html

[M05] 设置退出码
来源：http://hz.ydzc1.top/gtgicueoho.html

Py:   sys.exit(1)
来源：http://hz.yvedp.cn/gtfgevfcnf.html

PHP:  exit(1);
来源：http://hz.aibaodan.cn/gtrxdrdolv.html

JS:   process.exit(1)
来源：http://hz.meibo888.top/gtlhxzcjqg.html

TS:   process.exit(1)
来源：http://hz.yonumen.top/gtxkazamhh.html

Java: System.exit(1)
来源：http://hz.hammf.cn/gtuqawtruu.html

Go:   os.Exit(1)
来源：http://hz.hysaishi.cn/gtzaunmyed.html

Ruby: exit 1
来源：http://hz.hongshengwenyu.top/gtycembzas.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.gogol.net.cn/gtogiywvwb.html

[M06] 向标准错误输出
来源：http://hz.vqdsnc.cn/gtmyingxeb.html

Py:   print("err", file=sys.stderr)
来源：http://hz.gaohongyu789.top/gtferqokzp.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.meibo888.top/gtlqtvkrol.html

JS:   console.error("err")
来源：http://hz.ivvv.top/gtqkqnjlkf.html

TS:   console.error("err")
来源：http://hz.cqqwz.cn/gtipjochpy.html

Java: System.err.println("err")
来源：http://hz.0kj1m.cn/gtwraratjz.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.yj202588.top/gtphrfchus.html

Ruby: warn "err"
来源：http://hz.zhaomingkeji.xyz/gtdkdplmtl.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.smart0.xyz/gtxhfqaymq.html

[M07] 判断是否为主入口
来源：http://hz.ivvv.top/gtebkgxxix.html

Py:   if __name__ == "__main__":
来源：http://hz.ywan-chungtsiang.top/gtexyxvhmn.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.aizwys.cn/gtdxpdicmp.html

JS:   require.main === module
来源：http://hz.shanyushiyangtech.top/gtbjmxmipo.html

TS:   require.main === module
来源：http://hz.jlsjyb.cn/gtytopvmni.html

Java: public static void main(String[] args)
来源：http://hz.wangshuangyany.cn/gtattwxqes.html

Go:   func main()
来源：http://hz.ybcxt.top/gthlejuqyt.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.jinyuanbaomall.cn/gtvqpxstel.html

C#:   static void Main(string[] args)
来源：http://hz.tanke756.top/gtguvtqwdy.html

[M08] 获取系统与运行时信息
来源：http://hz.cheryme.top/gtqlagvivw.html

Py:   platform.system();  platform.python_version()
来源：http://hz.ybcxt.top/gteumfoaun.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.yj202588.top/gtemlwkcst.html

JS:   process.platform;  process.version
来源：http://hz.guowangkeji.top/gtibfistex.html

TS:   process.platform;  process.version
来源：http://hz.52xcode.cn/gtnrvjfqsw.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.nanxuanxn.top/gtmeceakbk.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.jlsjyb.cn/gtmytgxpxv.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.hnqzz.top/gtyymoyrgw.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.jianghu66.top/gtwwcvkrka.html

================================================================================
来源：http://hz.yuxming.cn/gtsmmgsflu.html

N. 数据结构与算法
来源：http://hz.ehwqpu.com/gtitfquzri.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtboaoptao.html

[N01] 二分查找（有序数组）
来源：http://hz.quarkkingdee.top/gtcsfpqwna.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.ywan-chungtsiang.top/gtgqlifuic.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.gotoacloud.top/gtgmqgsnwq.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.haohaochexian.top/gtjzfnaqcm.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.xuetiantiany.cn/gtfwapgrqa.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.feifeiyinyue.top/gturudgcyk.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.cheryme.top/gttvnszvzw.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.52xcode.cn/gtpaufctop.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.ivvv.top/gtxwixnxjt.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.iojbl.cn/gtexcenmbw.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jinyuanbaomall.cn/gtqwrdjjjl.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.jinghuilouyu.cn/gtxqrbujuo.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.feifeiyinyue.top/gtsgmpetps.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.bjfxy.top/gtkjdsjmwf.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.yanxiufei.cn/gtrkedzwaa.html

Go:   slices.Sort(arr)
来源：http://hz.andypj.xyz/gtserxjjgi.html

Ruby: arr.sort
来源：http://hz.feifeiyinyue.top/gtoxbcxhkd.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.meibo888.top/gtrowzgsav.html

[N03] 快速排序（分治示例）
来源：http://hz.hnxiangtu.top/gtjbeotkel.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.zhongyouzk.top/gthprxhydb.html

PHP:  // 递归实现，或用 usort
来源：http://hz.mhx1999.top/gtaqrqvgal.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yonumen.top/gtnnoealzv.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yanxiufei.cn/gtoqcltxdt.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.dashuyun.cn/gtfyxprrqb.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.nwbrower.top/gtirjsdunb.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.yuanzhike.top/gtzpzlsffo.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.kuanghao11.cn/gtvfarnmhp.html

[N04] 斐波那契数列
来源：http://hz.dashuyun.cn/gtuvgpwuhw.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.c1oappe.top/gtgnxdqanb.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.zhiwuduotai.top/gtmfquviwy.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.haohaochexian.top/gtzclqjkto.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.chenzaomai.com/gtnzvueuyc.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.tianlin.xyz/gtxevtoncp.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.9152youxi.cn/gtmwkswjwc.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.zdqjudy.top/gtdjhttgme.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.sysykeji.top/gtgwlblgeb.html

[N05] 最大公约数
来源：http://hz.gaohongyu789.top/gthafekcjs.html

Py:   math.gcd(a, b)
来源：http://hz.jinqigfzy.top/gtuaigvtpl.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.shzxlz.cn/gtikskifzy.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.ybcxt.top/gtyuwpptrl.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jianghu66.top/gtbdeleqti.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.hnxiangtu.top/gtmaeigvlz.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.cdnleiting.top/gtwbdrzxxa.html

Ruby: a.gcd(b)
来源：http://hz.zhoulong.xyz/gtevcmylua.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.cucudq.cn/gtcucrklbk.html

[N06] 判断回文字符串
来源：http://hz.jinghuilouyu.cn/gteuluvtxi.html

Py:   s == s[::-1]
来源：http://hz.cashguo.top/gtkhzoivbx.html

PHP:  $s === strrev($s);
来源：http://hz.wangdashe.top/gtedfhcyxv.html

JS:   s === [...s].reverse().join("")
来源：http://hz.cucudq.cn/gtrofsquvf.html

TS:   s === [...s].reverse().join("")
来源：http://hz.cqqwz.cn/gtzqsftgyj.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.jlsjyb.cn/gtatwwwxmj.html

Go:   // 双指针从两端比较
来源：http://hz.smart0.xyz/gtfgcwqmxp.html

Ruby: s == s.reverse
来源：http://hz.cashguo.top/gtryrscjvm.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.zhengqikj.top/gtozdadosq.html

[N07] 两数之和（返回下标）
来源：http://hz.xuanzx.com/gtlyykfady.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.hywenlv.cn/gtrprjqwyy.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.chenzaomai.com/gtjvpnaiix.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.haohaochexian.top/gtukchqmtp.html

TS:   // 手写 Map<string, number>
来源：http://hz.aibaodan.cn/gtwteyxcor.html

Java: // 手写 HashMap
来源：http://hz.cqqwz.cn/gtjeeamurx.html

Go:   // 手写 map[int]int
来源：http://hz.0kj1m.cn/gtsnmpijof.html

Ruby: // 手写 Hash
来源：http://hz.birdmap.top/gtzbwidqgd.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.chenzaomai.com/gtkjretrro.html

[N08] 生成全排列
来源：http://hz.jinqigfzy.top/gtwdmrzgjm.html

Py:   itertools.permutations(arr)
来源：http://hz.meibo888.top/gtellvgayx.html

PHP:  // 手写递归交换
来源：http://hz.xuanzx.com/gtqkeehpbk.html

JS:   // 手写回溯递归
来源：http://hz.gaohongyu789.top/gtxntmqoya.html

TS:   // 手写回溯递归
来源：http://hz.hywenlv.cn/gtoproxpco.html

Java: // 手写回溯递归
来源：http://hz.xylfe.cn/gtnmouoxtx.html

Go:   // 手写回溯递归
来源：http://hz.tanke756.top/gtyoajkyna.html

Ruby: arr.permutation.to_a
来源：http://hz.jinyuanbaomall.cn/gtcmafwbeo.html

C#:   // 手写回溯递归
来源：http://hz.nanxuanxn.top/gtortehger.html

[N09] 栈与队列
来源：http://hz.xuanzx.com/gtsvqbhrjw.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.birdmap.top/gtqhsfciti.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.ydzc1.top/gtchsslzgh.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.yuxming.cn/gtskzdgngi.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.yj202588.top/gtgqluaoiu.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.jinqigufen.top/gtftihotoe.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.jinyuanbaomall.cn/gtlunwcatb.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.yuanzhike.top/gtloyhkfqj.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.meibo888.top/gtyyqlzmhq.html

[N10] 链表节点定义
来源：http://hz.yonumen.top/gtyxdyriuz.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.jqgufenzy.top/gtrydbtsek.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.redwolf501.top/gtxtqdnlfr.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.hfpthk.cn/gtkejoiawh.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.xuanzx.com/gtlqirhynb.html

Java: class Node { int v; Node next; }
来源：http://hz.zhoulong.xyz/gtuyvzweay.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.zhixingplan.top/gtpbtosngr.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.aibaodan.cn/gtjcwfpdgp.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.fzhhl.top/gtnzmtixvd.html

[N11] 二叉树中序遍历
来源：http://hz.yj202588.top/gtsnpwstch.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.sufxvd.cn/gtkgpmncwm.html

PHP:  // 手写递归函数
来源：http://hz.zhiwuduotai.top/gtlcaivaoj.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.zhoulong.xyz/gtwzmlakuk.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.tian-w.cn/gthriredwl.html

Java: // 手写递归
来源：http://hz.jinyuanbaomall.cn/gtadexdlfn.html

Go:   // 手写递归
来源：http://hz.fzhhl.top/gtavxlmzfd.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.nwbrower.top/gthherexrt.html

C#:   // 手写递归
来源：http://hz.jlsjyb.cn/gticpghztr.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.cdnleiting.top/gtjakffafm.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.yj20258888.top/gtivenjzju.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.sweek.top/gttwkpsgip.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.cashguo.top/gtrhmbyvdk.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.zhijiandao.cn/gtdqyqzsiq.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.cdnleiting.top/gtebkvgmbo.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.hnqzz.top/gtuwjnbpkv.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.ydzc1.top/gtizkzyklq.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yuanzhike.top/gtsxtgvhhx.html


<!-- 参考信息 -->