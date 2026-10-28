代发 wailian999

Ruby: JSON.pretty_generate(obj)
来源：http://hz.gzhubu.top/gtnvmnlahx.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.jinqigfzy.top/gtobzmjjdr.html

[K04] 读取 JSON 文件
来源：http://hz.shangyingyoupin.top/gtmqzjcndn.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.dashuyun.cn/gtjgbuguzl.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.zhixingplan.top/gtzredidlc.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.aibaodan.cn/gtrdmkuzvy.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.tianlin.xyz/gtrcctqmie.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.jinyuanbaomall.cn/gtwryyxzng.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.xuetiantiany.cn/gtefrakqmh.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.andypj.xyz/gtuiqerysa.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.andypj.xyz/gtztcitypk.html

[K05] 深拷贝对象
来源：http://hz.cheryme.top/gtpxutzmgt.html

Py:   copy.deepcopy(obj)
来源：http://hz.sufxvd.cn/gtwlwxcrsz.html

PHP:  unserialize(serialize($obj));
来源：http://hz.jinqigfzy.top/gtcuwvzxkv.html

JS:   structuredClone(obj)
来源：http://hz.dianchejie.cn/gtddktuvnh.html

TS:   structuredClone(obj)
来源：http://hz.316326.xyz/gtqdyivhso.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.yongpay.top/gtkoohpkrc.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.yj20258888.top/gtaohwhxlx.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.jinyuanbaomall.cn/gtghsbbaqs.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.meibo888.top/gtwmklidxq.html

[K06] 解析 URL 查询串
来源：http://hz.aizwys.cn/gtsokmcwsr.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.redwolf501.top/gtzzsihxtx.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.dianchejie.cn/gtoyvpzwnu.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.andypj.xyz/gtkynyagxk.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.fzhhl.top/gtnygvhely.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.ydzc1.top/gtieaeozvn.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.ywan-chungtsiang.top/gtwegakfzr.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.ydzc1.top/gtjtbqrsqr.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.pycfn.com/gttxqxehga.html

[K07] 进制转换
来源：http://hz.shangyingyoupin.top/gtzgkqwrgw.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.jinqigufen.top/gtlmwgdvpj.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.ydjk.org.cn/gtarbwxlhk.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.yuxming.cn/gtzhbxogwp.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.jianghu66.top/gtpdnmnaxd.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.cqqwz.cn/gtyqjppxxy.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.yj202588.top/gtjnhaerca.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.gogol.net.cn/gtwfvijiva.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.iojbl.cn/gttaqbjpdn.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.guowangkeji.top/gtrmourfst.html

Py:   pickle.dumps(obj)
来源：http://hz.wangshuangyany.cn/gtzjgvntix.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.ehwqpu.com/gtibavxqsn.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.316326.xyz/gtxrukdier.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.zhaomingkeji.xyz/gtnwagxrgs.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.ywan-chungtsiang.top/gthnhnbilo.html

Go:   encoding/gob
来源：http://hz.cdnleiting.top/gtgtytjhds.html

Ruby: Marshal.dump(obj)
来源：http://hz.jinqigufen.top/gtdrmxgagj.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.zhoulong.xyz/gtiysthekq.html

================================================================================
来源：http://hz.cqqwz.cn/gtbbylzcyp.html

L. 网络请求
来源：http://hz.zycfv.cn/gtxapsjuwb.html

================================================================================
来源：http://hz.xuanzx.com/gtqxdshfaz.html

[L01] 发送 GET 请求
来源：http://hz.ppjwa.cn/gttxlhjmhc.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.zhijiandao.cn/gtzkwwemft.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.tanke756.top/gtlvfbkdwp.html

JS:   await fetch(url)
来源：http://hz.jinghuilouyu.cn/gttccntdcd.html

TS:   await fetch(url)
来源：http://hz.tanke756.top/gttfedlufs.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.nwbrower.top/gtqpkxccke.html

Go:   resp, err := http.Get(url)
来源：http://hz.yvedp.cn/gteavxuxyk.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.nanxuanxn.top/gtwdrvqwbt.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.smart0.xyz/gtyvzcyddl.html

[L02] 发送 POST JSON
来源：http://hz.snrcjt.cn/gtxwfwgdmy.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.bjfxy.top/gtolnbwokz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.cdnleiting.top/gttevghxcj.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.havefunace.top/gtjtbdsyzi.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.pengpengdd.cyou/gtbsytlmkc.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.yonumen.top/gthpwqaxkz.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.jinqigfzy.top/gtpihrhbau.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.aibaodan.cn/gtxgatszjv.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.jyoumei.cn/gtqvtorxbf.html

[L03] 设置自定义请求头
来源：http://hz.guannengcc.top/gtjkfaewji.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.tian-w.cn/gtjeyieeff.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.snrcjt.cn/gtdlzerevc.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.quarkkingdee.top/gttkgwuyij.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.daria6918.cn/gtqmcgfpzr.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.zdqjudy.top/gtousmhfrs.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.xuanzx.com/gtbbryjaev.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.iojbl.cn/gtfshejdwe.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.zhongyouzk.top/gtnstedhbe.html

[L04] 设置超时
来源：http://hz.316326.xyz/gtawsxpyak.html

Py:   requests.get(url, timeout=5)
来源：http://hz.tian-w.cn/gtonfzopme.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.jyoumei.cn/gtctxzfmdi.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.xingfuxueyuan.xyz/gtneprerqx.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.wangdashe.top/gtzcmxjuea.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.zdqjudy.top/gtmtkmzdbe.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.sufxvd.cn/gtfrjwbbld.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.andypj.xyz/gtynmlzpxg.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.dianchejie.cn/gtgedaorbw.html

[L05] 上传文件（multipart）
来源：http://hz.0kj1m.cn/gtpfzulncz.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.jinqigufen.top/gttohkojve.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.feifeiyinyue.top/gtqbjtfbrg.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.yvedp.cn/gtvdrnmeht.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.tian-w.cn/gtrlawsolg.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.yonumen.top/gtswdgkuvi.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.wangdashe.top/gtfunvfrja.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.havefunace.top/gtxuvtcpjo.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.guannengcc.top/gtsdrtjeoo.html

[L06] 解析响应为 JSON
来源：http://hz.shanyushiyangtech.top/gtrxxxlhqu.html

Py:   resp.json()
来源：http://hz.xylfe.cn/gtszbumpzr.html

PHP:  json_decode($body, true);
来源：http://hz.xuetiantiany.cn/gtpajzsvuz.html

JS:   await resp.json()
来源：http://hz.shangyingyoupin.top/gtnnwrjfer.html

TS:   await resp.json()
来源：http://hz.hnxiangtu.top/gtxoojbgiy.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.vqdsnc.cn/gtghniawfa.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.9152youxi.cn/gtiiajdlfc.html

Ruby: JSON.parse(resp.body)
来源：http://hz.gotoacloud.top/gtfdinwgwn.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.iojbl.cn/gtelpuzfhr.html

[L07] 处理 HTTP 状态码
来源：http://hz.zhijiandao.cn/gtfgndijsv.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.fengsongda.top/gtfgtjtmmo.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.guowangkeji.top/gtwowiqfiu.html

JS:   resp.ok;  resp.status
来源：http://hz.jinyuanbaomall.cn/gtmkxaeovl.html

TS:   resp.ok;  resp.status
来源：http://hz.c1oappe.top/gthvihpohi.html

Java: resp.statusCode()
来源：http://hz.daxiang520.top/gtyrdkuoli.html

Go:   resp.StatusCode
来源：http://hz.redwolf501.top/gtyqnsbhym.html

Ruby: resp.code.to_i
来源：http://hz.jianghu66.top/gtybwbjnso.html

C#:   (int)resp.StatusCode
来源：http://hz.ydzc1.top/gtxhmyqylf.html

[L08] 并发请求多个地址
来源：http://hz.tanke756.top/gtqffjpwoa.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.yangfankeji.com/gtckqlnxlg.html

PHP:  curl_multi_init() 系列
来源：http://hz.jinqigfzy.top/gtbbfzzark.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.havefunace.top/gtmdpdegli.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yuanzhike.top/gtkkfeqniy.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.jinyuanbaomall.cn/gtqvjishlx.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.ydzc1.top/gthakpthej.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.xinyue.icu/gtfitkkrwa.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.wangshuangyany.cn/gttiwicfws.html

================================================================================
来源：http://hz.smart0.xyz/gtkkhvkbje.html

M. 命令行 / 进程 / 环境
来源：http://hz.ivvv.top/gttdhwwamm.html

================================================================================
来源：http://hz.9152youxi.cn/gtivfzagsf.html

[M01] 读取命令行参数
来源：http://hz.jinyuanbaomall.cn/gtepjdtqqr.html

Py:   sys.argv[1:]
来源：http://hz.yueranfly.top/gtdrxdnahj.html

PHP:  $argv;  $argc;
来源：http://hz.yj20258.top/gthhzohjlp.html

JS:   process.argv.slice(2)
来源：http://hz.jinqigfzy.top/gtrfjgbiav.html

TS:   process.argv.slice(2)
来源：http://hz.aizwys.cn/gtdrnwtfxj.html

Java: args 数组（main 方法参数）
来源：http://hz.iojbl.cn/gtspbepeuc.html

Go:   os.Args[1:]
来源：http://hz.vqdsnc.cn/gtzhpifevf.html

Ruby: ARGV
来源：http://hz.cheryme.top/gtjpouswpf.html

C#:   args 数组（Main 方法参数）
来源：http://hz.chenjidiqi.icu/gtcqdspehs.html

[M02] 读取环境变量
来源：http://hz.ybcxt.top/gttuklqftq.html

Py:   os.environ.get("HOME")
来源：http://hz.xuanzx.com/gtdsmzzprd.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.andypj.xyz/gtxjxdrxdi.html

JS:   process.env.HOME
来源：http://hz.hammf.cn/gtieudmiuy.html

TS:   process.env.HOME
来源：http://hz.jinghuilouyu.cn/gtmkwhfqom.html

Java: System.getenv("HOME")
来源：http://hz.yuanzhike.top/gtldfqgyyr.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.fzhhl.top/gtpioltpym.html

Ruby: ENV["HOME"]
来源：http://hz.tian-w.cn/gtgdkopwyn.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.feifeiyinyue.top/gtcgpplfrf.html

[M03] 执行外部命令
来源：http://hz.shzxlz.cn/gtkpmwqvhm.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.havefunace.top/gtsvyknoxg.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.zhijiandao.cn/gtyddgzlek.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.zhijiandao.cn/gtmhebpezk.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.aizwys.cn/gtgidoreui.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.316326.xyz/gttnbpfzxv.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.meibo888.top/gtgsyfrrse.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.hywenlv.cn/gtlzivauun.html

C#:   Process.Start("ls", "-l");
来源：http://hz.cqqwz.cn/gtwhnilapw.html

[M04] 获取当前工作目录
来源：http://hz.cucudq.cn/gtozjaarzw.html

Py:   os.getcwd()
来源：http://hz.feifeiyinyue.top/gtntglobeg.html

PHP:  getcwd();
来源：http://hz.yuxming.cn/gtwkbqiehr.html

JS:   process.cwd()
来源：http://hz.tian-w.cn/gtdnefrgif.html

TS:   process.cwd()
来源：http://hz.sysykeji.top/gtojtnxvbq.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.hnxiangtu.top/gtgbpcgrft.html

Go:   os.Getwd()
来源：http://hz.nanxinkj.top/gtpdeeuhuv.html

Ruby: Dir.pwd
来源：http://hz.zhijiandao.cn/gtlqoafkpm.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.guannengcc.top/gtlkxguvhw.html

[M05] 设置退出码
来源：http://hz.xylfe.cn/gtcsmhhcfd.html

Py:   sys.exit(1)
来源：http://hz.ydzc1.top/gtkfyewbhg.html

PHP:  exit(1);
来源：http://hz.zhijiandao.cn/gtmiozqylp.html

JS:   process.exit(1)
来源：http://hz.andypj.xyz/gtfxhqxdlj.html

TS:   process.exit(1)
来源：http://hz.cdnleiting.top/gtmhxzuxqm.html

Java: System.exit(1)
来源：http://hz.aizwys.cn/gtfgibsmkl.html

Go:   os.Exit(1)
来源：http://hz.andypj.xyz/gtilhbbeeu.html

Ruby: exit 1
来源：http://hz.cashguo.top/gtftrewboq.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.nanxinkj.top/gthovrpuyt.html

[M06] 向标准错误输出
来源：http://hz.pycfn.com/gtucillwyo.html

Py:   print("err", file=sys.stderr)
来源：http://hz.jinqigufen.top/gtshukrcoa.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.shanyushiyangtech.top/gtacgdjppd.html

JS:   console.error("err")
来源：http://hz.vqdsnc.cn/gtpquhmomy.html

TS:   console.error("err")
来源：http://hz.pycfn.com/gtkmtexhdv.html

Java: System.err.println("err")
来源：http://hz.sufxvd.cn/gtmgfuwrca.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.hnxiangtu.top/gtunwcukzs.html

Ruby: warn "err"
来源：http://hz.zycfv.cn/gtjvrpuovu.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.c1oappe.top/gtqffeljgc.html

[M07] 判断是否为主入口
来源：http://hz.ppjwa.cn/gtvoefbibz.html

Py:   if __name__ == "__main__":
来源：http://hz.tanke756.top/gtezgwkrsk.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.c1oappe.top/gtraxiymtn.html

JS:   require.main === module
来源：http://hz.jiagoushi.top/gtxfesmfie.html

TS:   require.main === module
来源：http://hz.sweek.top/gtcvsekacb.html

Java: public static void main(String[] args)
来源：http://hz.cucudq.cn/gttqtsvxkb.html

Go:   func main()
来源：http://hz.guowangkeji.top/gtxpzenqpo.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.ehwqpu.com/gthdblfnyj.html

C#:   static void Main(string[] args)
来源：http://hz.meibo888.top/gtbcjzqrah.html

[M08] 获取系统与运行时信息
来源：http://hz.sweek.top/gtugqxaclp.html

Py:   platform.system();  platform.python_version()
来源：http://hz.dianchejie.cn/gtpuhshszm.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.ehwqpu.com/gtjdnyudoh.html

JS:   process.platform;  process.version
来源：http://hz.zhoulong.xyz/gtrrgxtwch.html

TS:   process.platform;  process.version
来源：http://hz.xuetiantiany.cn/gtanpnsdbt.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.xylfe.cn/gtzzxwtkkb.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.cheryme.top/gtwfalgvcm.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.mhx1999.top/gtlvvkcmbx.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.zycfv.cn/gtgkhxfhxl.html

================================================================================
来源：http://hz.zhixingplan.top/gtmhprrjud.html

N. 数据结构与算法
来源：http://hz.hammf.cn/gtxroukuqg.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtxqymjxdn.html

[N01] 二分查找（有序数组）
来源：http://hz.hnxiangtu.top/gtkgduvvnx.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.chenzaomai.com/gtscnadabv.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.xingfuxueyuan.xyz/gthmtqtjqk.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.quarkkingdee.top/gtyjyhwcaj.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.cheryme.top/gtrvisjsjf.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.zhoulong.xyz/gtzdgixlkt.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.ppjwa.cn/gtqjsrpcze.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.yonumen.top/gtbfdxfoqu.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.cqqwz.cn/gtwdrulieg.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.andypj.xyz/gtfgwaqhgg.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jqgfzy.top/gtiwdeijxe.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.redwolf501.top/gtvjjynefq.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.sxryk.cn/gtikilbxvg.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.ppjwa.cn/gtkmfwyyos.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.hongshengwenyu.top/gtgdrehqjf.html

Go:   slices.Sort(arr)
来源：http://hz.andypj.xyz/gtlhzlgdvn.html

Ruby: arr.sort
来源：http://hz.zhoulong.xyz/gtsxiysyzs.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.52xcode.cn/gtpsfxtoqc.html

[N03] 快速排序（分治示例）
来源：http://hz.pycfn.com/gtszdhvmqd.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.birdmap.top/gtfmjxjwli.html

PHP:  // 递归实现，或用 usort
来源：http://hz.sxryk.cn/gtirxiollu.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jqgfzy.top/gtwwlcvwqf.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.cashguo.top/gtovdbdrfa.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.kuanghao11.cn/gtgrrznqoh.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.bjfxy.top/gtjbqmfudq.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.chenlongwang.top/gttojthlla.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.wangshuangyany.cn/gthoqpjlhw.html

[N04] 斐波那契数列
来源：http://hz.jinghuilouyu.cn/gtzoldzmds.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.fengsongda.top/gtelodmxhf.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.daxiang520.top/gtczhldzxq.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.hysaishi.cn/gtelzcyids.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.cqqwz.cn/gttthwbdly.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.ppjwa.cn/gtrrvdhqti.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.xuetiantiany.cn/gtuevapxge.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.yanxiufei.cn/gtbphqkpit.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.xylfe.cn/gtsvnfragp.html

[N05] 最大公约数
来源：http://hz.svipenyu.cn/gtxcxgyren.html

Py:   math.gcd(a, b)
来源：http://hz.shuidangran.top/gttldjkmbp.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.shanyushiyangkeji.top/gtwqtggvwt.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yanxiufei.cn/gtzbziylvl.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.ehwqpu.com/gtqnmmtexj.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.zhiwuduotai.top/gthjqznolb.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.hammf.cn/gtuyyqaeex.html

Ruby: a.gcd(b)
来源：http://hz.yonumen.top/gtjubwpodc.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.wangshuangyany.cn/gtjbrigbjt.html

[N06] 判断回文字符串
来源：http://hz.zhaomingkeji.xyz/gtmitqejlt.html

Py:   s == s[::-1]
来源：http://hz.zhaomingkeji.xyz/gtsmmpvlfv.html

PHP:  $s === strrev($s);
来源：http://hz.shanyushiyangtech.top/gthomlsfah.html

JS:   s === [...s].reverse().join("")
来源：http://hz.chenzaomai.com/gtjaixhkss.html

TS:   s === [...s].reverse().join("")
来源：http://hz.dashuyun.cn/gtdpcryrhi.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.daria6918.cn/gtrvroxfil.html

Go:   // 双指针从两端比较
来源：http://hz.pengpengdd.cyou/gttgqatbcr.html

Ruby: s == s.reverse
来源：http://hz.jinghuilouyu.cn/gtfhhwnpdx.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.bjfxy.top/gtffqhtttd.html

[N07] 两数之和（返回下标）
来源：http://hz.yueranfly.top/gtvzrkguzb.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.tianlin.xyz/gtockkhkzi.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.xuanzx.com/gtiwbmeuhp.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.fzhhl.top/gtjizvzldn.html

TS:   // 手写 Map<string, number>
来源：http://hz.pengpengdd.cyou/gtliqohbay.html

Java: // 手写 HashMap
来源：http://hz.aizwys.cn/gtdsreytfu.html

Go:   // 手写 map[int]int
来源：http://hz.yuanzhike.top/gtpgydgpwm.html

Ruby: // 手写 Hash
来源：http://hz.yangfankeji.com/gtnrfslxer.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.jinqigufen.top/gteqeyhfxj.html

[N08] 生成全排列
来源：http://hz.sufxvd.cn/gthwyvnwvi.html

Py:   itertools.permutations(arr)
来源：http://hz.zdqjudy.top/gtykmzljcw.html

PHP:  // 手写递归交换
来源：http://hz.birdmap.top/gtrplwqeci.html

JS:   // 手写回溯递归
来源：http://hz.zhiwuduotai.top/gtfnnwtfyf.html

TS:   // 手写回溯递归
来源：http://hz.guowangkeji.top/gtufdepwnb.html

Java: // 手写回溯递归
来源：http://hz.mhx1999.top/gtunzhhnnz.html

Go:   // 手写回溯递归
来源：http://hz.daxiang520.top/gtmhabxudc.html

Ruby: arr.permutation.to_a
来源：http://hz.pengpengdd.cyou/gtwldlbwee.html

C#:   // 手写回溯递归
来源：http://hz.zhiwuduotai.top/gtxhdfapsc.html

[N09] 栈与队列
来源：http://hz.cqqwz.cn/gtyhmnhsam.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.yangfankeji.com/gtxlfiebom.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.shuidangran.top/gtmezpripl.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.zhongyouzk.top/gtnufvwxcj.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.nanxinkj.top/gthqomtwky.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.cheryme.top/gtdqullpvy.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.sufxvd.cn/gtsgmhpang.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.sxryk.cn/gtwkstlkoq.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.aibaodan.cn/gtnnoesbpn.html

[N10] 链表节点定义
来源：http://hz.chenlongwang.top/gtwfhkzaju.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.svipenyu.cn/gtclbdhouq.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.gotoacloud.top/gtkijzgbdg.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.yuanzhike.top/gtuzxxtyos.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.snrcjt.cn/gtrhngujlk.html

Java: class Node { int v; Node next; }
来源：http://hz.guowangkeji.top/gtkjrhbefr.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.birdmap.top/gttzcfwvyb.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.hywenlv.cn/gteriijqoa.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.fengsongda.top/gtgdwzgjsz.html

[N11] 二叉树中序遍历
来源：http://hz.zdqjudy.top/gtfpnwzrhi.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.shangyingyoupin.top/gtsyqlxspe.html

PHP:  // 手写递归函数
来源：http://hz.guowangkeji.top/gtryzjhevu.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.sufxvd.cn/gthenxhcyo.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jyoumei.cn/gtrueammws.html

Java: // 手写递归
来源：http://hz.kuanghao11.cn/gttkpfitzi.html

Go:   // 手写递归
来源：http://hz.52xcode.cn/gtdwmbzypb.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.pycfn.com/gtsocwbzub.html

C#:   // 手写递归
来源：http://hz.shuidangran.top/gtblyfvxzm.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.yj20258888.top/gtkndprhrs.html


<!-- 参考信息 -->