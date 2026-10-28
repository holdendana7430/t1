代发 wailian999

TS:   JSON.parse(s)
来源：http://hz.yvedp.cn/gtkjiyahez.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.yueranfly.top/gttoulcvqi.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.cheryme.top/gtnqqnfxpi.html

Ruby: JSON.parse(s)
来源：http://hz.redwolf501.top/gtcydkvlfb.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.tian-w.cn/gtevgoevbc.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.cashguo.top/gtomcwlcjw.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.hnqzz.top/gtzeczneoc.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.fengsongda.top/gtkqdgiuqt.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.zhiwuduotai.top/gtarjfeybm.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.9152youxi.cn/gtpzxgmhji.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.yangfankeji.com/gtsbbztyev.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.yj20258.top/gtylkyuaqt.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.zhoulong.xyz/gtvefkhllt.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.havefunace.top/gtvoepkfbx.html

[K04] 读取 JSON 文件
来源：http://hz.chenlongwang.top/gtdyybbkgj.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.tianlin.xyz/gtplfpvkpv.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.yonumen.top/gtwteyypdi.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.ydzc1.top/gtbeqwvqgj.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.ywan-chungtsiang.top/gtggmkruxa.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.zhiwuduotai.top/gtehbhdymp.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.hywenlv.cn/gtrzomledm.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.dashuyun.cn/gtgorlupit.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.hnxiangtu.top/gtrrqqyfwe.html

[K05] 深拷贝对象
来源：http://hz.pengpengdd.cyou/gtvzsgnjxs.html

Py:   copy.deepcopy(obj)
来源：http://hz.yj20258.top/gteooccwee.html

PHP:  unserialize(serialize($obj));
来源：http://hz.yj202588.top/gtulnrzxun.html

JS:   structuredClone(obj)
来源：http://hz.0kj1m.cn/gthnxghffy.html

TS:   structuredClone(obj)
来源：http://hz.hammf.cn/gtaoxwsfca.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.xuetiantiany.cn/gtjefzeojo.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.ywan-chungtsiang.top/gtnjtpxuqy.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.snrcjt.cn/gtnezdgmja.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.cqqwz.cn/gtmtuotwyg.html

[K06] 解析 URL 查询串
来源：http://hz.hammf.cn/gtkgjfahjq.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.shanyushiyangkeji.top/gtpqweafzg.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.pengpengdd.cyou/gttdnumxdg.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zhijiandao.cn/gtcrtfxcrg.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.cheryme.top/gttdkjtwsy.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.bjfxy.top/gtvhoxuljy.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.hfpthk.cn/gtienzktqr.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.jinyuanbaomall.cn/gtmxnjqpbm.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.nanxinkj.top/gtbnjtwsdc.html

[K07] 进制转换
来源：http://hz.zdqjudy.top/gtcneuyezq.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.hywenlv.cn/gtanxpgdms.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.ehwqpu.com/gtkwvhtmyy.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.cheryme.top/gtercyazgi.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.cdnleiting.top/gtkrurfffr.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.cqqwz.cn/gtvhlytdxa.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.yj202588.top/gteacrnbtz.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.sxryk.cn/gtbykghwds.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.birdmap.top/gtdshdwlfl.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.dianchejie.cn/gtgcswypxo.html

Py:   pickle.dumps(obj)
来源：http://hz.sweek.top/gtychhywfm.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.chenjidiqi.icu/gtrwnntajb.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.zhaomingkeji.xyz/gtdsijcrro.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.ehwqpu.com/gtzvfbjsll.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.zhixingplan.top/gtqilxwxqe.html

Go:   encoding/gob
来源：http://hz.chenjidiqi.icu/gtwdzdbsmm.html

Ruby: Marshal.dump(obj)
来源：http://hz.ehwqpu.com/gtaooiswty.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.xuanzx.com/gtfffwnmel.html

================================================================================
来源：http://hz.hnxiangtu.top/gtsqbjpdhz.html

L. 网络请求
来源：http://hz.c1oappe.top/gtucqezqat.html

================================================================================
来源：http://hz.daxiang520.top/gtrowccimt.html

[L01] 发送 GET 请求
来源：http://hz.shanyushiyangkeji.top/gtdtkhjmuf.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.xuetiantiany.cn/gtitukmvyh.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.pycfn.com/gthrkzwcsj.html

JS:   await fetch(url)
来源：http://hz.0kj1m.cn/gtshwhdpbe.html

TS:   await fetch(url)
来源：http://hz.dashuyun.cn/gtwidcwggw.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.shanyushiyangtech.top/gtuwnsqpjj.html

Go:   resp, err := http.Get(url)
来源：http://hz.jyoumei.cn/gtrfltzycc.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.shangyingyoupin.top/gtjcwhcqjz.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.sxryk.cn/gtcndrwlci.html

[L02] 发送 POST JSON
来源：http://hz.zhengqikj.top/gthkehvhyc.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.haohaochexian.top/gtmiagpuyq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.chenzaomai.com/gtarpatiwr.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.tian-w.cn/gtctutdtuv.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.c1oappe.top/gttxistyhk.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.ydzc1.top/gtypkobolw.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.zhijiandao.cn/gtyittcvbd.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.sxryk.cn/gtgrfkflra.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.tanke756.top/gtizrmkhnu.html

[L03] 设置自定义请求头
来源：http://hz.pengpengdd.cyou/gtpaouxoew.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.xuanzx.com/gtiolmloix.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.zycfv.cn/gtnqgxmocs.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.nanxuanxn.top/gtntuhvael.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jiagoushi.top/gtnatilhyk.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.ydjk.org.cn/gtcpdbbveg.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.chenzaomai.com/gtmiopgpwy.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.ydzc1.top/gtfcesgque.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.tian-w.cn/gtoqkmavan.html

[L04] 设置超时
来源：http://hz.nanxinkj.top/gtcmdtgkyn.html

Py:   requests.get(url, timeout=5)
来源：http://hz.shanyushiyangtech.top/gtalnyasne.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.yuanzhike.top/gtbmrwktih.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.hongshengwenyu.top/gtwwdxoqis.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.gaohongyu789.top/gtluimdhme.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.zhijiandao.cn/gtrzqpnubi.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.xuanzx.com/gtoyefpoid.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.0kj1m.cn/gthouaqqhi.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.wangdashe.top/gtfxxfpafc.html

[L05] 上传文件（multipart）
来源：http://hz.nanxuanxn.top/gtewuyyyjc.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.sufxvd.cn/gtghvezwfi.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.9152youxi.cn/gtffvgbfar.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.ehwqpu.com/gtzeklzttq.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.guowangkeji.top/gtjnjrdpim.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.hysaishi.cn/gtpfvppfqu.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.smart0.xyz/gtjcrxenbp.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.smart0.xyz/gtsjmaihlo.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.tianlin.xyz/gtwnkxkhes.html

[L06] 解析响应为 JSON
来源：http://hz.gaohongyu789.top/gtrzqmrcwm.html

Py:   resp.json()
来源：http://hz.yongpay.top/gtvbdmzpnm.html

PHP:  json_decode($body, true);
来源：http://hz.zhongyouzk.top/gtusirshkc.html

JS:   await resp.json()
来源：http://hz.jlsjyb.cn/gtmuxcruyp.html

TS:   await resp.json()
来源：http://hz.c1oappe.top/gtcrwsrngn.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.c1oappe.top/gtwpnitqqn.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.ydjk.org.cn/gtuamczkqk.html

Ruby: JSON.parse(resp.body)
来源：http://hz.meibo888.top/gtcvsyfyzc.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.kuanghao11.cn/gtoluqyvdd.html

[L07] 处理 HTTP 状态码
来源：http://hz.guowangkeji.top/gtyhhyopky.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.zhixingplan.top/gttlvnjdye.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.xuetiantiany.cn/gtkoprgazf.html

JS:   resp.ok;  resp.status
来源：http://hz.sweek.top/gtxkzconem.html

TS:   resp.ok;  resp.status
来源：http://hz.gaohongyu789.top/gtpzygmrut.html

Java: resp.statusCode()
来源：http://hz.feifeiyinyue.top/gtgzriyllq.html

Go:   resp.StatusCode
来源：http://hz.ybcxt.top/gtekrwaspg.html

Ruby: resp.code.to_i
来源：http://hz.52xcode.cn/gtjqbcckzy.html

C#:   (int)resp.StatusCode
来源：http://hz.xylfe.cn/gtdgcqdjkz.html

[L08] 并发请求多个地址
来源：http://hz.jinyuanbaomall.cn/gtpbeehdfv.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.cucudq.cn/gtuzesaeyv.html

PHP:  curl_multi_init() 系列
来源：http://hz.chenzaomai.com/gtfuggyxnj.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.fzhhl.top/gtpvgwsspu.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yvedp.cn/gtlvroawlv.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.jqgufenzy.top/gtqkijdqcz.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.cheryme.top/gtqtnfbwoq.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.hnqzz.top/gtoxabxega.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.ydzc1.top/gtgtdbqgvx.html

================================================================================
来源：http://hz.c1oappe.top/gtttmksbfc.html

M. 命令行 / 进程 / 环境
来源：http://hz.havefunace.top/gtvafptznt.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtixrutxre.html

[M01] 读取命令行参数
来源：http://hz.aizwys.cn/gtvqxsnzhq.html

Py:   sys.argv[1:]
来源：http://hz.nwbrower.top/gtvognbkhe.html

PHP:  $argv;  $argc;
来源：http://hz.gzhubu.top/gtgrsoyubh.html

JS:   process.argv.slice(2)
来源：http://hz.sxryk.cn/gtsuellefx.html

TS:   process.argv.slice(2)
来源：http://hz.shanyushiyangkeji.top/gtyuekqrsd.html

Java: args 数组（main 方法参数）
来源：http://hz.pengpengdd.cyou/gtgvhjeoge.html

Go:   os.Args[1:]
来源：http://hz.sysykeji.top/gtereocgfg.html

Ruby: ARGV
来源：http://hz.cqqwz.cn/gttneyfull.html

C#:   args 数组（Main 方法参数）
来源：http://hz.tanke756.top/gtvkqhafqo.html

[M02] 读取环境变量
来源：http://hz.nanxuanxn.top/gtehobopov.html

Py:   os.environ.get("HOME")
来源：http://hz.nanxinkj.top/gtjlkrwunw.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.yj20258888.top/gtwgsnpudx.html

JS:   process.env.HOME
来源：http://hz.jlsjyb.cn/gtljvfrsnt.html

TS:   process.env.HOME
来源：http://hz.feifeiyinyue.top/gttqpcprgf.html

Java: System.getenv("HOME")
来源：http://hz.redwolf501.top/gtcszauxmz.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.jinqigfzy.top/gtkvnkqpxt.html

Ruby: ENV["HOME"]
来源：http://hz.shangyingyoupin.top/gtgiseuijj.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.zhengqikj.top/gtskheagkm.html

[M03] 执行外部命令
来源：http://hz.sysykeji.top/gtgngymxck.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.havefunace.top/gtpxdtabzv.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.yuxming.cn/gthggwbqil.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.zdqjudy.top/gtbdqwdftc.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.cashguo.top/gtmywexunu.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.vqdsnc.cn/gtgrddsfes.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.xuetiantiany.cn/gtqkhkzaff.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.snrcjt.cn/gtcyyaoaly.html

C#:   Process.Start("ls", "-l");
来源：http://hz.jlsjyb.cn/gtvplasqhq.html

[M04] 获取当前工作目录
来源：http://hz.snrcjt.cn/gtmzkqmhvo.html

Py:   os.getcwd()
来源：http://hz.tian-w.cn/gtnqkhttbk.html

PHP:  getcwd();
来源：http://hz.52xcode.cn/gtcrhakqtf.html

JS:   process.cwd()
来源：http://hz.aizwys.cn/gttclndzjq.html

TS:   process.cwd()
来源：http://hz.quarkkingdee.top/gtvbrsukov.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.birdmap.top/gtozxyljop.html

Go:   os.Getwd()
来源：http://hz.andypj.xyz/gtcpofdkst.html

Ruby: Dir.pwd
来源：http://hz.vqdsnc.cn/gtbenrrajs.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.zhixingplan.top/gthhiceyjb.html

[M05] 设置退出码
来源：http://hz.ydjk.org.cn/gtfnezmxvd.html

Py:   sys.exit(1)
来源：http://hz.hongshengwenyu.top/gtzcnihrjf.html

PHP:  exit(1);
来源：http://hz.cqqwz.cn/gtujcghcxf.html

JS:   process.exit(1)
来源：http://hz.yj20258.top/gtufybwjca.html

TS:   process.exit(1)
来源：http://hz.sysykeji.top/gtpgquqqsk.html

Java: System.exit(1)
来源：http://hz.wangshuangyany.cn/gtjxzmeozu.html

Go:   os.Exit(1)
来源：http://hz.ppjwa.cn/gtvldtcbmv.html

Ruby: exit 1
来源：http://hz.hnqzz.top/gtkyqnabua.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.52xcode.cn/gttgdxuzai.html

[M06] 向标准错误输出
来源：http://hz.jqgfzy.top/gtexvsbdrr.html

Py:   print("err", file=sys.stderr)
来源：http://hz.nwbrower.top/gtmdmyquyc.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.zhiwuduotai.top/gtryaytmsi.html

JS:   console.error("err")
来源：http://hz.nanxuanxn.top/gtbwxzdiov.html

TS:   console.error("err")
来源：http://hz.shuidangran.top/gtoxejqftx.html

Java: System.err.println("err")
来源：http://hz.gzhubu.top/gtklipzgkx.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.nanxinkj.top/gtxmnoyrru.html

Ruby: warn "err"
来源：http://hz.sweek.top/gtqtatfviw.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.haohaochexian.top/gtbvjpqszi.html

[M07] 判断是否为主入口
来源：http://hz.pengpengdd.cyou/gtylipwrsj.html

Py:   if __name__ == "__main__":
来源：http://hz.hnxiangtu.top/gtpoilafaj.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.sweek.top/gtogwpksxb.html

JS:   require.main === module
来源：http://hz.zhoulong.xyz/gtnfvfvtfd.html

TS:   require.main === module
来源：http://hz.shanyushiyangtech.top/gteibmaqzh.html

Java: public static void main(String[] args)
来源：http://hz.yuxming.cn/gtsgjcnumv.html

Go:   func main()
来源：http://hz.hammf.cn/gtjelokmnt.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.sxryk.cn/gtccqrgxjx.html

C#:   static void Main(string[] args)
来源：http://hz.9152youxi.cn/gtkgruowuw.html

[M08] 获取系统与运行时信息
来源：http://hz.iojbl.cn/gtboxgwygr.html

Py:   platform.system();  platform.python_version()
来源：http://hz.cdnleiting.top/gtlqvdrdjy.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.nanxinkj.top/gtysiyvzmw.html

JS:   process.platform;  process.version
来源：http://hz.ehwqpu.com/gtutonmydb.html

TS:   process.platform;  process.version
来源：http://hz.xinyue.icu/gtyryqmqsz.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.ybcxt.top/gtpjldqpok.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.bjfxy.top/gtywbntzjx.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.smart0.xyz/gteksofltp.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.meibo888.top/gtsdjpojbe.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtljjfdhnt.html

N. 数据结构与算法
来源：http://hz.iojbl.cn/gtiukjtawl.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtsjxgjvom.html

[N01] 二分查找（有序数组）
来源：http://hz.yanxiufei.cn/gtsamffvzm.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.xinyue.icu/gtfdhdlwbf.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.jinghuilouyu.cn/gtstjxtemg.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zhengqikj.top/gtwbpocoxd.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.52xcode.cn/gtraibwxsi.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.hysaishi.cn/gticwjoyns.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.vqdsnc.cn/gthvhehjfx.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.zhixingplan.top/gtiyqdguxs.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.birdmap.top/gtbfvqvmbe.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.shangyingyoupin.top/gtqjtolepl.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.wangdashe.top/gttodfbtrr.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.fengsongda.top/gtzlckrcjv.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.snrcjt.cn/gteshjpxsd.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.smart0.xyz/gtikwwhfie.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.bjfxy.top/gtczqyctyx.html

Go:   slices.Sort(arr)
来源：http://hz.tanke756.top/gteuyaccil.html

Ruby: arr.sort
来源：http://hz.sweek.top/gtdxywobmq.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.nanxuanxn.top/gtozzjgkab.html

[N03] 快速排序（分治示例）
来源：http://hz.c1oappe.top/gtserftzkx.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.sufxvd.cn/gtomdijzhi.html

PHP:  // 递归实现，或用 usort
来源：http://hz.hnxiangtu.top/gtmxraexuy.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.dashuyun.cn/gtqpiapimj.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.ppjwa.cn/gtmwzfwcpr.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.pycfn.com/gtyzoljiiq.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.yangfankeji.com/gtwulcoopw.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.yuanzhike.top/gteyzxltdn.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.c1oappe.top/gtanqcqvxs.html

[N04] 斐波那契数列
来源：http://hz.guowangkeji.top/gtgrzrfvhr.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.guannengcc.top/gtslebvijh.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.ehwqpu.com/gtcphscqcx.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.hfpthk.cn/gtpouboabw.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.smart0.xyz/gtpnxtnnmz.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.chenlongwang.top/gttfnczelp.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.gotoacloud.top/gtdxjcbwsq.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.redwolf501.top/gteyvtmsoy.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.sxryk.cn/gtfainzadp.html

[N05] 最大公约数
来源：http://hz.yj20258888.top/gtuwkhbrcq.html

Py:   math.gcd(a, b)
来源：http://hz.hammf.cn/gtfrshrpmf.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.52xcode.cn/gtrroladts.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.aibaodan.cn/gtreynqoew.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.nanxinkj.top/gtqeuctstf.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.tianlin.xyz/gtiopjafvv.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.andypj.xyz/gtcxmclbsg.html

Ruby: a.gcd(b)
来源：http://hz.xuetiantiany.cn/gtzaogqacd.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.ydjk.org.cn/gtivaphesd.html

[N06] 判断回文字符串
来源：http://hz.jianghu66.top/gtiseqvdlj.html

Py:   s == s[::-1]
来源：http://hz.mhx1999.top/gtfqzydgkl.html

PHP:  $s === strrev($s);
来源：http://hz.aizwys.cn/gttjpllajp.html

JS:   s === [...s].reverse().join("")
来源：http://hz.yuanzhike.top/gtfdqsgdbn.html

TS:   s === [...s].reverse().join("")
来源：http://hz.havefunace.top/gtwkpgjkyo.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.jiagoushi.top/gtprejacra.html

Go:   // 双指针从两端比较
来源：http://hz.zhongyouzk.top/gtmjgfewye.html

Ruby: s == s.reverse
来源：http://hz.ydjk.org.cn/gtfvnzkmhe.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.gaohongyu789.top/gtsfuskavy.html

[N07] 两数之和（返回下标）
来源：http://hz.jinqigfzy.top/gtpnzvwnnq.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.sweek.top/gtrqxamqvq.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.cdnleiting.top/gtcmslmflo.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.snrcjt.cn/gtmqxdhikn.html

TS:   // 手写 Map<string, number>
来源：http://hz.mhx1999.top/gtfxtwvubb.html

Java: // 手写 HashMap
来源：http://hz.shangyingyoupin.top/gtezyzwvlt.html

Go:   // 手写 map[int]int
来源：http://hz.dianchejie.cn/gtrdudqsbe.html

Ruby: // 手写 Hash
来源：http://hz.jyoumei.cn/gtjrexkpkd.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.jinqigfzy.top/gtynvxnkbt.html

[N08] 生成全排列
来源：http://hz.jqgufenzy.top/gtljuawhdo.html

Py:   itertools.permutations(arr)
来源：http://hz.9152youxi.cn/gtkfyyhztf.html

PHP:  // 手写递归交换
来源：http://hz.shuidangran.top/gtbuedxsgs.html

JS:   // 手写回溯递归
来源：http://hz.hywenlv.cn/gtsriuusqb.html

TS:   // 手写回溯递归
来源：http://hz.quarkkingdee.top/gttoktjhpa.html

Java: // 手写回溯递归
来源：http://hz.c1oappe.top/gtcomkmgnx.html

Go:   // 手写回溯递归
来源：http://hz.yuanzhike.top/gtgpbwthga.html

Ruby: arr.permutation.to_a
来源：http://hz.daxiang520.top/gtvsnovyie.html

C#:   // 手写回溯递归
来源：http://hz.haohaochexian.top/gtuldkxvhf.html

[N09] 栈与队列
来源：http://hz.gotoacloud.top/gtiioneqfs.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.gogol.net.cn/gtpisbkrhc.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.cheryme.top/gtxjxyupei.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.zhoulong.xyz/gtgahqfrwo.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.yangfankeji.com/gtczddlxhy.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.hnqzz.top/gtljrrmeur.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.shangyingyoupin.top/gtvfohzxnw.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.yuanzhike.top/gtrnwqrips.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.havefunace.top/gtxrbnmimz.html

[N10] 链表节点定义
来源：http://hz.zhijiandao.cn/gtepaujjss.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.kuanghao11.cn/gtojmyknjl.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.hongshengwenyu.top/gthmswtcvo.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.jinghuilouyu.cn/gtnjqcpmur.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.0kj1m.cn/gtwkeewigs.html

Java: class Node { int v; Node next; }
来源：http://hz.shangyingyoupin.top/gtuotigeur.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.smart0.xyz/gtqbevzrkn.html


<!-- 参考信息 -->