代发 wailian999

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.shzxlz.cn/gtcykoydar.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.gzhubu.top/gtejnqxzaf.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.andypj.xyz/gtupheqlrg.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.yonumen.top/gttcmdaxak.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.yueranfly.top/gtmgvwxwhr.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.nwbrower.top/gtyjownjlb.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.ybcxt.top/gtkzpzzbkq.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.9152youxi.cn/gthivahshy.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.zhixingplan.top/gtowutiife.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.jyoumei.cn/gtxnqntjcs.html

[K04] 读取 JSON 文件
来源：http://hz.zhoulong.xyz/gtphgmczgn.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.xziqi.cn/gtvehvxbxf.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.fzhhl.top/gtorffkefd.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yj20258888.top/gtibkvmbpv.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.aibaodan.cn/gtakrbquwd.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.jinqigufen.top/gtttkehwyj.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.daxiang520.top/gthszmzlvs.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.chenjidiqi.icu/gtorsfbitd.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.yongpay.top/gtxlropzrg.html

[K05] 深拷贝对象
来源：http://hz.zhijiandao.cn/gtaegvsiov.html

Py:   copy.deepcopy(obj)
来源：http://hz.meibo888.top/gtglawbjsn.html

PHP:  unserialize(serialize($obj));
来源：http://hz.daxiang520.top/gteghnjhvy.html

JS:   structuredClone(obj)
来源：http://hz.hfpthk.cn/gtllkwpzqu.html

TS:   structuredClone(obj)
来源：http://hz.0kj1m.cn/gtedeawoom.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.tian-w.cn/gtenutwunh.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.gotoacloud.top/gtephjseug.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.shangyingyoupin.top/gtcdlmrhsu.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.snrcjt.cn/gtzcrbrgqu.html

[K06] 解析 URL 查询串
来源：http://hz.dashuyun.cn/gtmztcmkgp.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.ivvv.top/gtanejwyra.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.cqqwz.cn/gtxstshthb.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.xingfuxueyuan.xyz/gtzplosslh.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.bjfxy.top/gteqpyjnde.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.jlsjyb.cn/gtuznobtqv.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.shanyushiyangkeji.top/gtsblmntfx.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.gzhubu.top/gtgybufkjz.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.bjfxy.top/gtxjerlydf.html

[K07] 进制转换
来源：http://hz.cucudq.cn/gtnckbtsnd.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.cdnleiting.top/gtnbwzrnwu.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.zhiwuduotai.top/gtvndaapwt.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.gzhubu.top/gtpbipfuwv.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.shzxlz.cn/gtaylmljpq.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.daria6918.cn/gtetfcpida.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.dianchejie.cn/gtligpmxke.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.birdmap.top/gtnzjxnxoy.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.yvedp.cn/gtmxxectll.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.cashguo.top/gtwzjuvgew.html

Py:   pickle.dumps(obj)
来源：http://hz.ybcxt.top/gtpxbqtymk.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.dashuyun.cn/gtrvtndzmw.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.yongpay.top/gtgrqnxiag.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.ppjwa.cn/gtsnnljkwc.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.jqgufenzy.top/gtwhiprbuw.html

Go:   encoding/gob
来源：http://hz.redwolf501.top/gtqyvllmdk.html

Ruby: Marshal.dump(obj)
来源：http://hz.ydzc1.top/gtpcsxfuvn.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.316326.xyz/gtrotcgunw.html

================================================================================
来源：http://hz.aibaodan.cn/gtpmgamwkx.html

L. 网络请求
来源：http://hz.jqgfzy.top/gtdbivhwdy.html

================================================================================
来源：http://hz.ehwqpu.com/gtmqofdpvm.html

[L01] 发送 GET 请求
来源：http://hz.cheryme.top/gtzkmnduhw.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.aibaodan.cn/gttktgdhqy.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.jyoumei.cn/gtepvhhyqb.html

JS:   await fetch(url)
来源：http://hz.meibo888.top/gtfkccgcfl.html

TS:   await fetch(url)
来源：http://hz.yongpay.top/gtbebdxcfn.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.zhiwuduotai.top/gtehkkzyom.html

Go:   resp, err := http.Get(url)
来源：http://hz.snrcjt.cn/gtpsgqgwwn.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.zhixingplan.top/gtqxcbnrko.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.vqdsnc.cn/gtmimusznu.html

[L02] 发送 POST JSON
来源：http://hz.0kj1m.cn/gtbxkzkegl.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.shangyingyoupin.top/gtfrnidchd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.cucudq.cn/gtsotcjgpv.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.havefunace.top/gtrzeikksw.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jiagoushi.top/gtdoagveyb.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.zhiwuduotai.top/gtjxburqiz.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.nanxinkj.top/gtmylnxcrq.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.cucudq.cn/gtsvxmhoeg.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.andypj.xyz/gtlxhsmlxi.html

[L03] 设置自定义请求头
来源：http://hz.feifeiyinyue.top/gtfednrwlb.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.jinqigufen.top/gtgnshgqix.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.hongshengwenyu.top/gtbtuagwqt.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yangfankeji.com/gtsozrvvib.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zhixingplan.top/gtcvzidlmg.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.hammf.cn/gtfshnxutn.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.tian-w.cn/gtztjqimqz.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.yueranfly.top/gtefekddqm.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.ydjk.org.cn/gtrldkowja.html

[L04] 设置超时
来源：http://hz.guannengcc.top/gtmeyxvhcu.html

Py:   requests.get(url, timeout=5)
来源：http://hz.jqgfzy.top/gtnzvsyorl.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.yvedp.cn/gtymyvqrin.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zdqjudy.top/gtuqqxzvbm.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.guowangkeji.top/gtcxkubeit.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.gzhubu.top/gtfqweayrn.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.bjfxy.top/gtusiiikqr.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.xuanzx.com/gtfaxpppif.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.vqdsnc.cn/gtejqgkthr.html

[L05] 上传文件（multipart）
来源：http://hz.yj202588.top/gtdknsdzuy.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.zhongyouzk.top/gtyjimwrzs.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.hfpthk.cn/gtkxutgkpw.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.tianlin.xyz/gtdfvnjvme.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.sweek.top/gtgrhyoims.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.svipenyu.cn/gtxdiuciub.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.ydjk.org.cn/gtxnnwucfo.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.nanxinkj.top/gtrdueyoya.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.nanxuanxn.top/gtwzmoqhuu.html

[L06] 解析响应为 JSON
来源：http://hz.shanyushiyangtech.top/gtcazxdeaw.html

Py:   resp.json()
来源：http://hz.vqdsnc.cn/gtnzlyqvyg.html

PHP:  json_decode($body, true);
来源：http://hz.ydjk.org.cn/gtcpgvmnsn.html

JS:   await resp.json()
来源：http://hz.yj20258888.top/gtviztxayn.html

TS:   await resp.json()
来源：http://hz.chenlongwang.top/gtchshujyd.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.nanxuanxn.top/gtzdfhxwtv.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.cashguo.top/gtlqgnoaal.html

Ruby: JSON.parse(resp.body)
来源：http://hz.pycfn.com/gtiwabmzkk.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.tian-w.cn/gthaiijenw.html

[L07] 处理 HTTP 状态码
来源：http://hz.tianlin.xyz/gtsxnpjyqh.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.meibo888.top/gtlxgxzwix.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.xziqi.cn/gtpnkzvvwe.html

JS:   resp.ok;  resp.status
来源：http://hz.tianlin.xyz/gtlprpaxta.html

TS:   resp.ok;  resp.status
来源：http://hz.yuanzhike.top/gtnbwffonu.html

Java: resp.statusCode()
来源：http://hz.jinghuilouyu.cn/gtvpbxluqu.html

Go:   resp.StatusCode
来源：http://hz.zhengqikj.top/gtjzkzfdcd.html

Ruby: resp.code.to_i
来源：http://hz.jyoumei.cn/gtkxdglbhe.html

C#:   (int)resp.StatusCode
来源：http://hz.zhengqikj.top/gtnyqhblcm.html

[L08] 并发请求多个地址
来源：http://hz.chenzaomai.com/gtwiuijpio.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.yj20258888.top/gtkdirziqh.html

PHP:  curl_multi_init() 系列
来源：http://hz.svipenyu.cn/gthjhgixhj.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.xuetiantiany.cn/gtuxylcbag.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.hfpthk.cn/gtdbtpirbg.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.gaohongyu789.top/gtnrdqbqdp.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.shanyushiyangtech.top/gtarexfdga.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.mhx1999.top/gtvoirdgsv.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.ydjk.org.cn/gtsjxwiudl.html

================================================================================
来源：http://hz.yuanzhike.top/gtownnmbxa.html

M. 命令行 / 进程 / 环境
来源：http://hz.chenjidiqi.icu/gtvbfpfxyl.html

================================================================================
来源：http://hz.9152youxi.cn/gtgojmeikt.html

[M01] 读取命令行参数
来源：http://hz.feifeiyinyue.top/gtribbunfg.html

Py:   sys.argv[1:]
来源：http://hz.yvedp.cn/gtijtnrgis.html

PHP:  $argv;  $argc;
来源：http://hz.zhaomingkeji.xyz/gtrnocdbdl.html

JS:   process.argv.slice(2)
来源：http://hz.cucudq.cn/gtvontfwbr.html

TS:   process.argv.slice(2)
来源：http://hz.chenjidiqi.icu/gtascgvriy.html

Java: args 数组（main 方法参数）
来源：http://hz.yonumen.top/gtqvoocqdf.html

Go:   os.Args[1:]
来源：http://hz.gogol.net.cn/gtayfdncyf.html

Ruby: ARGV
来源：http://hz.feifeiyinyue.top/gtngpdebtn.html

C#:   args 数组（Main 方法参数）
来源：http://hz.xylfe.cn/gtykvszzye.html

[M02] 读取环境变量
来源：http://hz.hfpthk.cn/gtdkepmepq.html

Py:   os.environ.get("HOME")
来源：http://hz.tanke756.top/gtlxyblfaa.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.yj20258.top/gtzqmykrep.html

JS:   process.env.HOME
来源：http://hz.havefunace.top/gtpdegufej.html

TS:   process.env.HOME
来源：http://hz.tianlin.xyz/gtkmoxbzzj.html

Java: System.getenv("HOME")
来源：http://hz.fzhhl.top/gtdywgqhlx.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.yuanzhike.top/gtgjtqiwnn.html

Ruby: ENV["HOME"]
来源：http://hz.zhijiandao.cn/gtbgqzwkco.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.hammf.cn/gtqnmlchup.html

[M03] 执行外部命令
来源：http://hz.meibo888.top/gtiqosoivq.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.hnxiangtu.top/gtukgbyhet.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.shzxlz.cn/gtbysovsyk.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.ppjwa.cn/gtaljqwgpr.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.yuanzhike.top/gtcreeeash.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.mhx1999.top/gtonvjbhma.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.52xcode.cn/gtonjrpmat.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.xuetiantiany.cn/gtcmklykjr.html

C#:   Process.Start("ls", "-l");
来源：http://hz.shzxlz.cn/gtziutjrxt.html

[M04] 获取当前工作目录
来源：http://hz.mhx1999.top/gtdimwcmcj.html

Py:   os.getcwd()
来源：http://hz.cdnleiting.top/gtmlvczzik.html

PHP:  getcwd();
来源：http://hz.hnqzz.top/gtlumhoxfn.html

JS:   process.cwd()
来源：http://hz.hnqzz.top/gtectjppqt.html

TS:   process.cwd()
来源：http://hz.cdnleiting.top/gtjdgerfsy.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.aibaodan.cn/gtetzdtqts.html

Go:   os.Getwd()
来源：http://hz.yangfankeji.com/gtimpuhcje.html

Ruby: Dir.pwd
来源：http://hz.ivvv.top/gtydpypqoj.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.feifeiyinyue.top/gttzfrsvby.html

[M05] 设置退出码
来源：http://hz.dianchejie.cn/gtsnufhxpf.html

Py:   sys.exit(1)
来源：http://hz.jianghu66.top/gttbgktuue.html

PHP:  exit(1);
来源：http://hz.cheryme.top/gtoirawgfr.html

JS:   process.exit(1)
来源：http://hz.aizwys.cn/gtepxliigh.html

TS:   process.exit(1)
来源：http://hz.daria6918.cn/gtqcsoutzd.html

Java: System.exit(1)
来源：http://hz.nanxuanxn.top/gtguxkzmzy.html

Go:   os.Exit(1)
来源：http://hz.xingfuxueyuan.xyz/gtqgbndxvx.html

Ruby: exit 1
来源：http://hz.zhengqikj.top/gtdqnvslpr.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.shangyingyoupin.top/gtbdupfolv.html

[M06] 向标准错误输出
来源：http://hz.aizwys.cn/gtfaoeuqij.html

Py:   print("err", file=sys.stderr)
来源：http://hz.wangdashe.top/gtbygcraaq.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.meibo888.top/gtnqtebrgy.html

JS:   console.error("err")
来源：http://hz.hysaishi.cn/gtmydzxvrf.html

TS:   console.error("err")
来源：http://hz.ydzc1.top/gtiosdhxao.html

Java: System.err.println("err")
来源：http://hz.jiagoushi.top/gtsmdlzgjb.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.jinqigfzy.top/gtigxvfive.html

Ruby: warn "err"
来源：http://hz.shuidangran.top/gtwbqzxfaj.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.shanyushiyangtech.top/gtvtusnxjn.html

[M07] 判断是否为主入口
来源：http://hz.yuanzhike.top/gtagvhztok.html

Py:   if __name__ == "__main__":
来源：http://hz.yanxiufei.cn/gtvsiiuorr.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.tian-w.cn/gtgcuhoawa.html

JS:   require.main === module
来源：http://hz.dashuyun.cn/gtoppuuiim.html

TS:   require.main === module
来源：http://hz.jinqigufen.top/gtkmclwsjf.html

Java: public static void main(String[] args)
来源：http://hz.pengpengdd.cyou/gtacgltimz.html

Go:   func main()
来源：http://hz.yueranfly.top/gtbqzlcudg.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.haohaochexian.top/gtblzibqom.html

C#:   static void Main(string[] args)
来源：http://hz.sysykeji.top/gtjavcqkcs.html

[M08] 获取系统与运行时信息
来源：http://hz.birdmap.top/gtjykumgww.html

Py:   platform.system();  platform.python_version()
来源：http://hz.jiagoushi.top/gtdqzrazlp.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.ivvv.top/gtsuuuzkgc.html

JS:   process.platform;  process.version
来源：http://hz.shanyushiyangtech.top/gtzglinuau.html

TS:   process.platform;  process.version
来源：http://hz.shuidangran.top/gtxtvbhfoe.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.gogol.net.cn/gtduntxmin.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.havefunace.top/gtqlcqrxiv.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.hnqzz.top/gthybovbmw.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.cdnleiting.top/gtmnprcxiq.html

================================================================================
来源：http://hz.jlsjyb.cn/gttufwohhl.html

N. 数据结构与算法
来源：http://hz.cdnleiting.top/gtdusilphs.html

================================================================================
来源：http://hz.wangdashe.top/gtyaobrjjr.html

[N01] 二分查找（有序数组）
来源：http://hz.chenlongwang.top/gthvuwexkd.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.smart0.xyz/gtbeyyrtgp.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.quarkkingdee.top/gtzkjjveeu.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.fengsongda.top/gtmflrkvzj.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.xuetiantiany.cn/gtncggamtc.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.jiagoushi.top/gtgcjgaxnk.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.chenzaomai.com/gtkoqsurvu.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.tanke756.top/gtwnecqlnn.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.shuidangran.top/gttodkpvut.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.gogol.net.cn/gtyxbyhgnp.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.wangshuangyany.cn/gtndthxotb.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.xingfuxueyuan.xyz/gtjfbbiruv.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jinghuilouyu.cn/gtfqmdrfuq.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.c1oappe.top/gtydgqxius.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.jianghu66.top/gtuadbrzvr.html

Go:   slices.Sort(arr)
来源：http://hz.fzhhl.top/gtpsyrvqey.html

Ruby: arr.sort
来源：http://hz.chenlongwang.top/gtroflkfvf.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.fengsongda.top/gtupdotsjv.html

[N03] 快速排序（分治示例）
来源：http://hz.gaohongyu789.top/gtdthirtmn.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.zhixingplan.top/gtznulscmb.html

PHP:  // 递归实现，或用 usort
来源：http://hz.birdmap.top/gtmrkafcsr.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.0kj1m.cn/gtkbmngbud.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.xingfuxueyuan.xyz/gttrpcevuw.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.guannengcc.top/gtcpcqurvw.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.bjfxy.top/gtrqnnufhm.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.cqqwz.cn/gttisowvlp.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.birdmap.top/gtddhijlfs.html

[N04] 斐波那契数列
来源：http://hz.chenjidiqi.icu/gtucmsfwfu.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.ivvv.top/gtemkhcbrl.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.guowangkeji.top/gttonyymrl.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.nwbrower.top/gtzgrfbgdy.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.hammf.cn/gtkmolubeu.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.vqdsnc.cn/gthxgobsqy.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.sufxvd.cn/gtjrwqnvtv.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.hfpthk.cn/gtucfrzvae.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.jianghu66.top/gtzdcxbruh.html

[N05] 最大公约数
来源：http://hz.sufxvd.cn/gtypvcoswd.html

Py:   math.gcd(a, b)
来源：http://hz.gogol.net.cn/gttauoagix.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.feifeiyinyue.top/gtcjkihpaa.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.wangshuangyany.cn/gtksiaheoe.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.52xcode.cn/gtveghpubp.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.yj20258888.top/gtvcqcfpla.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.ydzc1.top/gtgvsenmzt.html

Ruby: a.gcd(b)
来源：http://hz.yuanzhike.top/gtlrmchixy.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.quarkkingdee.top/gtlnrfesch.html

[N06] 判断回文字符串
来源：http://hz.shanyushiyangtech.top/gtwuvotups.html

Py:   s == s[::-1]
来源：http://hz.ehwqpu.com/gteixcadvt.html

PHP:  $s === strrev($s);
来源：http://hz.yanxiufei.cn/gtuzkqieiz.html

JS:   s === [...s].reverse().join("")
来源：http://hz.yj20258888.top/gtjxkcneha.html

TS:   s === [...s].reverse().join("")
来源：http://hz.wangshuangyany.cn/gtnmfmljlm.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.ivvv.top/gtaazfhuhm.html

Go:   // 双指针从两端比较
来源：http://hz.havefunace.top/gtzoycrdai.html

Ruby: s == s.reverse
来源：http://hz.zhoulong.xyz/gtislqemxo.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.nwbrower.top/gtokmmygxi.html

[N07] 两数之和（返回下标）
来源：http://hz.yj202588.top/gtdvteapxx.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.yueranfly.top/gtfgcoeofx.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.haohaochexian.top/gtwikijucc.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.nwbrower.top/gtrdbvkjgg.html

TS:   // 手写 Map<string, number>
来源：http://hz.sxryk.cn/gtidyzmmho.html

Java: // 手写 HashMap
来源：http://hz.wangdashe.top/gtiiqdhdad.html

Go:   // 手写 map[int]int
来源：http://hz.ywan-chungtsiang.top/gtwgpbywha.html

Ruby: // 手写 Hash
来源：http://hz.xuanzx.com/gtlhycgfrh.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.chenzaomai.com/gtqbiqoipv.html

[N08] 生成全排列
来源：http://hz.sufxvd.cn/gtnvjakycm.html

Py:   itertools.permutations(arr)
来源：http://hz.ppjwa.cn/gthpukgbqh.html

PHP:  // 手写递归交换
来源：http://hz.hfpthk.cn/gtsyxlqxxx.html

JS:   // 手写回溯递归
来源：http://hz.chenjidiqi.icu/gtuqbavupz.html

TS:   // 手写回溯递归
来源：http://hz.daxiang520.top/gthtvtshdk.html

Java: // 手写回溯递归
来源：http://hz.xuanzx.com/gtzvtcbhlh.html

Go:   // 手写回溯递归
来源：http://hz.0kj1m.cn/gtbszpqtgj.html

Ruby: arr.permutation.to_a
来源：http://hz.aizwys.cn/gthqrrlzht.html

C#:   // 手写回溯递归
来源：http://hz.sweek.top/gtzvktzovg.html

[N09] 栈与队列
来源：http://hz.yuanzhike.top/gtjaahgiyq.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.snrcjt.cn/gtjgrhqqae.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.andypj.xyz/gtpufykcro.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.hywenlv.cn/gtnjwznwgz.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.0kj1m.cn/gtnokuwsek.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.xziqi.cn/gtsmrmuwfn.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.tian-w.cn/gtlovbfcjv.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.pycfn.com/gtywzdyrzi.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.shanyushiyangkeji.top/gtdizvvacy.html

[N10] 链表节点定义
来源：http://hz.jinyuanbaomall.cn/gtjlgapoiu.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.hnqzz.top/gtjumzlxvu.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.xingfuxueyuan.xyz/gtbpqvoezw.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.9152youxi.cn/gtoqokgfxh.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.cdnleiting.top/gtrwbahcmo.html

Java: class Node { int v; Node next; }
来源：http://hz.birdmap.top/gtgmvjsrbd.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.birdmap.top/gtllgwvjrn.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.c1oappe.top/gthbpbsyba.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.yueranfly.top/gtlcalvqwr.html

[N11] 二叉树中序遍历
来源：http://hz.jinghuilouyu.cn/gtordbcimy.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.yonumen.top/gtyzuccvah.html


<!-- 参考信息 -->