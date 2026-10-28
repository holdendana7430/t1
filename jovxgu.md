代发 wailian999

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.zhongyouzk.top/gtlbopcfbi.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.pengpengdd.cyou/gtviczomuu.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.shuidangran.top/gtsqpsxyvi.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.shanyushiyangkeji.top/gtmahtzqif.html

[K06] 解析 URL 查询串
来源：http://hz.redwolf501.top/gthggjkurj.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.tian-w.cn/gttfsjyggv.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.yuanzhike.top/gtlxklugvw.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.nwbrower.top/gthbfrlsya.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jinqigfzy.top/gtbzbvgaay.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.jqgufenzy.top/gtjnxunljr.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.yvedp.cn/gtfaexddmh.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.jinqigufen.top/gtkgctbgtz.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.andypj.xyz/gtymgkchal.html

[K07] 进制转换
来源：http://hz.9152youxi.cn/gtizahcbtx.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.hongshengwenyu.top/gtxtmlocgh.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.sysykeji.top/gtsqoebmmw.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.xuetiantiany.cn/gtbadherbv.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.hysaishi.cn/gtvueyqyhn.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.cucudq.cn/gtymbeheqk.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.iojbl.cn/gtxmvrdovp.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.yangfankeji.com/gtoldlewbb.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.zhongyouzk.top/gtdzqcfcyo.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.shanyushiyangkeji.top/gtdkumvnyd.html

Py:   pickle.dumps(obj)
来源：http://hz.chenlongwang.top/gtzzwxiitx.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.svipenyu.cn/gtbgvyncgj.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.zhiwuduotai.top/gtzadetvby.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.jyoumei.cn/gtsslypfqw.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.zhiwuduotai.top/gtdfynkqpa.html

Go:   encoding/gob
来源：http://hz.xingfuxueyuan.xyz/gttkqlfsbp.html

Ruby: Marshal.dump(obj)
来源：http://hz.jqgfzy.top/gtdmyfvvxk.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.birdmap.top/gtxhpbiery.html

================================================================================
来源：http://hz.aizwys.cn/gtxnvqfoau.html

L. 网络请求
来源：http://hz.hnqzz.top/gtlmngvlar.html

================================================================================
来源：http://hz.tianlin.xyz/gtxdphwajo.html

[L01] 发送 GET 请求
来源：http://hz.tianlin.xyz/gtffgshiho.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.quarkkingdee.top/gtnkuqmfsk.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.0kj1m.cn/gteewjhtaj.html

JS:   await fetch(url)
来源：http://hz.jinyuanbaomall.cn/gtbvzcfrgu.html

TS:   await fetch(url)
来源：http://hz.sxryk.cn/gtvkdywrvv.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.ehwqpu.com/gtecbbppsb.html

Go:   resp, err := http.Get(url)
来源：http://hz.hfpthk.cn/gtciwnpfcr.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.vqdsnc.cn/gtbzblqimr.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.fzhhl.top/gtshxvsxaz.html

[L02] 发送 POST JSON
来源：http://hz.gzhubu.top/gtwkxncwhc.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.sysykeji.top/gtdvkaucdn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.jlsjyb.cn/gtqikeufao.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.shanyushiyangkeji.top/gtnsxkwugd.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jianghu66.top/gtnonksgxt.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.nwbrower.top/gtimsenfwg.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.ydzc1.top/gtbrzuwoib.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.shuidangran.top/gticxaszjl.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.snrcjt.cn/gtfkpnmufj.html

[L03] 设置自定义请求头
来源：http://hz.9152youxi.cn/gtiwclbwtu.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.xinyue.icu/gtqgurvnzl.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.yueranfly.top/gtpgxrpxyx.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.vqdsnc.cn/gtbygtqtxf.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.kuanghao11.cn/gtrssqmmoe.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.sufxvd.cn/gttvtpudyf.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.zycfv.cn/gtfqkffgwi.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.birdmap.top/gtthaxxhqv.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.jinqigfzy.top/gtcjujfrqf.html

[L04] 设置超时
来源：http://hz.hnxiangtu.top/gtlbeoffqo.html

Py:   requests.get(url, timeout=5)
来源：http://hz.yonumen.top/gtgemxrzvq.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.cdnleiting.top/gtovoyroyo.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.guowangkeji.top/gtougymrgi.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.meibo888.top/gtvuhcoxxb.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.snrcjt.cn/gtcczwgzai.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.jianghu66.top/gtnwjrzizn.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.jinqigfzy.top/gtwcswtpof.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.c1oappe.top/gtoimhxtit.html

[L05] 上传文件（multipart）
来源：http://hz.xingfuxueyuan.xyz/gtuvdgsjan.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.yanxiufei.cn/gtrhtofugu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.dashuyun.cn/gtnzduyidc.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.tianlin.xyz/gtzznhtsxp.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.daria6918.cn/gtszllpmox.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.quarkkingdee.top/gtcksylsbi.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.jyoumei.cn/gtsocgfsjb.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.haohaochexian.top/gtgwlyxbyv.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.yvedp.cn/gtiqhpzeyb.html

[L06] 解析响应为 JSON
来源：http://hz.hammf.cn/gtcrwnczkm.html

Py:   resp.json()
来源：http://hz.shuidangran.top/gtgmcszdsu.html

PHP:  json_decode($body, true);
来源：http://hz.aizwys.cn/gtkjwzjmup.html

JS:   await resp.json()
来源：http://hz.shanyushiyangtech.top/gttyhfozrr.html

TS:   await resp.json()
来源：http://hz.vqdsnc.cn/gtodkbrnas.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.shangyingyoupin.top/gtgczhvukt.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.jqgfzy.top/gtinazzggn.html

Ruby: JSON.parse(resp.body)
来源：http://hz.tian-w.cn/gtkthjoftp.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.jinqigufen.top/gtswecqgvv.html

[L07] 处理 HTTP 状态码
来源：http://hz.nanxuanxn.top/gtcrbbjnqm.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.aizwys.cn/gtxhojnhfe.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.zycfv.cn/gtyigdjcsl.html

JS:   resp.ok;  resp.status
来源：http://hz.yuanzhike.top/gttittsdpo.html

TS:   resp.ok;  resp.status
来源：http://hz.gzhubu.top/gtizhgagcx.html

Java: resp.statusCode()
来源：http://hz.mhx1999.top/gtxoskaisj.html

Go:   resp.StatusCode
来源：http://hz.9152youxi.cn/gtsailqrle.html

Ruby: resp.code.to_i
来源：http://hz.jinqigfzy.top/gtlpqojgmq.html

C#:   (int)resp.StatusCode
来源：http://hz.0kj1m.cn/gtglvzifgg.html

[L08] 并发请求多个地址
来源：http://hz.wangdashe.top/gtvglwarmv.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.zhongyouzk.top/gtdvvxhxkl.html

PHP:  curl_multi_init() 系列
来源：http://hz.quarkkingdee.top/gtsbcoisga.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.xingfuxueyuan.xyz/gtcrisopjq.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.fengsongda.top/gtaccuqbev.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.ybcxt.top/gtvurkbgcl.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.iojbl.cn/gtbyudxume.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.xuanzx.com/gtpgpbsoen.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.nanxuanxn.top/gtdrilkywb.html

================================================================================
来源：http://hz.9152youxi.cn/gtraulydgj.html

M. 命令行 / 进程 / 环境
来源：http://hz.jiagoushi.top/gtztqgoegy.html

================================================================================
来源：http://hz.kuanghao11.cn/gtgdvkwmnf.html

[M01] 读取命令行参数
来源：http://hz.sxryk.cn/gthgxgofwb.html

Py:   sys.argv[1:]
来源：http://hz.xylfe.cn/gtvtdgamrr.html

PHP:  $argv;  $argc;
来源：http://hz.yj202588.top/gtkhrztkjc.html

JS:   process.argv.slice(2)
来源：http://hz.hywenlv.cn/gtiwhrlwjn.html

TS:   process.argv.slice(2)
来源：http://hz.dianchejie.cn/gtfbhzucuv.html

Java: args 数组（main 方法参数）
来源：http://hz.jyoumei.cn/gtqekbemag.html

Go:   os.Args[1:]
来源：http://hz.yonumen.top/gtaivxudnz.html

Ruby: ARGV
来源：http://hz.cashguo.top/gtdxywymsd.html

C#:   args 数组（Main 方法参数）
来源：http://hz.cdnleiting.top/gtbbighuxv.html

[M02] 读取环境变量
来源：http://hz.wangdashe.top/gtieyyvfse.html

Py:   os.environ.get("HOME")
来源：http://hz.pycfn.com/gtmwhdcmhx.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.jinyuanbaomall.cn/gtcubnxpkr.html

JS:   process.env.HOME
来源：http://hz.ywan-chungtsiang.top/gtygbfmgte.html

TS:   process.env.HOME
来源：http://hz.jianghu66.top/gtmybujsgf.html

Java: System.getenv("HOME")
来源：http://hz.shuidangran.top/gtzorwjihl.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.zhaomingkeji.xyz/gtnkjajjkr.html

Ruby: ENV["HOME"]
来源：http://hz.jqgufenzy.top/gtehqpigkm.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.jqgufenzy.top/gtgmzkmoic.html

[M03] 执行外部命令
来源：http://hz.wangshuangyany.cn/gtwfojtqed.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.ywan-chungtsiang.top/gtaitekdgn.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.xingfuxueyuan.xyz/gtbkvftbnz.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.kuanghao11.cn/gthnviaqzi.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.shuidangran.top/gtkhuqpymv.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.aizwys.cn/gtyuwglwsm.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.c1oappe.top/gtrloqynas.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.316326.xyz/gtxvlgbgey.html

C#:   Process.Start("ls", "-l");
来源：http://hz.yueranfly.top/gtbhjhkufn.html

[M04] 获取当前工作目录
来源：http://hz.guowangkeji.top/gtliwrzriu.html

Py:   os.getcwd()
来源：http://hz.xziqi.cn/gthlbeeoek.html

PHP:  getcwd();
来源：http://hz.xziqi.cn/gtmjahnnxv.html

JS:   process.cwd()
来源：http://hz.ywan-chungtsiang.top/gtysloeclr.html

TS:   process.cwd()
来源：http://hz.yongpay.top/gtuqfeshgj.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.tanke756.top/gtgxxiqhzf.html

Go:   os.Getwd()
来源：http://hz.redwolf501.top/gtrgnubvbc.html

Ruby: Dir.pwd
来源：http://hz.yuxming.cn/gtrmciuwol.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.zhaomingkeji.xyz/gtmiglwqxn.html

[M05] 设置退出码
来源：http://hz.sxryk.cn/gtigjizjfh.html

Py:   sys.exit(1)
来源：http://hz.c1oappe.top/gthwydbuqk.html

PHP:  exit(1);
来源：http://hz.ydzc1.top/gtyslueata.html

JS:   process.exit(1)
来源：http://hz.mhx1999.top/gtqknlwkaq.html

TS:   process.exit(1)
来源：http://hz.havefunace.top/gtihvuzbab.html

Java: System.exit(1)
来源：http://hz.jianghu66.top/gtxkvifeye.html

Go:   os.Exit(1)
来源：http://hz.hnqzz.top/gtiradkiyt.html

Ruby: exit 1
来源：http://hz.daria6918.cn/gtnaxdxmwq.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.tian-w.cn/gthwsbvrzr.html

[M06] 向标准错误输出
来源：http://hz.snrcjt.cn/gtuzhtoehh.html

Py:   print("err", file=sys.stderr)
来源：http://hz.wangdashe.top/gttadogeai.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.ppjwa.cn/gtbgiesbpn.html

JS:   console.error("err")
来源：http://hz.svipenyu.cn/gtotnszohi.html

TS:   console.error("err")
来源：http://hz.chenzaomai.com/gtnykyszpj.html

Java: System.err.println("err")
来源：http://hz.jinyuanbaomall.cn/gtkaupxxxq.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.yonumen.top/gttlxqenti.html

Ruby: warn "err"
来源：http://hz.zdqjudy.top/gtftqwzxqh.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.aizwys.cn/gtwmxtmytp.html

[M07] 判断是否为主入口
来源：http://hz.tian-w.cn/gttbyzgtxx.html

Py:   if __name__ == "__main__":
来源：http://hz.pengpengdd.cyou/gtsnlitdfx.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.ehwqpu.com/gteaeycnmb.html

JS:   require.main === module
来源：http://hz.chenjidiqi.icu/gtpkzbuafi.html

TS:   require.main === module
来源：http://hz.yuanzhike.top/gtijdasnzk.html

Java: public static void main(String[] args)
来源：http://hz.ydjk.org.cn/gtwqziksoa.html

Go:   func main()
来源：http://hz.daria6918.cn/gtxbihzhre.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.snrcjt.cn/gtwxupndrw.html

C#:   static void Main(string[] args)
来源：http://hz.zhengqikj.top/gtxvtajqep.html

[M08] 获取系统与运行时信息
来源：http://hz.aizwys.cn/gtktgpwmhz.html

Py:   platform.system();  platform.python_version()
来源：http://hz.gaohongyu789.top/gtpnstrbvj.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.hammf.cn/gtqinumzot.html

JS:   process.platform;  process.version
来源：http://hz.dianchejie.cn/gtgxjvnsiy.html

TS:   process.platform;  process.version
来源：http://hz.jinqigufen.top/gtswhkaxtl.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.yangfankeji.com/gtloqemtxg.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.tanke756.top/gtculshgwi.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.jlsjyb.cn/gtwmkdcdkd.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.ywan-chungtsiang.top/gteuwpcxec.html

================================================================================
来源：http://hz.cdnleiting.top/gtodlpkflj.html

N. 数据结构与算法
来源：http://hz.zhixingplan.top/gtwisixabt.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtlcknuksy.html

[N01] 二分查找（有序数组）
来源：http://hz.hammf.cn/gtlslcfzeq.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.zhengqikj.top/gtetfzmfha.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.ydjk.org.cn/gtajnkylar.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.shzxlz.cn/gttkjusunh.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.kuanghao11.cn/gtcwtebymu.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.chenjidiqi.icu/gtwlhtqfib.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.haohaochexian.top/gtqvxbmdcu.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.nanxuanxn.top/gtpkoupzzl.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.zhiwuduotai.top/gtrgqysypj.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.vqdsnc.cn/gtnmyeadjm.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.andypj.xyz/gtzyqmhtnw.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.hywenlv.cn/gtztvigqsr.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.ydzc1.top/gtcogeuhin.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.guowangkeji.top/gtubegilzn.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.gogol.net.cn/gtpyrkioas.html

Go:   slices.Sort(arr)
来源：http://hz.xinyue.icu/gtxnvvsyzg.html

Ruby: arr.sort
来源：http://hz.yonumen.top/gtslleobqi.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.ehwqpu.com/gtgnaetuoh.html

[N03] 快速排序（分治示例）
来源：http://hz.cucudq.cn/gtkqujfnig.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.xinyue.icu/gtzyhyoopo.html

PHP:  // 递归实现，或用 usort
来源：http://hz.guowangkeji.top/gtncdaqwdy.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.9152youxi.cn/gtoshrpwop.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.chenjidiqi.icu/gttrmmmqxn.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.yongpay.top/gtyhfkbplr.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.cucudq.cn/gtvuairaxr.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.yj202588.top/gtrtdageim.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.jinghuilouyu.cn/gtwkwmdego.html

[N04] 斐波那契数列
来源：http://hz.ydjk.org.cn/gttmnqsjsx.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.tianlin.xyz/gttmqxlwxk.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.nanxuanxn.top/gtqdubbljw.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.hongshengwenyu.top/gtrnqlpsih.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.iojbl.cn/gtjnermfdo.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.gaohongyu789.top/gtlewhvtpl.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.chenzaomai.com/gtddchhgwf.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.gaohongyu789.top/gthuuqoonc.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.xylfe.cn/gtokjszljt.html

[N05] 最大公约数
来源：http://hz.birdmap.top/gtoeyjytkw.html

Py:   math.gcd(a, b)
来源：http://hz.ppjwa.cn/gtsmubeoqw.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.tianlin.xyz/gthhbnjavs.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.wangdashe.top/gtrwndxoxc.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.shanyushiyangkeji.top/gtrwmjpjuh.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.xylfe.cn/gtbyznghyj.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.316326.xyz/gttgkhvufm.html

Ruby: a.gcd(b)
来源：http://hz.birdmap.top/gtgntxeank.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.52xcode.cn/gtytdqoxkp.html

[N06] 判断回文字符串
来源：http://hz.ehwqpu.com/gtpxpabuvp.html

Py:   s == s[::-1]
来源：http://hz.jiagoushi.top/gtbfqepbxn.html

PHP:  $s === strrev($s);
来源：http://hz.andypj.xyz/gtsntjzpax.html

JS:   s === [...s].reverse().join("")
来源：http://hz.zhengqikj.top/gtdndwxlbp.html

TS:   s === [...s].reverse().join("")
来源：http://hz.guowangkeji.top/gtvgnazyws.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.jqgfzy.top/gtqnbkrfyt.html

Go:   // 双指针从两端比较
来源：http://hz.svipenyu.cn/gtdqwgdbec.html

Ruby: s == s.reverse
来源：http://hz.ywan-chungtsiang.top/gtmecxqpjt.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.snrcjt.cn/gtkhhkszly.html

[N07] 两数之和（返回下标）
来源：http://hz.quarkkingdee.top/gtehodmmgj.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.xingfuxueyuan.xyz/gtctfxesbd.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.jlsjyb.cn/gtfouvvucf.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.gaohongyu789.top/gtxtbitxnu.html

TS:   // 手写 Map<string, number>
来源：http://hz.smart0.xyz/gtpndwnrbp.html

Java: // 手写 HashMap
来源：http://hz.sxryk.cn/gtfmjfxxyo.html

Go:   // 手写 map[int]int
来源：http://hz.yuanzhike.top/gtrtprmjyg.html

Ruby: // 手写 Hash
来源：http://hz.ppjwa.cn/gtccpnckjv.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.tanke756.top/gtbiyutxsr.html

[N08] 生成全排列
来源：http://hz.aibaodan.cn/gtlgdujpvq.html

Py:   itertools.permutations(arr)
来源：http://hz.dianchejie.cn/gtbddvvnjm.html

PHP:  // 手写递归交换
来源：http://hz.gaohongyu789.top/gthrepcsfc.html

JS:   // 手写回溯递归
来源：http://hz.chenjidiqi.icu/gttkrprthj.html

TS:   // 手写回溯递归
来源：http://hz.gzhubu.top/gthctzivpz.html

Java: // 手写回溯递归
来源：http://hz.jinyuanbaomall.cn/gtvzrkqkry.html

Go:   // 手写回溯递归
来源：http://hz.wangshuangyany.cn/gtbdnigkia.html

Ruby: arr.permutation.to_a
来源：http://hz.snrcjt.cn/gtilaultbq.html

C#:   // 手写回溯递归
来源：http://hz.chenzaomai.com/gthyrgdbbw.html

[N09] 栈与队列
来源：http://hz.nanxuanxn.top/gtkzrgnbkg.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.cucudq.cn/gtvsacrgkj.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.yuanzhike.top/gtwevlpyit.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.smart0.xyz/gtmzbmzrad.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.bjfxy.top/gtccreqlzt.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.meibo888.top/gtanipbdgg.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.sufxvd.cn/gtoveonkjf.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.yuxming.cn/gtijvvmzuw.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.redwolf501.top/gtqkbfpkyk.html

[N10] 链表节点定义
来源：http://hz.feifeiyinyue.top/gtcxotwxcg.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.chenzaomai.com/gtdudcutpf.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.yueranfly.top/gtqvwtsmuj.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.9152youxi.cn/gtvqypjjxc.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.nwbrower.top/gtrbdxeqhj.html

Java: class Node { int v; Node next; }
来源：http://hz.ivvv.top/gtrlwbcdev.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.feifeiyinyue.top/gtnqmwglyk.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.snrcjt.cn/gtsgumgiks.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.zhijiandao.cn/gtfslygiob.html

[N11] 二叉树中序遍历
来源：http://hz.guannengcc.top/gtfnasbwcc.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.daxiang520.top/gtkfgrnzbj.html

PHP:  // 手写递归函数
来源：http://hz.iojbl.cn/gtblpxsjsh.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.daria6918.cn/gtxqttdxto.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.dashuyun.cn/gtjgwbyten.html

Java: // 手写递归
来源：http://hz.iojbl.cn/gtybjvslpk.html

Go:   // 手写递归
来源：http://hz.tian-w.cn/gtmppvnopr.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.ppjwa.cn/gtpfdaboie.html

C#:   // 手写递归
来源：http://hz.zhixingplan.top/gtpnhmrcwh.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.ydzc1.top/gtjydhtmgx.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.jinghuilouyu.cn/gtiwabylym.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.shangyingyoupin.top/gtsqolrunr.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.hysaishi.cn/gtuvbpigpi.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.feifeiyinyue.top/gtydjjfman.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.shangyingyoupin.top/gtgctahchj.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.jinqigufen.top/gtiegxnion.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.aizwys.cn/gtfmqbhezs.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.jinghuilouyu.cn/gtofafggof.html

================================================================================
来源：http://hz.yanxiufei.cn/gtxzyizuap.html

O. 并发与异步
来源：http://hz.yvedp.cn/gtronxkuuu.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtegmnmgig.html

[O01] 启动一个线程
来源：http://hz.zycfv.cn/gtirtkegbb.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.nanxinkj.top/gtfmqtwhqj.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.jinqigfzy.top/gtzuapmayd.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.xziqi.cn/gtlaeosqdq.html

TS:   // 同 JS
来源：http://hz.tianlin.xyz/gtzgibamjb.html


<!-- 参考信息 -->