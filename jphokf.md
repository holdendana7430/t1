代发 wailian999

[K02] JSON 字符串转对象
来源：http://hz.yongpay.top/gtkvydwixl.html

Py:   json.loads(s)
来源：http://hz.yanxiufei.cn/gtxstjnmql.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.birdmap.top/gtrmftaccs.html

JS:   JSON.parse(s)
来源：http://hz.shanyushiyangtech.top/gtqjjkcpui.html

TS:   JSON.parse(s)
来源：http://hz.guowangkeji.top/gtdnwckdye.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.hongshengwenyu.top/gtywpkaxqv.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.jyoumei.cn/gtdmlekdsn.html

Ruby: JSON.parse(s)
来源：http://hz.c1oappe.top/gttljwuyqx.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.meibo888.top/gtptpyccce.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.shzxlz.cn/gtetrbhijo.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.yuanzhike.top/gtoczbtwjj.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.hywenlv.cn/gtluzvaomh.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.meibo888.top/gtdargjvmq.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.wangdashe.top/gtkgaolkya.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.aibaodan.cn/gtvmkjoqqn.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.andypj.xyz/gtdesxoepw.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.cashguo.top/gtmzsfotur.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.tianlin.xyz/gtqxtkduia.html

[K04] 读取 JSON 文件
来源：http://hz.xuetiantiany.cn/gtkgnglbhp.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.hongshengwenyu.top/gtqbydlelv.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.gotoacloud.top/gtearvjcsv.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.aizwys.cn/gtkncjfmqr.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jiagoushi.top/gtyasbxikn.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.tianlin.xyz/gtixgvmvsk.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.sxryk.cn/gtqpfiqaag.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.wangshuangyany.cn/gtwdgakyoa.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.aibaodan.cn/gtmydkdhgg.html

[K05] 深拷贝对象
来源：http://hz.c1oappe.top/gtjlyehkxb.html

Py:   copy.deepcopy(obj)
来源：http://hz.chenlongwang.top/gttfqnpbez.html

PHP:  unserialize(serialize($obj));
来源：http://hz.vqdsnc.cn/gtcwagphcz.html

JS:   structuredClone(obj)
来源：http://hz.ehwqpu.com/gtzxiimqrg.html

TS:   structuredClone(obj)
来源：http://hz.xinyue.icu/gtujmqtpvx.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.gotoacloud.top/gtlisldpnq.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.andypj.xyz/gtoharhhcu.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.redwolf501.top/gtllahrrfz.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.yj202588.top/gtaaubumnx.html

[K06] 解析 URL 查询串
来源：http://hz.vqdsnc.cn/gtoaqxwfoo.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.yueranfly.top/gtllocfasb.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.svipenyu.cn/gtfkbqtfog.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.daria6918.cn/gtnuxrebnk.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.hnqzz.top/gtwhbytowk.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.cqqwz.cn/gtwergcgiv.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.chenlongwang.top/gtpvyizbze.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.zhengqikj.top/gtxyirltbs.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.gaohongyu789.top/gtgcqvszcv.html

[K07] 进制转换
来源：http://hz.dashuyun.cn/gtkuysybab.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.daria6918.cn/gtasxammlp.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.wangshuangyany.cn/gtsysjpipv.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.zhijiandao.cn/gtowotkmjq.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.c1oappe.top/gtxtbagvvr.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.andypj.xyz/gtkxvdinoi.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.fzhhl.top/gtkhjlggdf.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.chenjidiqi.icu/gtrfppxhak.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.vqdsnc.cn/gthgwcontb.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.zhijiandao.cn/gtvyszywfs.html

Py:   pickle.dumps(obj)
来源：http://hz.svipenyu.cn/gtstyhvzec.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.cheryme.top/gtnvhzphvl.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.ydzc1.top/gtvemtbegn.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.aibaodan.cn/gtgyiswcxf.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.snrcjt.cn/gtpfooneuu.html

Go:   encoding/gob
来源：http://hz.9152youxi.cn/gtppvztpvb.html

Ruby: Marshal.dump(obj)
来源：http://hz.ehwqpu.com/gtvcxmqcxm.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.zhengqikj.top/gtqkmvcvuk.html

================================================================================
来源：http://hz.aibaodan.cn/gtfcojcjvs.html

L. 网络请求
来源：http://hz.zhongyouzk.top/gtcywdhzaw.html

================================================================================
来源：http://hz.sxryk.cn/gtmyisflze.html

[L01] 发送 GET 请求
来源：http://hz.gotoacloud.top/gtwawjgrdc.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.yvedp.cn/gtuwpufscj.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.gogol.net.cn/gtizqegeel.html

JS:   await fetch(url)
来源：http://hz.shanyushiyangtech.top/gtyveycvsd.html

TS:   await fetch(url)
来源：http://hz.chenjidiqi.icu/gtjnxbeelh.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.c1oappe.top/gteevxnzsm.html

Go:   resp, err := http.Get(url)
来源：http://hz.hnxiangtu.top/gtjotvgszq.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.quarkkingdee.top/gttteyydkm.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.gzhubu.top/gtmnwlfusp.html

[L02] 发送 POST JSON
来源：http://hz.yj20258888.top/gtnxowlmnj.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.chenzaomai.com/gtptumavbe.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.sufxvd.cn/gtxabbkmho.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.pycfn.com/gthzdbnsry.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.xuanzx.com/gtyrdrcass.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.sysykeji.top/gtbfhobvyg.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.dashuyun.cn/gtcpalnjym.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.yj20258.top/gtqotsvwlf.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.xinyue.icu/gtdabdolgl.html

[L03] 设置自定义请求头
来源：http://hz.yangfankeji.com/gtqqpvxaan.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.havefunace.top/gteelsuilb.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.pycfn.com/gtptabqvri.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.bjfxy.top/gtdxtcsnxf.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.0kj1m.cn/gtyoiokhtd.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.hywenlv.cn/gtbzdgkhcq.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.hnqzz.top/gtqlmkgrjc.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.cqqwz.cn/gtaqrwjfvr.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.snrcjt.cn/gtbilppvbm.html

[L04] 设置超时
来源：http://hz.meibo888.top/gtzkeiuwhf.html

Py:   requests.get(url, timeout=5)
来源：http://hz.zycfv.cn/gtizuouchh.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.fengsongda.top/gtjhdygjzb.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.ehwqpu.com/gtwlwcmtna.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.nwbrower.top/gtsungvrpd.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.zhiwuduotai.top/gthpwascee.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.cucudq.cn/gtqclhrsex.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.xinyue.icu/gtkaromppz.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.dashuyun.cn/gthpegugoq.html

[L05] 上传文件（multipart）
来源：http://hz.quarkkingdee.top/gtbzflljbo.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.shanyushiyangkeji.top/gtcqrjtrck.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.pengpengdd.cyou/gtjpfkusxk.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.xuanzx.com/gtnpmrcflt.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.zhiwuduotai.top/gtilxmcdav.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.shanyushiyangtech.top/gtpvdhnwmy.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.hongshengwenyu.top/gtescgcoij.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.jianghu66.top/gtwqwpsjgo.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.zhengqikj.top/gtpwtmiqcg.html

[L06] 解析响应为 JSON
来源：http://hz.shanyushiyangtech.top/gtgfatgvbs.html

Py:   resp.json()
来源：http://hz.sxryk.cn/gtcbidefue.html

PHP:  json_decode($body, true);
来源：http://hz.aizwys.cn/gtnedxeypj.html

JS:   await resp.json()
来源：http://hz.zhongyouzk.top/gtnfdusiep.html

TS:   await resp.json()
来源：http://hz.pengpengdd.cyou/gtgppdmafl.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.yueranfly.top/gtkeqsctvv.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.zdqjudy.top/gtyhkhulpe.html

Ruby: JSON.parse(resp.body)
来源：http://hz.zdqjudy.top/gthlcmhrnc.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.chenjidiqi.icu/gtegpcjcvp.html

[L07] 处理 HTTP 状态码
来源：http://hz.yuanzhike.top/gtyctfttvg.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.snrcjt.cn/gtodphhfrr.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.ywan-chungtsiang.top/gttkoiqsky.html

JS:   resp.ok;  resp.status
来源：http://hz.kuanghao11.cn/gtrumbeghm.html

TS:   resp.ok;  resp.status
来源：http://hz.gotoacloud.top/gtdhujgpdh.html

Java: resp.statusCode()
来源：http://hz.yuxming.cn/gtjozyfflt.html

Go:   resp.StatusCode
来源：http://hz.jiagoushi.top/gtrelxbhoy.html

Ruby: resp.code.to_i
来源：http://hz.sufxvd.cn/gtvffvoyxt.html

C#:   (int)resp.StatusCode
来源：http://hz.aibaodan.cn/gtymgpnriv.html

[L08] 并发请求多个地址
来源：http://hz.shuidangran.top/gtmnfzhsfp.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.gogol.net.cn/gtrhlsycyc.html

PHP:  curl_multi_init() 系列
来源：http://hz.shuidangran.top/gtcatsgior.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhaomingkeji.xyz/gtzflfwzmw.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.ydjk.org.cn/gttasfkftr.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.yuxming.cn/gtflugkvfl.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.xylfe.cn/gtgunggyue.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.pycfn.com/gtahzyhahc.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.jianghu66.top/gtpepavxdp.html

================================================================================
来源：http://hz.smart0.xyz/gtmlvrlkzn.html

M. 命令行 / 进程 / 环境
来源：http://hz.jyoumei.cn/gtqzbwyapg.html

================================================================================
来源：http://hz.nanxuanxn.top/gtxkrqxfvt.html

[M01] 读取命令行参数
来源：http://hz.mhx1999.top/gteiequklf.html

Py:   sys.argv[1:]
来源：http://hz.fengsongda.top/gtwgvwonqj.html

PHP:  $argv;  $argc;
来源：http://hz.feifeiyinyue.top/gtmxmqucxy.html

JS:   process.argv.slice(2)
来源：http://hz.shanyushiyangtech.top/gtdwqwxqte.html

TS:   process.argv.slice(2)
来源：http://hz.cucudq.cn/gtnubidjly.html

Java: args 数组（main 方法参数）
来源：http://hz.9152youxi.cn/gtvugjypln.html

Go:   os.Args[1:]
来源：http://hz.xuanzx.com/gtvaxkyfbk.html

Ruby: ARGV
来源：http://hz.hnxiangtu.top/gtvrmtoytr.html

C#:   args 数组（Main 方法参数）
来源：http://hz.zhiwuduotai.top/gttaqwhxhq.html

[M02] 读取环境变量
来源：http://hz.yangfankeji.com/gtttoibbow.html

Py:   os.environ.get("HOME")
来源：http://hz.gogol.net.cn/gtqjfesmfh.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.ywan-chungtsiang.top/gtwfkrmbeb.html

JS:   process.env.HOME
来源：http://hz.chenlongwang.top/gtnndywfga.html

TS:   process.env.HOME
来源：http://hz.zhaomingkeji.xyz/gtxoifhfri.html

Java: System.getenv("HOME")
来源：http://hz.zhengqikj.top/gtijwaqgnj.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.wangshuangyany.cn/gtbmhlagxn.html

Ruby: ENV["HOME"]
来源：http://hz.xuetiantiany.cn/gtffjfhydc.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.hammf.cn/gtrvpfoafn.html

[M03] 执行外部命令
来源：http://hz.birdmap.top/gtnpqrobvv.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.sysykeji.top/gtvnhclxxw.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.yangfankeji.com/gtamrhdhbp.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.sysykeji.top/gtxqmzevxi.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.dianchejie.cn/gtdbuvfmbb.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.cashguo.top/gtwtwzquex.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.ivvv.top/gtqwebtuoe.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.52xcode.cn/gtutqooymf.html

C#:   Process.Start("ls", "-l");
来源：http://hz.shanyushiyangkeji.top/gtmrusbxdh.html

[M04] 获取当前工作目录
来源：http://hz.daxiang520.top/gtzzevxbav.html

Py:   os.getcwd()
来源：http://hz.jqgufenzy.top/gtcjbyezxk.html

PHP:  getcwd();
来源：http://hz.zhongyouzk.top/gtjjcwegev.html

JS:   process.cwd()
来源：http://hz.redwolf501.top/gtnycbjwyk.html

TS:   process.cwd()
来源：http://hz.hfpthk.cn/gtointhryg.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.zhaomingkeji.xyz/gtihcdjwpc.html

Go:   os.Getwd()
来源：http://hz.havefunace.top/gtzjiyeudc.html

Ruby: Dir.pwd
来源：http://hz.zhijiandao.cn/gtqrdsykvw.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.c1oappe.top/gtbypcfkof.html

[M05] 设置退出码
来源：http://hz.havefunace.top/gtngcdhmtd.html

Py:   sys.exit(1)
来源：http://hz.shanyushiyangtech.top/gtspyxhooi.html

PHP:  exit(1);
来源：http://hz.gaohongyu789.top/gtxfqaowxr.html

JS:   process.exit(1)
来源：http://hz.ehwqpu.com/gtosqsgmzk.html

TS:   process.exit(1)
来源：http://hz.c1oappe.top/gtvzqimawv.html

Java: System.exit(1)
来源：http://hz.nanxuanxn.top/gtgguzyesr.html

Go:   os.Exit(1)
来源：http://hz.jianghu66.top/gtrodkbuod.html

Ruby: exit 1
来源：http://hz.tian-w.cn/gtjjukdllh.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.jinqigufen.top/gtbbnmsrji.html

[M06] 向标准错误输出
来源：http://hz.birdmap.top/gtzhoqydtu.html

Py:   print("err", file=sys.stderr)
来源：http://hz.smart0.xyz/gtavkogdrq.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.kuanghao11.cn/gtcqfmjyls.html

JS:   console.error("err")
来源：http://hz.cashguo.top/gtwvtwwsnm.html

TS:   console.error("err")
来源：http://hz.dianchejie.cn/gtelfmtwbc.html

Java: System.err.println("err")
来源：http://hz.xuanzx.com/gtymcrpgbq.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.xziqi.cn/gtpfyndgwd.html

Ruby: warn "err"
来源：http://hz.guannengcc.top/gtrjoojduq.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.hfpthk.cn/gtgsdecflw.html

[M07] 判断是否为主入口
来源：http://hz.zdqjudy.top/gttgvktgbd.html

Py:   if __name__ == "__main__":
来源：http://hz.vqdsnc.cn/gtcprlzmcf.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.shangyingyoupin.top/gtokooxqia.html

JS:   require.main === module
来源：http://hz.zhongyouzk.top/gtvcprgjot.html

TS:   require.main === module
来源：http://hz.smart0.xyz/gteyxwlwve.html

Java: public static void main(String[] args)
来源：http://hz.aibaodan.cn/gtathmzuqu.html

Go:   func main()
来源：http://hz.cashguo.top/gtmnvidlmj.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.quarkkingdee.top/gtandpvhvb.html

C#:   static void Main(string[] args)
来源：http://hz.zdqjudy.top/gtllkzgszv.html

[M08] 获取系统与运行时信息
来源：http://hz.zhixingplan.top/gtznbzjucq.html

Py:   platform.system();  platform.python_version()
来源：http://hz.zhoulong.xyz/gtpxtefzem.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.yanxiufei.cn/gtsxjyhmoq.html

JS:   process.platform;  process.version
来源：http://hz.xziqi.cn/gtjsoognzz.html

TS:   process.platform;  process.version
来源：http://hz.meibo888.top/gtqfvvunof.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.tian-w.cn/gtpnhmpnxp.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.jyoumei.cn/gticstgooa.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.c1oappe.top/gthziysfhp.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.zycfv.cn/gtrezpwikx.html

================================================================================
来源：http://hz.fengsongda.top/gtopcjuped.html

N. 数据结构与算法
来源：http://hz.havefunace.top/gtysnunxge.html

================================================================================
来源：http://hz.ivvv.top/gtrxblxdgb.html

[N01] 二分查找（有序数组）
来源：http://hz.zycfv.cn/gtkegrqxhz.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.cdnleiting.top/gtixkiylvk.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.cdnleiting.top/gtawgaluqk.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.tianlin.xyz/gtuopbhxxt.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.vqdsnc.cn/gtsxryhulq.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.quarkkingdee.top/gtwutohgvz.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.meibo888.top/gtwmsnhusa.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.guannengcc.top/gtmavdoggd.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.hfpthk.cn/gtialpgtnw.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.jiagoushi.top/gtqetlmgnw.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.fzhhl.top/gtjavjfhij.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.cashguo.top/gtwxqfmtlu.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.guowangkeji.top/gthfvezycw.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.guowangkeji.top/gtqnjrormu.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.havefunace.top/gtwxrdrcoz.html

Go:   slices.Sort(arr)
来源：http://hz.pengpengdd.cyou/gtubqlhlek.html

Ruby: arr.sort
来源：http://hz.ivvv.top/gtvsxvckjm.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.c1oappe.top/gtsspiwmzf.html

[N03] 快速排序（分治示例）
来源：http://hz.cashguo.top/gtjomexoda.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.jinghuilouyu.cn/gtaijyqsod.html

PHP:  // 递归实现，或用 usort
来源：http://hz.hysaishi.cn/gtsdukgdez.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jinghuilouyu.cn/gtetjyqqwj.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.nanxinkj.top/gtcooluifq.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.chenzaomai.com/gtzbfhiqvl.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.xziqi.cn/gtkpfuijzd.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.xuanzx.com/gtxvnoktcf.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.fzhhl.top/gtgmpnnnwr.html

[N04] 斐波那契数列
来源：http://hz.yuanzhike.top/gtmlrtbcma.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.fengsongda.top/gtpcpvkvcm.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.shanyushiyangkeji.top/gtqxigqqfq.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.chenlongwang.top/gtojswnxtz.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.cqqwz.cn/gtevwjyqxf.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.hnxiangtu.top/gtknmmyioj.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.yj202588.top/gtokxchtne.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.zhiwuduotai.top/gtgzchiawz.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.hnqzz.top/gtphmniuaf.html

[N05] 最大公约数
来源：http://hz.tanke756.top/gtlojzybkt.html

Py:   math.gcd(a, b)
来源：http://hz.chenzaomai.com/gtlymbkttt.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.jianghu66.top/gtpeswiaxv.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jinqigfzy.top/gtrvohdrfs.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yongpay.top/gtjjbafitw.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.cqqwz.cn/gtfjkhzvho.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.kuanghao11.cn/gtcockjsed.html

Ruby: a.gcd(b)
来源：http://hz.gzhubu.top/gtruaxibfw.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.kuanghao11.cn/gtpesytrxe.html

[N06] 判断回文字符串
来源：http://hz.cheryme.top/gtzzkhyokj.html

Py:   s == s[::-1]
来源：http://hz.sxryk.cn/gtyxqbtpwu.html

PHP:  $s === strrev($s);
来源：http://hz.dianchejie.cn/gtemqdowvo.html

JS:   s === [...s].reverse().join("")
来源：http://hz.chenlongwang.top/gtsehugfip.html

TS:   s === [...s].reverse().join("")
来源：http://hz.nanxuanxn.top/gtqgvconiq.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.smart0.xyz/gtecrddfij.html

Go:   // 双指针从两端比较
来源：http://hz.kuanghao11.cn/gtjlgixeay.html

Ruby: s == s.reverse
来源：http://hz.gogol.net.cn/gtmlddatod.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.sysykeji.top/gtuepyasxe.html

[N07] 两数之和（返回下标）
来源：http://hz.bjfxy.top/gtluqxukvh.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.iojbl.cn/gtgzcembvt.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.ydzc1.top/gtulovfkck.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.xingfuxueyuan.xyz/gtynflhben.html

TS:   // 手写 Map<string, number>
来源：http://hz.quarkkingdee.top/gtassezqpa.html

Java: // 手写 HashMap
来源：http://hz.hywenlv.cn/gtapckilyj.html

Go:   // 手写 map[int]int
来源：http://hz.mhx1999.top/gtwhgwcoeu.html

Ruby: // 手写 Hash
来源：http://hz.yonumen.top/gtfsarectr.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.pengpengdd.cyou/gttmjilymu.html

[N08] 生成全排列
来源：http://hz.shanyushiyangtech.top/gtqjquyjgf.html

Py:   itertools.permutations(arr)
来源：http://hz.9152youxi.cn/gtxqfgejpf.html

PHP:  // 手写递归交换
来源：http://hz.sufxvd.cn/gtnygonmbr.html

JS:   // 手写回溯递归
来源：http://hz.svipenyu.cn/gtfayonmmy.html

TS:   // 手写回溯递归
来源：http://hz.hywenlv.cn/gtswhwpovq.html

Java: // 手写回溯递归
来源：http://hz.yueranfly.top/gtlqdwhezu.html

Go:   // 手写回溯递归
来源：http://hz.hfpthk.cn/gtutiordos.html

Ruby: arr.permutation.to_a
来源：http://hz.tianlin.xyz/gtlrklobpw.html

C#:   // 手写回溯递归
来源：http://hz.zhixingplan.top/gtkypdxoin.html

[N09] 栈与队列
来源：http://hz.ydzc1.top/gtmhnztraa.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.jinqigufen.top/gtyvctvutt.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.jinghuilouyu.cn/gtlkfwmjim.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.sysykeji.top/gtcpkxytzd.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.shuidangran.top/gtijehyjlr.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.chenzaomai.com/gtqfoptcal.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.jinqigfzy.top/gtynolprgb.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.jianghu66.top/gtsmeolhfu.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.jlsjyb.cn/gtmlpfrxbs.html

[N10] 链表节点定义
来源：http://hz.yongpay.top/gtspxgwucj.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.ydjk.org.cn/gtcsgyfzea.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.jyoumei.cn/gtcpimcggl.html


<!-- 参考信息 -->