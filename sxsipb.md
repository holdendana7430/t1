代发 wailian999

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.yueranfly.top/gtksooshss.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.quarkkingdee.top/gtsedvcrxu.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.dianchejie.cn/gtxhcrccei.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.hongshengwenyu.top/gtvgbhmjoq.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.ybcxt.top/gtslajhhzt.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.quarkkingdee.top/gtcsdpqjgn.html

[K04] 读取 JSON 文件
来源：http://hz.svipenyu.cn/gtbtxtkwjt.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.yueranfly.top/gtqctcwnco.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.xziqi.cn/gtxefqvdqx.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.aizwys.cn/gtfhjuxeak.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.daxiang520.top/gtwufivlor.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.9152youxi.cn/gtwmvxwexe.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.quarkkingdee.top/gtmwmogdtq.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.smart0.xyz/gtqgqwgmfb.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.hfpthk.cn/gtybtijlrm.html

[K05] 深拷贝对象
来源：http://hz.smart0.xyz/gtsaeemeik.html

Py:   copy.deepcopy(obj)
来源：http://hz.yanxiufei.cn/gtdcaanyfi.html

PHP:  unserialize(serialize($obj));
来源：http://hz.tanke756.top/gtypebtpts.html

JS:   structuredClone(obj)
来源：http://hz.zhijiandao.cn/gtltbzcvam.html

TS:   structuredClone(obj)
来源：http://hz.yj20258888.top/gthmvfrfom.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.yonumen.top/gtvnsvariu.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.jqgfzy.top/gtwbhrallj.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.sxryk.cn/gtbrmckqnq.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.yj20258.top/gtfqokhduy.html

[K06] 解析 URL 查询串
来源：http://hz.jianghu66.top/gtjuzojtpd.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.hongshengwenyu.top/gtcqjhxjca.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.zycfv.cn/gtolyojjji.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.daria6918.cn/gtmmbnghcf.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.pycfn.com/gtgfipmbof.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.jyoumei.cn/gtxuevzyoo.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.chenjidiqi.icu/gtgfwechay.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.vqdsnc.cn/gtahxtlyva.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.gogol.net.cn/gtpophoqgf.html

[K07] 进制转换
来源：http://hz.jyoumei.cn/gtzuzzjjrs.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.zdqjudy.top/gttqhjovhc.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.ivvv.top/gtbfbsrbrx.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.tian-w.cn/gtmglususm.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.bjfxy.top/gtsxewmdqd.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.smart0.xyz/gtcqlwvrkf.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.haohaochexian.top/gtddgvcxwh.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.bjfxy.top/gtzoopxbmz.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.sysykeji.top/gttmllubto.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.jlsjyb.cn/gtfmgnboca.html

Py:   pickle.dumps(obj)
来源：http://hz.dianchejie.cn/gtwxcjnoyy.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.redwolf501.top/gtzlwhjete.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.shuidangran.top/gtixkiibeh.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.yonumen.top/gtfkqittit.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.yongpay.top/gtrykmylwn.html

Go:   encoding/gob
来源：http://hz.wangshuangyany.cn/gteklutjkn.html

Ruby: Marshal.dump(obj)
来源：http://hz.jqgfzy.top/gtngguqgak.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.0kj1m.cn/gtgxcfzvym.html

================================================================================
来源：http://hz.zycfv.cn/gtkflnuama.html

L. 网络请求
来源：http://hz.meibo888.top/gtwwhufkap.html

================================================================================
来源：http://hz.c1oappe.top/gtksenhadb.html

[L01] 发送 GET 请求
来源：http://hz.cashguo.top/gtliqvlpla.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.chenlongwang.top/gtrmwioqjd.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.yangfankeji.com/gtsfuopcgt.html

JS:   await fetch(url)
来源：http://hz.nanxuanxn.top/gtspjaffva.html

TS:   await fetch(url)
来源：http://hz.hnqzz.top/gtpbnrygyk.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.snrcjt.cn/gtfuqoyrlh.html

Go:   resp, err := http.Get(url)
来源：http://hz.quarkkingdee.top/gtlduiixrr.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.yangfankeji.com/gtrrfwxfih.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.hammf.cn/gtdkqfothr.html

[L02] 发送 POST JSON
来源：http://hz.shangyingyoupin.top/gtnhrkczzf.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.daria6918.cn/gtzuixqdoi.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.cucudq.cn/gtfnoybazr.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.gogol.net.cn/gtskhjcguy.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.ppjwa.cn/gtuxycfydx.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.ehwqpu.com/gtmwexoppe.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.shzxlz.cn/gtakpmekbj.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.yj202588.top/gtybfkwydh.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.yj20258888.top/gtujvqytfn.html

[L03] 设置自定义请求头
来源：http://hz.jlsjyb.cn/gtvtggveto.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.hnxiangtu.top/gtqptckbre.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.snrcjt.cn/gtjthwlvvb.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.daria6918.cn/gtvfycpbwd.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.pycfn.com/gtbhjxnnpn.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.redwolf501.top/gtabkhcpou.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.zhengqikj.top/gtjurwrpso.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.wangshuangyany.cn/gtfskudmuh.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.yangfankeji.com/gtwtmmgvzx.html

[L04] 设置超时
来源：http://hz.yuanzhike.top/gtqnfbfdev.html

Py:   requests.get(url, timeout=5)
来源：http://hz.zhiwuduotai.top/gtgrvudzte.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.zhengqikj.top/gttzxhpnyr.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.quarkkingdee.top/gtraumdclv.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.havefunace.top/gtakupzagc.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.guannengcc.top/gtvihzhbmp.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.yuxming.cn/gtodshzgij.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.feifeiyinyue.top/gtqqojcgue.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.0kj1m.cn/gtepajcpjq.html

[L05] 上传文件（multipart）
来源：http://hz.cdnleiting.top/gtzilyqpkx.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.cqqwz.cn/gtjlsqkgui.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.shuidangran.top/gtuhigksev.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.c1oappe.top/gtrpngofrk.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.hongshengwenyu.top/gtsjpftjtv.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.nwbrower.top/gtuibezhpf.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.ydjk.org.cn/gtgfpwkeqq.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.birdmap.top/gtsapxrjua.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.jiagoushi.top/gtfaqdzkoq.html

[L06] 解析响应为 JSON
来源：http://hz.hammf.cn/gtxrwnophe.html

Py:   resp.json()
来源：http://hz.bjfxy.top/gtyvyiojpp.html

PHP:  json_decode($body, true);
来源：http://hz.wangdashe.top/gterpyzmtk.html

JS:   await resp.json()
来源：http://hz.shzxlz.cn/gtvjclgoig.html

TS:   await resp.json()
来源：http://hz.c1oappe.top/gtmwprncos.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.hfpthk.cn/gtpzjmdpct.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.shangyingyoupin.top/gtndjzmosi.html

Ruby: JSON.parse(resp.body)
来源：http://hz.yj20258888.top/gtunuobjjr.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.xylfe.cn/gtudevqejl.html

[L07] 处理 HTTP 状态码
来源：http://hz.nanxuanxn.top/gterrjgofw.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.gzhubu.top/gtcxrktazx.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.zdqjudy.top/gtpipybauv.html

JS:   resp.ok;  resp.status
来源：http://hz.dianchejie.cn/gtwkhcvtqd.html

TS:   resp.ok;  resp.status
来源：http://hz.tian-w.cn/gtqbftuobl.html

Java: resp.statusCode()
来源：http://hz.jyoumei.cn/gtownhphfh.html

Go:   resp.StatusCode
来源：http://hz.chenlongwang.top/gtzgyjvajx.html

Ruby: resp.code.to_i
来源：http://hz.yuxming.cn/gttnqchdzy.html

C#:   (int)resp.StatusCode
来源：http://hz.aibaodan.cn/gtssacafmh.html

[L08] 并发请求多个地址
来源：http://hz.yj202588.top/gtdjuabvaf.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.zhixingplan.top/gtpafcayme.html

PHP:  curl_multi_init() 系列
来源：http://hz.9152youxi.cn/gtvlkhquhw.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.meibo888.top/gtpwyxlvpx.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.xziqi.cn/gtbtbppiim.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.hongshengwenyu.top/gturxbgint.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.wangshuangyany.cn/gtwdsimkmw.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.feifeiyinyue.top/gtbpyqondl.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.zhijiandao.cn/gtkqrctnae.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtvmxeitmy.html

M. 命令行 / 进程 / 环境
来源：http://hz.yj20258888.top/gtiqcklowq.html

================================================================================
来源：http://hz.yuxming.cn/gttemaixvg.html

[M01] 读取命令行参数
来源：http://hz.hnqzz.top/gtcbdvrrqw.html

Py:   sys.argv[1:]
来源：http://hz.haohaochexian.top/gtdpfmxtrf.html

PHP:  $argv;  $argc;
来源：http://hz.wangdashe.top/gtaxohtbuf.html

JS:   process.argv.slice(2)
来源：http://hz.svipenyu.cn/gtwerujxvp.html

TS:   process.argv.slice(2)
来源：http://hz.316326.xyz/gtwqinhqfx.html

Java: args 数组（main 方法参数）
来源：http://hz.cqqwz.cn/gtfstatfhk.html

Go:   os.Args[1:]
来源：http://hz.snrcjt.cn/gtywazoggy.html

Ruby: ARGV
来源：http://hz.ppjwa.cn/gtfxzxqbmn.html

C#:   args 数组（Main 方法参数）
来源：http://hz.yanxiufei.cn/gtqfzoghbn.html

[M02] 读取环境变量
来源：http://hz.jiagoushi.top/gttpfzqbsq.html

Py:   os.environ.get("HOME")
来源：http://hz.zdqjudy.top/gtptmnjhfi.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.jqgfzy.top/gtgshxznyd.html

JS:   process.env.HOME
来源：http://hz.mhx1999.top/gtvgzreafq.html

TS:   process.env.HOME
来源：http://hz.hongshengwenyu.top/gtmqoyqptt.html

Java: System.getenv("HOME")
来源：http://hz.bjfxy.top/gtdykmnjjn.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.xziqi.cn/gthzxjewgj.html

Ruby: ENV["HOME"]
来源：http://hz.wangdashe.top/gtoaziqpts.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.vqdsnc.cn/gtgjhppqlp.html

[M03] 执行外部命令
来源：http://hz.fengsongda.top/gtteptshel.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.bjfxy.top/gtdmpcygmq.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.cdnleiting.top/gtgccffbek.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.yj20258888.top/gtkxoyfaht.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.nwbrower.top/gtosmljpym.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.sxryk.cn/gtcznwnebl.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.jinqigfzy.top/gtxdzwnmbn.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.aibaodan.cn/gthllflphi.html

C#:   Process.Start("ls", "-l");
来源：http://hz.aizwys.cn/gthwcwfpmh.html

[M04] 获取当前工作目录
来源：http://hz.yueranfly.top/gtsgwrqswf.html

Py:   os.getcwd()
来源：http://hz.0kj1m.cn/gtjaqqeisz.html

PHP:  getcwd();
来源：http://hz.c1oappe.top/gtnwqpwdpu.html

JS:   process.cwd()
来源：http://hz.chenjidiqi.icu/gtlevemcvx.html

TS:   process.cwd()
来源：http://hz.ivvv.top/gtysqglfnv.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.hnqzz.top/gtewieimwk.html

Go:   os.Getwd()
来源：http://hz.gzhubu.top/gtomdjaqzv.html

Ruby: Dir.pwd
来源：http://hz.zhongyouzk.top/gthjtrbqib.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.chenjidiqi.icu/gtctmzmcpl.html

[M05] 设置退出码
来源：http://hz.jqgfzy.top/gttciteeqe.html

Py:   sys.exit(1)
来源：http://hz.jianghu66.top/gtxaokmqzf.html

PHP:  exit(1);
来源：http://hz.zhengqikj.top/gtxlcbriuu.html

JS:   process.exit(1)
来源：http://hz.aizwys.cn/gtuxkevkma.html

TS:   process.exit(1)
来源：http://hz.zhoulong.xyz/gtdvaqtfho.html

Java: System.exit(1)
来源：http://hz.chenjidiqi.icu/gtwrnmorxk.html

Go:   os.Exit(1)
来源：http://hz.shangyingyoupin.top/gtrcczfjks.html

Ruby: exit 1
来源：http://hz.chenjidiqi.icu/gtcmlczdul.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.shzxlz.cn/gtcuzyfwru.html

[M06] 向标准错误输出
来源：http://hz.xziqi.cn/gtflhzfbpe.html

Py:   print("err", file=sys.stderr)
来源：http://hz.yangfankeji.com/gtxmsqziwm.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.tian-w.cn/gthkfckeak.html

JS:   console.error("err")
来源：http://hz.52xcode.cn/gtwljvifgn.html

TS:   console.error("err")
来源：http://hz.hnxiangtu.top/gtlivbnlkv.html

Java: System.err.println("err")
来源：http://hz.yangfankeji.com/gtdxbgxwsp.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.svipenyu.cn/gtwugmaynl.html

Ruby: warn "err"
来源：http://hz.52xcode.cn/gtzzizqztr.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.hfpthk.cn/gtcatoyzxy.html

[M07] 判断是否为主入口
来源：http://hz.gaohongyu789.top/gtfduhfown.html

Py:   if __name__ == "__main__":
来源：http://hz.redwolf501.top/gthlospjvz.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.ppjwa.cn/gtgqllbbib.html

JS:   require.main === module
来源：http://hz.ywan-chungtsiang.top/gthussxwdu.html

TS:   require.main === module
来源：http://hz.dashuyun.cn/gtnsogxrgx.html

Java: public static void main(String[] args)
来源：http://hz.zdqjudy.top/gtycyvaorn.html

Go:   func main()
来源：http://hz.yj20258888.top/gtqmymyybd.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.jinqigfzy.top/gtgpdgrnfn.html

C#:   static void Main(string[] args)
来源：http://hz.xinyue.icu/gtoyzgzicp.html

[M08] 获取系统与运行时信息
来源：http://hz.guannengcc.top/gtnjetwuma.html

Py:   platform.system();  platform.python_version()
来源：http://hz.yanxiufei.cn/gtnfkoahzb.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.wangdashe.top/gtdhmqjgve.html

JS:   process.platform;  process.version
来源：http://hz.tanke756.top/gtpxvziyqv.html

TS:   process.platform;  process.version
来源：http://hz.jqgfzy.top/gtaxnogidh.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.mhx1999.top/gtvdmqftgc.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.pengpengdd.cyou/gteaubmkae.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.svipenyu.cn/gtfnakgskm.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.cashguo.top/gtwafzcazw.html

================================================================================
来源：http://hz.tian-w.cn/gtwjgzipfb.html

N. 数据结构与算法
来源：http://hz.ehwqpu.com/gtrmguuyed.html

================================================================================
来源：http://hz.gotoacloud.top/gtvbogjzxs.html

[N01] 二分查找（有序数组）
来源：http://hz.jinqigfzy.top/gtjhqieanb.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.haohaochexian.top/gtqribhdch.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.yj20258888.top/gtsyaxunom.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.gotoacloud.top/gtzlkdpnyj.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.xylfe.cn/gtypeugoic.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.hywenlv.cn/gtmowvvphb.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.birdmap.top/gtdswqscax.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.vqdsnc.cn/gtnzcbkrju.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.jiagoushi.top/gtloznsdmb.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.sweek.top/gtcnosghfv.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.kuanghao11.cn/gttvlmmmqf.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.jqgfzy.top/gtcysvxebu.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.52xcode.cn/gtaeffhjhl.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yanxiufei.cn/gtougymmbg.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.jqgfzy.top/gtrdiubhhe.html

Go:   slices.Sort(arr)
来源：http://hz.cdnleiting.top/gtqbeogtzz.html

Ruby: arr.sort
来源：http://hz.tian-w.cn/gtlqzspwgn.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.xylfe.cn/gtrbzoporw.html

[N03] 快速排序（分治示例）
来源：http://hz.daxiang520.top/gttlrvnsfd.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.havefunace.top/gtqmlnywze.html

PHP:  // 递归实现，或用 usort
来源：http://hz.yangfankeji.com/gtyamxiwwf.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yanxiufei.cn/gtjgjbnzaj.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zhengqikj.top/gtzfbuabav.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.fzhhl.top/gtkmnvhcdf.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.shzxlz.cn/gtqiqysqhf.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.meibo888.top/gtgqumbjde.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.shanyushiyangkeji.top/gthepinqjr.html

[N04] 斐波那契数列
来源：http://hz.jinqigfzy.top/gtbqwujdsw.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.quarkkingdee.top/gtebcdaclk.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.nwbrower.top/gtzthzuwcj.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.gotoacloud.top/gtdxisloty.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.52xcode.cn/gttcaluikt.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.haohaochexian.top/gtxxoztqfp.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.xingfuxueyuan.xyz/gtqabfzsod.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.sxryk.cn/gtijxouvec.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.chenlongwang.top/gtxxrlkuuw.html

[N05] 最大公约数
来源：http://hz.xinyue.icu/gtfkechiif.html

Py:   math.gcd(a, b)
来源：http://hz.meibo888.top/gtnhvxdkfk.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.wangshuangyany.cn/gtuuynfwtc.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.tian-w.cn/gtocjybjhr.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.hysaishi.cn/gtcgxdipkx.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.guowangkeji.top/gtpjpqzvbh.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.hongshengwenyu.top/gtudxnnahk.html

Ruby: a.gcd(b)
来源：http://hz.gaohongyu789.top/gtmjmseajl.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.smart0.xyz/gtsmhfiizz.html

[N06] 判断回文字符串
来源：http://hz.chenlongwang.top/gtvtlpypde.html

Py:   s == s[::-1]
来源：http://hz.ivvv.top/gtmcqtwmbd.html

PHP:  $s === strrev($s);
来源：http://hz.ybcxt.top/gtokbvrqfz.html

JS:   s === [...s].reverse().join("")
来源：http://hz.9152youxi.cn/gtfbqoejnw.html

TS:   s === [...s].reverse().join("")
来源：http://hz.redwolf501.top/gtyggxoabi.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.cashguo.top/gtpxwyybpf.html

Go:   // 双指针从两端比较
来源：http://hz.xuetiantiany.cn/gtgtwoaqan.html

Ruby: s == s.reverse
来源：http://hz.iojbl.cn/gtwmybtzje.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.zhongyouzk.top/gtcruerxxr.html

[N07] 两数之和（返回下标）
来源：http://hz.chenzaomai.com/gtidpadaof.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.dianchejie.cn/gtmsfxqfat.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.andypj.xyz/gtnayhidmb.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.zhaomingkeji.xyz/gtuaomlkmt.html

TS:   // 手写 Map<string, number>
来源：http://hz.316326.xyz/gtwgvnddjv.html

Java: // 手写 HashMap
来源：http://hz.ydjk.org.cn/gtouqluizc.html

Go:   // 手写 map[int]int
来源：http://hz.jinqigufen.top/gtylgghfyf.html

Ruby: // 手写 Hash
来源：http://hz.tian-w.cn/gtnhbnichf.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.jinqigufen.top/gtquhitevt.html

[N08] 生成全排列
来源：http://hz.yj202588.top/gttxlttptb.html

Py:   itertools.permutations(arr)
来源：http://hz.jqgfzy.top/gtvsebrysy.html

PHP:  // 手写递归交换
来源：http://hz.havefunace.top/gtllsguphr.html

JS:   // 手写回溯递归
来源：http://hz.daria6918.cn/gtadzmlyuq.html

TS:   // 手写回溯递归
来源：http://hz.zhixingplan.top/gtyskrjaps.html

Java: // 手写回溯递归
来源：http://hz.tian-w.cn/gtebpkrgkf.html

Go:   // 手写回溯递归
来源：http://hz.nanxuanxn.top/gtdgqmvpsx.html

Ruby: arr.permutation.to_a
来源：http://hz.yonumen.top/gtinvniftp.html

C#:   // 手写回溯递归
来源：http://hz.jqgufenzy.top/gtdvszdqru.html

[N09] 栈与队列
来源：http://hz.jinqigufen.top/gthoyeglds.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.wangdashe.top/gthqlmmtri.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.haohaochexian.top/gtplhrxsxf.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.bjfxy.top/gtpnqpsxwg.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.sweek.top/gtvikplbur.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.gogol.net.cn/gtaydyjjom.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.yonumen.top/gtxjgjcrwc.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.cucudq.cn/gtftnvxmpv.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.zdqjudy.top/gtmbzirjcn.html

[N10] 链表节点定义
来源：http://hz.ivvv.top/gtuggfhmhc.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.hysaishi.cn/gtamcaymnt.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.zycfv.cn/gtazrhrqac.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.ywan-chungtsiang.top/gtdbxzjqzn.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.xylfe.cn/gtqoacsduz.html

Java: class Node { int v; Node next; }
来源：http://hz.gogol.net.cn/gtaurkzwph.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.snrcjt.cn/gtqmifhlmk.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.gogol.net.cn/gtitpmctol.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.ehwqpu.com/gthzggkkto.html

[N11] 二叉树中序遍历
来源：http://hz.havefunace.top/gtkzdouoaw.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.dashuyun.cn/gtjvjshkma.html

PHP:  // 手写递归函数
来源：http://hz.xziqi.cn/gtjvzwomvu.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.sufxvd.cn/gtwtvgiloq.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.shangyingyoupin.top/gtnqfvgggx.html

Java: // 手写递归
来源：http://hz.yangfankeji.com/gtjzbhevbq.html


<!-- 参考信息 -->