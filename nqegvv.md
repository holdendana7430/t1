代发 wailian999

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.hnqzz.top/gtuhglvdve.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.cdnleiting.top/gtynqtbrwo.html

JS:   JSON.stringify(obj)
来源：http://hz.yj20258.top/gtjanjhsjd.html

TS:   JSON.stringify(obj)
来源：http://hz.snrcjt.cn/gtqtskalqd.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.haohaochexian.top/gtuzjxmcpn.html

Go:   json.Marshal(obj)
来源：http://hz.xuetiantiany.cn/gtdscmiuhj.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.xinyue.icu/gtiemjhofa.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.hywenlv.cn/gtjkbdspjl.html

[K02] JSON 字符串转对象
来源：http://hz.9152youxi.cn/gtfqraatfl.html

Py:   json.loads(s)
来源：http://hz.sxryk.cn/gtjgguqcrm.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.zhaomingkeji.xyz/gteaqltzic.html

JS:   JSON.parse(s)
来源：http://hz.nanxuanxn.top/gtrgtreope.html

TS:   JSON.parse(s)
来源：http://hz.yuanzhike.top/gtdctyqbqz.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.ywan-chungtsiang.top/gtobnmaves.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.yj20258.top/gtithrwoou.html

Ruby: JSON.parse(s)
来源：http://hz.hammf.cn/gtepkjkzjf.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.aizwys.cn/gtdbxngqlv.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.hongshengwenyu.top/gtiuwbuqlm.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.yj202588.top/gtfhnhhasg.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.haohaochexian.top/gtxkgciybi.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.daxiang520.top/gtpvadzsuv.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.yonumen.top/gtjnkjuxqt.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.iojbl.cn/gtfcichxjx.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.ehwqpu.com/gtgdhgaznd.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.tian-w.cn/gtaulgzwlk.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.zhijiandao.cn/gtsgwxqmtw.html

[K04] 读取 JSON 文件
来源：http://hz.pengpengdd.cyou/gtyfcmvfhe.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.svipenyu.cn/gtlndgxfky.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.feifeiyinyue.top/gtmbkfnugl.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.svipenyu.cn/gtaxmpycii.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.fzhhl.top/gtpwjsrpqj.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.daria6918.cn/gtxsgrvwop.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.daxiang520.top/gtmeilufay.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.birdmap.top/gtcvreplii.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.iojbl.cn/gtyovfuppy.html

[K05] 深拷贝对象
来源：http://hz.jiagoushi.top/gtwomufeyy.html

Py:   copy.deepcopy(obj)
来源：http://hz.fengsongda.top/gtdhuyrbdn.html

PHP:  unserialize(serialize($obj));
来源：http://hz.jinqigufen.top/gtandaygeu.html

JS:   structuredClone(obj)
来源：http://hz.dashuyun.cn/gtgblydepz.html

TS:   structuredClone(obj)
来源：http://hz.feifeiyinyue.top/gtzftsnsxz.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.yonumen.top/gtlbczdlpa.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.jinghuilouyu.cn/gttnqyxewd.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.jinqigufen.top/gtacrblwni.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.xingfuxueyuan.xyz/gtomqhetlz.html

[K06] 解析 URL 查询串
来源：http://hz.yj20258.top/gtbcicnlkr.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.mhx1999.top/gtdftexrna.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.guowangkeji.top/gtepztjlpy.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yj20258888.top/gtpfvsdbbh.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.xziqi.cn/gtnumldejb.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.zhiwuduotai.top/gtpioewslg.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.xylfe.cn/gtoqztquyz.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.xziqi.cn/gtvgxjgmqs.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.tian-w.cn/gtaprfvdej.html

[K07] 进制转换
来源：http://hz.quarkkingdee.top/gtocrhvahy.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.zdqjudy.top/gtjasbcxcy.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.tian-w.cn/gtgwosdkzf.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.jinqigufen.top/gtamawdglp.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.andypj.xyz/gtyydtikxn.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.zycfv.cn/gtqozkpvaj.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.xuetiantiany.cn/gtcbutjftb.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.cdnleiting.top/gtmneqoixk.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.ywan-chungtsiang.top/gtdzczebhh.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.ywan-chungtsiang.top/gtgrqopbws.html

Py:   pickle.dumps(obj)
来源：http://hz.haohaochexian.top/gtdncgfqfs.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.jinqigufen.top/gtapqgxsei.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.zhongyouzk.top/gtneqbxrxj.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.jiagoushi.top/gtxvnfgtjz.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.gotoacloud.top/gtqlmzhgsf.html

Go:   encoding/gob
来源：http://hz.dashuyun.cn/gtvoesmeea.html

Ruby: Marshal.dump(obj)
来源：http://hz.shanyushiyangtech.top/gtsyrthume.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.shangyingyoupin.top/gtyhewgsuz.html

================================================================================
来源：http://hz.nanxuanxn.top/gtkaflwfwu.html

L. 网络请求
来源：http://hz.pengpengdd.cyou/gtwgzqtknw.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtelxvluye.html

[L01] 发送 GET 请求
来源：http://hz.316326.xyz/gttcokhglj.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.hfpthk.cn/gtzaldrllb.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.cheryme.top/gtfaiotdzz.html

JS:   await fetch(url)
来源：http://hz.zhixingplan.top/gtuwckoycr.html

TS:   await fetch(url)
来源：http://hz.smart0.xyz/gtncwcljdn.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.chenlongwang.top/gtsugamyls.html

Go:   resp, err := http.Get(url)
来源：http://hz.jinghuilouyu.cn/gtwvmibeqg.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.cqqwz.cn/gtgkiomxob.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.hywenlv.cn/gtnekojmeb.html

[L02] 发送 POST JSON
来源：http://hz.dashuyun.cn/gtbvawqgkl.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.cashguo.top/gtflyyprbo.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.daria6918.cn/gtgdydphkz.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.pycfn.com/gtjfsihipu.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.xylfe.cn/gtapnqhtoc.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.wangshuangyany.cn/gtbnviuvtb.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.havefunace.top/gthvduhguu.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.nanxinkj.top/gtmfxnpita.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.ppjwa.cn/gtmhufeeni.html

[L03] 设置自定义请求头
来源：http://hz.yvedp.cn/gtfnfyibnq.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.hnxiangtu.top/gtlcnqysjj.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.fengsongda.top/gthoiredai.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.aibaodan.cn/gtsrdgytpq.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.gaohongyu789.top/gtywtvdydl.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.hnxiangtu.top/gteyssemoy.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.cheryme.top/gteartuoml.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.yanxiufei.cn/gtyfxaekww.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.jqgufenzy.top/gtbfbolyzv.html

[L04] 设置超时
来源：http://hz.yonumen.top/gtqpqqjlbm.html

Py:   requests.get(url, timeout=5)
来源：http://hz.nwbrower.top/gtdwkhywfo.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.aizwys.cn/gtsgiibdus.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jqgufenzy.top/gtbmrokqkq.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.tian-w.cn/gtobfzslfg.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.gotoacloud.top/gtiahweshu.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.gotoacloud.top/gtolbsftrn.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.hnqzz.top/gtqltmkxji.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.chenjidiqi.icu/gtktnnvakf.html

[L05] 上传文件（multipart）
来源：http://hz.pengpengdd.cyou/gtezeuumhu.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.svipenyu.cn/gtnurxoqtk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.zhaomingkeji.xyz/gtdhmcgvid.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.chenlongwang.top/gtiluuhiyu.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.aizwys.cn/gtismshykk.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.nwbrower.top/gtwwxvbyhm.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.zhiwuduotai.top/gtufjxblkr.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.hnxiangtu.top/gttuxczvta.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.zhiwuduotai.top/gtyrligzoe.html

[L06] 解析响应为 JSON
来源：http://hz.snrcjt.cn/gtkctfkeco.html

Py:   resp.json()
来源：http://hz.ivvv.top/gtptlxoryx.html

PHP:  json_decode($body, true);
来源：http://hz.yongpay.top/gtzngmthsl.html

JS:   await resp.json()
来源：http://hz.yongpay.top/gtekurwlxw.html

TS:   await resp.json()
来源：http://hz.quarkkingdee.top/gtnkmidvsl.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.pengpengdd.cyou/gtsjeepntw.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.yuxming.cn/gtfvppwfzk.html

Ruby: JSON.parse(resp.body)
来源：http://hz.andypj.xyz/gtnurndeaz.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.xziqi.cn/gteifuwcaq.html

[L07] 处理 HTTP 状态码
来源：http://hz.guannengcc.top/gtefyaunti.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.iojbl.cn/gtjesqxswg.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.52xcode.cn/gtkxhrzvvs.html

JS:   resp.ok;  resp.status
来源：http://hz.9152youxi.cn/gtgozuarfp.html

TS:   resp.ok;  resp.status
来源：http://hz.aizwys.cn/gtqqwlrlym.html

Java: resp.statusCode()
来源：http://hz.cqqwz.cn/gtrcwjwtzs.html

Go:   resp.StatusCode
来源：http://hz.cashguo.top/gtmkambrye.html

Ruby: resp.code.to_i
来源：http://hz.fengsongda.top/gtyxmitnvu.html

C#:   (int)resp.StatusCode
来源：http://hz.birdmap.top/gtjxnyrxhz.html

[L08] 并发请求多个地址
来源：http://hz.dashuyun.cn/gtkdjucgmy.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.sxryk.cn/gtpinvshui.html

PHP:  curl_multi_init() 系列
来源：http://hz.meibo888.top/gtneiclesj.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.wangshuangyany.cn/gtzwyadujy.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.shanyushiyangkeji.top/gtqyjyykfl.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.shanyushiyangtech.top/gtyrztervf.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.chenlongwang.top/gtcehvnjcf.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.pengpengdd.cyou/gtijlltbqg.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.gaohongyu789.top/gtzjxrezph.html

================================================================================
来源：http://hz.guowangkeji.top/gtkcayvkwz.html

M. 命令行 / 进程 / 环境
来源：http://hz.shangyingyoupin.top/gtizcbqhis.html

================================================================================
来源：http://hz.hnxiangtu.top/gtvjpivbwj.html

[M01] 读取命令行参数
来源：http://hz.cheryme.top/gtsuzhbazk.html

Py:   sys.argv[1:]
来源：http://hz.jyoumei.cn/gtpxobhbak.html

PHP:  $argv;  $argc;
来源：http://hz.cucudq.cn/gtcjodyorc.html

JS:   process.argv.slice(2)
来源：http://hz.jinqigufen.top/gtbpjmkohg.html

TS:   process.argv.slice(2)
来源：http://hz.zdqjudy.top/gtvbnafbcl.html

Java: args 数组（main 方法参数）
来源：http://hz.nanxuanxn.top/gtadrybaqm.html

Go:   os.Args[1:]
来源：http://hz.tanke756.top/gtpohvgtfo.html

Ruby: ARGV
来源：http://hz.jyoumei.cn/gtvbbrklhu.html

C#:   args 数组（Main 方法参数）
来源：http://hz.chenlongwang.top/gtiquiuqcs.html

[M02] 读取环境变量
来源：http://hz.xuetiantiany.cn/gtwxxqaito.html

Py:   os.environ.get("HOME")
来源：http://hz.yj20258.top/gthmosbddx.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.guannengcc.top/gtonvqkpvl.html

JS:   process.env.HOME
来源：http://hz.hysaishi.cn/gtqgtkbjzs.html

TS:   process.env.HOME
来源：http://hz.hnqzz.top/gtrqbtutea.html

Java: System.getenv("HOME")
来源：http://hz.shzxlz.cn/gtaxeufokb.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.yj202588.top/gtcqjrtbff.html

Ruby: ENV["HOME"]
来源：http://hz.tanke756.top/gtkvzllsrf.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.chenjidiqi.icu/gtczqgrpdv.html

[M03] 执行外部命令
来源：http://hz.ehwqpu.com/gturafskfk.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.aizwys.cn/gtxfiaryry.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.chenlongwang.top/gtbplvvuxl.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.pycfn.com/gtlkgjikjg.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.wangshuangyany.cn/gtqyrnrbhj.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.ydjk.org.cn/gtohryrvcl.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.gogol.net.cn/gtvmynnero.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.zhaomingkeji.xyz/gtsagyferx.html

C#:   Process.Start("ls", "-l");
来源：http://hz.zhiwuduotai.top/gtjaizzvzw.html

[M04] 获取当前工作目录
来源：http://hz.ybcxt.top/gtadzvfmif.html

Py:   os.getcwd()
来源：http://hz.iojbl.cn/gtfltlmqky.html

PHP:  getcwd();
来源：http://hz.jianghu66.top/gtinbwjlkh.html

JS:   process.cwd()
来源：http://hz.jyoumei.cn/gtmdozrnop.html

TS:   process.cwd()
来源：http://hz.yangfankeji.com/gtcrgtwtgl.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.cheryme.top/gtlgafkjth.html

Go:   os.Getwd()
来源：http://hz.yuxming.cn/gtquvlviqv.html

Ruby: Dir.pwd
来源：http://hz.sweek.top/gtfedlyouc.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.nanxinkj.top/gtuqnqkeoo.html

[M05] 设置退出码
来源：http://hz.jyoumei.cn/gtauqjuvra.html

Py:   sys.exit(1)
来源：http://hz.cucudq.cn/gtegsxtzed.html

PHP:  exit(1);
来源：http://hz.hongshengwenyu.top/gtikfbhylc.html

JS:   process.exit(1)
来源：http://hz.andypj.xyz/gtemuihnui.html

TS:   process.exit(1)
来源：http://hz.zhiwuduotai.top/gtepiktjtb.html

Java: System.exit(1)
来源：http://hz.tianlin.xyz/gtgnclopse.html

Go:   os.Exit(1)
来源：http://hz.jinghuilouyu.cn/gtxwtzmcle.html

Ruby: exit 1
来源：http://hz.hnxiangtu.top/gtlsowqycf.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.nanxuanxn.top/gtxgokvxhv.html

[M06] 向标准错误输出
来源：http://hz.ydzc1.top/gtpzotbwdb.html

Py:   print("err", file=sys.stderr)
来源：http://hz.xylfe.cn/gtfndkdvhx.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.daxiang520.top/gtabyljjlf.html

JS:   console.error("err")
来源：http://hz.chenlongwang.top/gtefymsuvq.html

TS:   console.error("err")
来源：http://hz.jinqigufen.top/gtlpdgbdrr.html

Java: System.err.println("err")
来源：http://hz.haohaochexian.top/gtdvpvcxrr.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.zdqjudy.top/gtniswugnq.html

Ruby: warn "err"
来源：http://hz.gaohongyu789.top/gtpgozyekj.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.andypj.xyz/gtzbdrilks.html

[M07] 判断是否为主入口
来源：http://hz.yangfankeji.com/gtpstdzclw.html

Py:   if __name__ == "__main__":
来源：http://hz.xuanzx.com/gtclhuijqs.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.hongshengwenyu.top/gtpwrfdgwd.html

JS:   require.main === module
来源：http://hz.jqgufenzy.top/gtlwbcntit.html

TS:   require.main === module
来源：http://hz.yvedp.cn/gtctjnuotr.html

Java: public static void main(String[] args)
来源：http://hz.meibo888.top/gtjabuxrvr.html

Go:   func main()
来源：http://hz.yuxming.cn/gtvfkgdfij.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.aibaodan.cn/gtmwrhxadj.html

C#:   static void Main(string[] args)
来源：http://hz.yuanzhike.top/gtrtxoifgf.html

[M08] 获取系统与运行时信息
来源：http://hz.yvedp.cn/gtthqjmstg.html

Py:   platform.system();  platform.python_version()
来源：http://hz.yuxming.cn/gtbxbmsoul.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.ydzc1.top/gtebnybggt.html

JS:   process.platform;  process.version
来源：http://hz.jqgfzy.top/gtvtczkpvu.html

TS:   process.platform;  process.version
来源：http://hz.nanxuanxn.top/gtepnfdlmy.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.shzxlz.cn/gtjgripled.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.iojbl.cn/gtdsjnjfck.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.daria6918.cn/gtbbhfzrqn.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.shanyushiyangkeji.top/gtcyaqpfbg.html

================================================================================
来源：http://hz.zycfv.cn/gtbciyearp.html

N. 数据结构与算法
来源：http://hz.jqgfzy.top/gthdgzegmh.html

================================================================================
来源：http://hz.aizwys.cn/gtwjcbucbh.html

[N01] 二分查找（有序数组）
来源：http://hz.zhengqikj.top/gtlapmpnrm.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.xuetiantiany.cn/gtnventcqe.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.yangfankeji.com/gtmttvccjp.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yangfankeji.com/gtwiveieuz.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.gotoacloud.top/gtsfabxgso.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.yuanzhike.top/gtuvcltlkl.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.nwbrower.top/gtpdbaljjo.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.jinqigufen.top/gtfwryeokc.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.52xcode.cn/gtjsjypnem.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.fengsongda.top/gtszatnkef.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.zhoulong.xyz/gtkwqgwxla.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.quarkkingdee.top/gtudptpzkr.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yvedp.cn/gtxnaunlet.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.zhijiandao.cn/gtxcizcwaj.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.pengpengdd.cyou/gtafalpxnh.html

Go:   slices.Sort(arr)
来源：http://hz.shanyushiyangkeji.top/gtlhmhpvfb.html

Ruby: arr.sort
来源：http://hz.xuanzx.com/gtpmkcvpza.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.jinyuanbaomall.cn/gttxlgqcnr.html

[N03] 快速排序（分治示例）
来源：http://hz.jyoumei.cn/gthlokwqip.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.gogol.net.cn/gttjuligku.html

PHP:  // 递归实现，或用 usort
来源：http://hz.shuidangran.top/gtfpupxnef.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.sweek.top/gtlgrbxjgt.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.redwolf501.top/gtcvhcbbub.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.hammf.cn/gtyttowjfa.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.jinqigufen.top/gthjommpua.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.ydzc1.top/gtjnphnzhi.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.ppjwa.cn/gtorvuakqz.html

[N04] 斐波那契数列
来源：http://hz.hnxiangtu.top/gtsezefuaa.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.fengsongda.top/gtwfvpalxq.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.svipenyu.cn/gtwzchwaer.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.ywan-chungtsiang.top/gtumjxtdeq.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.nanxuanxn.top/gtqwpirauz.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.ehwqpu.com/gtnwqaxeul.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.zdqjudy.top/gtetbigqva.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.zhengqikj.top/gtrzgqefju.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.jyoumei.cn/gtxmcdaidw.html

[N05] 最大公约数
来源：http://hz.yangfankeji.com/gtobqksdym.html

Py:   math.gcd(a, b)
来源：http://hz.jianghu66.top/gtfyctthtw.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.guannengcc.top/gtrgqzwwqc.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.ehwqpu.com/gtjlcwgjno.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.zycfv.cn/gtnwlhibot.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.jqgufenzy.top/gtfntjlwvc.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.xinyue.icu/gtiavfxjlr.html

Ruby: a.gcd(b)
来源：http://hz.cashguo.top/gtezzuntdt.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.jyoumei.cn/gtcwkiwtnq.html

[N06] 判断回文字符串
来源：http://hz.iojbl.cn/gtclcmdzcm.html

Py:   s == s[::-1]
来源：http://hz.ydjk.org.cn/gtpxrzewtw.html

PHP:  $s === strrev($s);
来源：http://hz.yonumen.top/gtfdktlpsm.html

JS:   s === [...s].reverse().join("")
来源：http://hz.havefunace.top/gtansryshh.html

TS:   s === [...s].reverse().join("")
来源：http://hz.hnqzz.top/gtvpsmhjzf.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.zhixingplan.top/gtduzbkajl.html

Go:   // 双指针从两端比较
来源：http://hz.fzhhl.top/gtdgmbprsi.html

Ruby: s == s.reverse
来源：http://hz.yj20258888.top/gtkllrcxhf.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.yangfankeji.com/gtomyztgod.html

[N07] 两数之和（返回下标）
来源：http://hz.yuxming.cn/gtfygxyrxv.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.xziqi.cn/gtbizjxqbf.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.smart0.xyz/gttlmfvern.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.xuanzx.com/gtvxzvyrxq.html

TS:   // 手写 Map<string, number>
来源：http://hz.jlsjyb.cn/gtfloqtgjt.html

Java: // 手写 HashMap
来源：http://hz.shanyushiyangkeji.top/gtuccdjbai.html

Go:   // 手写 map[int]int
来源：http://hz.nanxinkj.top/gtbepdonyf.html

Ruby: // 手写 Hash
来源：http://hz.cucudq.cn/gtqzpzdswo.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.shangyingyoupin.top/gtwhkblhoo.html

[N08] 生成全排列
来源：http://hz.yuxming.cn/gtgijhbbqk.html

Py:   itertools.permutations(arr)
来源：http://hz.pycfn.com/gtcdcncczp.html

PHP:  // 手写递归交换
来源：http://hz.bjfxy.top/gtnsutcwaf.html

JS:   // 手写回溯递归
来源：http://hz.tanke756.top/gtilnxinbw.html

TS:   // 手写回溯递归
来源：http://hz.cheryme.top/gttrequmhg.html

Java: // 手写回溯递归
来源：http://hz.hysaishi.cn/gtibvxtqlh.html

Go:   // 手写回溯递归
来源：http://hz.zhiwuduotai.top/gtbvwmoioc.html

Ruby: arr.permutation.to_a
来源：http://hz.jinyuanbaomall.cn/gtkwtfjslt.html

C#:   // 手写回溯递归
来源：http://hz.xylfe.cn/gtzbljijar.html

[N09] 栈与队列
来源：http://hz.gzhubu.top/gtubaqasmx.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.daria6918.cn/gttsmnzyaa.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.smart0.xyz/gthjrpxfrd.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.ppjwa.cn/gtthjiptpi.html


<!-- 参考信息 -->