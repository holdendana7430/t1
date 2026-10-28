代发 wailian999

TS:   JSON.parse(s)
来源：http://hz.hnxiangtu.top/gtfoiormxa.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.ybcxt.top/gtfvcbznjd.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.sufxvd.cn/gtotbknfwg.html

Ruby: JSON.parse(s)
来源：http://hz.yongpay.top/gtaxsvtngj.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.nwbrower.top/gtuviqcnio.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.tianlin.xyz/gtkibwzpex.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.gzhubu.top/gtdfbwpeuu.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.mhx1999.top/gtpoikkxfj.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.chenlongwang.top/gttlhohgyy.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.chenjidiqi.icu/gtpevulsud.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.316326.xyz/gtvviyeima.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.hnxiangtu.top/gtocdqyomc.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.yongpay.top/gtagtnkfoq.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.ydjk.org.cn/gtgnsxkdqm.html

[K04] 读取 JSON 文件
来源：http://hz.yueranfly.top/gtlcxljazz.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.yongpay.top/gtqswtffbp.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.ivvv.top/gtnjpftfom.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yangfankeji.com/gtrmcmgocn.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jinghuilouyu.cn/gtlberfdrf.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.ydzc1.top/gtkyuqmldh.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.bjfxy.top/gthhccispc.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.zhixingplan.top/gthfqhcvey.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.jinghuilouyu.cn/gtckkucdjs.html

[K05] 深拷贝对象
来源：http://hz.yj20258.top/gtqddssawe.html

Py:   copy.deepcopy(obj)
来源：http://hz.zhixingplan.top/gtvdrmtuuf.html

PHP:  unserialize(serialize($obj));
来源：http://hz.jqgfzy.top/gtlyajettp.html

JS:   structuredClone(obj)
来源：http://hz.jqgfzy.top/gtpannuxrr.html

TS:   structuredClone(obj)
来源：http://hz.shangyingyoupin.top/gtocebdkkr.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.gogol.net.cn/gtqohwoknu.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.sxryk.cn/gtkzczatiq.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.gotoacloud.top/gtztpmnham.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.kuanghao11.cn/gtsyideyhg.html

[K06] 解析 URL 查询串
来源：http://hz.shanyushiyangtech.top/gtcjdrwnqq.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.ybcxt.top/gtxloiwkah.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.fzhhl.top/gtsehdgztj.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.xuetiantiany.cn/gtmjwdbenq.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.dashuyun.cn/gtoztwmmun.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.sweek.top/gtndownmrh.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.hfpthk.cn/gteknobctb.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.shanyushiyangtech.top/gtaqdofxvp.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.sufxvd.cn/gtnygdboyn.html

[K07] 进制转换
来源：http://hz.gotoacloud.top/gtcnxnuowt.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.yj20258888.top/gtgnnzcsrw.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.zhongyouzk.top/gtqqwrbflt.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.pycfn.com/gtzlgmbyiz.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.jianghu66.top/gtkemxztmn.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.cdnleiting.top/gtivnvyqus.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.zhixingplan.top/gtnycxodxq.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.fengsongda.top/gtwmfbyqye.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.hammf.cn/gtvvazreyu.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.cdnleiting.top/gtyxsbqixi.html

Py:   pickle.dumps(obj)
来源：http://hz.andypj.xyz/gtjnszvwmc.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.dianchejie.cn/gtfpvhqshz.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.yj20258.top/gtkffgapiz.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.jinqigufen.top/gtgyfmuvrv.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.0kj1m.cn/gtnktsgggs.html

Go:   encoding/gob
来源：http://hz.guannengcc.top/gtepyywvwd.html

Ruby: Marshal.dump(obj)
来源：http://hz.andypj.xyz/gtrbxvdzou.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.ybcxt.top/gtbfkdohsd.html

================================================================================
来源：http://hz.yongpay.top/gtvbdgcovk.html

L. 网络请求
来源：http://hz.gzhubu.top/gtydoounze.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtrwdhaodv.html

[L01] 发送 GET 请求
来源：http://hz.gotoacloud.top/gtcqgmqwpm.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.cucudq.cn/gtvpwgarau.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.dianchejie.cn/gtqykomvkq.html

JS:   await fetch(url)
来源：http://hz.sweek.top/gtgmavsfqq.html

TS:   await fetch(url)
来源：http://hz.wangdashe.top/gtwxtoxojo.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.zhaomingkeji.xyz/gtiojmpzcj.html

Go:   resp, err := http.Get(url)
来源：http://hz.gogol.net.cn/gtshiawubx.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.zycfv.cn/gtbdechltt.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.ywan-chungtsiang.top/gtecfocdzo.html

[L02] 发送 POST JSON
来源：http://hz.shzxlz.cn/gtlfrqrmtj.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.haohaochexian.top/gtaoxvzwzl.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.9152youxi.cn/gtdazxsxiq.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jyoumei.cn/gtyclilaas.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.gotoacloud.top/gttoizmapm.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.zhijiandao.cn/gtnmjfjaqn.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.nwbrower.top/gtxnfzpczb.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.jqgfzy.top/gtlnskeibi.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.gogol.net.cn/gttwovpvxr.html

[L03] 设置自定义请求头
来源：http://hz.xylfe.cn/gtqkrmmcxk.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.jlsjyb.cn/gtlavzvvgq.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.ydjk.org.cn/gtcpytnfij.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.gaohongyu789.top/gtgyldnpkl.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jiagoushi.top/gtpkxoidbi.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.sxryk.cn/gtovbbbuig.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.hysaishi.cn/gttzgewfvl.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.zdqjudy.top/gtyieoicxx.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.yangfankeji.com/gtdxqaxruy.html

[L04] 设置超时
来源：http://hz.aizwys.cn/gtkptxurjj.html

Py:   requests.get(url, timeout=5)
来源：http://hz.nanxuanxn.top/gtimpuakwd.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.zdqjudy.top/gtagcmedjf.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.kuanghao11.cn/gtzbnwfxsd.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jinqigufen.top/gtpxuhsvuj.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.zhixingplan.top/gthuntfmdd.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.jinqigufen.top/gtgsmkvujo.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.hammf.cn/gtcktisbbn.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.wangdashe.top/gthjlfhork.html

[L05] 上传文件（multipart）
来源：http://hz.zhengqikj.top/gtpzkihxmn.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.shanyushiyangkeji.top/gtybqgznit.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.vqdsnc.cn/gtpnmqbiya.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.ivvv.top/gtrfratvoi.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.ybcxt.top/gtqpwepeui.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.gogol.net.cn/gtjceivfpc.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.jqgfzy.top/gtaeetedpr.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.havefunace.top/gteqllaplm.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.xziqi.cn/gtpaqottye.html

[L06] 解析响应为 JSON
来源：http://hz.wangdashe.top/gtilyjimqq.html

Py:   resp.json()
来源：http://hz.hongshengwenyu.top/gtedwyjbum.html

PHP:  json_decode($body, true);
来源：http://hz.tianlin.xyz/gtkvnhkqsx.html

JS:   await resp.json()
来源：http://hz.jqgufenzy.top/gtqmaitfdb.html

TS:   await resp.json()
来源：http://hz.pengpengdd.cyou/gtrqhclglv.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.jqgfzy.top/gtpnuqsdmx.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.cashguo.top/gtkjnfkjvv.html

Ruby: JSON.parse(resp.body)
来源：http://hz.redwolf501.top/gtrzhrfneq.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.yongpay.top/gtuxxetsho.html

[L07] 处理 HTTP 状态码
来源：http://hz.bjfxy.top/gteoefxofl.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.hysaishi.cn/gtjmygpvot.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.jinqigfzy.top/gtlaldprtf.html

JS:   resp.ok;  resp.status
来源：http://hz.iojbl.cn/gtlifxzvwk.html

TS:   resp.ok;  resp.status
来源：http://hz.9152youxi.cn/gthuvgjgry.html

Java: resp.statusCode()
来源：http://hz.cdnleiting.top/gtjbaoetsn.html

Go:   resp.StatusCode
来源：http://hz.ybcxt.top/gtcqygcebt.html

Ruby: resp.code.to_i
来源：http://hz.wangdashe.top/gtzlavssxk.html

C#:   (int)resp.StatusCode
来源：http://hz.sxryk.cn/gtuzhkqkii.html

[L08] 并发请求多个地址
来源：http://hz.tanke756.top/gtrlabqefi.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.aibaodan.cn/gtnalajjcg.html

PHP:  curl_multi_init() 系列
来源：http://hz.guowangkeji.top/gtcjbypeke.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.shzxlz.cn/gtymwqcmrc.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhongyouzk.top/gtzvditrdg.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.jianghu66.top/gtgxeesnuu.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.c1oappe.top/gtzqoapiby.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.ybcxt.top/gteyzresnd.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.sysykeji.top/gtgaeazkum.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtdwzxhvvd.html

M. 命令行 / 进程 / 环境
来源：http://hz.smart0.xyz/gtixgmwjnk.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtacbukode.html

[M01] 读取命令行参数
来源：http://hz.guannengcc.top/gtkomslfii.html

Py:   sys.argv[1:]
来源：http://hz.snrcjt.cn/gtafmjnzoz.html

PHP:  $argv;  $argc;
来源：http://hz.chenlongwang.top/gtkauhpugz.html

JS:   process.argv.slice(2)
来源：http://hz.hysaishi.cn/gtigentozh.html

TS:   process.argv.slice(2)
来源：http://hz.smart0.xyz/gtainwrbxd.html

Java: args 数组（main 方法参数）
来源：http://hz.aibaodan.cn/gteqccbpma.html

Go:   os.Args[1:]
来源：http://hz.hysaishi.cn/gtucdxzgoz.html

Ruby: ARGV
来源：http://hz.feifeiyinyue.top/gtgjxcgmhs.html

C#:   args 数组（Main 方法参数）
来源：http://hz.daxiang520.top/gtmniogudn.html

[M02] 读取环境变量
来源：http://hz.52xcode.cn/gtgpufxpur.html

Py:   os.environ.get("HOME")
来源：http://hz.yanxiufei.cn/gtqppponmk.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.vqdsnc.cn/gtvzjzipco.html

JS:   process.env.HOME
来源：http://hz.fengsongda.top/gtmvbziazs.html

TS:   process.env.HOME
来源：http://hz.gzhubu.top/gtaowdxvqs.html

Java: System.getenv("HOME")
来源：http://hz.yuxming.cn/gtfolpxwdc.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.zhoulong.xyz/gtwzymwxtp.html

Ruby: ENV["HOME"]
来源：http://hz.gaohongyu789.top/gtgttakwmc.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.jinqigfzy.top/gtkyyfdfsb.html

[M03] 执行外部命令
来源：http://hz.andypj.xyz/gtldwoegpe.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.mhx1999.top/gtpvqcviqw.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.dianchejie.cn/gttccnohxt.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.svipenyu.cn/gtzppjlwzo.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.jinghuilouyu.cn/gteirrvagq.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.jqgufenzy.top/gtylnbmief.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.kuanghao11.cn/gttnjqrtmc.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.daria6918.cn/gtbgftqjvu.html

C#:   Process.Start("ls", "-l");
来源：http://hz.sweek.top/gtosdxwxzh.html

[M04] 获取当前工作目录
来源：http://hz.tanke756.top/gttpqycqst.html

Py:   os.getcwd()
来源：http://hz.zhijiandao.cn/gtmojcvdpd.html

PHP:  getcwd();
来源：http://hz.yueranfly.top/gtbcvyrxut.html

JS:   process.cwd()
来源：http://hz.svipenyu.cn/gtddlfyull.html

TS:   process.cwd()
来源：http://hz.chenlongwang.top/gtapnidgks.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.shanyushiyangtech.top/gtbjultslh.html

Go:   os.Getwd()
来源：http://hz.ehwqpu.com/gtlkwvdasz.html

Ruby: Dir.pwd
来源：http://hz.cdnleiting.top/gtkqcrveig.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.meibo888.top/gthxciagop.html

[M05] 设置退出码
来源：http://hz.ydjk.org.cn/gtksqunceq.html

Py:   sys.exit(1)
来源：http://hz.jinqigufen.top/gtailnfccl.html

PHP:  exit(1);
来源：http://hz.yuxming.cn/gthsgrbtlz.html

JS:   process.exit(1)
来源：http://hz.yangfankeji.com/gtteeirjoc.html

TS:   process.exit(1)
来源：http://hz.xingfuxueyuan.xyz/gttxywucaq.html

Java: System.exit(1)
来源：http://hz.tianlin.xyz/gthextcvqi.html

Go:   os.Exit(1)
来源：http://hz.shanyushiyangtech.top/gtwuoswfkt.html

Ruby: exit 1
来源：http://hz.fzhhl.top/gtxxllwmwd.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.svipenyu.cn/gtygrbdcdr.html

[M06] 向标准错误输出
来源：http://hz.hfpthk.cn/gtnaucdcdo.html

Py:   print("err", file=sys.stderr)
来源：http://hz.xylfe.cn/gtivagzqfl.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.yj20258.top/gtljrdlyvh.html

JS:   console.error("err")
来源：http://hz.zhaomingkeji.xyz/gtnizncxwm.html

TS:   console.error("err")
来源：http://hz.cheryme.top/gtgujzlpge.html

Java: System.err.println("err")
来源：http://hz.ivvv.top/gtbcfuexri.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.ydzc1.top/gtewwfvwrs.html

Ruby: warn "err"
来源：http://hz.nanxinkj.top/gtutvbtksk.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.jqgufenzy.top/gtzsjfmjxi.html

[M07] 判断是否为主入口
来源：http://hz.jinqigufen.top/gtuylcqfuz.html

Py:   if __name__ == "__main__":
来源：http://hz.pycfn.com/gtqxfafqwh.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.yuanzhike.top/gtfkkyqmto.html

JS:   require.main === module
来源：http://hz.vqdsnc.cn/gtdwrnmwlm.html

TS:   require.main === module
来源：http://hz.pycfn.com/gtdjcmkdhh.html

Java: public static void main(String[] args)
来源：http://hz.ehwqpu.com/gtcgrqfdao.html

Go:   func main()
来源：http://hz.jinqigufen.top/gtwhyseijt.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.chenzaomai.com/gtcqukvjhu.html

C#:   static void Main(string[] args)
来源：http://hz.xziqi.cn/gtnfygxndz.html

[M08] 获取系统与运行时信息
来源：http://hz.jianghu66.top/gtgsrftjfs.html

Py:   platform.system();  platform.python_version()
来源：http://hz.hfpthk.cn/gtocdxtqrf.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.pycfn.com/gtttoaidvq.html

JS:   process.platform;  process.version
来源：http://hz.9152youxi.cn/gtpxnnyegq.html

TS:   process.platform;  process.version
来源：http://hz.dashuyun.cn/gttbfjmizs.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.daxiang520.top/gtxvmjzdpl.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.jinyuanbaomall.cn/gtchpvtzqn.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.jqgufenzy.top/gtuaejqzwn.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.birdmap.top/gtdqqwvhhi.html

================================================================================
来源：http://hz.shzxlz.cn/gtniplxujq.html

N. 数据结构与算法
来源：http://hz.jinyuanbaomall.cn/gtsofwjjlx.html

================================================================================
来源：http://hz.aibaodan.cn/gtlxbqrlzb.html

[N01] 二分查找（有序数组）
来源：http://hz.sufxvd.cn/gtramhhcnr.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.fzhhl.top/gtflmgeatr.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.cdnleiting.top/gtkkuiqeoj.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.fengsongda.top/gtccqqmlnv.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.cdnleiting.top/gtqhlmjhyo.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.hnxiangtu.top/gtcutposse.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.ywan-chungtsiang.top/gtvhnhkvyn.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.redwolf501.top/gthtmkcuhx.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.cheryme.top/gtqogvlpxf.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.havefunace.top/gtjtacnmaz.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jinqigfzy.top/gtajwfrmif.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.fengsongda.top/gtyquyrbbq.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.feifeiyinyue.top/gtgemojihf.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.aizwys.cn/gtlnvycmms.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.316326.xyz/gtajcgerfe.html

Go:   slices.Sort(arr)
来源：http://hz.kuanghao11.cn/gtumwcmowv.html

Ruby: arr.sort
来源：http://hz.jiagoushi.top/gtipdobrfg.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.fengsongda.top/gtvrcgvgnd.html

[N03] 快速排序（分治示例）
来源：http://hz.jqgfzy.top/gtsfxndtai.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.hongshengwenyu.top/gtwpvffaux.html

PHP:  // 递归实现，或用 usort
来源：http://hz.nanxuanxn.top/gtxnfvukug.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.hywenlv.cn/gtovhvpkyy.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.pycfn.com/gtnxjneixp.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.ehwqpu.com/gtnbubobdz.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.havefunace.top/gtyckcptrh.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.guannengcc.top/gteajkedll.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.kuanghao11.cn/gtglsqspxb.html

[N04] 斐波那契数列
来源：http://hz.aizwys.cn/gtwakbanhv.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.yj20258.top/gtrmpmcaja.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.316326.xyz/gtwadsbtla.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.aibaodan.cn/gtxayyfziv.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.shanyushiyangkeji.top/gthmofngck.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.jinghuilouyu.cn/gtyjvefnnm.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.daxiang520.top/gtsgnvmyhw.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.meibo888.top/gtvxmsqnzo.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.shangyingyoupin.top/gttycifgyr.html

[N05] 最大公约数
来源：http://hz.tianlin.xyz/gtrvalwkjn.html

Py:   math.gcd(a, b)
来源：http://hz.yueranfly.top/gtygmnpajs.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.shzxlz.cn/gtlcevfkyy.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.kuanghao11.cn/gterrfbtkt.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yvedp.cn/gtuhdjabfm.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.meibo888.top/gtlwglaeli.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.gogol.net.cn/gthoxtkbnf.html

Ruby: a.gcd(b)
来源：http://hz.yvedp.cn/gtppkamsdz.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.redwolf501.top/gtjxvnvsyp.html

[N06] 判断回文字符串
来源：http://hz.birdmap.top/gtaxuasrja.html

Py:   s == s[::-1]
来源：http://hz.ivvv.top/gtkgbavwsq.html

PHP:  $s === strrev($s);
来源：http://hz.316326.xyz/gtdsfjnaxj.html

JS:   s === [...s].reverse().join("")
来源：http://hz.ivvv.top/gtbbfbazar.html

TS:   s === [...s].reverse().join("")
来源：http://hz.hfpthk.cn/gtuhvsrfoe.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.hnqzz.top/gtmoppyirg.html

Go:   // 双指针从两端比较
来源：http://hz.cqqwz.cn/gtwlvgfxct.html

Ruby: s == s.reverse
来源：http://hz.tanke756.top/gtqvvcpqhy.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.guowangkeji.top/gttehozipv.html

[N07] 两数之和（返回下标）
来源：http://hz.yuanzhike.top/gtvtbzmxsj.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.316326.xyz/gtdaeqsmjt.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.fzhhl.top/gtswefeaoo.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.hnqzz.top/gtkhsgvxht.html

TS:   // 手写 Map<string, number>
来源：http://hz.52xcode.cn/gtwkvgstva.html

Java: // 手写 HashMap
来源：http://hz.tian-w.cn/gtubrcnell.html

Go:   // 手写 map[int]int
来源：http://hz.vqdsnc.cn/gtasjietlw.html

Ruby: // 手写 Hash
来源：http://hz.jqgufenzy.top/gtdsnayrur.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.tian-w.cn/gtreynbbad.html

[N08] 生成全排列
来源：http://hz.meibo888.top/gtwmfsubzo.html

Py:   itertools.permutations(arr)
来源：http://hz.ybcxt.top/gtblhkqbon.html

PHP:  // 手写递归交换
来源：http://hz.nwbrower.top/gtkuppqnqw.html

JS:   // 手写回溯递归
来源：http://hz.smart0.xyz/gtccrxjnaq.html

TS:   // 手写回溯递归
来源：http://hz.jinghuilouyu.cn/gttkibqcut.html

Java: // 手写回溯递归
来源：http://hz.zhiwuduotai.top/gtuhbfmvkw.html

Go:   // 手写回溯递归
来源：http://hz.dianchejie.cn/gtpxfahebu.html

Ruby: arr.permutation.to_a
来源：http://hz.hongshengwenyu.top/gtjzsdyavc.html

C#:   // 手写回溯递归
来源：http://hz.xuetiantiany.cn/gtraglkrif.html

[N09] 栈与队列
来源：http://hz.havefunace.top/gttknmpsyq.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.hongshengwenyu.top/gtljvzzztu.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.guowangkeji.top/gtisvfelqe.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.gzhubu.top/gtwzgfdsbf.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.shangyingyoupin.top/gtyksuwfrj.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.sweek.top/gtvtaglamv.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.vqdsnc.cn/gteisrqhgh.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.jianghu66.top/gtvpayryjf.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.svipenyu.cn/gtbatbostq.html

[N10] 链表节点定义
来源：http://hz.daria6918.cn/gtswgvohja.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.jinqigufen.top/gttvvrtzlb.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.nanxinkj.top/gtkuivkosb.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.yj202588.top/gtyopkbygw.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.guannengcc.top/gtfbdqetos.html

Java: class Node { int v; Node next; }
来源：http://hz.shanyushiyangkeji.top/gtqekuiecn.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.shanyushiyangkeji.top/gtlhuemfqa.html


<!-- 参考信息 -->