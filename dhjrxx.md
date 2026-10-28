代发 wailian999

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.cdnleiting.top/gtijvfwovm.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.ehwqpu.com/gtiqhflksq.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.andypj.xyz/gtkwukdsqe.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.jinyuanbaomall.cn/gtauvefjwe.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.cheryme.top/gtmwrafkxr.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.bjfxy.top/gtdwiinxuz.html

[K04] 读取 JSON 文件
来源：http://hz.sxryk.cn/gtsbngfgyx.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.vqdsnc.cn/gtocrqiqen.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.bjfxy.top/gtwgnhcetj.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.shanyushiyangkeji.top/gtvjvienwg.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.ydzc1.top/gtszpkqwih.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.gaohongyu789.top/gttlkssukg.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.ydjk.org.cn/gttsxfunpo.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.nwbrower.top/gttdlcmxxg.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.hywenlv.cn/gtypcedfiq.html

[K05] 深拷贝对象
来源：http://hz.hnxiangtu.top/gtupcxsguz.html

Py:   copy.deepcopy(obj)
来源：http://hz.dashuyun.cn/gtiqwscthz.html

PHP:  unserialize(serialize($obj));
来源：http://hz.jinqigfzy.top/gthinnfghr.html

JS:   structuredClone(obj)
来源：http://hz.aizwys.cn/gtvzjpyhmh.html

TS:   structuredClone(obj)
来源：http://hz.dianchejie.cn/gtvgiszpli.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.nanxuanxn.top/gttapnmijd.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.nwbrower.top/gticbjojwl.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.gzhubu.top/gtxsdbzwgp.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.fengsongda.top/gtmuouahhh.html

[K06] 解析 URL 查询串
来源：http://hz.zhiwuduotai.top/gtszwlprpc.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.ppjwa.cn/gtsodmybmh.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.dashuyun.cn/gtcmxequur.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.sxryk.cn/gtfpdxewml.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.wangdashe.top/gtdgisuyea.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.aibaodan.cn/gtdgvpclbs.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.yangfankeji.com/gtvxwgpbrw.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.yuanzhike.top/gtwnmveacm.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.svipenyu.cn/gtomufdket.html

[K07] 进制转换
来源：http://hz.tian-w.cn/gtgormphiz.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.yj202588.top/gteqypbbcl.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.jqgufenzy.top/gtwozrdzaq.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.gzhubu.top/gtrkstynaw.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.hysaishi.cn/gthxqabups.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.zhijiandao.cn/gtpfxfpdry.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.jlsjyb.cn/gtwrjjpprd.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.hongshengwenyu.top/gtzvqlwfjs.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.meibo888.top/gtugwspfhv.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.kuanghao11.cn/gtoxaryejg.html

Py:   pickle.dumps(obj)
来源：http://hz.chenjidiqi.icu/gtybnscewl.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.ywan-chungtsiang.top/gtstuodtdn.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.yonumen.top/gtggtaqpnm.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.chenjidiqi.icu/gtmebkqcqn.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.kuanghao11.cn/gttjiwflfc.html

Go:   encoding/gob
来源：http://hz.shanyushiyangkeji.top/gtvqghzeuw.html

Ruby: Marshal.dump(obj)
来源：http://hz.yj20258.top/gtppdvwvjy.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.yanxiufei.cn/gtxojobtod.html

================================================================================
来源：http://hz.quarkkingdee.top/gtupcvpcfu.html

L. 网络请求
来源：http://hz.hammf.cn/gtiuesjzjp.html

================================================================================
来源：http://hz.zycfv.cn/gtmgqjluew.html

[L01] 发送 GET 请求
来源：http://hz.ydjk.org.cn/gtogxdkqcg.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.snrcjt.cn/gteznnsjsx.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.zhaomingkeji.xyz/gtbgjaiwxk.html

JS:   await fetch(url)
来源：http://hz.jlsjyb.cn/gtsxomtlqn.html

TS:   await fetch(url)
来源：http://hz.jiagoushi.top/gtfzxtbppt.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.andypj.xyz/gtcbchmbxw.html

Go:   resp, err := http.Get(url)
来源：http://hz.shangyingyoupin.top/gtunznzvcc.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.redwolf501.top/gtpkzdhjiu.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.yj20258888.top/gtybkuowaa.html

[L02] 发送 POST JSON
来源：http://hz.52xcode.cn/gtnwofnudk.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.yueranfly.top/gtfhqozzal.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.xziqi.cn/gtgzqpyufd.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhongyouzk.top/gtupqeywxh.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.pycfn.com/gtprhpnzpo.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.shangyingyoupin.top/gtfgcwygzg.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.yangfankeji.com/gtlttbadmo.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.ppjwa.cn/gtdenaghjo.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.ywan-chungtsiang.top/gtpelttuav.html

[L03] 设置自定义请求头
来源：http://hz.jianghu66.top/gtfsxttree.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.guannengcc.top/gtzcmnxuwt.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.tian-w.cn/gtraqtbjzp.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.ehwqpu.com/gtfrltywkx.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yuanzhike.top/gtfbgcqtfu.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.tanke756.top/gtvbypfqdi.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.zhengqikj.top/gtentpkvaz.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.ydzc1.top/gtkzjqskpo.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.yvedp.cn/gtogswpbwn.html

[L04] 设置超时
来源：http://hz.smart0.xyz/gtnjvjzlba.html

Py:   requests.get(url, timeout=5)
来源：http://hz.shangyingyoupin.top/gtwxzuzokb.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.aizwys.cn/gtsrlidpot.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.sweek.top/gtnqokufge.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.guowangkeji.top/gtnonbszpb.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.jyoumei.cn/gtkzabvguw.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.yongpay.top/gtuhogqstc.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.jinqigfzy.top/gtevmacuyd.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.pengpengdd.cyou/gtbbphwxii.html

[L05] 上传文件（multipart）
来源：http://hz.shanyushiyangkeji.top/gthbaogkif.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.xuanzx.com/gtloncbkto.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.kuanghao11.cn/gtzyykxbrf.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.redwolf501.top/gtzrkstovg.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.guannengcc.top/gtujusadlh.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.iojbl.cn/gtpvgmzrna.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.xylfe.cn/gtoaofagxu.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.yangfankeji.com/gtcekgldxj.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.jianghu66.top/gtkjmlbbkf.html

[L06] 解析响应为 JSON
来源：http://hz.redwolf501.top/gtpffypuzm.html

Py:   resp.json()
来源：http://hz.yj202588.top/gtmrzodayu.html

PHP:  json_decode($body, true);
来源：http://hz.yonumen.top/gtbhuukvkp.html

JS:   await resp.json()
来源：http://hz.xylfe.cn/gtydhhlihd.html

TS:   await resp.json()
来源：http://hz.sxryk.cn/gtcildmoyl.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.hysaishi.cn/gtuutgqdol.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.cheryme.top/gthxbhmoat.html

Ruby: JSON.parse(resp.body)
来源：http://hz.feifeiyinyue.top/gtombdglar.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.zhijiandao.cn/gtyyhnjdso.html

[L07] 处理 HTTP 状态码
来源：http://hz.sysykeji.top/gtqjdtcutk.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.svipenyu.cn/gtjyvibldn.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.zhengqikj.top/gtsfrnjifn.html

JS:   resp.ok;  resp.status
来源：http://hz.nwbrower.top/gtafiwiufi.html

TS:   resp.ok;  resp.status
来源：http://hz.snrcjt.cn/gtmfkkkyvk.html

Java: resp.statusCode()
来源：http://hz.yvedp.cn/gtqvehguoo.html

Go:   resp.StatusCode
来源：http://hz.chenzaomai.com/gttihssutf.html

Ruby: resp.code.to_i
来源：http://hz.zhijiandao.cn/gttnqiztcv.html

C#:   (int)resp.StatusCode
来源：http://hz.iojbl.cn/gtjibnepbz.html

[L08] 并发请求多个地址
来源：http://hz.guowangkeji.top/gtdghtofkh.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.ppjwa.cn/gtcrzpzupr.html

PHP:  curl_multi_init() 系列
来源：http://hz.hysaishi.cn/gtpntbcxgs.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.kuanghao11.cn/gtwphniogi.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.316326.xyz/gtqcmddjrc.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.quarkkingdee.top/gtelkmcufp.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.nanxinkj.top/gtzpghpyvn.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.hnqzz.top/gtcwyxkhvc.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.xziqi.cn/gtcyzcrvnn.html

================================================================================
来源：http://hz.cdnleiting.top/gtiekpstou.html

M. 命令行 / 进程 / 环境
来源：http://hz.iojbl.cn/gttuikpuxy.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtvrghbevo.html

[M01] 读取命令行参数
来源：http://hz.cqqwz.cn/gtmzbwwcjz.html

Py:   sys.argv[1:]
来源：http://hz.aizwys.cn/gtubuafepi.html

PHP:  $argv;  $argc;
来源：http://hz.cashguo.top/gtbeyeraze.html

JS:   process.argv.slice(2)
来源：http://hz.hywenlv.cn/gtnmzssthd.html

TS:   process.argv.slice(2)
来源：http://hz.gogol.net.cn/gtlpijastf.html

Java: args 数组（main 方法参数）
来源：http://hz.hfpthk.cn/gtlmjiwqya.html

Go:   os.Args[1:]
来源：http://hz.dashuyun.cn/gtzxipuylx.html

Ruby: ARGV
来源：http://hz.hongshengwenyu.top/gtjqmohghz.html

C#:   args 数组（Main 方法参数）
来源：http://hz.jqgfzy.top/gtyvwozyzw.html

[M02] 读取环境变量
来源：http://hz.jlsjyb.cn/gtqvkiidvr.html

Py:   os.environ.get("HOME")
来源：http://hz.zhixingplan.top/gtbianktid.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.shanyushiyangkeji.top/gtyvvxxwjy.html

JS:   process.env.HOME
来源：http://hz.feifeiyinyue.top/gtyuulszry.html

TS:   process.env.HOME
来源：http://hz.zycfv.cn/gtaqisddff.html

Java: System.getenv("HOME")
来源：http://hz.cheryme.top/gttehgbben.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.jinqigufen.top/gtatrgdwrq.html

Ruby: ENV["HOME"]
来源：http://hz.pycfn.com/gtoedbwifn.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.yueranfly.top/gtmyynyigl.html

[M03] 执行外部命令
来源：http://hz.jinyuanbaomall.cn/gtqurqrdzj.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.fzhhl.top/gtbiajwucb.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.sweek.top/gtsuamklna.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.tanke756.top/gteayvlnae.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.aizwys.cn/gtzsqvlwlk.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.zhoulong.xyz/gtfokfwxau.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.jlsjyb.cn/gtsfebshfx.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.tian-w.cn/gtucrntygz.html

C#:   Process.Start("ls", "-l");
来源：http://hz.jyoumei.cn/gtifygrabw.html

[M04] 获取当前工作目录
来源：http://hz.ehwqpu.com/gttsgqqnyy.html

Py:   os.getcwd()
来源：http://hz.xuetiantiany.cn/gtgyvbqvab.html

PHP:  getcwd();
来源：http://hz.gogol.net.cn/gturbgadkt.html

JS:   process.cwd()
来源：http://hz.cqqwz.cn/gtfrcklpso.html

TS:   process.cwd()
来源：http://hz.chenlongwang.top/gtciqovxwf.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.aizwys.cn/gtvdzozomp.html

Go:   os.Getwd()
来源：http://hz.9152youxi.cn/gtcrliptbf.html

Ruby: Dir.pwd
来源：http://hz.smart0.xyz/gtqrvvmnvr.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.cdnleiting.top/gtdnaxmwwu.html

[M05] 设置退出码
来源：http://hz.birdmap.top/gtyxikehlr.html

Py:   sys.exit(1)
来源：http://hz.aibaodan.cn/gtiyxigbus.html

PHP:  exit(1);
来源：http://hz.jqgufenzy.top/gtrrsldbmk.html

JS:   process.exit(1)
来源：http://hz.pycfn.com/gtlejifqvd.html

TS:   process.exit(1)
来源：http://hz.quarkkingdee.top/gtpmztxtxc.html

Java: System.exit(1)
来源：http://hz.daxiang520.top/gtdyajmpbs.html

Go:   os.Exit(1)
来源：http://hz.havefunace.top/gtowmnyfqn.html

Ruby: exit 1
来源：http://hz.shzxlz.cn/gtwytbpqze.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.cashguo.top/gtffmejdwp.html

[M06] 向标准错误输出
来源：http://hz.ybcxt.top/gtdinnzsbe.html

Py:   print("err", file=sys.stderr)
来源：http://hz.tian-w.cn/gtmudevuvl.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.zhongyouzk.top/gtzhdttlsw.html

JS:   console.error("err")
来源：http://hz.havefunace.top/gtlxjmelrf.html

TS:   console.error("err")
来源：http://hz.birdmap.top/gtoibcxnta.html

Java: System.err.println("err")
来源：http://hz.jqgufenzy.top/gtadqzkjnn.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.guowangkeji.top/gtcimhrmfo.html

Ruby: warn "err"
来源：http://hz.jqgufenzy.top/gtpuibkvyg.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.zhengqikj.top/gtobmcnicn.html

[M07] 判断是否为主入口
来源：http://hz.cucudq.cn/gttfqjhmlt.html

Py:   if __name__ == "__main__":
来源：http://hz.jiagoushi.top/gtclvfzhqn.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.redwolf501.top/gtjnyqmbpn.html

JS:   require.main === module
来源：http://hz.aibaodan.cn/gtdgdhkswp.html

TS:   require.main === module
来源：http://hz.daria6918.cn/gtgrjuvgqu.html

Java: public static void main(String[] args)
来源：http://hz.chenjidiqi.icu/gtmcnndyjm.html

Go:   func main()
来源：http://hz.xinyue.icu/gtnlnimfak.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.yuanzhike.top/gtxcdbxqlg.html

C#:   static void Main(string[] args)
来源：http://hz.chenjidiqi.icu/gtjuljxsyt.html

[M08] 获取系统与运行时信息
来源：http://hz.hfpthk.cn/gtrdbsshwl.html

Py:   platform.system();  platform.python_version()
来源：http://hz.mhx1999.top/gthuwjadna.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.sxryk.cn/gtgrohavur.html

JS:   process.platform;  process.version
来源：http://hz.dashuyun.cn/gtpnlyizkp.html

TS:   process.platform;  process.version
来源：http://hz.meibo888.top/gtoybhufwd.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.ppjwa.cn/gtxexhomfa.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.fzhhl.top/gtzrzrsmqq.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.yanxiufei.cn/gtcmdgxdst.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.zhengqikj.top/gtkuaaenpd.html

================================================================================
来源：http://hz.ppjwa.cn/gtibtxvnwu.html

N. 数据结构与算法
来源：http://hz.havefunace.top/gtqzixxemb.html

================================================================================
来源：http://hz.yongpay.top/gtwivjvkqc.html

[N01] 二分查找（有序数组）
来源：http://hz.iojbl.cn/gtyhrvumul.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.nwbrower.top/gtvdoggijy.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.0kj1m.cn/gtmhrlcljr.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.shangyingyoupin.top/gtdxplrfzy.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jianghu66.top/gtjlorgkkm.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.nanxinkj.top/gtumdhhudh.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.meibo888.top/gtynbvsmft.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.zdqjudy.top/gttsenlbzi.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.jqgfzy.top/gtzhrbmeqb.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.sysykeji.top/gtobwtcdbd.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.hywenlv.cn/gtjnyhzqqa.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.wangdashe.top/gtkwtmzfgn.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.nwbrower.top/gtqzqkgwjw.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.zycfv.cn/gtcdophdzi.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.nwbrower.top/gtrcpovegz.html

Go:   slices.Sort(arr)
来源：http://hz.gogol.net.cn/gtbakjnjnk.html

Ruby: arr.sort
来源：http://hz.cqqwz.cn/gtxtpmtxfc.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.zhixingplan.top/gtbwrmnkcp.html

[N03] 快速排序（分治示例）
来源：http://hz.meibo888.top/gtvooblvqw.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.jqgufenzy.top/gtfcvjvuwq.html

PHP:  // 递归实现，或用 usort
来源：http://hz.ehwqpu.com/gtgwpnusps.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.ehwqpu.com/gtofxqragl.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yj20258.top/gtdiupfwcw.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.birdmap.top/gtrhfogxkt.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.yuanzhike.top/gtqtvhqkns.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.ydjk.org.cn/gteprqkfyi.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.jiagoushi.top/gtynekixae.html

[N04] 斐波那契数列
来源：http://hz.chenzaomai.com/gtwupdrckv.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.9152youxi.cn/gtivpjwgtf.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.guannengcc.top/gtofxftgus.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.feifeiyinyue.top/gtxhgbfnbq.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.nanxuanxn.top/gttbslbhop.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.yvedp.cn/gtvhszhrra.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.gotoacloud.top/gtyxhtoeay.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.zhijiandao.cn/gteueluhat.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.svipenyu.cn/gtaxuiutbq.html

[N05] 最大公约数
来源：http://hz.ehwqpu.com/gtjsyvmssw.html

Py:   math.gcd(a, b)
来源：http://hz.jinqigfzy.top/gtyjcegico.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.xylfe.cn/gtyfxknnho.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jinghuilouyu.cn/gtiexooskr.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.ywan-chungtsiang.top/gtaegpyfyg.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.pengpengdd.cyou/gtpmxlrqrq.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.fengsongda.top/gtgvijjydt.html

Ruby: a.gcd(b)
来源：http://hz.andypj.xyz/gteptkhszc.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.jinghuilouyu.cn/gtokvslzow.html

[N06] 判断回文字符串
来源：http://hz.shanyushiyangkeji.top/gtqyjvrlez.html

Py:   s == s[::-1]
来源：http://hz.jyoumei.cn/gtvvohpqqw.html

PHP:  $s === strrev($s);
来源：http://hz.aizwys.cn/gtyxaillot.html

JS:   s === [...s].reverse().join("")
来源：http://hz.snrcjt.cn/gtjcjlocbq.html

TS:   s === [...s].reverse().join("")
来源：http://hz.fengsongda.top/gtqagrgpvw.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.andypj.xyz/gtqwogjvvk.html

Go:   // 双指针从两端比较
来源：http://hz.iojbl.cn/gtubdqxpdq.html

Ruby: s == s.reverse
来源：http://hz.pengpengdd.cyou/gtongcigrq.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.meibo888.top/gtrqcsgpdi.html

[N07] 两数之和（返回下标）
来源：http://hz.316326.xyz/gturywqwqb.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.shanyushiyangkeji.top/gtwdfsynuu.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.yj202588.top/gtxjqkrmlc.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.mhx1999.top/gtkbjtjztg.html

TS:   // 手写 Map<string, number>
来源：http://hz.guowangkeji.top/gttragwzcm.html

Java: // 手写 HashMap
来源：http://hz.zdqjudy.top/gttsskclcn.html

Go:   // 手写 map[int]int
来源：http://hz.sysykeji.top/gtaicyisau.html

Ruby: // 手写 Hash
来源：http://hz.xziqi.cn/gthmjzyfig.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.sxryk.cn/gtjokduvbi.html

[N08] 生成全排列
来源：http://hz.yuxming.cn/gtwdijswfs.html

Py:   itertools.permutations(arr)
来源：http://hz.aibaodan.cn/gtccpmisew.html

PHP:  // 手写递归交换
来源：http://hz.tian-w.cn/gtsvxylget.html

JS:   // 手写回溯递归
来源：http://hz.aizwys.cn/gtgcktnprp.html

TS:   // 手写回溯递归
来源：http://hz.yj202588.top/gtzcwfrbbv.html

Java: // 手写回溯递归
来源：http://hz.sysykeji.top/gtlgkmiazh.html

Go:   // 手写回溯递归
来源：http://hz.sufxvd.cn/gtoawoyetx.html

Ruby: arr.permutation.to_a
来源：http://hz.sweek.top/gtgaqfpoin.html

C#:   // 手写回溯递归
来源：http://hz.nwbrower.top/gtbnlfmkea.html

[N09] 栈与队列
来源：http://hz.snrcjt.cn/gtxlglecei.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.meibo888.top/gtgzcoilul.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.jiagoushi.top/gtyxtxiciv.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.shangyingyoupin.top/gtcyikrytw.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.havefunace.top/gtvjyflilg.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.xingfuxueyuan.xyz/gtitevxihw.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.fengsongda.top/gttvitposl.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.316326.xyz/gtpjsmacnx.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.mhx1999.top/gtermzgihc.html

[N10] 链表节点定义
来源：http://hz.cheryme.top/gtifmrrmvb.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.jianghu66.top/gtvzrekbhm.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.bjfxy.top/gtqtpkqffi.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.svipenyu.cn/gtfpsxcpxq.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.shanyushiyangkeji.top/gtfwgfzrwo.html

Java: class Node { int v; Node next; }
来源：http://hz.ybcxt.top/gtasohxcch.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.meibo888.top/gtiuqnvaxg.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.hysaishi.cn/gtvgjwfgze.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.pengpengdd.cyou/gtuukslyba.html

[N11] 二叉树中序遍历
来源：http://hz.ybcxt.top/gtouozdilv.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.tian-w.cn/gtdhdbadmh.html

PHP:  // 手写递归函数
来源：http://hz.xylfe.cn/gttoelsdde.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.xuanzx.com/gthlhavphe.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jqgfzy.top/gtaaefjyro.html

Java: // 手写递归
来源：http://hz.nanxuanxn.top/gtxvqtrlhy.html


<!-- 参考信息 -->