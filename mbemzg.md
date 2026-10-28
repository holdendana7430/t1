代发 wailian999

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.zhijiandao.cn/gtwrgdffej.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.hongshengwenyu.top/gtkwyxsscw.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.dianchejie.cn/gtrxilgxxl.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.ivvv.top/gtsmqfwnin.html

[K06] 解析 URL 查询串
来源：http://hz.daria6918.cn/gthzfgyvnj.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.daxiang520.top/gttbhmimge.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.meibo888.top/gtngzlqvvf.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.fengsongda.top/gtupqavqer.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.nanxuanxn.top/gtojaffvpj.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.aibaodan.cn/gtavtfqgdu.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.zhixingplan.top/gtykjsbdtq.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.shzxlz.cn/gtoasylfsw.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.daxiang520.top/gtmppwfkjn.html

[K07] 进制转换
来源：http://hz.dianchejie.cn/gtvfeupbjo.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.zhengqikj.top/gtqdfjccpg.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.guowangkeji.top/gtrsjcluoj.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.dianchejie.cn/gtssbtnebh.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.cheryme.top/gtgdtwjuye.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.ivvv.top/gtyxpvkkrk.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.ydzc1.top/gtjnqjbgxv.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.xingfuxueyuan.xyz/gtubwumxzr.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.shangyingyoupin.top/gtgukqlzwo.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.ydzc1.top/gtjgqwwwqf.html

Py:   pickle.dumps(obj)
来源：http://hz.yueranfly.top/gtwqdcarkz.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.dashuyun.cn/gthlafoaoj.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.feifeiyinyue.top/gtgxrdnwnx.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.zhengqikj.top/gtbzmqxxuq.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.xuanzx.com/gtxjxbhixg.html

Go:   encoding/gob
来源：http://hz.havefunace.top/gtxkkgruyc.html

Ruby: Marshal.dump(obj)
来源：http://hz.hywenlv.cn/gtmzpgtstz.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.xziqi.cn/gtcdhdkfsc.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtdvxrdlgd.html

L. 网络请求
来源：http://hz.havefunace.top/gtmbfdzxqx.html

================================================================================
来源：http://hz.guannengcc.top/gtzpguhiti.html

[L01] 发送 GET 请求
来源：http://hz.fzhhl.top/gttsdjlyat.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.bjfxy.top/gtjsxfzkrc.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.zdqjudy.top/gtbhbhyask.html

JS:   await fetch(url)
来源：http://hz.pycfn.com/gtcwnxogry.html

TS:   await fetch(url)
来源：http://hz.yongpay.top/gtlrawrxvt.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.yj20258888.top/gtgrlojgvh.html

Go:   resp, err := http.Get(url)
来源：http://hz.vqdsnc.cn/gtjwifsmgj.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.smart0.xyz/gtbdwcargy.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.yj202588.top/gtugodmkzd.html

[L02] 发送 POST JSON
来源：http://hz.cqqwz.cn/gtnrsiquze.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.sweek.top/gtvjvrniku.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.cqqwz.cn/gtodzkxgnr.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.0kj1m.cn/gtngxsofaz.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.ybcxt.top/gtmewjqnjm.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.xuetiantiany.cn/gtqyyjgqno.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.sxryk.cn/gthmzouesm.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.zdqjudy.top/gtfzajcqyx.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.jyoumei.cn/gtpfdayqfv.html

[L03] 设置自定义请求头
来源：http://hz.ywan-chungtsiang.top/gtrvionmng.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.yj20258888.top/gtvhiowlju.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.yangfankeji.com/gtkjczrjef.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.guannengcc.top/gtnhxmxncr.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.tanke756.top/gtkxhtbxes.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.zycfv.cn/gtndtrfyfy.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.nanxinkj.top/gtbfnkzepp.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.ybcxt.top/gtrdopmqht.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.zhixingplan.top/gteglrghdz.html

[L04] 设置超时
来源：http://hz.cdnleiting.top/gtyqydwljf.html

Py:   requests.get(url, timeout=5)
来源：http://hz.bjfxy.top/gtfzmxrvum.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.jiagoushi.top/gtawcmaote.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.nwbrower.top/gtfxetwdoc.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.chenjidiqi.icu/gtfxonhrql.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.jinqigfzy.top/gtugkydfsp.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.yj20258888.top/gtufibkzta.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.mhx1999.top/gteciwaytc.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.aizwys.cn/gtudmomjot.html

[L05] 上传文件（multipart）
来源：http://hz.chenlongwang.top/gtfgiinour.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.zhixingplan.top/gtduprpeet.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.bjfxy.top/gtffzunwfu.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.shzxlz.cn/gtapcthopr.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.hnqzz.top/gtpzorjwxb.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.xingfuxueyuan.xyz/gtqnmxyemm.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.jinqigfzy.top/gtmlciaicr.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.zhixingplan.top/gtfkvyuxfz.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.gzhubu.top/gtfdbseybj.html

[L06] 解析响应为 JSON
来源：http://hz.aibaodan.cn/gtdpviifld.html

Py:   resp.json()
来源：http://hz.hammf.cn/gtzqldcctk.html

PHP:  json_decode($body, true);
来源：http://hz.quarkkingdee.top/gtyawckkax.html

JS:   await resp.json()
来源：http://hz.hammf.cn/gtbkyfeohj.html

TS:   await resp.json()
来源：http://hz.zhijiandao.cn/gtzlcdprhy.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.hysaishi.cn/gtnambmvzu.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.daria6918.cn/gtjxjpsftj.html

Ruby: JSON.parse(resp.body)
来源：http://hz.daria6918.cn/gtmqehwowt.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.pengpengdd.cyou/gtoxvmtlmg.html

[L07] 处理 HTTP 状态码
来源：http://hz.zdqjudy.top/gtlgadczih.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.fzhhl.top/gtvehrrszd.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.jinqigufen.top/gttvrfemdt.html

JS:   resp.ok;  resp.status
来源：http://hz.birdmap.top/gtamovlslu.html

TS:   resp.ok;  resp.status
来源：http://hz.yj20258.top/gtbnknipqo.html

Java: resp.statusCode()
来源：http://hz.cashguo.top/gtumhndmow.html

Go:   resp.StatusCode
来源：http://hz.jqgfzy.top/gtaihhcuzq.html

Ruby: resp.code.to_i
来源：http://hz.feifeiyinyue.top/gtyqvpdljy.html

C#:   (int)resp.StatusCode
来源：http://hz.dianchejie.cn/gtqfcbyfxv.html

[L08] 并发请求多个地址
来源：http://hz.pycfn.com/gtgkubpwmn.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.yuanzhike.top/gtxuowdkur.html

PHP:  curl_multi_init() 系列
来源：http://hz.xuetiantiany.cn/gtcowgdwwa.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.316326.xyz/gtmtpafnrs.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhixingplan.top/gtjlzvmhxn.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.zhengqikj.top/gttxvuecej.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.shanyushiyangtech.top/gtednselhq.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.ywan-chungtsiang.top/gtmzlontdy.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.xziqi.cn/gtmiullzov.html

================================================================================
来源：http://hz.fengsongda.top/gtfozazffw.html

M. 命令行 / 进程 / 环境
来源：http://hz.cashguo.top/gttkfajyhf.html

================================================================================
来源：http://hz.jinqigfzy.top/gtywqbluzq.html

[M01] 读取命令行参数
来源：http://hz.wangshuangyany.cn/gtfotueaty.html

Py:   sys.argv[1:]
来源：http://hz.yonumen.top/gttovujsrz.html

PHP:  $argv;  $argc;
来源：http://hz.xziqi.cn/gtzceyrayb.html

JS:   process.argv.slice(2)
来源：http://hz.cqqwz.cn/gtuepioasp.html

TS:   process.argv.slice(2)
来源：http://hz.jinqigfzy.top/gtwniucvmf.html

Java: args 数组（main 方法参数）
来源：http://hz.svipenyu.cn/gtgqumzrjr.html

Go:   os.Args[1:]
来源：http://hz.chenzaomai.com/gtayfydmch.html

Ruby: ARGV
来源：http://hz.hammf.cn/gtazkuyawc.html

C#:   args 数组（Main 方法参数）
来源：http://hz.zdqjudy.top/gtqiarqjdi.html

[M02] 读取环境变量
来源：http://hz.yangfankeji.com/gtxcmudmow.html

Py:   os.environ.get("HOME")
来源：http://hz.ydzc1.top/gtpxuqxhnu.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.mhx1999.top/gtwviyjkto.html

JS:   process.env.HOME
来源：http://hz.yj20258888.top/gtijcpfxsn.html

TS:   process.env.HOME
来源：http://hz.hysaishi.cn/gtoljoteio.html

Java: System.getenv("HOME")
来源：http://hz.zycfv.cn/gtwwesabhu.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.yueranfly.top/gtkujgqizq.html

Ruby: ENV["HOME"]
来源：http://hz.hywenlv.cn/gtyspbgddl.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.xuanzx.com/gtclfsyoza.html

[M03] 执行外部命令
来源：http://hz.xziqi.cn/gtnljbvgww.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.nanxuanxn.top/gtvrpimuji.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.svipenyu.cn/gtqbbdunlj.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.shanyushiyangtech.top/gteyfxfviz.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.316326.xyz/gtzejxvnon.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.birdmap.top/gtojmuuykv.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.redwolf501.top/gtafsonnac.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.fengsongda.top/gtspgvaeiz.html

C#:   Process.Start("ls", "-l");
来源：http://hz.hnxiangtu.top/gtkoobalwb.html

[M04] 获取当前工作目录
来源：http://hz.daxiang520.top/gtvtpxpkqw.html

Py:   os.getcwd()
来源：http://hz.zhiwuduotai.top/gtfbmbbequ.html

PHP:  getcwd();
来源：http://hz.zhiwuduotai.top/gtbaqeuefe.html

JS:   process.cwd()
来源：http://hz.ydjk.org.cn/gtniuuukzf.html

TS:   process.cwd()
来源：http://hz.feifeiyinyue.top/gtnqrgmgvx.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.jinqigfzy.top/gtelhtjksq.html

Go:   os.Getwd()
来源：http://hz.nwbrower.top/gtgtawztkw.html

Ruby: Dir.pwd
来源：http://hz.aibaodan.cn/gtjecclvgc.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.hywenlv.cn/gtsdrqswsc.html

[M05] 设置退出码
来源：http://hz.shzxlz.cn/gtixvtpfxb.html

Py:   sys.exit(1)
来源：http://hz.c1oappe.top/gtbprzrmuj.html

PHP:  exit(1);
来源：http://hz.guowangkeji.top/gthpsgqskm.html

JS:   process.exit(1)
来源：http://hz.daria6918.cn/gtkhahfsqm.html

TS:   process.exit(1)
来源：http://hz.zhengqikj.top/gtaxzsmzon.html

Java: System.exit(1)
来源：http://hz.hnxiangtu.top/gtsixmfyyp.html

Go:   os.Exit(1)
来源：http://hz.daria6918.cn/gtzbnglhll.html

Ruby: exit 1
来源：http://hz.guowangkeji.top/gtjhuenaem.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.jianghu66.top/gtdgdkzpoa.html

[M06] 向标准错误输出
来源：http://hz.yanxiufei.cn/gtltlusmxv.html

Py:   print("err", file=sys.stderr)
来源：http://hz.jinghuilouyu.cn/gtvgryacnl.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.cashguo.top/gtqwueqsya.html

JS:   console.error("err")
来源：http://hz.tianlin.xyz/gtrwbnhnpm.html

TS:   console.error("err")
来源：http://hz.zhaomingkeji.xyz/gtlsfddetg.html

Java: System.err.println("err")
来源：http://hz.gzhubu.top/gtfgufgozx.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.jiagoushi.top/gthnyatvya.html

Ruby: warn "err"
来源：http://hz.gaohongyu789.top/gtrzxexfmd.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.gogol.net.cn/gtiouccykl.html

[M07] 判断是否为主入口
来源：http://hz.wangdashe.top/gtowrjdwog.html

Py:   if __name__ == "__main__":
来源：http://hz.guowangkeji.top/gtvqezaand.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.yueranfly.top/gtylcgvwhu.html

JS:   require.main === module
来源：http://hz.dashuyun.cn/gttunkxjbn.html

TS:   require.main === module
来源：http://hz.iojbl.cn/gtxighpcdj.html

Java: public static void main(String[] args)
来源：http://hz.cheryme.top/gtotmhypso.html

Go:   func main()
来源：http://hz.52xcode.cn/gtlkpxfsnw.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.ywan-chungtsiang.top/gtxzheggub.html

C#:   static void Main(string[] args)
来源：http://hz.iojbl.cn/gtzamvkbhs.html

[M08] 获取系统与运行时信息
来源：http://hz.xuanzx.com/gtemvsgned.html

Py:   platform.system();  platform.python_version()
来源：http://hz.fzhhl.top/gtfiuotzzv.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.wangshuangyany.cn/gtofhidvmi.html

JS:   process.platform;  process.version
来源：http://hz.jqgufenzy.top/gtesdntnax.html

TS:   process.platform;  process.version
来源：http://hz.sufxvd.cn/gtrvbhgslr.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.feifeiyinyue.top/gtufqnfsai.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.ybcxt.top/gtqtlhefxw.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.jinyuanbaomall.cn/gtgfplyfca.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.yonumen.top/gtgvkyvial.html

================================================================================
来源：http://hz.hammf.cn/gtxikpzpiz.html

N. 数据结构与算法
来源：http://hz.ydjk.org.cn/gtijbtsxok.html

================================================================================
来源：http://hz.cashguo.top/gtglctfpwq.html

[N01] 二分查找（有序数组）
来源：http://hz.yj20258.top/gtpdqcqntg.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.yangfankeji.com/gtkceozgvf.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.sufxvd.cn/gtxztzlhnl.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.daria6918.cn/gtdagqfbou.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.fzhhl.top/gtndfaymqm.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.zhiwuduotai.top/gtowniiijz.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.gzhubu.top/gtzwzsrbuz.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.fengsongda.top/gtykngupkv.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.yj202588.top/gtlbfdnyey.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.wangshuangyany.cn/gttbqikltp.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.xziqi.cn/gtgfbtnfsm.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.chenlongwang.top/gtzapmbatx.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.vqdsnc.cn/gtrbzoujrh.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.quarkkingdee.top/gthdblpjpl.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.jinghuilouyu.cn/gtgaeqdfdq.html

Go:   slices.Sort(arr)
来源：http://hz.jqgufenzy.top/gtbxtmneuy.html

Ruby: arr.sort
来源：http://hz.shangyingyoupin.top/gtqfkehsat.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.ywan-chungtsiang.top/gtxwesvzwp.html

[N03] 快速排序（分治示例）
来源：http://hz.nanxinkj.top/gtlyjgobuu.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.hongshengwenyu.top/gtiquwicgj.html

PHP:  // 递归实现，或用 usort
来源：http://hz.gzhubu.top/gtoqlagzha.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jinyuanbaomall.cn/gtagzbdlnc.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.hongshengwenyu.top/gthxnixphy.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.zhongyouzk.top/gtnowlumqk.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.wangshuangyany.cn/gtjbppctwp.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.hongshengwenyu.top/gtpdtcbmmo.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.birdmap.top/gtcazursxa.html

[N04] 斐波那契数列
来源：http://hz.yj20258.top/gtfswjtayp.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.jqgufenzy.top/gtdwchxhly.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.zhongyouzk.top/gtsxcwmglq.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.svipenyu.cn/gtyhrzutpc.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.aizwys.cn/gtpbbsxazv.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.feifeiyinyue.top/gtxvbkxcjk.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.zhixingplan.top/gtikiukgoj.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.dianchejie.cn/gtpbexyotk.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.yangfankeji.com/gtrffemnsg.html

[N05] 最大公约数
来源：http://hz.feifeiyinyue.top/gtgulpyowb.html

Py:   math.gcd(a, b)
来源：http://hz.zhixingplan.top/gtnaeazhjh.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.zhongyouzk.top/gtlmrzodvr.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jinyuanbaomall.cn/gtiivaewjd.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yuxming.cn/gthfuldnjr.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.birdmap.top/gtsdwubdsm.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.aibaodan.cn/gttfjowgdf.html

Ruby: a.gcd(b)
来源：http://hz.yj20258888.top/gtgxicacuw.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.zhongyouzk.top/gtpstzxviu.html

[N06] 判断回文字符串
来源：http://hz.jianghu66.top/gtzspjzfsr.html

Py:   s == s[::-1]
来源：http://hz.mhx1999.top/gtivkupxgf.html

PHP:  $s === strrev($s);
来源：http://hz.ehwqpu.com/gtgrezxgdi.html

JS:   s === [...s].reverse().join("")
来源：http://hz.52xcode.cn/gtigbwiawf.html

TS:   s === [...s].reverse().join("")
来源：http://hz.52xcode.cn/gtfbezovyp.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.xuetiantiany.cn/gtnsmddeot.html

Go:   // 双指针从两端比较
来源：http://hz.smart0.xyz/gtbgdqysti.html

Ruby: s == s.reverse
来源：http://hz.nwbrower.top/gtfjqepnnf.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.birdmap.top/gtedpoqnfw.html

[N07] 两数之和（返回下标）
来源：http://hz.xingfuxueyuan.xyz/gttwxlwell.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.nanxinkj.top/gtumaknvai.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.yj20258888.top/gtrzeakeqd.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.xuanzx.com/gtvgubpphs.html

TS:   // 手写 Map<string, number>
来源：http://hz.dianchejie.cn/gtnsqipmnx.html

Java: // 手写 HashMap
来源：http://hz.xylfe.cn/gtcftyaimu.html

Go:   // 手写 map[int]int
来源：http://hz.jianghu66.top/gtaeelytes.html

Ruby: // 手写 Hash
来源：http://hz.svipenyu.cn/gtcawmwxad.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.cheryme.top/gtzembjmiy.html

[N08] 生成全排列
来源：http://hz.zycfv.cn/gtamgijosx.html

Py:   itertools.permutations(arr)
来源：http://hz.yj20258888.top/gtsvapmfkv.html

PHP:  // 手写递归交换
来源：http://hz.dashuyun.cn/gtpbsqliid.html

JS:   // 手写回溯递归
来源：http://hz.shuidangran.top/gtamdsvgib.html

TS:   // 手写回溯递归
来源：http://hz.c1oappe.top/gtqkjdjvqd.html

Java: // 手写回溯递归
来源：http://hz.birdmap.top/gtuhlkczuu.html

Go:   // 手写回溯递归
来源：http://hz.hfpthk.cn/gtdpgrolkt.html

Ruby: arr.permutation.to_a
来源：http://hz.tianlin.xyz/gthhtvseru.html

C#:   // 手写回溯递归
来源：http://hz.c1oappe.top/gtpkqfgaxw.html

[N09] 栈与队列
来源：http://hz.wangdashe.top/gtgnfsdboa.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.vqdsnc.cn/gtnyubmasu.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.shangyingyoupin.top/gtigexinis.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.9152youxi.cn/gttlljsmhy.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.cdnleiting.top/gtdhkusjni.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.aibaodan.cn/gtlesxibix.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.gzhubu.top/gtukcfzisk.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.52xcode.cn/gtcwoaiyfg.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.nwbrower.top/gteqdeihdk.html

[N10] 链表节点定义
来源：http://hz.jlsjyb.cn/gtrncuwvwf.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.quarkkingdee.top/gtntxrjlak.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.xziqi.cn/gteylwegam.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.quarkkingdee.top/gtxtyirrva.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.chenlongwang.top/gtszkzwjkh.html

Java: class Node { int v; Node next; }
来源：http://hz.sweek.top/gtdmbsnedi.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.hnqzz.top/gtncoqcrqa.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.fengsongda.top/gtbiuickuf.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.yuanzhike.top/gttcoajhex.html

[N11] 二叉树中序遍历
来源：http://hz.jqgfzy.top/gtksirrfxc.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.0kj1m.cn/gtsiocmulf.html

PHP:  // 手写递归函数
来源：http://hz.jianghu66.top/gtvuqkoxoq.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.tianlin.xyz/gtcztlungi.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yuxming.cn/gthkoawydw.html

Java: // 手写递归
来源：http://hz.xingfuxueyuan.xyz/gtundzqrye.html

Go:   // 手写递归
来源：http://hz.gaohongyu789.top/gtfdiemooa.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.ivvv.top/gtlbwrazfe.html

C#:   // 手写递归
来源：http://hz.yj202588.top/gtzsgluhtl.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.jinqigfzy.top/gtbuegbjwa.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.yanxiufei.cn/gtwpfbvohq.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.ywan-chungtsiang.top/gtglrmkjct.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.shanyushiyangkeji.top/gtvysgpilh.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.meibo888.top/gtdxmhaqwr.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yangfankeji.com/gtcpqcaxfe.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.guowangkeji.top/gtccxcqrrm.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.guowangkeji.top/gtulmxplto.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.cheryme.top/gtuugopgxp.html

================================================================================
来源：http://hz.zhengqikj.top/gthwiwetkx.html

O. 并发与异步
来源：http://hz.shangyingyoupin.top/gtlysrcowy.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtpdhfuvxo.html

[O01] 启动一个线程
来源：http://hz.ehwqpu.com/gtucewdspz.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.cashguo.top/gtttibgchn.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.zycfv.cn/gthsrpoyud.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.zdqjudy.top/gtsyhcboyo.html

TS:   // 同 JS
来源：http://hz.0kj1m.cn/gttspoqwsb.html


<!-- 参考信息 -->