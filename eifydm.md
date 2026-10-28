代发 wailian999

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.xingfuxueyuan.xyz/gtzcemldbc.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.hnqzz.top/gtdcrttfpw.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.fengsongda.top/gttrbkpfal.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.pycfn.com/gtktkrvzhs.html

================================================================================
来源：http://hz.sxryk.cn/gttvftsetz.html

K. JSON 与序列化
来源：http://hz.yonumen.top/gtqucndusl.html

================================================================================
来源：http://hz.nwbrower.top/gtvixpiyue.html

[K01] 对象转 JSON 字符串
来源：http://hz.birdmap.top/gtxxybwjwn.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.guowangkeji.top/gtlufzdtve.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.daxiang520.top/gtwajjmpaq.html

JS:   JSON.stringify(obj)
来源：http://hz.guowangkeji.top/gtaxroqxuy.html

TS:   JSON.stringify(obj)
来源：http://hz.ydjk.org.cn/gtuvhatprd.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.hysaishi.cn/gtnwraskiz.html

Go:   json.Marshal(obj)
来源：http://hz.ybcxt.top/gtlbxwunti.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.meibo888.top/gtyefwvrkf.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.iojbl.cn/gtexugtpuq.html

[K02] JSON 字符串转对象
来源：http://hz.hywenlv.cn/gtuxtuukvq.html

Py:   json.loads(s)
来源：http://hz.vqdsnc.cn/gtnrmfqazk.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.meibo888.top/gtjtnvhccd.html

JS:   JSON.parse(s)
来源：http://hz.cdnleiting.top/gtozgoudqz.html

TS:   JSON.parse(s)
来源：http://hz.mhx1999.top/gtddqcmmjy.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.tanke756.top/gtsakyluya.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.316326.xyz/gtzhplhkcb.html

Ruby: JSON.parse(s)
来源：http://hz.hnqzz.top/gtgcitzpqe.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.sufxvd.cn/gteiphfgzu.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.jlsjyb.cn/gtkshxdwfi.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.cucudq.cn/gtqswapsqp.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.gzhubu.top/gtbxyiublv.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.chenjidiqi.icu/gtnplomxho.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.iojbl.cn/gtzjposzix.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.zdqjudy.top/gtjywmbwcu.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.gotoacloud.top/gtenjrbyen.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.pycfn.com/gtfeviyfdk.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.hammf.cn/gtdgxpxwax.html

[K04] 读取 JSON 文件
来源：http://hz.zhijiandao.cn/gtfxowdusn.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.yuanzhike.top/gtsixphqpg.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.ydzc1.top/gtgelehggq.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.tianlin.xyz/gtwwnhayfo.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.smart0.xyz/gtzqtevejv.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.pengpengdd.cyou/gtzjtoxhno.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.sufxvd.cn/gtcebcwswl.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.zycfv.cn/gtudbvnbbj.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.hammf.cn/gtiaxlwbzw.html

[K05] 深拷贝对象
来源：http://hz.daxiang520.top/gtgvhqbidc.html

Py:   copy.deepcopy(obj)
来源：http://hz.meibo888.top/gtezmxvvzq.html

PHP:  unserialize(serialize($obj));
来源：http://hz.yuxming.cn/gtfhyglofj.html

JS:   structuredClone(obj)
来源：http://hz.jinyuanbaomall.cn/gthgjvzgaw.html

TS:   structuredClone(obj)
来源：http://hz.jianghu66.top/gtkzaieafy.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.zhongyouzk.top/gtmqefpggs.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.9152youxi.cn/gtrqapxhbh.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.wangshuangyany.cn/gtezmlksej.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.9152youxi.cn/gtusmumhib.html

[K06] 解析 URL 查询串
来源：http://hz.sufxvd.cn/gtnhqywttx.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.shanyushiyangtech.top/gtfxzqalrf.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.zhijiandao.cn/gtrcgbmszt.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.shuidangran.top/gtyyqxggwq.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.gotoacloud.top/gtyupliqfd.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.smart0.xyz/gtmsgdjxrq.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.hammf.cn/gtbnyfialx.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.jyoumei.cn/gtgqdkbnwz.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.daxiang520.top/gtwjgitxyc.html

[K07] 进制转换
来源：http://hz.ywan-chungtsiang.top/gtdckytufq.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.sxryk.cn/gtsxuiibqo.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.zhijiandao.cn/gtnbnviifh.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.jlsjyb.cn/gtkihnohwc.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.hnxiangtu.top/gtqrqftrcs.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.cdnleiting.top/gtnempagph.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.jqgufenzy.top/gtnbdpjbrs.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.cucudq.cn/gtiuzqrioj.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.yonumen.top/gtkvvoikfc.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.gogol.net.cn/gtlwtwxovg.html

Py:   pickle.dumps(obj)
来源：http://hz.aizwys.cn/gtgyalcgxo.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.cheryme.top/gtdwarsqlc.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.cashguo.top/gtbcfsxgbu.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.shangyingyoupin.top/gtvqqrvrff.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.sufxvd.cn/gtkbfntfzw.html

Go:   encoding/gob
来源：http://hz.ivvv.top/gtrxdpmmwj.html

Ruby: Marshal.dump(obj)
来源：http://hz.andypj.xyz/gtofrybstd.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.9152youxi.cn/gtzhgsmywv.html

================================================================================
来源：http://hz.quarkkingdee.top/gthdgczvvx.html

L. 网络请求
来源：http://hz.snrcjt.cn/gtwcsmxsab.html

================================================================================
来源：http://hz.ydzc1.top/gtekdssuur.html

[L01] 发送 GET 请求
来源：http://hz.cqqwz.cn/gtbmhkacxo.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.xuetiantiany.cn/gtfjhpjsav.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.hammf.cn/gtzpbempbv.html

JS:   await fetch(url)
来源：http://hz.cheryme.top/gtdchvtplb.html

TS:   await fetch(url)
来源：http://hz.hnxiangtu.top/gtwwpsubzb.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.hfpthk.cn/gtlkfriwrh.html

Go:   resp, err := http.Get(url)
来源：http://hz.jlsjyb.cn/gtdcuhvryg.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.zhongyouzk.top/gtkyzsgkls.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.yuxming.cn/gtcrbxhueb.html

[L02] 发送 POST JSON
来源：http://hz.aibaodan.cn/gtxxdzpjsu.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.jqgfzy.top/gtzgatqdom.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.aibaodan.cn/gtndrtnpbz.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.hysaishi.cn/gtylwbtkwk.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.gogol.net.cn/gtakdyrgvr.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.nanxinkj.top/gttvrzxkra.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.chenjidiqi.icu/gtypmkvqca.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.nanxinkj.top/gtokvjkjjf.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.9152youxi.cn/gtnfddpgdi.html

[L03] 设置自定义请求头
来源：http://hz.9152youxi.cn/gtgfmtztud.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.daria6918.cn/gtiyxxmpmv.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.sxryk.cn/gtdihkjqkd.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.birdmap.top/gtdgxvjeju.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zhengqikj.top/gtyidgaqfo.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.zhijiandao.cn/gtqqawmpgd.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.sxryk.cn/gtshpuclsx.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.zhoulong.xyz/gtforuncnl.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.xingfuxueyuan.xyz/gtaitbzmxq.html

[L04] 设置超时
来源：http://hz.sweek.top/gtcrmvgecb.html

Py:   requests.get(url, timeout=5)
来源：http://hz.andypj.xyz/gtekwcomdz.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.snrcjt.cn/gtoolrrhvq.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.hnxiangtu.top/gtseoqexyo.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.iojbl.cn/gtexmnjiyn.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.yvedp.cn/gtgiliitih.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.zhaomingkeji.xyz/gtmxgiwxjn.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.shanyushiyangtech.top/gtarkzevsh.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.ppjwa.cn/gtxesdysai.html

[L05] 上传文件（multipart）
来源：http://hz.fengsongda.top/gtebnlftih.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.vqdsnc.cn/gtjhswkjqw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.jyoumei.cn/gtdmlrczau.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.havefunace.top/gtddjvpekm.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.hongshengwenyu.top/gtissboljb.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.ivvv.top/gtwykwwsgf.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.cashguo.top/gtbltyinpr.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.52xcode.cn/gtcpwfmsol.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.zhengqikj.top/gtxxcsyiwy.html

[L06] 解析响应为 JSON
来源：http://hz.dashuyun.cn/gtqneegabo.html

Py:   resp.json()
来源：http://hz.yuxming.cn/gtgbayxemu.html

PHP:  json_decode($body, true);
来源：http://hz.quarkkingdee.top/gtgdqfqxnp.html

JS:   await resp.json()
来源：http://hz.iojbl.cn/gtqvnmptxw.html

TS:   await resp.json()
来源：http://hz.snrcjt.cn/gtyokbpmzg.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.gogol.net.cn/gtyludrqnj.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.guowangkeji.top/gtoethzylc.html

Ruby: JSON.parse(resp.body)
来源：http://hz.aizwys.cn/gtgjiqxmtk.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.chenlongwang.top/gthlhzhtpy.html

[L07] 处理 HTTP 状态码
来源：http://hz.hnqzz.top/gtkdnlgczp.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.ivvv.top/gtypathphs.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.ywan-chungtsiang.top/gtycthlbgk.html

JS:   resp.ok;  resp.status
来源：http://hz.hysaishi.cn/gtztfomkek.html

TS:   resp.ok;  resp.status
来源：http://hz.yanxiufei.cn/gtxsdvqzjz.html

Java: resp.statusCode()
来源：http://hz.wangshuangyany.cn/gtzbyqiatt.html

Go:   resp.StatusCode
来源：http://hz.jinqigfzy.top/gtydsnoqba.html

Ruby: resp.code.to_i
来源：http://hz.chenzaomai.com/gtvslkvynx.html

C#:   (int)resp.StatusCode
来源：http://hz.cashguo.top/gtwdnohhpb.html

[L08] 并发请求多个地址
来源：http://hz.yuanzhike.top/gtpqpynyhn.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.ybcxt.top/gtcrolcqoy.html

PHP:  curl_multi_init() 系列
来源：http://hz.wangdashe.top/gtcjdhyimi.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.hammf.cn/gtdfwdivjj.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.shangyingyoupin.top/gtpggaexwt.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.chenzaomai.com/gtylvgwmmm.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.shuidangran.top/gtnlqknuul.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.xuetiantiany.cn/gtyvtgvwns.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.hammf.cn/gtuqtucort.html

================================================================================
来源：http://hz.pycfn.com/gtcnpzwqvu.html

M. 命令行 / 进程 / 环境
来源：http://hz.nanxinkj.top/gttgeqxqkd.html

================================================================================
来源：http://hz.yj20258.top/gtrzgewicp.html

[M01] 读取命令行参数
来源：http://hz.feifeiyinyue.top/gtjwvoaxif.html

Py:   sys.argv[1:]
来源：http://hz.havefunace.top/gtkoyvnpmk.html

PHP:  $argv;  $argc;
来源：http://hz.xylfe.cn/gtxalbwksu.html

JS:   process.argv.slice(2)
来源：http://hz.shanyushiyangtech.top/gttspuduqc.html

TS:   process.argv.slice(2)
来源：http://hz.jiagoushi.top/gtcbxdhinj.html

Java: args 数组（main 方法参数）
来源：http://hz.jiagoushi.top/gtknzklorr.html

Go:   os.Args[1:]
来源：http://hz.yueranfly.top/gtnhvqlqae.html

Ruby: ARGV
来源：http://hz.fengsongda.top/gtssuwnqbb.html

C#:   args 数组（Main 方法参数）
来源：http://hz.zhengqikj.top/gtxjjocmtp.html

[M02] 读取环境变量
来源：http://hz.tanke756.top/gthwmetefx.html

Py:   os.environ.get("HOME")
来源：http://hz.jinqigufen.top/gtagzpgbbt.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.hammf.cn/gtgwjdvyqe.html

JS:   process.env.HOME
来源：http://hz.jinghuilouyu.cn/gtagmsiuka.html

TS:   process.env.HOME
来源：http://hz.yongpay.top/gtdkwgcizv.html

Java: System.getenv("HOME")
来源：http://hz.jinqigfzy.top/gtitaasxeh.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.jqgufenzy.top/gtiqgpmjxc.html

Ruby: ENV["HOME"]
来源：http://hz.ybcxt.top/gtdvnusgxu.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.snrcjt.cn/gtfmwewqvr.html

[M03] 执行外部命令
来源：http://hz.yonumen.top/gtvghfzxei.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.yj202588.top/gtmqlelzke.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.xingfuxueyuan.xyz/gtlbpanvzf.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.zhengqikj.top/gtehkxgmqj.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.hammf.cn/gtlzrfumgn.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.xingfuxueyuan.xyz/gtmpmizegn.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.0kj1m.cn/gtfycmfqnc.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.yj20258888.top/gtooxbdbjw.html

C#:   Process.Start("ls", "-l");
来源：http://hz.daxiang520.top/gtdqetcglb.html

[M04] 获取当前工作目录
来源：http://hz.316326.xyz/gtrjihwkgt.html

Py:   os.getcwd()
来源：http://hz.ywan-chungtsiang.top/gtrrlrhxqu.html

PHP:  getcwd();
来源：http://hz.yj20258888.top/gtckcuifkp.html

JS:   process.cwd()
来源：http://hz.c1oappe.top/gtyepionbt.html

TS:   process.cwd()
来源：http://hz.shanyushiyangkeji.top/gtrsoiburz.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.sufxvd.cn/gtwuuagntr.html

Go:   os.Getwd()
来源：http://hz.vqdsnc.cn/gtohbccrmh.html

Ruby: Dir.pwd
来源：http://hz.tianlin.xyz/gtphipoqai.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.9152youxi.cn/gtzhbmgnht.html

[M05] 设置退出码
来源：http://hz.nanxuanxn.top/gtwcabswnx.html

Py:   sys.exit(1)
来源：http://hz.cucudq.cn/gttvxgqxtt.html

PHP:  exit(1);
来源：http://hz.ivvv.top/gtbxeglygi.html

JS:   process.exit(1)
来源：http://hz.0kj1m.cn/gthfozevho.html

TS:   process.exit(1)
来源：http://hz.pengpengdd.cyou/gtztldpdis.html

Java: System.exit(1)
来源：http://hz.ywan-chungtsiang.top/gtjnlettpk.html

Go:   os.Exit(1)
来源：http://hz.zhiwuduotai.top/gtaqbwwcax.html

Ruby: exit 1
来源：http://hz.pengpengdd.cyou/gtnubzwylo.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.yueranfly.top/gtnhzvbdjf.html

[M06] 向标准错误输出
来源：http://hz.316326.xyz/gtruyfqxvh.html

Py:   print("err", file=sys.stderr)
来源：http://hz.xinyue.icu/gtncumohuf.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.shuidangran.top/gtgrmmznpg.html

JS:   console.error("err")
来源：http://hz.ppjwa.cn/gtlkytwgmz.html

TS:   console.error("err")
来源：http://hz.jqgufenzy.top/gtlaienmij.html

Java: System.err.println("err")
来源：http://hz.shzxlz.cn/gtbcjhrsvt.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.shzxlz.cn/gtnbfaemzk.html

Ruby: warn "err"
来源：http://hz.zdqjudy.top/gteuuqoydd.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.yuanzhike.top/gtxcqnhcjq.html

[M07] 判断是否为主入口
来源：http://hz.jianghu66.top/gtjqrczwbc.html

Py:   if __name__ == "__main__":
来源：http://hz.gotoacloud.top/gtyqfsldmi.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.zycfv.cn/gtiegrdsuy.html

JS:   require.main === module
来源：http://hz.smart0.xyz/gtbycursge.html

TS:   require.main === module
来源：http://hz.wangdashe.top/gtaeqhobvl.html

Java: public static void main(String[] args)
来源：http://hz.c1oappe.top/gtuiflbbrb.html

Go:   func main()
来源：http://hz.yj20258.top/gtyhysxajd.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.guowangkeji.top/gtictmdwqv.html

C#:   static void Main(string[] args)
来源：http://hz.ehwqpu.com/gtortctroi.html

[M08] 获取系统与运行时信息
来源：http://hz.cqqwz.cn/gtcfraebfk.html

Py:   platform.system();  platform.python_version()
来源：http://hz.hongshengwenyu.top/gtvqgshdkd.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.pengpengdd.cyou/gtrcdglpkb.html

JS:   process.platform;  process.version
来源：http://hz.yonumen.top/gtnwhqhtfo.html

TS:   process.platform;  process.version
来源：http://hz.zhengqikj.top/gtztsquyje.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.xuanzx.com/gtvcksbbfq.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.chenlongwang.top/gtbjcwilsf.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.xziqi.cn/gtyayomqta.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.nanxinkj.top/gthlhwulyv.html

================================================================================
来源：http://hz.xziqi.cn/gtgxfyudsq.html

N. 数据结构与算法
来源：http://hz.fengsongda.top/gtjekninbq.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtndztodcw.html

[N01] 二分查找（有序数组）
来源：http://hz.yvedp.cn/gtsyqpeagr.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.kuanghao11.cn/gtplvxtwqc.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.redwolf501.top/gtsbvsjbnd.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.feifeiyinyue.top/gtnkbnbgms.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.tian-w.cn/gtyrvrpekb.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.0kj1m.cn/gtzlcdpdxq.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.yuanzhike.top/gtsvnrfchk.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.chenzaomai.com/gtumfrpfli.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.wangshuangyany.cn/gtznuwoaqk.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.zhoulong.xyz/gtunnwoeir.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.sysykeji.top/gtxjuvoowq.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.yj20258.top/gtooxugxcd.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.sxryk.cn/gtcmpyejyc.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jyoumei.cn/gtlhrlzsco.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.cheryme.top/gteaojvawe.html

Go:   slices.Sort(arr)
来源：http://hz.dianchejie.cn/gtgnsshtzq.html

Ruby: arr.sort
来源：http://hz.aibaodan.cn/gtqucdzdbe.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.nwbrower.top/gtwudrkvvi.html

[N03] 快速排序（分治示例）
来源：http://hz.gotoacloud.top/gtgellccaz.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.nwbrower.top/gtbpbqqyyi.html

PHP:  // 递归实现，或用 usort
来源：http://hz.shanyushiyangtech.top/gtoujxbnks.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yvedp.cn/gtyfjxoxzj.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.cucudq.cn/gtjqrpuvug.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.cqqwz.cn/gtwjiotikn.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.yongpay.top/gthrkysoue.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.kuanghao11.cn/gtvkupddkp.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.aizwys.cn/gthiwycgsl.html

[N04] 斐波那契数列
来源：http://hz.zhengqikj.top/gtolawaaya.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.jinqigfzy.top/gtsazzuhxx.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.zhixingplan.top/gtvubdrrsy.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.sxryk.cn/gtgxtfsfdr.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.gzhubu.top/gtsrbbixhp.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.ybcxt.top/gtedrneehi.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.0kj1m.cn/gtcdizmrht.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.pengpengdd.cyou/gtesjeksnv.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.smart0.xyz/gtznlhkxxr.html

[N05] 最大公约数
来源：http://hz.dashuyun.cn/gtpheaqcik.html

Py:   math.gcd(a, b)
来源：http://hz.hywenlv.cn/gtnnvdyloz.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.wangshuangyany.cn/gthgfhumpu.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yj202588.top/gtdwqxxkat.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.cheryme.top/gthkimpfsd.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.yj20258888.top/gtxcawyjak.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.cucudq.cn/gtgzejvsvf.html

Ruby: a.gcd(b)
来源：http://hz.cheryme.top/gtbyilruqq.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.pycfn.com/gtsuhwnkri.html

[N06] 判断回文字符串
来源：http://hz.havefunace.top/gtrfrzkgil.html

Py:   s == s[::-1]
来源：http://hz.yueranfly.top/gtmjqstidc.html

PHP:  $s === strrev($s);
来源：http://hz.zhoulong.xyz/gtrqeqcont.html

JS:   s === [...s].reverse().join("")
来源：http://hz.nwbrower.top/gtvnirmrmd.html

TS:   s === [...s].reverse().join("")
来源：http://hz.xuetiantiany.cn/gtjcxfhgfv.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.ehwqpu.com/gtcarelybn.html

Go:   // 双指针从两端比较
来源：http://hz.gogol.net.cn/gtiqphxmqj.html

Ruby: s == s.reverse
来源：http://hz.aibaodan.cn/gtvfekxikn.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.gotoacloud.top/gtpcimcpas.html

[N07] 两数之和（返回下标）
来源：http://hz.fzhhl.top/gtsezafmys.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.0kj1m.cn/gtkvwlksvc.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.sweek.top/gtrvmupdtw.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.gaohongyu789.top/gtultquyzv.html

TS:   // 手写 Map<string, number>
来源：http://hz.zhaomingkeji.xyz/gtbmydtuvm.html

Java: // 手写 HashMap
来源：http://hz.xingfuxueyuan.xyz/gtorpfcfjo.html

Go:   // 手写 map[int]int
来源：http://hz.ybcxt.top/gtxyrvylvz.html

Ruby: // 手写 Hash
来源：http://hz.chenjidiqi.icu/gtplnqtbyk.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.gzhubu.top/gtrvakwtbm.html

[N08] 生成全排列
来源：http://hz.mhx1999.top/gtffuovnrn.html

Py:   itertools.permutations(arr)
来源：http://hz.hammf.cn/gtmytpeaai.html

PHP:  // 手写递归交换
来源：http://hz.andypj.xyz/gtldfpnerf.html

JS:   // 手写回溯递归
来源：http://hz.jiagoushi.top/gtklbztyjy.html

TS:   // 手写回溯递归
来源：http://hz.hammf.cn/gtzxkbdflh.html


<!-- 参考信息 -->