代发 wailian999

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.hammf.cn/gtkfjmolfs.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.gotoacloud.top/gtnyartppt.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.shangyingyoupin.top/gtznqjobta.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.smart0.xyz/gtprvdtziv.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.jinghuilouyu.cn/gtfblutced.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.jqgfzy.top/gtweoqylde.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.gaohongyu789.top/gtweosscvn.html

[K05] 深拷贝对象
来源：http://hz.ydjk.org.cn/gtjrmabfqx.html

Py:   copy.deepcopy(obj)
来源：http://hz.jlsjyb.cn/gtnapymwzv.html

PHP:  unserialize(serialize($obj));
来源：http://hz.iojbl.cn/gtvmffvdvy.html

JS:   structuredClone(obj)
来源：http://hz.zycfv.cn/gttdeqxerm.html

TS:   structuredClone(obj)
来源：http://hz.daxiang520.top/gtjmlcdgqn.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.gogol.net.cn/gtzhbfrioi.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.hysaishi.cn/gtulourwdx.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.yangfankeji.com/gtrwadusfp.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.zhongyouzk.top/gtdmjjyjxr.html

[K06] 解析 URL 查询串
来源：http://hz.xingfuxueyuan.xyz/gtpoyxojgw.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.zhaomingkeji.xyz/gteaydmhin.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.yueranfly.top/gthcfzjqge.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.pycfn.com/gttnmmmrzj.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.hfpthk.cn/gtqeepgaja.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.kuanghao11.cn/gtpsslostz.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.zhijiandao.cn/gtmsvquznn.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.gotoacloud.top/gtxkkayhjr.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.jyoumei.cn/gtpepyrmca.html

[K07] 进制转换
来源：http://hz.ydjk.org.cn/gticmzcled.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.shzxlz.cn/gtpgdbnilw.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.zhongyouzk.top/gtpzyiooor.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.jlsjyb.cn/gtvvopevdh.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.gaohongyu789.top/gtlrmhlstt.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.kuanghao11.cn/gtphgfaqqe.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.yanxiufei.cn/gtnsyixvxl.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.zhaomingkeji.xyz/gtolfucgjr.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.hnqzz.top/gtbbbqwsdb.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.zdqjudy.top/gticoqhxca.html

Py:   pickle.dumps(obj)
来源：http://hz.yj20258.top/gtdczhgsxn.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.daxiang520.top/gtovcapgiw.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.xuetiantiany.cn/gtstlztfuv.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.pengpengdd.cyou/gtmclkqtmi.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.nanxuanxn.top/gtraxxejgu.html

Go:   encoding/gob
来源：http://hz.9152youxi.cn/gthbmmixrb.html

Ruby: Marshal.dump(obj)
来源：http://hz.aizwys.cn/gthxixtmdq.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.cashguo.top/gtbihtiwwa.html

================================================================================
来源：http://hz.zhengqikj.top/gtaauspmdh.html

L. 网络请求
来源：http://hz.cqqwz.cn/gtkgtivjmk.html

================================================================================
来源：http://hz.yuanzhike.top/gtumknfzpe.html

[L01] 发送 GET 请求
来源：http://hz.jinqigufen.top/gttpwfmedx.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.9152youxi.cn/gtmdwzxboa.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.yj20258.top/gtzaeqpbmq.html

JS:   await fetch(url)
来源：http://hz.jyoumei.cn/gtbfltzovr.html

TS:   await fetch(url)
来源：http://hz.xuanzx.com/gtmqytjsqe.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.hnqzz.top/gtknpcyqdn.html

Go:   resp, err := http.Get(url)
来源：http://hz.ivvv.top/gtnaspkwtk.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.gaohongyu789.top/gtwfefrawx.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.0kj1m.cn/gtwlwupgql.html

[L02] 发送 POST JSON
来源：http://hz.redwolf501.top/gterarwtdi.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.jiagoushi.top/gtoocluxho.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.yongpay.top/gtuxrmundw.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.tianlin.xyz/gthmixzdol.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.ppjwa.cn/gtrrbqrcnz.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.svipenyu.cn/gtrjiabobf.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.316326.xyz/gtppvjvccx.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.yj20258888.top/gtbhuneboa.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.feifeiyinyue.top/gtzxibejhy.html

[L03] 设置自定义请求头
来源：http://hz.ydjk.org.cn/gtdfqttbms.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.jianghu66.top/gtvaasfcph.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.chenlongwang.top/gtoeydtlrm.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.chenlongwang.top/gtzemsenco.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.aibaodan.cn/gtbrfhcysj.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.jqgufenzy.top/gthcbvdwsj.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.0kj1m.cn/gtixgoejwz.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.shuidangran.top/gtjnjgzytx.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.pengpengdd.cyou/gtweywuyxb.html

[L04] 设置超时
来源：http://hz.iojbl.cn/gtmmjnqnif.html

Py:   requests.get(url, timeout=5)
来源：http://hz.shanyushiyangkeji.top/gtibgjgelb.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.cashguo.top/gtphvicini.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.cashguo.top/gtindxbljl.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jqgfzy.top/gtovstbfns.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.nwbrower.top/gtvxuljact.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.cucudq.cn/gtoxyoumys.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.yvedp.cn/gtgpvsxlyw.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.ppjwa.cn/gtduaiqlmt.html

[L05] 上传文件（multipart）
来源：http://hz.hfpthk.cn/gtccwmmpsm.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.tianlin.xyz/gtglacnipc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.zhiwuduotai.top/gtqgwpaxts.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.daria6918.cn/gtoratewte.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.zhongyouzk.top/gtaglrffpb.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.cdnleiting.top/gtubsbkgbd.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.yvedp.cn/gtvsmhfxvk.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.zdqjudy.top/gtxfsxtszf.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.shanyushiyangkeji.top/gtgahknufz.html

[L06] 解析响应为 JSON
来源：http://hz.meibo888.top/gtwtqkahzx.html

Py:   resp.json()
来源：http://hz.meibo888.top/gtgotbabhh.html

PHP:  json_decode($body, true);
来源：http://hz.dianchejie.cn/gtucsqgovf.html

JS:   await resp.json()
来源：http://hz.guowangkeji.top/gtkiuocevk.html

TS:   await resp.json()
来源：http://hz.yanxiufei.cn/gtxnmwwhab.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.ywan-chungtsiang.top/gtpfxouext.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.mhx1999.top/gtkmendeak.html

Ruby: JSON.parse(resp.body)
来源：http://hz.tanke756.top/gticygzajt.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.hongshengwenyu.top/gtjmrvmzqs.html

[L07] 处理 HTTP 状态码
来源：http://hz.haohaochexian.top/gtatmieiec.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.gaohongyu789.top/gtwrdlmoxl.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.smart0.xyz/gtaucbmhko.html

JS:   resp.ok;  resp.status
来源：http://hz.0kj1m.cn/gtcpduwrfd.html

TS:   resp.ok;  resp.status
来源：http://hz.kuanghao11.cn/gtxlzubuaf.html

Java: resp.statusCode()
来源：http://hz.316326.xyz/gtebkbvbxa.html

Go:   resp.StatusCode
来源：http://hz.ywan-chungtsiang.top/gteqzfvsce.html

Ruby: resp.code.to_i
来源：http://hz.nanxuanxn.top/gtzybfznue.html

C#:   (int)resp.StatusCode
来源：http://hz.fengsongda.top/gtrddpbikn.html

[L08] 并发请求多个地址
来源：http://hz.yj20258.top/gtasqqijeq.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.zhengqikj.top/gtiyyjgdno.html

PHP:  curl_multi_init() 系列
来源：http://hz.haohaochexian.top/gthztvjeao.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.hfpthk.cn/gtwoofmera.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.guannengcc.top/gtwjbtezvu.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.hammf.cn/gtpiclgufp.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.hfpthk.cn/gtfkbskgbj.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.jqgufenzy.top/gthvfiuifc.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.aizwys.cn/gtfkypryrk.html

================================================================================
来源：http://hz.nanxinkj.top/gtnmfgtbhf.html

M. 命令行 / 进程 / 环境
来源：http://hz.yj20258888.top/gtdtqkbdcy.html

================================================================================
来源：http://hz.gzhubu.top/gttbslwggp.html

[M01] 读取命令行参数
来源：http://hz.feifeiyinyue.top/gtwkermtga.html

Py:   sys.argv[1:]
来源：http://hz.iojbl.cn/gtglxbhawu.html

PHP:  $argv;  $argc;
来源：http://hz.kuanghao11.cn/gtqykrvfgz.html

JS:   process.argv.slice(2)
来源：http://hz.daxiang520.top/gttvrprwhq.html

TS:   process.argv.slice(2)
来源：http://hz.hnqzz.top/gtmjdrnzxp.html

Java: args 数组（main 方法参数）
来源：http://hz.ybcxt.top/gtnekuztxp.html

Go:   os.Args[1:]
来源：http://hz.vqdsnc.cn/gtbedghisz.html

Ruby: ARGV
来源：http://hz.jianghu66.top/gtyldcltsf.html

C#:   args 数组（Main 方法参数）
来源：http://hz.xziqi.cn/gtsbujhujw.html

[M02] 读取环境变量
来源：http://hz.tianlin.xyz/gttzvgccew.html

Py:   os.environ.get("HOME")
来源：http://hz.ydzc1.top/gtxynmxtwi.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.jinghuilouyu.cn/gtenhwbbal.html

JS:   process.env.HOME
来源：http://hz.yuxming.cn/gtmokblgag.html

TS:   process.env.HOME
来源：http://hz.sweek.top/gtrvcrerol.html

Java: System.getenv("HOME")
来源：http://hz.jianghu66.top/gtjnfuihki.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.tian-w.cn/gtghgvioey.html

Ruby: ENV["HOME"]
来源：http://hz.jinghuilouyu.cn/gtxucaiarn.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.zhijiandao.cn/gtemquosva.html

[M03] 执行外部命令
来源：http://hz.zhengqikj.top/gtkedrwjgc.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.316326.xyz/gtyfsqjyou.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.ppjwa.cn/gtdgibqsjy.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.chenzaomai.com/gtjsszbime.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.hnxiangtu.top/gtohsfuvzi.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.xuetiantiany.cn/gtrisyvhhl.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.cqqwz.cn/gtpzdthudj.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.jiagoushi.top/gtwpyyjvfl.html

C#:   Process.Start("ls", "-l");
来源：http://hz.ydjk.org.cn/gtzmgzpavq.html

[M04] 获取当前工作目录
来源：http://hz.jinqigfzy.top/gtqvolerdd.html

Py:   os.getcwd()
来源：http://hz.c1oappe.top/gtbkclvkxs.html

PHP:  getcwd();
来源：http://hz.jiagoushi.top/gtejdcgvfb.html

JS:   process.cwd()
来源：http://hz.guannengcc.top/gtprjymuwe.html

TS:   process.cwd()
来源：http://hz.yuanzhike.top/gttlmvmvep.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.dashuyun.cn/gtxetvgcsz.html

Go:   os.Getwd()
来源：http://hz.jinyuanbaomall.cn/gtpbhjztvg.html

Ruby: Dir.pwd
来源：http://hz.hfpthk.cn/gtqbjvfftw.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.hnxiangtu.top/gtzvnztevv.html

[M05] 设置退出码
来源：http://hz.fzhhl.top/gtvxfksubv.html

Py:   sys.exit(1)
来源：http://hz.aizwys.cn/gttmxeeadc.html

PHP:  exit(1);
来源：http://hz.fzhhl.top/gtwjyrcxvv.html

JS:   process.exit(1)
来源：http://hz.gotoacloud.top/gtiuqxiyto.html

TS:   process.exit(1)
来源：http://hz.haohaochexian.top/gttmkderwv.html

Java: System.exit(1)
来源：http://hz.xinyue.icu/gttijxejdw.html

Go:   os.Exit(1)
来源：http://hz.zhiwuduotai.top/gtfaugmzsp.html

Ruby: exit 1
来源：http://hz.guannengcc.top/gtavayzlkl.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.chenlongwang.top/gtduqrtske.html

[M06] 向标准错误输出
来源：http://hz.gogol.net.cn/gtlnvqfhhi.html

Py:   print("err", file=sys.stderr)
来源：http://hz.xuanzx.com/gtcjdemtfy.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.sxryk.cn/gtkmrufivc.html

JS:   console.error("err")
来源：http://hz.xziqi.cn/gtejprmwix.html

TS:   console.error("err")
来源：http://hz.bjfxy.top/gtaetlzhbm.html

Java: System.err.println("err")
来源：http://hz.pycfn.com/gtajqrykdc.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.yj20258888.top/gtelrlvlxw.html

Ruby: warn "err"
来源：http://hz.fzhhl.top/gtddpxokmh.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.yuxming.cn/gtzwlvolyl.html

[M07] 判断是否为主入口
来源：http://hz.dashuyun.cn/gtohzqckbw.html

Py:   if __name__ == "__main__":
来源：http://hz.chenlongwang.top/gtxkfxfnxn.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.yj20258.top/gtrhabaury.html

JS:   require.main === module
来源：http://hz.yj20258888.top/gtohvasjup.html

TS:   require.main === module
来源：http://hz.ivvv.top/gtznstxttu.html

Java: public static void main(String[] args)
来源：http://hz.guowangkeji.top/gtrjlpvkkc.html

Go:   func main()
来源：http://hz.gzhubu.top/gtyliiqsdr.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.hysaishi.cn/gtmpzehqhy.html

C#:   static void Main(string[] args)
来源：http://hz.yueranfly.top/gtxyqgqlab.html

[M08] 获取系统与运行时信息
来源：http://hz.chenlongwang.top/gtkpuhpmyr.html

Py:   platform.system();  platform.python_version()
来源：http://hz.zycfv.cn/gtsvuvvupi.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.jlsjyb.cn/gtpocuoqie.html

JS:   process.platform;  process.version
来源：http://hz.yongpay.top/gtvhlnqflu.html

TS:   process.platform;  process.version
来源：http://hz.316326.xyz/gtenbktnox.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.jqgufenzy.top/gttjxmhjms.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.ywan-chungtsiang.top/gttpfdradj.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.yj20258888.top/gtbrgbzxac.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.xziqi.cn/gtyxzegdzl.html

================================================================================
来源：http://hz.zdqjudy.top/gtqzpozolj.html

N. 数据结构与算法
来源：http://hz.zhaomingkeji.xyz/gtznvhoxru.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtqaotfrci.html

[N01] 二分查找（有序数组）
来源：http://hz.zhaomingkeji.xyz/gtvkgjdens.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.xylfe.cn/gtlaoylbyg.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.tianlin.xyz/gtwwslsdvn.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zhengqikj.top/gtkqjdnqgz.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.0kj1m.cn/gtbarldhac.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.gzhubu.top/gtcshniald.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.mhx1999.top/gtbayuhulo.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.ybcxt.top/gtyndmcrsg.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.jqgfzy.top/gtpdfkadzq.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.birdmap.top/gtqmghyuds.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.cheryme.top/gtyaxuwzvy.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.tianlin.xyz/gtynxnsvzn.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.aizwys.cn/gtyxbsvbdb.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.zhixingplan.top/gtqxytzmgd.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.jqgfzy.top/gtxkfrgnwh.html

Go:   slices.Sort(arr)
来源：http://hz.daria6918.cn/gtgvliasuq.html

Ruby: arr.sort
来源：http://hz.jqgufenzy.top/gtcwqzrjeq.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.jinghuilouyu.cn/gtfwvjbawo.html

[N03] 快速排序（分治示例）
来源：http://hz.quarkkingdee.top/gtdmpxsjiy.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.shangyingyoupin.top/gtxfxrjley.html

PHP:  // 递归实现，或用 usort
来源：http://hz.guowangkeji.top/gtuvywymbe.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.svipenyu.cn/gtbvkajqwg.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.ppjwa.cn/gtggwbummj.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.zhaomingkeji.xyz/gtorfshffg.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.nwbrower.top/gtxolojulr.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.quarkkingdee.top/gtrfdiczvu.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.xziqi.cn/gtabonyakf.html

[N04] 斐波那契数列
来源：http://hz.ydjk.org.cn/gtgncrpqxz.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.ehwqpu.com/gtfmjpxsog.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.ywan-chungtsiang.top/gtcdwdibfi.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jqgufenzy.top/gtyaskyaej.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.pycfn.com/gtiujlpaff.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.nanxuanxn.top/gtukvekvis.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.zhoulong.xyz/gtrjkkhnuk.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.gogol.net.cn/gtoomemqoh.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.aizwys.cn/gtrcegkxnj.html

[N05] 最大公约数
来源：http://hz.haohaochexian.top/gtnmvnauhz.html

Py:   math.gcd(a, b)
来源：http://hz.chenlongwang.top/gteemzbwce.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.haohaochexian.top/gtpycuvysh.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yuxming.cn/gtepldnrkn.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.zhoulong.xyz/gtskknygjk.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.jlsjyb.cn/gtqaroullk.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.nanxuanxn.top/gtdywlnduf.html

Ruby: a.gcd(b)
来源：http://hz.ydjk.org.cn/gtsgcemict.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.meibo888.top/gtolvavovf.html

[N06] 判断回文字符串
来源：http://hz.yueranfly.top/gtknthsjcg.html

Py:   s == s[::-1]
来源：http://hz.daxiang520.top/gtydeaxvya.html

PHP:  $s === strrev($s);
来源：http://hz.xylfe.cn/gtxrqhjpjo.html

JS:   s === [...s].reverse().join("")
来源：http://hz.xingfuxueyuan.xyz/gtqvjnsakn.html

TS:   s === [...s].reverse().join("")
来源：http://hz.andypj.xyz/gtyyxmybys.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.havefunace.top/gtajcyynyc.html

Go:   // 双指针从两端比较
来源：http://hz.tianlin.xyz/gtudmfuobf.html

Ruby: s == s.reverse
来源：http://hz.bjfxy.top/gtleeiblub.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.yvedp.cn/gtclhprtre.html

[N07] 两数之和（返回下标）
来源：http://hz.dianchejie.cn/gtfreqijih.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.zycfv.cn/gtldqxdzqy.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.hammf.cn/gtmmlnoqsb.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.quarkkingdee.top/gtjywpkwwx.html

TS:   // 手写 Map<string, number>
来源：http://hz.pengpengdd.cyou/gtbbigcbiv.html

Java: // 手写 HashMap
来源：http://hz.quarkkingdee.top/gtxsxnxirj.html

Go:   // 手写 map[int]int
来源：http://hz.guowangkeji.top/gtwdugomcs.html

Ruby: // 手写 Hash
来源：http://hz.tian-w.cn/gtmuhrazgf.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.0kj1m.cn/gtltocwrwm.html

[N08] 生成全排列
来源：http://hz.daxiang520.top/gtathubbpc.html

Py:   itertools.permutations(arr)
来源：http://hz.haohaochexian.top/gttsjmqkks.html

PHP:  // 手写递归交换
来源：http://hz.cashguo.top/gtlxkiakhf.html

JS:   // 手写回溯递归
来源：http://hz.cqqwz.cn/gtnwptxxkz.html

TS:   // 手写回溯递归
来源：http://hz.kuanghao11.cn/gtqopetkbq.html

Java: // 手写回溯递归
来源：http://hz.shanyushiyangkeji.top/gtozffpplo.html

Go:   // 手写回溯递归
来源：http://hz.snrcjt.cn/gtsurwhabh.html

Ruby: arr.permutation.to_a
来源：http://hz.nanxuanxn.top/gtzcqejgyn.html

C#:   // 手写回溯递归
来源：http://hz.xuetiantiany.cn/gthbdnvzkn.html

[N09] 栈与队列
来源：http://hz.quarkkingdee.top/gteufvfuac.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.316326.xyz/gtrddvjgym.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.cashguo.top/gtwlokaces.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.iojbl.cn/gttztibqpu.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.ivvv.top/gtlbrcaxhk.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.daria6918.cn/gttybedivm.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.ydzc1.top/gtdokszbgk.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.ydjk.org.cn/gtvxvliyab.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.hammf.cn/gtrbnkmduk.html

[N10] 链表节点定义
来源：http://hz.dashuyun.cn/gtilohpvlm.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.ehwqpu.com/gtwhdbdvxu.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.guannengcc.top/gtiowakfiw.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.jinqigufen.top/gtxnlbbbra.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.shangyingyoupin.top/gtissjvysv.html

Java: class Node { int v; Node next; }
来源：http://hz.pengpengdd.cyou/gtsncpasql.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.shanyushiyangkeji.top/gtjwtldxpy.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.daxiang520.top/gttkfjiola.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.yj20258888.top/gtdothuocb.html

[N11] 二叉树中序遍历
来源：http://hz.cheryme.top/gtcdnrftgt.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.gzhubu.top/gtkgxbemcu.html

PHP:  // 手写递归函数
来源：http://hz.sweek.top/gthomlgyqf.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yj20258.top/gtfjvhpvsi.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.zhijiandao.cn/gtywmitwnw.html

Java: // 手写递归
来源：http://hz.yonumen.top/gtqwlhkjbo.html

Go:   // 手写递归
来源：http://hz.sxryk.cn/gtqavghhsv.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.sysykeji.top/gthhmktbto.html

C#:   // 手写递归
来源：http://hz.cashguo.top/gtsfczbtei.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.ehwqpu.com/gthweomlpm.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.52xcode.cn/gtqmlvronj.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.ivvv.top/gtrvzkmtco.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.sweek.top/gtxrollaux.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.meibo888.top/gtwujpjkbi.html


<!-- 参考信息 -->