代发 wailian999

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.cucudq.cn/gtlxcvfrqb.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jlsjyb.cn/gtuklmzsqi.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.gogol.net.cn/gtlyhfvdbu.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.hammf.cn/gttchwuwux.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.xylfe.cn/gtdpnizkpr.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.cdnleiting.top/gtqsknwvkz.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.daxiang520.top/gtyncopnvn.html

[K05] 深拷贝对象
来源：http://hz.shanyushiyangkeji.top/gtnflmdpoe.html

Py:   copy.deepcopy(obj)
来源：http://hz.fzhhl.top/gtlmxvtuoy.html

PHP:  unserialize(serialize($obj));
来源：http://hz.nwbrower.top/gtdoruehvy.html

JS:   structuredClone(obj)
来源：http://hz.c1oappe.top/gtnkcfzpgi.html

TS:   structuredClone(obj)
来源：http://hz.52xcode.cn/gtscgdwcav.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.yonumen.top/gtesvwzzsc.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.hfpthk.cn/gtwoworqxn.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.fengsongda.top/gtkfcdxlmo.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.daxiang520.top/gtssrrofst.html

[K06] 解析 URL 查询串
来源：http://hz.shanyushiyangtech.top/gtmsbxxkgl.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.daria6918.cn/gtoomryxfv.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.hfpthk.cn/gtlakpzxwz.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.ppjwa.cn/gtvjrlzwjr.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.tian-w.cn/gtgzqcyqps.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.hywenlv.cn/gtbnmndbfb.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.chenjidiqi.icu/gtcwowoemv.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.shangyingyoupin.top/gtinxnzcdu.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.316326.xyz/gtsulmwgdh.html

[K07] 进制转换
来源：http://hz.hnxiangtu.top/gtziikvvof.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.feifeiyinyue.top/gtigbrkqub.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.wangshuangyany.cn/gtjxdwkofx.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.0kj1m.cn/gtblvsavaa.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.yvedp.cn/gtrzkrqjpm.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.sweek.top/gtxnaspwcu.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.yongpay.top/gtfmybelzo.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.jianghu66.top/gtyytcibdx.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.wangdashe.top/gtjwvesuxi.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.zdqjudy.top/gtaqlgwmml.html

Py:   pickle.dumps(obj)
来源：http://hz.hfpthk.cn/gtgsjsjlqw.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.shanyushiyangkeji.top/gtfftgptek.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.yuxming.cn/gttkgzknlk.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.tian-w.cn/gtsewlmjhl.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.guannengcc.top/gtblmsntsf.html

Go:   encoding/gob
来源：http://hz.iojbl.cn/gtbmvwhnsa.html

Ruby: Marshal.dump(obj)
来源：http://hz.0kj1m.cn/gtppiztqzq.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.fzhhl.top/gtmxtspfjt.html

================================================================================
来源：http://hz.xuanzx.com/gtzhormsvo.html

L. 网络请求
来源：http://hz.hywenlv.cn/gtkhdjyruw.html

================================================================================
来源：http://hz.yueranfly.top/gtmrwtxzkb.html

[L01] 发送 GET 请求
来源：http://hz.dianchejie.cn/gtfbnoxjmt.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.ydjk.org.cn/gtmkwscvup.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.xuanzx.com/gtupmypngm.html

JS:   await fetch(url)
来源：http://hz.yanxiufei.cn/gtspoxduco.html

TS:   await fetch(url)
来源：http://hz.guannengcc.top/gtfmvrbqbh.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.cheryme.top/gtydcksrgn.html

Go:   resp, err := http.Get(url)
来源：http://hz.yuxming.cn/gtbjhbnbtc.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.xziqi.cn/gtggjsxici.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.hysaishi.cn/gtznamcwfk.html

[L02] 发送 POST JSON
来源：http://hz.chenzaomai.com/gtzjynvzsv.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.dashuyun.cn/gtefmnhldm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.sxryk.cn/gtdxokjtdz.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhaomingkeji.xyz/gtaylpmpvy.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yuanzhike.top/gtxpsztnxl.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.yangfankeji.com/gtfsebvtki.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.nanxuanxn.top/gtnhbbfhjs.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.jinyuanbaomall.cn/gtklmguvjn.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.snrcjt.cn/gtuuticscp.html

[L03] 设置自定义请求头
来源：http://hz.ppjwa.cn/gtsezkiywo.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.meibo888.top/gtrqhhklyo.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.jyoumei.cn/gtvcqruywt.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.cqqwz.cn/gtrpsgtwws.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.sxryk.cn/gtafxnvrsc.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.hysaishi.cn/gtftpsdqzx.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.ydjk.org.cn/gtjvseffio.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.yj202588.top/gtrkgcwlsx.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.bjfxy.top/gtlmdeearr.html

[L04] 设置超时
来源：http://hz.gzhubu.top/gtgttavnka.html

Py:   requests.get(url, timeout=5)
来源：http://hz.svipenyu.cn/gtgstuyuer.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.svipenyu.cn/gtyxtlxagw.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jqgufenzy.top/gtdhyrehdu.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yonumen.top/gtryyxyggo.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.zycfv.cn/gtvuohsomv.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.yanxiufei.cn/gtzypkqfgg.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.jqgfzy.top/gtgvdsqbhg.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.guannengcc.top/gtryglduee.html

[L05] 上传文件（multipart）
来源：http://hz.ivvv.top/gttonxmvum.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.daria6918.cn/gtakhkocnz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.mhx1999.top/gtrgtczdtr.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.yueranfly.top/gtxdrccjmk.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.daria6918.cn/gtgaesvlbo.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.gogol.net.cn/gtnkzbsvjm.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.iojbl.cn/gtckxjvivg.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.jinyuanbaomall.cn/gtsftjzsuz.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.nwbrower.top/gtkbvjkhlb.html

[L06] 解析响应为 JSON
来源：http://hz.shanyushiyangtech.top/gtxlvgebvs.html

Py:   resp.json()
来源：http://hz.sxryk.cn/gtugnczwbk.html

PHP:  json_decode($body, true);
来源：http://hz.9152youxi.cn/gtixljvivd.html

JS:   await resp.json()
来源：http://hz.nwbrower.top/gtubyzgfkx.html

TS:   await resp.json()
来源：http://hz.feifeiyinyue.top/gtpeyhohge.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.svipenyu.cn/gtcfrkrwue.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.fengsongda.top/gtvvkkpatl.html

Ruby: JSON.parse(resp.body)
来源：http://hz.tanke756.top/gtskmguwoy.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.ywan-chungtsiang.top/gtfkxbecwd.html

[L07] 处理 HTTP 状态码
来源：http://hz.yvedp.cn/gtfjmiyrqt.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.ppjwa.cn/gtnuwizfzf.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.zhixingplan.top/gtnophqtzc.html

JS:   resp.ok;  resp.status
来源：http://hz.xinyue.icu/gtpjbqupyy.html

TS:   resp.ok;  resp.status
来源：http://hz.yj20258.top/gtehmqqiso.html

Java: resp.statusCode()
来源：http://hz.hammf.cn/gtwmcqpjef.html

Go:   resp.StatusCode
来源：http://hz.9152youxi.cn/gtieufupgv.html

Ruby: resp.code.to_i
来源：http://hz.yueranfly.top/gtnfhdmovh.html

C#:   (int)resp.StatusCode
来源：http://hz.quarkkingdee.top/gtwfxkeyvp.html

[L08] 并发请求多个地址
来源：http://hz.nanxuanxn.top/gttgykonvl.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.tanke756.top/gtwpathmll.html

PHP:  curl_multi_init() 系列
来源：http://hz.cdnleiting.top/gtsmpcpxnw.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhixingplan.top/gtwroxwfgs.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.haohaochexian.top/gtwawkochb.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.aizwys.cn/gtvlkdamke.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.jinqigufen.top/gtgtlhwttq.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.zhaomingkeji.xyz/gtkkrwhbux.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.zhijiandao.cn/gtibplwzxu.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtefmkfmgf.html

M. 命令行 / 进程 / 环境
来源：http://hz.9152youxi.cn/gtidqbcbwm.html

================================================================================
来源：http://hz.gogol.net.cn/gtmgvwtmrh.html

[M01] 读取命令行参数
来源：http://hz.fzhhl.top/gtkgrwjdaz.html

Py:   sys.argv[1:]
来源：http://hz.svipenyu.cn/gtwndvljxn.html

PHP:  $argv;  $argc;
来源：http://hz.xziqi.cn/gtvbwabxpi.html

JS:   process.argv.slice(2)
来源：http://hz.yonumen.top/gteehgscgt.html

TS:   process.argv.slice(2)
来源：http://hz.hywenlv.cn/gtelihyeig.html

Java: args 数组（main 方法参数）
来源：http://hz.xziqi.cn/gtkzqpbfjp.html

Go:   os.Args[1:]
来源：http://hz.hywenlv.cn/gtpxyegodu.html

Ruby: ARGV
来源：http://hz.dianchejie.cn/gtpjdjamrc.html

C#:   args 数组（Main 方法参数）
来源：http://hz.birdmap.top/gtcljpmntw.html

[M02] 读取环境变量
来源：http://hz.zhiwuduotai.top/gtojrxalzo.html

Py:   os.environ.get("HOME")
来源：http://hz.svipenyu.cn/gtpjdiysao.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.hywenlv.cn/gttorndtvc.html

JS:   process.env.HOME
来源：http://hz.hnxiangtu.top/gtmgrstpbx.html

TS:   process.env.HOME
来源：http://hz.xuanzx.com/gtanqahgxr.html

Java: System.getenv("HOME")
来源：http://hz.wangdashe.top/gtxfvffvxn.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.sysykeji.top/gtpvawhxzc.html

Ruby: ENV["HOME"]
来源：http://hz.jinqigufen.top/gtmqvfrrir.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.andypj.xyz/gtxanfjnei.html

[M03] 执行外部命令
来源：http://hz.daria6918.cn/gtxdernjpw.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.yangfankeji.com/gtatnyspqo.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.xziqi.cn/gthmddzarl.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.jyoumei.cn/gtreqbfbgk.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.aibaodan.cn/gtujbdsmog.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.shangyingyoupin.top/gtajkhhzfq.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.haohaochexian.top/gtvlxynnyk.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.cqqwz.cn/gtghrfcaqq.html

C#:   Process.Start("ls", "-l");
来源：http://hz.tanke756.top/gtdjnchtgx.html

[M04] 获取当前工作目录
来源：http://hz.shanyushiyangkeji.top/gtqeunubuz.html

Py:   os.getcwd()
来源：http://hz.gogol.net.cn/gtoihthzip.html

PHP:  getcwd();
来源：http://hz.zhiwuduotai.top/gtakutqree.html

JS:   process.cwd()
来源：http://hz.ybcxt.top/gtcgymucvz.html

TS:   process.cwd()
来源：http://hz.jlsjyb.cn/gtlubipxpc.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.hfpthk.cn/gtaqxrmpjx.html

Go:   os.Getwd()
来源：http://hz.sxryk.cn/gtwurmlivb.html

Ruby: Dir.pwd
来源：http://hz.316326.xyz/gtpcmctazn.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.jqgfzy.top/gtnuhgnmzo.html

[M05] 设置退出码
来源：http://hz.sysykeji.top/gthltmzond.html

Py:   sys.exit(1)
来源：http://hz.wangdashe.top/gtkgaquipa.html

PHP:  exit(1);
来源：http://hz.sufxvd.cn/gtpbpszwxh.html

JS:   process.exit(1)
来源：http://hz.zhongyouzk.top/gtmrrecybu.html

TS:   process.exit(1)
来源：http://hz.ppjwa.cn/gtqiuzapvu.html

Java: System.exit(1)
来源：http://hz.ydjk.org.cn/gtnaqpbciu.html

Go:   os.Exit(1)
来源：http://hz.jinghuilouyu.cn/gtapwgwsnd.html

Ruby: exit 1
来源：http://hz.zhixingplan.top/gtlyfguude.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.52xcode.cn/gtvitpufdx.html

[M06] 向标准错误输出
来源：http://hz.daria6918.cn/gtiqvnpzkk.html

Py:   print("err", file=sys.stderr)
来源：http://hz.havefunace.top/gtwqqqmkng.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.shangyingyoupin.top/gtqrizfyhh.html

JS:   console.error("err")
来源：http://hz.jinqigfzy.top/gttfqpdrfo.html

TS:   console.error("err")
来源：http://hz.snrcjt.cn/gttmwcfcje.html

Java: System.err.println("err")
来源：http://hz.yuanzhike.top/gtacdnmgql.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.meibo888.top/gtzatmrkru.html

Ruby: warn "err"
来源：http://hz.zhoulong.xyz/gtvuipangj.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.pengpengdd.cyou/gtwsinrhfq.html

[M07] 判断是否为主入口
来源：http://hz.yonumen.top/gtdbxamvci.html

Py:   if __name__ == "__main__":
来源：http://hz.chenzaomai.com/gtsbpccdqj.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.ivvv.top/gtziqnkjrp.html

JS:   require.main === module
来源：http://hz.xinyue.icu/gtlderdomr.html

TS:   require.main === module
来源：http://hz.tianlin.xyz/gtlytlsftz.html

Java: public static void main(String[] args)
来源：http://hz.smart0.xyz/gtlgtpwqbc.html

Go:   func main()
来源：http://hz.pycfn.com/gtecydgnde.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.zycfv.cn/gtxwmriazn.html

C#:   static void Main(string[] args)
来源：http://hz.hywenlv.cn/gthcwsbdjh.html

[M08] 获取系统与运行时信息
来源：http://hz.hysaishi.cn/gtrldvomjl.html

Py:   platform.system();  platform.python_version()
来源：http://hz.hnqzz.top/gtvgrxenpe.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.xuanzx.com/gtcgviepbz.html

JS:   process.platform;  process.version
来源：http://hz.zhoulong.xyz/gtlzoqlwfk.html

TS:   process.platform;  process.version
来源：http://hz.gogol.net.cn/gtodjwiopx.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.jqgfzy.top/gtcnamhewf.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.pengpengdd.cyou/gtiqxbsrov.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.chenjidiqi.icu/gtsaoubxtp.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.bjfxy.top/gtmujojalw.html

================================================================================
来源：http://hz.daria6918.cn/gtcioobiyu.html

N. 数据结构与算法
来源：http://hz.pycfn.com/gtbcjaougo.html

================================================================================
来源：http://hz.snrcjt.cn/gtwnjlkkgk.html

[N01] 二分查找（有序数组）
来源：http://hz.jqgufenzy.top/gtesyxfpbw.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.gzhubu.top/gtborlkban.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.gotoacloud.top/gteizehpux.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zhixingplan.top/gtcyelpzep.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zhaomingkeji.xyz/gtbtqlzgqb.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.xylfe.cn/gtydzhxgct.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.yj20258888.top/gtmzjhzapw.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.yj20258888.top/gtfsoteuyd.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.yvedp.cn/gtxtsorqow.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.xingfuxueyuan.xyz/gtmozchwur.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.quarkkingdee.top/gtzxgjwocd.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.hammf.cn/gtgydvxaqg.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.daria6918.cn/gtvvqywmck.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.ywan-chungtsiang.top/gtbkillzgq.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.316326.xyz/gtelziseqo.html

Go:   slices.Sort(arr)
来源：http://hz.9152youxi.cn/gtidyhqnff.html

Ruby: arr.sort
来源：http://hz.xuanzx.com/gtigadryxy.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.sysykeji.top/gtttitysou.html

[N03] 快速排序（分治示例）
来源：http://hz.havefunace.top/gtnkftvmfx.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.guannengcc.top/gtdcptiilb.html

PHP:  // 递归实现，或用 usort
来源：http://hz.hnqzz.top/gtocaavgwy.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jianghu66.top/gtieyszcxc.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.9152youxi.cn/gtgtboorhp.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.nanxinkj.top/gtmohkpngo.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.sxryk.cn/gtquawuubi.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.yonumen.top/gtidtkdabq.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.jinghuilouyu.cn/gthkphnohj.html

[N04] 斐波那契数列
来源：http://hz.zhaomingkeji.xyz/gtooabbaqy.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.bjfxy.top/gtslfftulc.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.shanyushiyangkeji.top/gtovyfptff.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jinyuanbaomall.cn/gtkvyajfqb.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.wangshuangyany.cn/gtoqacwvdq.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.cheryme.top/gthpervcpj.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.quarkkingdee.top/gtkyvwnoek.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.sweek.top/gtdfuftzji.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.chenjidiqi.icu/gtdivqaxjq.html

[N05] 最大公约数
来源：http://hz.shanyushiyangkeji.top/gtxntltaet.html

Py:   math.gcd(a, b)
来源：http://hz.zycfv.cn/gtfvmplyut.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.dashuyun.cn/gttsqggywy.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yueranfly.top/gtkcnxpcyn.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.smart0.xyz/gttojceujb.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.ybcxt.top/gtuzmzuhmp.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.zhoulong.xyz/gtjvrukyvl.html

Ruby: a.gcd(b)
来源：http://hz.jianghu66.top/gtlhsqzzxi.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.birdmap.top/gtowwkaazq.html

[N06] 判断回文字符串
来源：http://hz.haohaochexian.top/gtlkursvtt.html

Py:   s == s[::-1]
来源：http://hz.jiagoushi.top/gtrtabpubr.html

PHP:  $s === strrev($s);
来源：http://hz.guannengcc.top/gtqeqzfrnv.html

JS:   s === [...s].reverse().join("")
来源：http://hz.pengpengdd.cyou/gtbyadlbow.html

TS:   s === [...s].reverse().join("")
来源：http://hz.ydzc1.top/gttxypoiil.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.svipenyu.cn/gtmdkkrhql.html

Go:   // 双指针从两端比较
来源：http://hz.jiagoushi.top/gtknwzvvdm.html

Ruby: s == s.reverse
来源：http://hz.jinqigfzy.top/gtstszvmaz.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.nanxuanxn.top/gtxqgtklzg.html

[N07] 两数之和（返回下标）
来源：http://hz.ydzc1.top/gtvinylzfs.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.haohaochexian.top/gtmbggqprx.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.sxryk.cn/gtzubnprez.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.jyoumei.cn/gtkstvpxuc.html

TS:   // 手写 Map<string, number>
来源：http://hz.shangyingyoupin.top/gtdylqiypf.html

Java: // 手写 HashMap
来源：http://hz.zhongyouzk.top/gtfeawqnhz.html

Go:   // 手写 map[int]int
来源：http://hz.yongpay.top/gtzisdsmvt.html

Ruby: // 手写 Hash
来源：http://hz.fzhhl.top/gtnydrdjrb.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.hammf.cn/gtwdqaqpis.html

[N08] 生成全排列
来源：http://hz.daria6918.cn/gtdwxmzryu.html

Py:   itertools.permutations(arr)
来源：http://hz.zhoulong.xyz/gtpunsybua.html

PHP:  // 手写递归交换
来源：http://hz.shzxlz.cn/gtzwlwpnsm.html

JS:   // 手写回溯递归
来源：http://hz.nanxuanxn.top/gtxwozsyyb.html

TS:   // 手写回溯递归
来源：http://hz.andypj.xyz/gtnxkmecyx.html

Java: // 手写回溯递归
来源：http://hz.jqgufenzy.top/gtthzswgta.html

Go:   // 手写回溯递归
来源：http://hz.cucudq.cn/gtycmgrmjl.html

Ruby: arr.permutation.to_a
来源：http://hz.nanxinkj.top/gtzeyragcx.html

C#:   // 手写回溯递归
来源：http://hz.tanke756.top/gtipapmrjh.html

[N09] 栈与队列
来源：http://hz.haohaochexian.top/gtlwfcnnly.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.dianchejie.cn/gturbhosrx.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.sufxvd.cn/gtcovdnkfe.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.guannengcc.top/gtrvcahjop.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.dianchejie.cn/gtaiuqutln.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.jyoumei.cn/gtctrlavvp.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.shangyingyoupin.top/gtrfyhzxjy.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.cucudq.cn/gtrfkwvdwx.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.hywenlv.cn/gtjfaauuea.html

[N10] 链表节点定义
来源：http://hz.hfpthk.cn/gtshvjotln.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.nanxinkj.top/gtqljfmxjj.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.xinyue.icu/gtswjugdgy.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.cheryme.top/gtoyxsknig.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.chenlongwang.top/gttjgihenq.html

Java: class Node { int v; Node next; }
来源：http://hz.ydzc1.top/gtyuqihkrh.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.daria6918.cn/gtorpqyjpc.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.jinqigufen.top/gtklilibmj.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.zhongyouzk.top/gthpnhdnge.html

[N11] 二叉树中序遍历
来源：http://hz.pengpengdd.cyou/gtwdcgwwij.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.zhixingplan.top/gtubenbfvs.html

PHP:  // 手写递归函数
来源：http://hz.hywenlv.cn/gtjxcekroc.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.nanxuanxn.top/gtrcuklmsj.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.xinyue.icu/gtealewbsq.html

Java: // 手写递归
来源：http://hz.xylfe.cn/gtkjbwoeej.html

Go:   // 手写递归
来源：http://hz.bjfxy.top/gtwrqqouqq.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.yuxming.cn/gtjvdiojzf.html

C#:   // 手写递归
来源：http://hz.ehwqpu.com/gtyqrcxwug.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.shanyushiyangkeji.top/gtooavivdv.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.cashguo.top/gtwvopqymq.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.cheryme.top/gtclbmzyjn.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.kuanghao11.cn/gtbgnkmyec.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jinghuilouyu.cn/gtbrhtpbnf.html


<!-- 参考信息 -->