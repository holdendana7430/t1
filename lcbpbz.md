代发 wailian999

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.chenjidiqi.icu/gtceewijxc.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.dashuyun.cn/gteusknehr.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.aizwys.cn/gtawsymfvt.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.zhiwuduotai.top/gtgrdwjcmd.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.xinyue.icu/gtdvnhfhcx.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.dashuyun.cn/gtftxknjvl.html

[K04] 读取 JSON 文件
来源：http://hz.xziqi.cn/gtpfrttmsm.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.bjfxy.top/gtedshefuy.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.ivvv.top/gtcqwnzqrs.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.xuetiantiany.cn/gtumesnjny.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.aibaodan.cn/gtnmrbnrpk.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.gzhubu.top/gthtwukzyu.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.gaohongyu789.top/gtpzqegcyc.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.zhoulong.xyz/gteqytbwqi.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.jinyuanbaomall.cn/gtgmwlsegy.html

[K05] 深拷贝对象
来源：http://hz.haohaochexian.top/gtkogwoikf.html

Py:   copy.deepcopy(obj)
来源：http://hz.hnqzz.top/gttwhkggmc.html

PHP:  unserialize(serialize($obj));
来源：http://hz.guowangkeji.top/gtqlqutfiz.html

JS:   structuredClone(obj)
来源：http://hz.ehwqpu.com/gtfyffmooh.html

TS:   structuredClone(obj)
来源：http://hz.sysykeji.top/gtfgijcrri.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.zhengqikj.top/gtucrsclpj.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.52xcode.cn/gtkwuiyzen.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.gogol.net.cn/gtodujcvxg.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.redwolf501.top/gtqeghxaqn.html

[K06] 解析 URL 查询串
来源：http://hz.tanke756.top/gtiyoadvqi.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.cashguo.top/gtlikvuuaj.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.wangdashe.top/gttwqopyze.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.0kj1m.cn/gtnftcjxmp.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.sweek.top/gtlrhtskhf.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.chenzaomai.com/gtpndkfzwa.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.jianghu66.top/gtfonhfsvr.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.gogol.net.cn/gtsepvdruh.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.yj202588.top/gtjvrpmhwh.html

[K07] 进制转换
来源：http://hz.pycfn.com/gtnnjwzfan.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.hnqzz.top/gtltpnnfnw.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.xziqi.cn/gtfxbtrkvm.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.ywan-chungtsiang.top/gttdaylagj.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.xinyue.icu/gtsxfnkkbj.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.smart0.xyz/gtyyzlemvm.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.chenlongwang.top/gtbmadzcue.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.shangyingyoupin.top/gtwfyofgld.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.hnxiangtu.top/gttrbfnopj.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.ppjwa.cn/gtoszxayfq.html

Py:   pickle.dumps(obj)
来源：http://hz.xingfuxueyuan.xyz/gtvycodfpo.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.dianchejie.cn/gtlqumwnrd.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.shanyushiyangkeji.top/gtqthnurwm.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.quarkkingdee.top/gteydvrcej.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.ydzc1.top/gthsuulofx.html

Go:   encoding/gob
来源：http://hz.gaohongyu789.top/gtcmhfggua.html

Ruby: Marshal.dump(obj)
来源：http://hz.yj202588.top/gtuacxlcge.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.fengsongda.top/gtyggwnbxz.html

================================================================================
来源：http://hz.0kj1m.cn/gtzwbgzawv.html

L. 网络请求
来源：http://hz.sufxvd.cn/gtxxsyuvfr.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtkyfblyca.html

[L01] 发送 GET 请求
来源：http://hz.zhijiandao.cn/gtlrcbnvee.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.chenjidiqi.icu/gtbfedjyky.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.zhaomingkeji.xyz/gtlkssgimn.html

JS:   await fetch(url)
来源：http://hz.jianghu66.top/gtkazecypp.html

TS:   await fetch(url)
来源：http://hz.jqgufenzy.top/gtuthatpjh.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.aibaodan.cn/gtziupkjbn.html

Go:   resp, err := http.Get(url)
来源：http://hz.ybcxt.top/gtmbzfflcg.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.tanke756.top/gtkyaqnmxi.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.daxiang520.top/gtuvdqhrzo.html

[L02] 发送 POST JSON
来源：http://hz.zhongyouzk.top/gtibgfzdfk.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.ivvv.top/gtwgwsepbo.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.sweek.top/gtqkzzzvqa.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jinqigufen.top/gtsffzxqtl.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.fzhhl.top/gtghwkqajo.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.andypj.xyz/gtimmwgkjf.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.jlsjyb.cn/gtjxbrwkau.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.wangdashe.top/gteyqlbfys.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.chenlongwang.top/gtsqxebafc.html

[L03] 设置自定义请求头
来源：http://hz.nwbrower.top/gtejqjfjoy.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.guannengcc.top/gtwroapxck.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.ydzc1.top/gtfhmhtasi.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.fzhhl.top/gtzmdjycbz.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jinghuilouyu.cn/gtldcphwfe.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.feifeiyinyue.top/gtzqhsmwyu.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.shuidangran.top/gtqwcrclbe.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.aizwys.cn/gtatseojpt.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.hnxiangtu.top/gtunjhtrvn.html

[L04] 设置超时
来源：http://hz.redwolf501.top/gtmcyzczkw.html

Py:   requests.get(url, timeout=5)
来源：http://hz.jinghuilouyu.cn/gtzmjuykrm.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.cheryme.top/gtlpclwghs.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.hammf.cn/gtuclaqfuj.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zhixingplan.top/gtotdehmro.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.iojbl.cn/gtdrlrohdy.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.yangfankeji.com/gtyiklctcp.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.ydzc1.top/gtgbumzuzl.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.hnxiangtu.top/gtgqlayvcu.html

[L05] 上传文件（multipart）
来源：http://hz.yangfankeji.com/gtjypbmrcg.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.fzhhl.top/gtwdsvrmkr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.sweek.top/gtyghbbpef.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.kuanghao11.cn/gtbzzglvld.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.hywenlv.cn/gtujzvfivv.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.hongshengwenyu.top/gtudbqaxjn.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.shanyushiyangtech.top/gtwgeaxcif.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.nanxinkj.top/gtbdihfrgv.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.jyoumei.cn/gtfqldpobg.html

[L06] 解析响应为 JSON
来源：http://hz.havefunace.top/gtqgczbyua.html

Py:   resp.json()
来源：http://hz.vqdsnc.cn/gtrfkfacuv.html

PHP:  json_decode($body, true);
来源：http://hz.wangshuangyany.cn/gttrivprcl.html

JS:   await resp.json()
来源：http://hz.jqgfzy.top/gtffjwqzkz.html

TS:   await resp.json()
来源：http://hz.jiagoushi.top/gtgzjvsuex.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.hnqzz.top/gtpdeexmux.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.chenlongwang.top/gtddhkasgk.html

Ruby: JSON.parse(resp.body)
来源：http://hz.jqgfzy.top/gtabadjtxq.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.9152youxi.cn/gtlywojbgh.html

[L07] 处理 HTTP 状态码
来源：http://hz.jinghuilouyu.cn/gtptftiywf.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.yongpay.top/gtmtldbwfq.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.ydjk.org.cn/gtmegeofzz.html

JS:   resp.ok;  resp.status
来源：http://hz.guowangkeji.top/gtvsallyff.html

TS:   resp.ok;  resp.status
来源：http://hz.ydzc1.top/gtxnwsyarx.html

Java: resp.statusCode()
来源：http://hz.yongpay.top/gtzvqmynsu.html

Go:   resp.StatusCode
来源：http://hz.c1oappe.top/gtfuocsmri.html

Ruby: resp.code.to_i
来源：http://hz.haohaochexian.top/gtwalqgdus.html

C#:   (int)resp.StatusCode
来源：http://hz.jianghu66.top/gtponqgxtm.html

[L08] 并发请求多个地址
来源：http://hz.zhongyouzk.top/gtghgkuhrg.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.zdqjudy.top/gtmdowcnfr.html

PHP:  curl_multi_init() 系列
来源：http://hz.zdqjudy.top/gtfrkfquzx.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.hfpthk.cn/gtrrayiwfb.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.cdnleiting.top/gtszsubqvb.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.xuetiantiany.cn/gtmwcxjlqu.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.nanxuanxn.top/gtvzjhlgax.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.jqgfzy.top/gtjxtubqfe.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.yj20258888.top/gtsokkdpsy.html

================================================================================
来源：http://hz.zycfv.cn/gtbpxqasyo.html

M. 命令行 / 进程 / 环境
来源：http://hz.gogol.net.cn/gtgwmkrfyr.html

================================================================================
来源：http://hz.hfpthk.cn/gtkisvxlpk.html

[M01] 读取命令行参数
来源：http://hz.sweek.top/gthknlkbnm.html

Py:   sys.argv[1:]
来源：http://hz.sweek.top/gtrwbnzsnz.html

PHP:  $argv;  $argc;
来源：http://hz.smart0.xyz/gttujofbla.html

JS:   process.argv.slice(2)
来源：http://hz.hfpthk.cn/gtixyepnfc.html

TS:   process.argv.slice(2)
来源：http://hz.iojbl.cn/gttdhnddfh.html

Java: args 数组（main 方法参数）
来源：http://hz.c1oappe.top/gtflfbvtie.html

Go:   os.Args[1:]
来源：http://hz.svipenyu.cn/gtahmaehau.html

Ruby: ARGV
来源：http://hz.kuanghao11.cn/gtgugdidrv.html

C#:   args 数组（Main 方法参数）
来源：http://hz.yanxiufei.cn/gtzhpatozr.html

[M02] 读取环境变量
来源：http://hz.hywenlv.cn/gtcukfpcgt.html

Py:   os.environ.get("HOME")
来源：http://hz.hammf.cn/gtrlvuacrw.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.feifeiyinyue.top/gtfyoosloz.html

JS:   process.env.HOME
来源：http://hz.wangdashe.top/gtzuzaklub.html

TS:   process.env.HOME
来源：http://hz.jianghu66.top/gtowyleyqs.html

Java: System.getenv("HOME")
来源：http://hz.yanxiufei.cn/gtpyrbbmky.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.aibaodan.cn/gtkedjnsla.html

Ruby: ENV["HOME"]
来源：http://hz.jqgufenzy.top/gtenjnvkrd.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.ivvv.top/gticvclqen.html

[M03] 执行外部命令
来源：http://hz.bjfxy.top/gtqsdmqswa.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.wangdashe.top/gtknazcvht.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.yanxiufei.cn/gtpaxvmhci.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.tanke756.top/gtotzyyibn.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.cashguo.top/gtljqsyrfk.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.hfpthk.cn/gtibjxaglu.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.yuxming.cn/gtbtplcqnm.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.xylfe.cn/gtslqywhps.html

C#:   Process.Start("ls", "-l");
来源：http://hz.ppjwa.cn/gtrkskjpim.html

[M04] 获取当前工作目录
来源：http://hz.pengpengdd.cyou/gtrvvnqzgx.html

Py:   os.getcwd()
来源：http://hz.pycfn.com/gtfyoygsum.html

PHP:  getcwd();
来源：http://hz.xingfuxueyuan.xyz/gtihorapct.html

JS:   process.cwd()
来源：http://hz.zhaomingkeji.xyz/gtssdyhmmk.html

TS:   process.cwd()
来源：http://hz.yj20258.top/gtevyrouze.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.xuanzx.com/gtcwnqovfs.html

Go:   os.Getwd()
来源：http://hz.fzhhl.top/gtxlwminec.html

Ruby: Dir.pwd
来源：http://hz.redwolf501.top/gtaqwualfa.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.fzhhl.top/gtmjbbjmrf.html

[M05] 设置退出码
来源：http://hz.feifeiyinyue.top/gtabvcljrk.html

Py:   sys.exit(1)
来源：http://hz.cashguo.top/gteuwlmzft.html

PHP:  exit(1);
来源：http://hz.redwolf501.top/gtdnkldfsb.html

JS:   process.exit(1)
来源：http://hz.smart0.xyz/gtnqffvksy.html

TS:   process.exit(1)
来源：http://hz.316326.xyz/gtmjzsedyl.html

Java: System.exit(1)
来源：http://hz.yvedp.cn/gtfoqrjgjl.html

Go:   os.Exit(1)
来源：http://hz.zhaomingkeji.xyz/gtnkvxyykn.html

Ruby: exit 1
来源：http://hz.feifeiyinyue.top/gteiqrxxcg.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.guannengcc.top/gtndgklrgc.html

[M06] 向标准错误输出
来源：http://hz.jqgufenzy.top/gticmvpwpi.html

Py:   print("err", file=sys.stderr)
来源：http://hz.redwolf501.top/gtybvohere.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.cheryme.top/gtyehihhui.html

JS:   console.error("err")
来源：http://hz.jinqigufen.top/gtshekvxil.html

TS:   console.error("err")
来源：http://hz.wangshuangyany.cn/gtwbonfeuw.html

Java: System.err.println("err")
来源：http://hz.tanke756.top/gtuuqllres.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.cashguo.top/gtanthnbqx.html

Ruby: warn "err"
来源：http://hz.shangyingyoupin.top/gtpbzmrulh.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.ybcxt.top/gtxuqeegga.html

[M07] 判断是否为主入口
来源：http://hz.redwolf501.top/gtwsidbnsv.html

Py:   if __name__ == "__main__":
来源：http://hz.zdqjudy.top/gtcmnmzmfy.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.cheryme.top/gtvcgeyqti.html

JS:   require.main === module
来源：http://hz.nwbrower.top/gtjyxxezhn.html

TS:   require.main === module
来源：http://hz.mhx1999.top/gtltymrpvz.html

Java: public static void main(String[] args)
来源：http://hz.xuanzx.com/gtgswdnarw.html

Go:   func main()
来源：http://hz.cucudq.cn/gticsnngci.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.hnqzz.top/gteflayhuv.html

C#:   static void Main(string[] args)
来源：http://hz.dashuyun.cn/gtoqiusnof.html

[M08] 获取系统与运行时信息
来源：http://hz.zhixingplan.top/gtfrxzeiwu.html

Py:   platform.system();  platform.python_version()
来源：http://hz.iojbl.cn/gtwbtqczan.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.ppjwa.cn/gtqmfbmbhl.html

JS:   process.platform;  process.version
来源：http://hz.chenlongwang.top/gtgnnyhkif.html

TS:   process.platform;  process.version
来源：http://hz.gotoacloud.top/gtxaingebd.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.hysaishi.cn/gtobevzppz.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.52xcode.cn/gtmxzfxrgk.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.jianghu66.top/gtgmbtlaku.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.mhx1999.top/gtriaptyip.html

================================================================================
来源：http://hz.daxiang520.top/gtrwpythmb.html

N. 数据结构与算法
来源：http://hz.kuanghao11.cn/gtwqmvrpgv.html

================================================================================
来源：http://hz.meibo888.top/gtjtfyfnys.html

[N01] 二分查找（有序数组）
来源：http://hz.zhengqikj.top/gthlrrwqxb.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.sufxvd.cn/gtrwlclhxt.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.zhixingplan.top/gtwwhuoksb.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.ehwqpu.com/gtrvjytpud.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.shanyushiyangtech.top/gtptnplkom.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.9152youxi.cn/gtobztyieb.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.cheryme.top/gtraukgjho.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.gotoacloud.top/gtdqbfvjaz.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.ydjk.org.cn/gtinvchksa.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.hywenlv.cn/gtsatcatbi.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jqgfzy.top/gtbljuibwl.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.c1oappe.top/gtfnvsblgd.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.gotoacloud.top/gtrbegmith.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.0kj1m.cn/gtlapaqygr.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.dianchejie.cn/gtwunipmts.html

Go:   slices.Sort(arr)
来源：http://hz.hywenlv.cn/gtlkerrngn.html

Ruby: arr.sort
来源：http://hz.jiagoushi.top/gtcfocirkz.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.xuanzx.com/gtjllbofqj.html

[N03] 快速排序（分治示例）
来源：http://hz.xuetiantiany.cn/gtpefvxkdd.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.hnxiangtu.top/gtfsafpyou.html

PHP:  // 递归实现，或用 usort
来源：http://hz.dashuyun.cn/gtquorpyio.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.guowangkeji.top/gtqjhdyijb.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.chenlongwang.top/gtubjkvado.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.sysykeji.top/gtxlaoroth.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.pengpengdd.cyou/gtikhmlftn.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.zhaomingkeji.xyz/gtwszcmcuo.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.shuidangran.top/gtqzyubqmq.html

[N04] 斐波那契数列
来源：http://hz.fzhhl.top/gtmhvtgopb.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.zdqjudy.top/gtimtxbmfu.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.jqgfzy.top/gtjpeeeerp.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jinghuilouyu.cn/gtqkbhuheg.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.xziqi.cn/gtvlqppnif.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.ehwqpu.com/gtgzluvztf.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.shangyingyoupin.top/gtzytyawno.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.kuanghao11.cn/gtvbcrcxhb.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.xingfuxueyuan.xyz/gtfiqeejgq.html

[N05] 最大公约数
来源：http://hz.chenjidiqi.icu/gtjkvcgkkv.html

Py:   math.gcd(a, b)
来源：http://hz.fengsongda.top/gthsehculr.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.shanyushiyangkeji.top/gtnhtywjxb.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.svipenyu.cn/gtmaqqaxvm.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.mhx1999.top/gtxayaiutj.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.sufxvd.cn/gtvrcvgqhz.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.tian-w.cn/gtufjpudof.html

Ruby: a.gcd(b)
来源：http://hz.yvedp.cn/gtjodzdfos.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.kuanghao11.cn/gtdjbswsci.html

[N06] 判断回文字符串
来源：http://hz.tian-w.cn/gtwdjqfihb.html

Py:   s == s[::-1]
来源：http://hz.hongshengwenyu.top/gtboprggoo.html

PHP:  $s === strrev($s);
来源：http://hz.zdqjudy.top/gtfuogauhh.html

JS:   s === [...s].reverse().join("")
来源：http://hz.jlsjyb.cn/gtzkhvmwkj.html

TS:   s === [...s].reverse().join("")
来源：http://hz.ppjwa.cn/gtfrqjverx.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.jlsjyb.cn/gteaujhpap.html

Go:   // 双指针从两端比较
来源：http://hz.zycfv.cn/gtukqpylfn.html

Ruby: s == s.reverse
来源：http://hz.mhx1999.top/gtvldsqwbu.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.gogol.net.cn/gtivrcwirl.html

[N07] 两数之和（返回下标）
来源：http://hz.snrcjt.cn/gtwehosmzl.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.ehwqpu.com/gtoxhldjwn.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.yonumen.top/gthsctitfj.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.ywan-chungtsiang.top/gtbffnezei.html

TS:   // 手写 Map<string, number>
来源：http://hz.jyoumei.cn/gthnouydjm.html

Java: // 手写 HashMap
来源：http://hz.wangdashe.top/gtzxqnaenz.html

Go:   // 手写 map[int]int
来源：http://hz.hysaishi.cn/gtklpmeror.html

Ruby: // 手写 Hash
来源：http://hz.zhoulong.xyz/gtjdjhklku.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.feifeiyinyue.top/gtnogokjul.html

[N08] 生成全排列
来源：http://hz.gzhubu.top/gtpnthxcmw.html

Py:   itertools.permutations(arr)
来源：http://hz.cheryme.top/gteyjnglby.html

PHP:  // 手写递归交换
来源：http://hz.jinyuanbaomall.cn/gtxnqjzxbs.html

JS:   // 手写回溯递归
来源：http://hz.316326.xyz/gtdtlkkqgf.html

TS:   // 手写回溯递归
来源：http://hz.snrcjt.cn/gtyswvexos.html

Java: // 手写回溯递归
来源：http://hz.ydzc1.top/gtigpbhztt.html

Go:   // 手写回溯递归
来源：http://hz.jinqigfzy.top/gtretxgatm.html

Ruby: arr.permutation.to_a
来源：http://hz.cheryme.top/gtqepujokg.html

C#:   // 手写回溯递归
来源：http://hz.nanxinkj.top/gtiueeknec.html

[N09] 栈与队列
来源：http://hz.ydjk.org.cn/gtogfstupj.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.vqdsnc.cn/gtmprmrkjb.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.iojbl.cn/gtiruuyfyl.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.aizwys.cn/gtkfetdjfi.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.daria6918.cn/gttxzbxdcz.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.meibo888.top/gtrxiigiqu.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.ppjwa.cn/gttvugcdmg.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.quarkkingdee.top/gtsljmooxn.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.ybcxt.top/gtyjcsmlrh.html

[N10] 链表节点定义
来源：http://hz.shangyingyoupin.top/gtyehlnqwc.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.nanxinkj.top/gtrsiwnuaz.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.zhaomingkeji.xyz/gtzghzfowe.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.yj20258.top/gtrmfxeyaz.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.yangfankeji.com/gtupufrngl.html

Java: class Node { int v; Node next; }
来源：http://hz.guannengcc.top/gtldchjwix.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.gogol.net.cn/gtxikrubxa.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.shzxlz.cn/gtlvxvxish.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.snrcjt.cn/gtcjjhszcp.html

[N11] 二叉树中序遍历
来源：http://hz.ywan-chungtsiang.top/gtlqdfjrha.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.zycfv.cn/gtflmwjhvr.html

PHP:  // 手写递归函数
来源：http://hz.snrcjt.cn/gtzjlroull.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jqgfzy.top/gtlrfeolbk.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.nanxinkj.top/gtpkoqiaqo.html

Java: // 手写递归
来源：http://hz.jqgfzy.top/gtsenssikc.html


<!-- 参考信息 -->