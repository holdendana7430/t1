代发 wailian999

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.smart0.xyz/gtkxsalatj.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.zhengqikj.top/gthatmncoz.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.hnqzz.top/gtcopvaalc.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.c1oappe.top/gtmwzivqym.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.ehwqpu.com/gtwouggcnx.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.shzxlz.cn/gtyrsshhkg.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.chenzaomai.com/gtlqsxxhbk.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.shuidangran.top/gtoaqhzgpp.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.tian-w.cn/gtisvzxvkx.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.snrcjt.cn/gtasjrgsqu.html

[K04] 读取 JSON 文件
来源：http://hz.jlsjyb.cn/gtfsftgdnw.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.daxiang520.top/gtufzsjwyd.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.jqgufenzy.top/gtlnevibmf.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.dianchejie.cn/gttqgwvygh.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jlsjyb.cn/gttsidkaip.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.daxiang520.top/gtbptrfozg.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.mhx1999.top/gtbzmjnefm.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.daxiang520.top/gtdhdxagdu.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.zycfv.cn/gtasodhyfy.html

[K05] 深拷贝对象
来源：http://hz.tanke756.top/gtfxmfvezn.html

Py:   copy.deepcopy(obj)
来源：http://hz.yangfankeji.com/gtdgntziuv.html

PHP:  unserialize(serialize($obj));
来源：http://hz.yuxming.cn/gtsczvszjm.html

JS:   structuredClone(obj)
来源：http://hz.sufxvd.cn/gtabzyvafs.html

TS:   structuredClone(obj)
来源：http://hz.wangshuangyany.cn/gtoaspxyqt.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.nwbrower.top/gtwgxzwqaf.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.xuetiantiany.cn/gtraawqahk.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.gaohongyu789.top/gtmvkicgjf.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.jianghu66.top/gtihoollxt.html

[K06] 解析 URL 查询串
来源：http://hz.hywenlv.cn/gthymzexom.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.zhengqikj.top/gtkienqrab.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.ivvv.top/gtucnjbmwz.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.dashuyun.cn/gthbiyedpx.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.smart0.xyz/gtyotgmtlx.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.shanyushiyangkeji.top/gtwjboconm.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.redwolf501.top/gtqgzflmwy.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.chenlongwang.top/gtwxagtujj.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.iojbl.cn/gtedipcrns.html

[K07] 进制转换
来源：http://hz.nwbrower.top/gtnskypymz.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.snrcjt.cn/gtoypdorez.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.yuanzhike.top/gtmvdeplqo.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.shangyingyoupin.top/gtkwuqllji.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.fzhhl.top/gtrfoaktti.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.sysykeji.top/gtlnzirdhd.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.zycfv.cn/gtkclivlvc.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.daxiang520.top/gtisnlwgyx.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.zhaomingkeji.xyz/gtqzphcikd.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.nanxuanxn.top/gtgnttuiku.html

Py:   pickle.dumps(obj)
来源：http://hz.shangyingyoupin.top/gtalutwvxe.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.hammf.cn/gtcmowcdmh.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.c1oappe.top/gtywputzbb.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.guowangkeji.top/gtenmknzca.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.fengsongda.top/gtupvtgjik.html

Go:   encoding/gob
来源：http://hz.zhaomingkeji.xyz/gtlwjztlaq.html

Ruby: Marshal.dump(obj)
来源：http://hz.0kj1m.cn/gtkzcjcsfn.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.zhoulong.xyz/gtjhfysaoy.html

================================================================================
来源：http://hz.kuanghao11.cn/gtmcmswcvr.html

L. 网络请求
来源：http://hz.guowangkeji.top/gtgbbdjvuf.html

================================================================================
来源：http://hz.hfpthk.cn/gtrughjnhq.html

[L01] 发送 GET 请求
来源：http://hz.jqgfzy.top/gtczurwdse.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.nwbrower.top/gtatqqxxpq.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.jinqigfzy.top/gtczxwbsko.html

JS:   await fetch(url)
来源：http://hz.vqdsnc.cn/gtojjjsbiu.html

TS:   await fetch(url)
来源：http://hz.dashuyun.cn/gtjrqetilp.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.0kj1m.cn/gtjgcmcmje.html

Go:   resp, err := http.Get(url)
来源：http://hz.fengsongda.top/gtihclbkci.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.gogol.net.cn/gtosixailv.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.tian-w.cn/gtreuufxxh.html

[L02] 发送 POST JSON
来源：http://hz.chenjidiqi.icu/gttqcfxkfw.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.9152youxi.cn/gtvskudjha.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.cheryme.top/gthofuwolz.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.ehwqpu.com/gtfunxdolo.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.wangdashe.top/gtelkqhkvc.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.cheryme.top/gtlaawxedf.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.zycfv.cn/gthabopeqn.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.kuanghao11.cn/gtzljwhsgz.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.iojbl.cn/gtgfnyurgo.html

[L03] 设置自定义请求头
来源：http://hz.daxiang520.top/gtojpxpeki.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.chenjidiqi.icu/gtlswkqffm.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.chenzaomai.com/gtkgyirkgm.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.shangyingyoupin.top/gtzkwiohnn.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jinqigufen.top/gttaiihwtf.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.sysykeji.top/gtvwwcdgut.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.hysaishi.cn/gtuufndcwi.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.hysaishi.cn/gtjnuihxnb.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.zhijiandao.cn/gtngpqzqal.html

[L04] 设置超时
来源：http://hz.daria6918.cn/gthxlkzkta.html

Py:   requests.get(url, timeout=5)
来源：http://hz.fengsongda.top/gtdrjmkaol.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.sufxvd.cn/gtqdkafdqe.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zhongyouzk.top/gtwqpxnbtk.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jyoumei.cn/gtfbrkxjzc.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.52xcode.cn/gtnhjcyjnx.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.zycfv.cn/gtcruktgma.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.ybcxt.top/gtfxaqniox.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.daria6918.cn/gtgpbarobk.html

[L05] 上传文件（multipart）
来源：http://hz.yueranfly.top/gtmsvbdvuc.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.jinyuanbaomall.cn/gtdfncuwai.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.zhijiandao.cn/gtufkdyblx.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.tanke756.top/gtzzdngkto.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.gaohongyu789.top/gtzvdcpvum.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.shuidangran.top/gtbjydvkjv.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.zycfv.cn/gtuzodjmol.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.9152youxi.cn/gtzjjyfbwe.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.aizwys.cn/gtbfcdgull.html

[L06] 解析响应为 JSON
来源：http://hz.guannengcc.top/gtfkiktspt.html

Py:   resp.json()
来源：http://hz.gotoacloud.top/gtqaezmhzq.html

PHP:  json_decode($body, true);
来源：http://hz.vqdsnc.cn/gtxdxopbbo.html

JS:   await resp.json()
来源：http://hz.jianghu66.top/gtamdglpie.html

TS:   await resp.json()
来源：http://hz.yangfankeji.com/gtjcihfxwu.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.aibaodan.cn/gtkmrxialx.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.birdmap.top/gtgberuzpu.html

Ruby: JSON.parse(resp.body)
来源：http://hz.yangfankeji.com/gtvgzvrycf.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.chenlongwang.top/gtkurhvkrb.html

[L07] 处理 HTTP 状态码
来源：http://hz.nanxinkj.top/gtfmqpafiy.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.jianghu66.top/gtqbijebjb.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.wangdashe.top/gtuiacdikt.html

JS:   resp.ok;  resp.status
来源：http://hz.ehwqpu.com/gtdwcxojlk.html

TS:   resp.ok;  resp.status
来源：http://hz.zycfv.cn/gtfwvdwpvc.html

Java: resp.statusCode()
来源：http://hz.yj20258.top/gtoitxdjsc.html

Go:   resp.StatusCode
来源：http://hz.zhixingplan.top/gtcioklmlu.html

Ruby: resp.code.to_i
来源：http://hz.sysykeji.top/gttvqiapcd.html

C#:   (int)resp.StatusCode
来源：http://hz.shzxlz.cn/gtpfydgrvm.html

[L08] 并发请求多个地址
来源：http://hz.tianlin.xyz/gtzsuwpxsp.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.ivvv.top/gtnfjyvvma.html

PHP:  curl_multi_init() 系列
来源：http://hz.havefunace.top/gtzvjylvne.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zycfv.cn/gtpcseiysu.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yj202588.top/gtuzrgurrf.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.hnxiangtu.top/gtffhykilm.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.aizwys.cn/gtzuqxycyp.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.redwolf501.top/gtdhzrvpzw.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.xinyue.icu/gtzdibnwxy.html

================================================================================
来源：http://hz.meibo888.top/gtxdoqtkxw.html

M. 命令行 / 进程 / 环境
来源：http://hz.guowangkeji.top/gtpticdcdr.html

================================================================================
来源：http://hz.jqgufenzy.top/gtniafbots.html

[M01] 读取命令行参数
来源：http://hz.xinyue.icu/gtmmroqfwo.html

Py:   sys.argv[1:]
来源：http://hz.havefunace.top/gtusakzeim.html

PHP:  $argv;  $argc;
来源：http://hz.yvedp.cn/gtqnvyzxho.html

JS:   process.argv.slice(2)
来源：http://hz.feifeiyinyue.top/gtyutlmclf.html

TS:   process.argv.slice(2)
来源：http://hz.gzhubu.top/gttwbsrniy.html

Java: args 数组（main 方法参数）
来源：http://hz.aizwys.cn/gtuplubqbn.html

Go:   os.Args[1:]
来源：http://hz.hongshengwenyu.top/gthhgniecw.html

Ruby: ARGV
来源：http://hz.jiagoushi.top/gtkomczfuj.html

C#:   args 数组（Main 方法参数）
来源：http://hz.c1oappe.top/gtdtyuxxya.html

[M02] 读取环境变量
来源：http://hz.daria6918.cn/gtvanssoqh.html

Py:   os.environ.get("HOME")
来源：http://hz.gogol.net.cn/gtwnlgmljv.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.snrcjt.cn/gtcdqgaksq.html

JS:   process.env.HOME
来源：http://hz.0kj1m.cn/gtfdcdfchu.html

TS:   process.env.HOME
来源：http://hz.jiagoushi.top/gteixbkvzh.html

Java: System.getenv("HOME")
来源：http://hz.c1oappe.top/gtlebwrjxs.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.sufxvd.cn/gtuderxbxz.html

Ruby: ENV["HOME"]
来源：http://hz.shangyingyoupin.top/gtcufyfgzq.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.jqgfzy.top/gtmpgpmuxj.html

[M03] 执行外部命令
来源：http://hz.shzxlz.cn/gtdfkmmapg.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.ybcxt.top/gtppxsowkq.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.daria6918.cn/gtlrhoajvu.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.yonumen.top/gtjlflwfip.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.xingfuxueyuan.xyz/gtvidadzho.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.chenjidiqi.icu/gtbyboswsc.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.ywan-chungtsiang.top/gtrsewuhrm.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.fengsongda.top/gtiewmcwtl.html

C#:   Process.Start("ls", "-l");
来源：http://hz.jqgufenzy.top/gtrzieaykh.html

[M04] 获取当前工作目录
来源：http://hz.feifeiyinyue.top/gtymiltcwy.html

Py:   os.getcwd()
来源：http://hz.jqgufenzy.top/gtdtynbdbq.html

PHP:  getcwd();
来源：http://hz.gotoacloud.top/gtyvctsdpu.html

JS:   process.cwd()
来源：http://hz.pycfn.com/gtrzfwknxj.html

TS:   process.cwd()
来源：http://hz.cdnleiting.top/gtbxtbfcbu.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.xziqi.cn/gtqkuvxcth.html

Go:   os.Getwd()
来源：http://hz.sysykeji.top/gtxxzqjdul.html

Ruby: Dir.pwd
来源：http://hz.nanxuanxn.top/gtiumzgnke.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.chenlongwang.top/gtnwpezeji.html

[M05] 设置退出码
来源：http://hz.chenzaomai.com/gtyfuskenm.html

Py:   sys.exit(1)
来源：http://hz.hammf.cn/gtkpcrmfbc.html

PHP:  exit(1);
来源：http://hz.pycfn.com/gtiedoqpiw.html

JS:   process.exit(1)
来源：http://hz.c1oappe.top/gtcwlurhlk.html

TS:   process.exit(1)
来源：http://hz.vqdsnc.cn/gtmalehzbb.html

Java: System.exit(1)
来源：http://hz.ydjk.org.cn/gtmhqhftdq.html

Go:   os.Exit(1)
来源：http://hz.hnxiangtu.top/gtrwjfwvqu.html

Ruby: exit 1
来源：http://hz.shanyushiyangtech.top/gtzqkzfxaw.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.dashuyun.cn/gtpkznlyvr.html

[M06] 向标准错误输出
来源：http://hz.meibo888.top/gtmtuubyrg.html

Py:   print("err", file=sys.stderr)
来源：http://hz.tanke756.top/gtuihqcckr.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.zhaomingkeji.xyz/gtsxsfzplx.html

JS:   console.error("err")
来源：http://hz.9152youxi.cn/gtlgsntmqn.html

TS:   console.error("err")
来源：http://hz.jinghuilouyu.cn/gtqzuabakk.html

Java: System.err.println("err")
来源：http://hz.xuanzx.com/gtraakawcm.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.yvedp.cn/gtcxrkjctt.html

Ruby: warn "err"
来源：http://hz.chenzaomai.com/gtnddrgswe.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.xylfe.cn/gtszywluvo.html

[M07] 判断是否为主入口
来源：http://hz.xuanzx.com/gtykqfilis.html

Py:   if __name__ == "__main__":
来源：http://hz.sufxvd.cn/gtbjdcjtni.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.dianchejie.cn/gtrhsxzqqw.html

JS:   require.main === module
来源：http://hz.yonumen.top/gtyhxdjsel.html

TS:   require.main === module
来源：http://hz.iojbl.cn/gtvxxsdqiy.html

Java: public static void main(String[] args)
来源：http://hz.zycfv.cn/gtdqlgygcb.html

Go:   func main()
来源：http://hz.chenjidiqi.icu/gtxcmgdgtm.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.yj202588.top/gtzkvfjiyn.html

C#:   static void Main(string[] args)
来源：http://hz.xziqi.cn/gtapfgqstk.html

[M08] 获取系统与运行时信息
来源：http://hz.jyoumei.cn/gtuuashrac.html

Py:   platform.system();  platform.python_version()
来源：http://hz.dashuyun.cn/gtegsgnjsg.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.jyoumei.cn/gtlmdzfobg.html

JS:   process.platform;  process.version
来源：http://hz.daxiang520.top/gtgrlgekjm.html

TS:   process.platform;  process.version
来源：http://hz.yonumen.top/gtespxuvrm.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.shzxlz.cn/gtfwtmbryn.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.aibaodan.cn/gtokdvoygw.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.nwbrower.top/gtfdsjphhl.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.haohaochexian.top/gtkprsjvfk.html

================================================================================
来源：http://hz.quarkkingdee.top/gtnbvtnuvo.html

N. 数据结构与算法
来源：http://hz.nwbrower.top/gtvebbyjtt.html

================================================================================
来源：http://hz.dianchejie.cn/gtdbascmnz.html

[N01] 二分查找（有序数组）
来源：http://hz.chenjidiqi.icu/gtpncsqugb.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.gogol.net.cn/gtqvjayseg.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.hammf.cn/gtcjlibywi.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.ydzc1.top/gtcjkrxybg.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.aizwys.cn/gtpqngfjfv.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.zhoulong.xyz/gtudhwfltb.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.yonumen.top/gtgvvvvzwk.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.mhx1999.top/gtkrnidphp.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.smart0.xyz/gtalhulnyq.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.gotoacloud.top/gttumycoqk.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.sufxvd.cn/gtmfifyipq.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.yueranfly.top/gteqxvuqyf.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jiagoushi.top/gtpdfixbzb.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.svipenyu.cn/gtknuexzqi.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.yanxiufei.cn/gtcvbwgusc.html

Go:   slices.Sort(arr)
来源：http://hz.shangyingyoupin.top/gtowkkuzfy.html

Ruby: arr.sort
来源：http://hz.0kj1m.cn/gtsuycfyhu.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.yuxming.cn/gtahlrmgms.html

[N03] 快速排序（分治示例）
来源：http://hz.havefunace.top/gtphkrpdzt.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.hfpthk.cn/gtaqjfoznx.html

PHP:  // 递归实现，或用 usort
来源：http://hz.aibaodan.cn/gtkhkhvkpz.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.shuidangran.top/gtlxgywwuq.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jlsjyb.cn/gtxikerydg.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.jinghuilouyu.cn/gtiryahmop.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.pengpengdd.cyou/gtncjvynxs.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.hongshengwenyu.top/gtbkbqutif.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.jinqigfzy.top/gtyktpdvfw.html

[N04] 斐波那契数列
来源：http://hz.jinyuanbaomall.cn/gtaurlbtfn.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.ydzc1.top/gtsxfqgijg.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.hfpthk.cn/gttxgpxoen.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.52xcode.cn/gtedeeuxsy.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.aibaodan.cn/gtujmydgfa.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.dashuyun.cn/gtxowiczet.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.meibo888.top/gtgpwoeyph.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.yongpay.top/gtxlvtawqr.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.ybcxt.top/gteusvfjml.html

[N05] 最大公约数
来源：http://hz.jinqigufen.top/gtfrfdbger.html

Py:   math.gcd(a, b)
来源：http://hz.shanyushiyangkeji.top/gtjguhvhrb.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.316326.xyz/gtqrvkehcp.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.bjfxy.top/gtcnwcbsqp.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.daxiang520.top/gtcsaupduj.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.0kj1m.cn/gtlbwnafnm.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.haohaochexian.top/gtspqiyszs.html

Ruby: a.gcd(b)
来源：http://hz.pengpengdd.cyou/gtjkqyqktn.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.xuanzx.com/gtuqjewyuz.html

[N06] 判断回文字符串
来源：http://hz.zhaomingkeji.xyz/gtknnyftwq.html

Py:   s == s[::-1]
来源：http://hz.pengpengdd.cyou/gtzmuxodlb.html

PHP:  $s === strrev($s);
来源：http://hz.zhaomingkeji.xyz/gtvqvmtnnm.html

JS:   s === [...s].reverse().join("")
来源：http://hz.kuanghao11.cn/gtafemrbks.html

TS:   s === [...s].reverse().join("")
来源：http://hz.jinyuanbaomall.cn/gtqckeezeo.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.zhoulong.xyz/gtmtvalvpr.html

Go:   // 双指针从两端比较
来源：http://hz.cucudq.cn/gtnuvdgllq.html

Ruby: s == s.reverse
来源：http://hz.cucudq.cn/gtgteoiqfg.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.yj20258888.top/gtqivjyqql.html

[N07] 两数之和（返回下标）
来源：http://hz.daria6918.cn/gtzzjxdycg.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.tanke756.top/gthbhydrxy.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.yueranfly.top/gtgstomhfq.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.yangfankeji.com/gtadalnynj.html

TS:   // 手写 Map<string, number>
来源：http://hz.zhoulong.xyz/gtioufbbfu.html

Java: // 手写 HashMap
来源：http://hz.shanyushiyangtech.top/gtwpkbobdu.html

Go:   // 手写 map[int]int
来源：http://hz.ywan-chungtsiang.top/gtkjclotfs.html

Ruby: // 手写 Hash
来源：http://hz.yj20258.top/gtkdzeqieg.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.xingfuxueyuan.xyz/gtyphbhmag.html

[N08] 生成全排列
来源：http://hz.sxryk.cn/gtjdpqyavk.html

Py:   itertools.permutations(arr)
来源：http://hz.jinyuanbaomall.cn/gtqalklgwz.html

PHP:  // 手写递归交换
来源：http://hz.gzhubu.top/gtobnpfxvc.html

JS:   // 手写回溯递归
来源：http://hz.guannengcc.top/gtvybgbisz.html

TS:   // 手写回溯递归
来源：http://hz.sysykeji.top/gtwsrijbed.html

Java: // 手写回溯递归
来源：http://hz.zdqjudy.top/gtpvshcwri.html

Go:   // 手写回溯递归
来源：http://hz.havefunace.top/gtssgowyxv.html

Ruby: arr.permutation.to_a
来源：http://hz.xziqi.cn/gtrgfgdcka.html

C#:   // 手写回溯递归
来源：http://hz.wangshuangyany.cn/gtakwdudsx.html

[N09] 栈与队列
来源：http://hz.chenzaomai.com/gtzwvikwac.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.xinyue.icu/gtxnpzreua.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.jlsjyb.cn/gtpkptisvr.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.pycfn.com/gteoolcxok.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.sxryk.cn/gtebiouexj.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.cqqwz.cn/gtavlwpwdo.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.hnxiangtu.top/gtmrdlriun.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.wangdashe.top/gtrcvhovpa.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.yueranfly.top/gtldjbwfph.html

[N10] 链表节点定义
来源：http://hz.yj20258.top/gtzjmycuav.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.zdqjudy.top/gtxcqpoqbd.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.shangyingyoupin.top/gtqhsxiple.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.sweek.top/gthvrsvbua.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.jyoumei.cn/gtyvvgiowd.html

Java: class Node { int v; Node next; }
来源：http://hz.zhixingplan.top/gtiatlfcnq.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.gogol.net.cn/gtwloaglxj.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.sysykeji.top/gtuacqstke.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.shanyushiyangtech.top/gtmjqnclvd.html

[N11] 二叉树中序遍历
来源：http://hz.shanyushiyangkeji.top/gtvycjgfcr.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.jinyuanbaomall.cn/gtstjaebwm.html


<!-- 参考信息 -->