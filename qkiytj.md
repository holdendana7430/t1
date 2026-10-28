代发 wailian999

================================================================================
来源：http://hz.yanxiufei.cn/gttbzskhjg.html

K. JSON 与序列化
来源：http://hz.zdqjudy.top/gtxmscqrdm.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtkrtzjagn.html

[K01] 对象转 JSON 字符串
来源：http://hz.chenjidiqi.icu/gtejkbnoxr.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.jianghu66.top/gtfurhrudr.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.chenlongwang.top/gtdtricsyk.html

JS:   JSON.stringify(obj)
来源：http://hz.gogol.net.cn/gtxwxzygmo.html

TS:   JSON.stringify(obj)
来源：http://hz.gotoacloud.top/gtukgqkvno.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.wangshuangyany.cn/gtfpmejhqp.html

Go:   json.Marshal(obj)
来源：http://hz.zhengqikj.top/gtrieyixuk.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.ehwqpu.com/gtyudcarwt.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.yj20258888.top/gthyiqyxdl.html

[K02] JSON 字符串转对象
来源：http://hz.ivvv.top/gtrueugwtu.html

Py:   json.loads(s)
来源：http://hz.mhx1999.top/gtzmhulyku.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.cheryme.top/gtitqyjcea.html

JS:   JSON.parse(s)
来源：http://hz.guowangkeji.top/gtxuwptxai.html

TS:   JSON.parse(s)
来源：http://hz.zhongyouzk.top/gtpolgwmhk.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.zhaomingkeji.xyz/gtjgvwmbmx.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.yangfankeji.com/gtqjxhfxfg.html

Ruby: JSON.parse(s)
来源：http://hz.xziqi.cn/gtfvvzfcvk.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.jianghu66.top/gtoxbuoqnh.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.yj20258.top/gtmbdkfpvm.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.chenlongwang.top/gtddmgunll.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.ivvv.top/gtpqzgnjmq.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.jianghu66.top/gtnuxogtgm.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.zycfv.cn/gtsxnnofqu.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.vqdsnc.cn/gtigrpajab.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.chenlongwang.top/gtlgakdmcs.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.ydjk.org.cn/gttqqddtrc.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.shangyingyoupin.top/gtnprojbcn.html

[K04] 读取 JSON 文件
来源：http://hz.chenjidiqi.icu/gtadwpnvpn.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.jqgfzy.top/gtkainfaqs.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.daria6918.cn/gtbcqsmsyl.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.aizwys.cn/gtjqyicrxe.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.ehwqpu.com/gtbdpysuzh.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.svipenyu.cn/gtkokdwrjg.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.yangfankeji.com/gtwtsmdlwk.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.yongpay.top/gtskfwxmlu.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.hywenlv.cn/gtwzgvirft.html

[K05] 深拷贝对象
来源：http://hz.ehwqpu.com/gtnhiiqaiv.html

Py:   copy.deepcopy(obj)
来源：http://hz.hnxiangtu.top/gtxrhnhrmk.html

PHP:  unserialize(serialize($obj));
来源：http://hz.yvedp.cn/gtvahwrslq.html

JS:   structuredClone(obj)
来源：http://hz.ppjwa.cn/gtjlommhza.html

TS:   structuredClone(obj)
来源：http://hz.gogol.net.cn/gtyredjyso.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.zhaomingkeji.xyz/gtttptnuuj.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.jiagoushi.top/gtlcedjvnq.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.yj20258888.top/gtyfniyiye.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.sysykeji.top/gtupvxqqxm.html

[K06] 解析 URL 查询串
来源：http://hz.cdnleiting.top/gtoiqozrnx.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.316326.xyz/gtkhgrtcce.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.52xcode.cn/gtmbkhlpyx.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.guannengcc.top/gtbvlqlncf.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jyoumei.cn/gtlyjhgnzz.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.redwolf501.top/gtcxfmpddn.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.nwbrower.top/gtjgzufhhi.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.snrcjt.cn/gtdtsyzcri.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.zhoulong.xyz/gtyudrbksh.html

[K07] 进制转换
来源：http://hz.zhongyouzk.top/gtbviaqlsk.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.hammf.cn/gtuhtodzpj.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.xingfuxueyuan.xyz/gttfnttokp.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.c1oappe.top/gtzhgpofpb.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.tanke756.top/gtxvjjzkqc.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.sufxvd.cn/gtulnoyqht.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.hysaishi.cn/gttasdcdpz.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.meibo888.top/gtlsskrslj.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.zhixingplan.top/gtwkxfnaob.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.hongshengwenyu.top/gtjxkbtqyz.html

Py:   pickle.dumps(obj)
来源：http://hz.sysykeji.top/gtesouybon.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.hammf.cn/gtslrqysdi.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.iojbl.cn/gthadfhsng.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.yanxiufei.cn/gtdtxtvsot.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.ydzc1.top/gtttjtvmjp.html

Go:   encoding/gob
来源：http://hz.jinghuilouyu.cn/gtrhskfyrk.html

Ruby: Marshal.dump(obj)
来源：http://hz.smart0.xyz/gtzodjqjra.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.iojbl.cn/gtufikkalz.html

================================================================================
来源：http://hz.tanke756.top/gtcazhzjlz.html

L. 网络请求
来源：http://hz.bjfxy.top/gtoxcmvxjk.html

================================================================================
来源：http://hz.zhijiandao.cn/gtympyicmd.html

[L01] 发送 GET 请求
来源：http://hz.yongpay.top/gthfaxqang.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.pengpengdd.cyou/gtjhaejkgm.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.c1oappe.top/gtudorvcbz.html

JS:   await fetch(url)
来源：http://hz.sysykeji.top/gtvtxddgic.html

TS:   await fetch(url)
来源：http://hz.haohaochexian.top/gtzyywpwzg.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.zhongyouzk.top/gtafklylwp.html

Go:   resp, err := http.Get(url)
来源：http://hz.cqqwz.cn/gtdjrvaiuu.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.gogol.net.cn/gtxrxvlsqp.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.jyoumei.cn/gttebhyabj.html

[L02] 发送 POST JSON
来源：http://hz.9152youxi.cn/gtjfeufccm.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.hfpthk.cn/gtjjizkwpa.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.chenzaomai.com/gtfdzdmwrm.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.shanyushiyangkeji.top/gtlhosspjs.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.birdmap.top/gtdpkypcqz.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.xingfuxueyuan.xyz/gtxqwmubik.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.chenzaomai.com/gthqybdrpw.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.chenlongwang.top/gthxlelquz.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.yanxiufei.cn/gtbsyqwbah.html

[L03] 设置自定义请求头
来源：http://hz.aibaodan.cn/gtrlvtvllx.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.fzhhl.top/gtvhomfeea.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.jlsjyb.cn/gtwadlbawg.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.xuetiantiany.cn/gtdfxqxwcn.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yangfankeji.com/gtnjfikmpt.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.9152youxi.cn/gtgeoeakmf.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.shzxlz.cn/gtltvofrmt.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.nanxinkj.top/gtmljgcrgo.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.cqqwz.cn/gtcnzuwjms.html

[L04] 设置超时
来源：http://hz.hywenlv.cn/gtrpxpiibm.html

Py:   requests.get(url, timeout=5)
来源：http://hz.nwbrower.top/gtravbzpeo.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.ywan-chungtsiang.top/gtnxuawhpf.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jyoumei.cn/gtrjutqbcb.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.gotoacloud.top/gtouftumtx.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.meibo888.top/gtjzzomokj.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.gzhubu.top/gttqjztncd.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.jlsjyb.cn/gtcmvngpju.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.snrcjt.cn/gtquiehqfu.html

[L05] 上传文件（multipart）
来源：http://hz.xinyue.icu/gtzmcquffs.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.zhiwuduotai.top/gtvuavsztx.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.tanke756.top/gtibfspoqa.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.hfpthk.cn/gtfuwopkdn.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.zhoulong.xyz/gtvftcnamg.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.ydzc1.top/gteuhwzzsy.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.yangfankeji.com/gthlsblmje.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.daria6918.cn/gtqmehstra.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.hfpthk.cn/gtnvohmazz.html

[L06] 解析响应为 JSON
来源：http://hz.kuanghao11.cn/gtwrpcpgov.html

Py:   resp.json()
来源：http://hz.birdmap.top/gtvmkjtyxa.html

PHP:  json_decode($body, true);
来源：http://hz.wangshuangyany.cn/gtwkrkemvd.html

JS:   await resp.json()
来源：http://hz.hongshengwenyu.top/gtoutobdwt.html

TS:   await resp.json()
来源：http://hz.shangyingyoupin.top/gtidtnxudx.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.shanyushiyangtech.top/gthxvryngu.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.jqgfzy.top/gtnljugtbo.html

Ruby: JSON.parse(resp.body)
来源：http://hz.ehwqpu.com/gtwhbakkre.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.zhongyouzk.top/gtbbcorctp.html

[L07] 处理 HTTP 状态码
来源：http://hz.nwbrower.top/gtcldbidbe.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.yuanzhike.top/gtymouuymw.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.sxryk.cn/gtnelprxnd.html

JS:   resp.ok;  resp.status
来源：http://hz.tian-w.cn/gtdvjbkppj.html

TS:   resp.ok;  resp.status
来源：http://hz.havefunace.top/gtnzubobbx.html

Java: resp.statusCode()
来源：http://hz.xziqi.cn/gtubairsqq.html

Go:   resp.StatusCode
来源：http://hz.snrcjt.cn/gtvzfdrziv.html

Ruby: resp.code.to_i
来源：http://hz.birdmap.top/gtqvmdkvji.html

C#:   (int)resp.StatusCode
来源：http://hz.daxiang520.top/gtqpoxeold.html

[L08] 并发请求多个地址
来源：http://hz.zdqjudy.top/gtjrtunxvc.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.jinqigfzy.top/gthhrhqfym.html

PHP:  curl_multi_init() 系列
来源：http://hz.kuanghao11.cn/gtnunibbax.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.hnqzz.top/gtskqnhdau.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yj20258888.top/gtbzlagyjw.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.shuidangran.top/gtdordqknn.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.52xcode.cn/gtkpyaexwl.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.shanyushiyangkeji.top/gtiwmiqxml.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.fzhhl.top/gtjfsyckde.html

================================================================================
来源：http://hz.zdqjudy.top/gtphrerffp.html

M. 命令行 / 进程 / 环境
来源：http://hz.dashuyun.cn/gtcnulijjb.html

================================================================================
来源：http://hz.gzhubu.top/gtlykmvctm.html

[M01] 读取命令行参数
来源：http://hz.yj202588.top/gtcmokbhxh.html

Py:   sys.argv[1:]
来源：http://hz.jlsjyb.cn/gtquyypgxd.html

PHP:  $argv;  $argc;
来源：http://hz.jinqigufen.top/gtyesngwbf.html

JS:   process.argv.slice(2)
来源：http://hz.yangfankeji.com/gtlppqoxtd.html

TS:   process.argv.slice(2)
来源：http://hz.zycfv.cn/gtvksbngix.html

Java: args 数组（main 方法参数）
来源：http://hz.cdnleiting.top/gtthqxrgmj.html

Go:   os.Args[1:]
来源：http://hz.yonumen.top/gtwivpwoof.html

Ruby: ARGV
来源：http://hz.shuidangran.top/gtkaxafhow.html

C#:   args 数组（Main 方法参数）
来源：http://hz.zhongyouzk.top/gtowuppgjt.html

[M02] 读取环境变量
来源：http://hz.yueranfly.top/gtpyipusam.html

Py:   os.environ.get("HOME")
来源：http://hz.cheryme.top/gtenpxepin.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.yongpay.top/gthsiaybnp.html

JS:   process.env.HOME
来源：http://hz.yvedp.cn/gtmctauwnp.html

TS:   process.env.HOME
来源：http://hz.zhixingplan.top/gterwdgimf.html

Java: System.getenv("HOME")
来源：http://hz.ydjk.org.cn/gtqrxfqiyx.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.xinyue.icu/gtkowppnsw.html

Ruby: ENV["HOME"]
来源：http://hz.zhiwuduotai.top/gtodniovyp.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.dianchejie.cn/gtltluqasc.html

[M03] 执行外部命令
来源：http://hz.ppjwa.cn/gthtycuift.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.fzhhl.top/gtfeihhvpd.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.zhixingplan.top/gtiyvfhwof.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.xingfuxueyuan.xyz/gtwkptwftc.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.tanke756.top/gtkxakxhmy.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.c1oappe.top/gtbqaijqrc.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.shangyingyoupin.top/gtyzhxdode.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.jinyuanbaomall.cn/gtpwbpmint.html

C#:   Process.Start("ls", "-l");
来源：http://hz.dianchejie.cn/gtkudhyqtj.html

[M04] 获取当前工作目录
来源：http://hz.redwolf501.top/gtkbxnnksn.html

Py:   os.getcwd()
来源：http://hz.xinyue.icu/gtnjfzjjyq.html

PHP:  getcwd();
来源：http://hz.hywenlv.cn/gtndyhkphz.html

JS:   process.cwd()
来源：http://hz.yuxming.cn/gtyeecrxuy.html

TS:   process.cwd()
来源：http://hz.cucudq.cn/gtvnssexvg.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.yangfankeji.com/gtgvfrholf.html

Go:   os.Getwd()
来源：http://hz.hnxiangtu.top/gtumjstwdz.html

Ruby: Dir.pwd
来源：http://hz.316326.xyz/gtvgcjjpxa.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.chenlongwang.top/gtwvkhrgda.html

[M05] 设置退出码
来源：http://hz.gzhubu.top/gtugjeatmc.html

Py:   sys.exit(1)
来源：http://hz.birdmap.top/gtulnafvzx.html

PHP:  exit(1);
来源：http://hz.ywan-chungtsiang.top/gtadudynoz.html

JS:   process.exit(1)
来源：http://hz.smart0.xyz/gtldwxdftt.html

TS:   process.exit(1)
来源：http://hz.yvedp.cn/gttrpyskzl.html

Java: System.exit(1)
来源：http://hz.ydzc1.top/gtecpaxwqb.html

Go:   os.Exit(1)
来源：http://hz.vqdsnc.cn/gtifniuazm.html

Ruby: exit 1
来源：http://hz.shuidangran.top/gtlsjnmttx.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.jiagoushi.top/gtytnsqvba.html

[M06] 向标准错误输出
来源：http://hz.quarkkingdee.top/gtlbeygani.html

Py:   print("err", file=sys.stderr)
来源：http://hz.zdqjudy.top/gtrnoxhfzc.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.feifeiyinyue.top/gthotndcdb.html

JS:   console.error("err")
来源：http://hz.jinghuilouyu.cn/gtwxhzaven.html

TS:   console.error("err")
来源：http://hz.xuetiantiany.cn/gtfuqzuoow.html

Java: System.err.println("err")
来源：http://hz.sysykeji.top/gtgjpluiol.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.gzhubu.top/gtxfwqeuss.html

Ruby: warn "err"
来源：http://hz.sufxvd.cn/gtwcyxfnpa.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.shzxlz.cn/gtwzlqseru.html

[M07] 判断是否为主入口
来源：http://hz.smart0.xyz/gtjsqxvotf.html

Py:   if __name__ == "__main__":
来源：http://hz.vqdsnc.cn/gtnrhbqlrp.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.fengsongda.top/gtxzdqvgze.html

JS:   require.main === module
来源：http://hz.0kj1m.cn/gtndiwzmfw.html

TS:   require.main === module
来源：http://hz.daxiang520.top/gtxknarocv.html

Java: public static void main(String[] args)
来源：http://hz.xziqi.cn/gtxrshykbv.html

Go:   func main()
来源：http://hz.gaohongyu789.top/gtmgnitrxi.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.zhaomingkeji.xyz/gtsnzbpnso.html

C#:   static void Main(string[] args)
来源：http://hz.jyoumei.cn/gtjpykndbq.html

[M08] 获取系统与运行时信息
来源：http://hz.jinqigfzy.top/gtytedqlkk.html

Py:   platform.system();  platform.python_version()
来源：http://hz.shanyushiyangkeji.top/gtkugizfvw.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.aibaodan.cn/gtqwjncovv.html

JS:   process.platform;  process.version
来源：http://hz.xuetiantiany.cn/gtnqiiukdv.html

TS:   process.platform;  process.version
来源：http://hz.cucudq.cn/gtcwxfsdzd.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.jiagoushi.top/gtfyssdwwo.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.hysaishi.cn/gttsbuogjz.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.zhixingplan.top/gtpoyxxssv.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.cashguo.top/gthqdnqnsr.html

================================================================================
来源：http://hz.hfpthk.cn/gtzieaspte.html

N. 数据结构与算法
来源：http://hz.tanke756.top/gtzjxfdvhm.html

================================================================================
来源：http://hz.52xcode.cn/gtjkwczobw.html

[N01] 二分查找（有序数组）
来源：http://hz.316326.xyz/gtvmzsyiiu.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.yongpay.top/gtczpfxhqv.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.bjfxy.top/gttjummrci.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.pycfn.com/gtgtifvjew.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.smart0.xyz/gttlwyyrow.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.hongshengwenyu.top/gtijnifmiw.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.jianghu66.top/gtssenfkii.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.xylfe.cn/gtjifmfoks.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.zhoulong.xyz/gtdgvxwjkf.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.tianlin.xyz/gtrkdydxjk.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jqgufenzy.top/gtturybagv.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.svipenyu.cn/gtnjdayvyz.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.wangshuangyany.cn/gtcifswafs.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.chenzaomai.com/gthxflntyl.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.jinqigufen.top/gtfvjuccvh.html

Go:   slices.Sort(arr)
来源：http://hz.jinqigufen.top/gtrjpuyjjw.html

Ruby: arr.sort
来源：http://hz.kuanghao11.cn/gtsiarsetq.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.tianlin.xyz/gtnwdrmqpo.html

[N03] 快速排序（分治示例）
来源：http://hz.fzhhl.top/gtoewtxqax.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.chenjidiqi.icu/gtvkmezbni.html

PHP:  // 递归实现，或用 usort
来源：http://hz.gotoacloud.top/gtjmbydovn.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zhixingplan.top/gtrcvyrkwv.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.316326.xyz/gtdbszbois.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.yueranfly.top/gtggjdhfsl.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.hongshengwenyu.top/gtougyfklo.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.gzhubu.top/gtcjcviisz.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.xziqi.cn/gtznwzicgd.html

[N04] 斐波那契数列
来源：http://hz.dianchejie.cn/gtbesgmflg.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.havefunace.top/gtabxzemix.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.ydjk.org.cn/gteaxjrdav.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.guannengcc.top/gtbbszmiwg.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yanxiufei.cn/gtlmswaqoi.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.yuanzhike.top/gtedwzkamk.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.xingfuxueyuan.xyz/gtqawepwit.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.hfpthk.cn/gtdtzypcxc.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.chenzaomai.com/gthcszkwkb.html

[N05] 最大公约数
来源：http://hz.jqgufenzy.top/gtzaubsghj.html

Py:   math.gcd(a, b)
来源：http://hz.cashguo.top/gtxljbqemi.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.snrcjt.cn/gtrkohhsxu.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.hfpthk.cn/gtzzejwuau.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.sweek.top/gtyzyieplt.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.ybcxt.top/gtdlsvkpyb.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.havefunace.top/gtgdfjgmqf.html

Ruby: a.gcd(b)
来源：http://hz.dashuyun.cn/gtthrudigz.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.yanxiufei.cn/gthmplfthk.html

[N06] 判断回文字符串
来源：http://hz.zhaomingkeji.xyz/gtehhwgaav.html

Py:   s == s[::-1]
来源：http://hz.chenlongwang.top/gtrqdsfzfa.html

PHP:  $s === strrev($s);
来源：http://hz.xziqi.cn/gthmsjrsrs.html

JS:   s === [...s].reverse().join("")
来源：http://hz.shanyushiyangkeji.top/gtnxkmbjqi.html

TS:   s === [...s].reverse().join("")
来源：http://hz.yuanzhike.top/gtzqmhahax.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.yj20258.top/gtgojukcrb.html

Go:   // 双指针从两端比较
来源：http://hz.yj20258888.top/gtupwpxywo.html

Ruby: s == s.reverse
来源：http://hz.cashguo.top/gtamihnqgy.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.tanke756.top/gtbambiouj.html

[N07] 两数之和（返回下标）
来源：http://hz.gaohongyu789.top/gtrhppfltr.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.yongpay.top/gtzigowppo.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.jinyuanbaomall.cn/gtahnovlde.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.hywenlv.cn/gtzybrypxv.html

TS:   // 手写 Map<string, number>
来源：http://hz.yangfankeji.com/gtpjjgazzj.html

Java: // 手写 HashMap
来源：http://hz.iojbl.cn/gtexybkhhu.html

Go:   // 手写 map[int]int
来源：http://hz.xinyue.icu/gtidfgsmyc.html

Ruby: // 手写 Hash
来源：http://hz.yangfankeji.com/gtqrgibdzo.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.ydzc1.top/gtnothpqnn.html

[N08] 生成全排列
来源：http://hz.nanxuanxn.top/gtqycekkgc.html

Py:   itertools.permutations(arr)
来源：http://hz.zhiwuduotai.top/gtbyqqprfg.html

PHP:  // 手写递归交换
来源：http://hz.zhaomingkeji.xyz/gtmdyexynk.html

JS:   // 手写回溯递归
来源：http://hz.ydjk.org.cn/gtawikvdsf.html

TS:   // 手写回溯递归
来源：http://hz.ivvv.top/gtneiedkpu.html

Java: // 手写回溯递归
来源：http://hz.yonumen.top/gtttwithdn.html

Go:   // 手写回溯递归
来源：http://hz.feifeiyinyue.top/gtcixvqxfa.html

Ruby: arr.permutation.to_a
来源：http://hz.gogol.net.cn/gtygfleuha.html

C#:   // 手写回溯递归
来源：http://hz.vqdsnc.cn/gtttnwvdiz.html


<!-- 参考信息 -->