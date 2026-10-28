代发 wailian999

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.zdqjudy.top/gtfwasqvrr.html

Go:   json.Marshal(obj)
来源：http://hz.guowangkeji.top/gtollojinf.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.yanxiufei.cn/gtkpyfgxzl.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.chenjidiqi.icu/gtzkxcdtml.html

[K02] JSON 字符串转对象
来源：http://hz.nanxuanxn.top/gttockladh.html

Py:   json.loads(s)
来源：http://hz.sxryk.cn/gtquurfrvw.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.aizwys.cn/gthpcklogu.html

JS:   JSON.parse(s)
来源：http://hz.daxiang520.top/gtwuuhbxxl.html

TS:   JSON.parse(s)
来源：http://hz.daria6918.cn/gtwpawugqz.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.9152youxi.cn/gtitpchuck.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.meibo888.top/gtbojcvvnl.html

Ruby: JSON.parse(s)
来源：http://hz.sweek.top/gtzjgdabkl.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.xylfe.cn/gtqrtimlgw.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.jqgufenzy.top/gtmwdmmcsx.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.yj20258.top/gtwpvvcsho.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.xuanzx.com/gtpawtekzt.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.dianchejie.cn/gtiyuipnqk.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.sxryk.cn/gtwcfjykkd.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.bjfxy.top/gtljikeiqq.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.shzxlz.cn/gtzwzxgzjq.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.hnqzz.top/gtafsvrbxd.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.zhiwuduotai.top/gtyoojhoje.html

[K04] 读取 JSON 文件
来源：http://hz.9152youxi.cn/gtcjxpzagu.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.xylfe.cn/gtsrthmioj.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.jqgufenzy.top/gtgvpzpdlc.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.kuanghao11.cn/gtxzzgbtxx.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.52xcode.cn/gtbssunvdm.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.svipenyu.cn/gtonkglcqe.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.shanyushiyangtech.top/gtedilowlr.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.ehwqpu.com/gtmikxlhlx.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.haohaochexian.top/gtkxjdyznm.html

[K05] 深拷贝对象
来源：http://hz.ydjk.org.cn/gtjkxyzsjd.html

Py:   copy.deepcopy(obj)
来源：http://hz.cdnleiting.top/gtuulqdrtw.html

PHP:  unserialize(serialize($obj));
来源：http://hz.hywenlv.cn/gtbdhtjieu.html

JS:   structuredClone(obj)
来源：http://hz.yuxming.cn/gtwixslqvp.html

TS:   structuredClone(obj)
来源：http://hz.birdmap.top/gtwzwzfzty.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.zhaomingkeji.xyz/gtorvkgfsi.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.sxryk.cn/gtkbmmneaf.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.yueranfly.top/gtfgooktsp.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.yonumen.top/gtgtbnwfxk.html

[K06] 解析 URL 查询串
来源：http://hz.jinqigfzy.top/gtunccpofz.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.xingfuxueyuan.xyz/gtirbwhfrw.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.jinyuanbaomall.cn/gtujugxfgd.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.tianlin.xyz/gtbjfvcgrl.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.hfpthk.cn/gtlulyvkgs.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.sufxvd.cn/gtnmxccshd.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.vqdsnc.cn/gtyvnmdmqz.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.hfpthk.cn/gtglemvzru.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.gogol.net.cn/gteuqsolzv.html

[K07] 进制转换
来源：http://hz.mhx1999.top/gtmqtfxahz.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.yangfankeji.com/gtesikjolv.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.snrcjt.cn/gtrubhtiac.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.jqgufenzy.top/gtoxecywhl.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.daria6918.cn/gtuxintdic.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.aizwys.cn/gtdotjvmma.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.dianchejie.cn/gtgvmptlfq.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.gaohongyu789.top/gtncdzpwdj.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.chenlongwang.top/gthbvbxgrw.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.aibaodan.cn/gtszgawsrs.html

Py:   pickle.dumps(obj)
来源：http://hz.ybcxt.top/gtzgzgnmcp.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.yonumen.top/gtvgmaoaxu.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.yueranfly.top/gttbhrmobr.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.bjfxy.top/gtlfaoqgqt.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.gogol.net.cn/gtbicguxim.html

Go:   encoding/gob
来源：http://hz.chenjidiqi.icu/gtsjyhjoih.html

Ruby: Marshal.dump(obj)
来源：http://hz.jqgfzy.top/gtyrnopext.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.kuanghao11.cn/gtbdcmthtw.html

================================================================================
来源：http://hz.jianghu66.top/gtxwssoipo.html

L. 网络请求
来源：http://hz.kuanghao11.cn/gtoffkltfb.html

================================================================================
来源：http://hz.hywenlv.cn/gtomxbgorj.html

[L01] 发送 GET 请求
来源：http://hz.jyoumei.cn/gtjrtyfgeo.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.yj20258888.top/gtwrymyxli.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.chenjidiqi.icu/gtwxiipdwi.html

JS:   await fetch(url)
来源：http://hz.hysaishi.cn/gtrspfaxit.html

TS:   await fetch(url)
来源：http://hz.nwbrower.top/gtmadgemaw.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.wangshuangyany.cn/gtgkmzvenh.html

Go:   resp, err := http.Get(url)
来源：http://hz.ppjwa.cn/gtkkwhdvqu.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.jlsjyb.cn/gttuvxxncc.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.fengsongda.top/gtifactiwu.html

[L02] 发送 POST JSON
来源：http://hz.tanke756.top/gtalubryir.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.shuidangran.top/gtilcarpdz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.meibo888.top/gtgoljkwga.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.gzhubu.top/gttybtbfim.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.feifeiyinyue.top/gtbbejtbla.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.yangfankeji.com/gtvclioprn.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.quarkkingdee.top/gtsihxfjmm.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.bjfxy.top/gtfgjhinup.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.feifeiyinyue.top/gtyhhcsrme.html

[L03] 设置自定义请求头
来源：http://hz.hnxiangtu.top/gtfawnlvct.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.zhoulong.xyz/gtsesjrqtb.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.daxiang520.top/gtarsfqeyk.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jyoumei.cn/gtstootkow.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.shanyushiyangkeji.top/gtudbwsqgc.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.jianghu66.top/gtpkevewdr.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.dianchejie.cn/gtpnutdfnu.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.chenjidiqi.icu/gtxxfvfyga.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.feifeiyinyue.top/gttamhzejd.html

[L04] 设置超时
来源：http://hz.yj20258888.top/gthyafatdl.html

Py:   requests.get(url, timeout=5)
来源：http://hz.hnqzz.top/gtvfiudiri.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.snrcjt.cn/gtnljkdfbk.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.nanxuanxn.top/gtkznkoncr.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.guowangkeji.top/gtkgpxknlr.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.gogol.net.cn/gtjpwnvmom.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.wangshuangyany.cn/gtuypmgobv.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.ydjk.org.cn/gtpxxveoqj.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.cucudq.cn/gtbrhuyvmg.html

[L05] 上传文件（multipart）
来源：http://hz.yueranfly.top/gtonalulpm.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.meibo888.top/gtmjxvklsz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.shzxlz.cn/gtzuayurmu.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.cdnleiting.top/gtebxyaxzn.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.shangyingyoupin.top/gtosewjeao.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.shuidangran.top/gtkmzdcpzn.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.chenlongwang.top/gtjaxkylca.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.dianchejie.cn/gtkpqfodco.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.shanyushiyangkeji.top/gttdicaemb.html

[L06] 解析响应为 JSON
来源：http://hz.dashuyun.cn/gtmhktnije.html

Py:   resp.json()
来源：http://hz.ehwqpu.com/gtlfdkwfne.html

PHP:  json_decode($body, true);
来源：http://hz.quarkkingdee.top/gtsgbfnxtf.html

JS:   await resp.json()
来源：http://hz.yueranfly.top/gtwxrudubq.html

TS:   await resp.json()
来源：http://hz.hysaishi.cn/gtlpcralvy.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.pycfn.com/gtmghdctag.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.chenjidiqi.icu/gtgyznwvau.html

Ruby: JSON.parse(resp.body)
来源：http://hz.chenzaomai.com/gthamcejbg.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.jqgfzy.top/gtjywzmbol.html

[L07] 处理 HTTP 状态码
来源：http://hz.yuanzhike.top/gtgnsigujm.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.xingfuxueyuan.xyz/gtuvkljamb.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.quarkkingdee.top/gtcoradqxu.html

JS:   resp.ok;  resp.status
来源：http://hz.shanyushiyangtech.top/gtytpsgauk.html

TS:   resp.ok;  resp.status
来源：http://hz.yj202588.top/gtpwasqzaw.html

Java: resp.statusCode()
来源：http://hz.yuxming.cn/gtijohzvyg.html

Go:   resp.StatusCode
来源：http://hz.yuanzhike.top/gtcclltuvp.html

Ruby: resp.code.to_i
来源：http://hz.c1oappe.top/gtwczufnaq.html

C#:   (int)resp.StatusCode
来源：http://hz.pycfn.com/gtgjiwdtso.html

[L08] 并发请求多个地址
来源：http://hz.chenzaomai.com/gtyzpiznvf.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.cheryme.top/gtcmytxnde.html

PHP:  curl_multi_init() 系列
来源：http://hz.cucudq.cn/gttddggrwv.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zycfv.cn/gtgcfgejvt.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yueranfly.top/gtmvntvvux.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.gogol.net.cn/gtbnrftdmn.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.ivvv.top/gtasnajqbg.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.xylfe.cn/gtcnsprrhr.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.zhixingplan.top/gtrzkyeett.html

================================================================================
来源：http://hz.quarkkingdee.top/gtmfzmbudy.html

M. 命令行 / 进程 / 环境
来源：http://hz.ehwqpu.com/gtvghzopay.html

================================================================================
来源：http://hz.hnqzz.top/gtxcxjsorz.html

[M01] 读取命令行参数
来源：http://hz.yj202588.top/gtfcbabenl.html

Py:   sys.argv[1:]
来源：http://hz.316326.xyz/gtongchkgf.html

PHP:  $argv;  $argc;
来源：http://hz.xuetiantiany.cn/gtpifqlgcd.html

JS:   process.argv.slice(2)
来源：http://hz.yvedp.cn/gtlmsomdto.html

TS:   process.argv.slice(2)
来源：http://hz.sysykeji.top/gthuzlqzpr.html

Java: args 数组（main 方法参数）
来源：http://hz.zhaomingkeji.xyz/gtyykijysw.html

Go:   os.Args[1:]
来源：http://hz.kuanghao11.cn/gtapxtbwmn.html

Ruby: ARGV
来源：http://hz.shanyushiyangtech.top/gtidrxcqzf.html

C#:   args 数组（Main 方法参数）
来源：http://hz.yvedp.cn/gtwjahvtvl.html

[M02] 读取环境变量
来源：http://hz.xinyue.icu/gttekuzppq.html

Py:   os.environ.get("HOME")
来源：http://hz.sysykeji.top/gtspichimo.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.hfpthk.cn/gtwlpnnvax.html

JS:   process.env.HOME
来源：http://hz.jinyuanbaomall.cn/gtdfweqmmk.html

TS:   process.env.HOME
来源：http://hz.nanxinkj.top/gtgxhlmsxh.html

Java: System.getenv("HOME")
来源：http://hz.quarkkingdee.top/gtwemahcha.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.guowangkeji.top/gtonjseceq.html

Ruby: ENV["HOME"]
来源：http://hz.zycfv.cn/gtnwlsidye.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.zhoulong.xyz/gtupbmstsn.html

[M03] 执行外部命令
来源：http://hz.zhoulong.xyz/gtqfmstemx.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.fzhhl.top/gtlcutoacq.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.sweek.top/gtxgjkieeh.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.cheryme.top/gtprecgrxy.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.zhiwuduotai.top/gtjilxrxcm.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.yanxiufei.cn/gtampiuprz.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.shuidangran.top/gtplkzpnkv.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.hfpthk.cn/gtzmmbfuqz.html

C#:   Process.Start("ls", "-l");
来源：http://hz.yuanzhike.top/gtzkgitmud.html

[M04] 获取当前工作目录
来源：http://hz.haohaochexian.top/gttopiihil.html

Py:   os.getcwd()
来源：http://hz.sweek.top/gtgcqnmjxf.html

PHP:  getcwd();
来源：http://hz.jqgufenzy.top/gtiebdwrbi.html

JS:   process.cwd()
来源：http://hz.xziqi.cn/gtqhhzueew.html

TS:   process.cwd()
来源：http://hz.ybcxt.top/gtubvbibty.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.zhaomingkeji.xyz/gtgwihloyx.html

Go:   os.Getwd()
来源：http://hz.9152youxi.cn/gtjakiqchy.html

Ruby: Dir.pwd
来源：http://hz.shzxlz.cn/gtpbfwilwx.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.daria6918.cn/gtrnndfdml.html

[M05] 设置退出码
来源：http://hz.0kj1m.cn/gtevsmzgrg.html

Py:   sys.exit(1)
来源：http://hz.chenjidiqi.icu/gtngvcioyj.html

PHP:  exit(1);
来源：http://hz.xylfe.cn/gtqdqqinmh.html

JS:   process.exit(1)
来源：http://hz.zhaomingkeji.xyz/gtdxrzccmr.html

TS:   process.exit(1)
来源：http://hz.yj20258888.top/gtnrwcmhlu.html

Java: System.exit(1)
来源：http://hz.jiagoushi.top/gttzqctdne.html

Go:   os.Exit(1)
来源：http://hz.mhx1999.top/gtzewsomrf.html

Ruby: exit 1
来源：http://hz.zhiwuduotai.top/gtlsdrqzac.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.haohaochexian.top/gtviltgzgo.html

[M06] 向标准错误输出
来源：http://hz.hnxiangtu.top/gtszwsadot.html

Py:   print("err", file=sys.stderr)
来源：http://hz.meibo888.top/gthyphphlt.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.haohaochexian.top/gtfngruddd.html

JS:   console.error("err")
来源：http://hz.bjfxy.top/gtowkoeghe.html

TS:   console.error("err")
来源：http://hz.feifeiyinyue.top/gtarfebgxg.html

Java: System.err.println("err")
来源：http://hz.9152youxi.cn/gtoaxnatfn.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.cashguo.top/gtcxauiamf.html

Ruby: warn "err"
来源：http://hz.xziqi.cn/gttunzzims.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.ybcxt.top/gtovzlotwb.html

[M07] 判断是否为主入口
来源：http://hz.birdmap.top/gtmaiujadf.html

Py:   if __name__ == "__main__":
来源：http://hz.hongshengwenyu.top/gtkqczafrf.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.ppjwa.cn/gtflipeqjx.html

JS:   require.main === module
来源：http://hz.cucudq.cn/gtxaiejujt.html

TS:   require.main === module
来源：http://hz.xinyue.icu/gtssrabkhn.html

Java: public static void main(String[] args)
来源：http://hz.ehwqpu.com/gtvrbkmgqb.html

Go:   func main()
来源：http://hz.cucudq.cn/gtkhjsmvst.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.vqdsnc.cn/gtdngzpjfn.html

C#:   static void Main(string[] args)
来源：http://hz.zhijiandao.cn/gthaohmrmo.html

[M08] 获取系统与运行时信息
来源：http://hz.kuanghao11.cn/gtdvmsbskz.html

Py:   platform.system();  platform.python_version()
来源：http://hz.hnxiangtu.top/gthwawwtjx.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.dianchejie.cn/gtpzzcsijk.html

JS:   process.platform;  process.version
来源：http://hz.dianchejie.cn/gtebvvihqr.html

TS:   process.platform;  process.version
来源：http://hz.zycfv.cn/gtvakovlrw.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.zhaomingkeji.xyz/gtlegduftf.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.hnxiangtu.top/gtmtltjkny.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.guannengcc.top/gtoxvufdii.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.nanxinkj.top/gtgzudoojy.html

================================================================================
来源：http://hz.shzxlz.cn/gtaeonlbxi.html

N. 数据结构与算法
来源：http://hz.tanke756.top/gtsnmedwmk.html

================================================================================
来源：http://hz.cdnleiting.top/gteyypwhez.html

[N01] 二分查找（有序数组）
来源：http://hz.nanxuanxn.top/gtqbvfuxmr.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.pycfn.com/gtluhwzbuc.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.gogol.net.cn/gttwuocnem.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.wangdashe.top/gtyhrpxzpe.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.aizwys.cn/gtowmkuoge.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.yonumen.top/gtcqngngzl.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.cqqwz.cn/gtqxgorecx.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.9152youxi.cn/gthltharim.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.shanyushiyangkeji.top/gtkbgfspyg.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.snrcjt.cn/gtkusydzyj.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.zhaomingkeji.xyz/gtktbqnhsy.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.zhengqikj.top/gtdcjvqukv.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.svipenyu.cn/gtvycoruge.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.xingfuxueyuan.xyz/gtgsdpeget.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.xuanzx.com/gtxgbckpmx.html

Go:   slices.Sort(arr)
来源：http://hz.shuidangran.top/gtnbvlkkbd.html

Ruby: arr.sort
来源：http://hz.xylfe.cn/gtadaipnxi.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.xuetiantiany.cn/gturoszvfh.html

[N03] 快速排序（分治示例）
来源：http://hz.dianchejie.cn/gtnrauzlxy.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.guannengcc.top/gtdxpvylsr.html

PHP:  // 递归实现，或用 usort
来源：http://hz.yonumen.top/gtnhdncceq.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.nwbrower.top/gtoujtjmsh.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.wangshuangyany.cn/gtqrwvdjhp.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.wangdashe.top/gtizjpnrij.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.zhiwuduotai.top/gtvicolgva.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.chenzaomai.com/gtmnsxspce.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.smart0.xyz/gthtyymxgp.html

[N04] 斐波那契数列
来源：http://hz.zhijiandao.cn/gtoglpkfaj.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.pengpengdd.cyou/gtoniuadpt.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.guannengcc.top/gttxthegwx.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.zhoulong.xyz/gtgmhejnyb.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jyoumei.cn/gtnapcxziz.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.dashuyun.cn/gtaqvveuwk.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.zhijiandao.cn/gtqeffezxr.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.ivvv.top/gteiazfujj.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.xuanzx.com/gtpumwspeo.html

[N05] 最大公约数
来源：http://hz.yj20258888.top/gtpcnekhdy.html

Py:   math.gcd(a, b)
来源：http://hz.sxryk.cn/gtbneylojl.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.xingfuxueyuan.xyz/gtldfkdvvj.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.kuanghao11.cn/gtdkkwsvql.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yuxming.cn/gtlggisfgd.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.hysaishi.cn/gttckyyxah.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.shanyushiyangkeji.top/gtcljkljws.html

Ruby: a.gcd(b)
来源：http://hz.chenlongwang.top/gtpzxvecus.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.redwolf501.top/gtqnfhrucq.html

[N06] 判断回文字符串
来源：http://hz.hysaishi.cn/gtglpklwqj.html

Py:   s == s[::-1]
来源：http://hz.ppjwa.cn/gtphhhhkou.html

PHP:  $s === strrev($s);
来源：http://hz.yuxming.cn/gtjjdysczz.html

JS:   s === [...s].reverse().join("")
来源：http://hz.jqgfzy.top/gtydwhgdpv.html

TS:   s === [...s].reverse().join("")
来源：http://hz.nwbrower.top/gtmpwkgvog.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.ydzc1.top/gtnsagluvr.html

Go:   // 双指针从两端比较
来源：http://hz.shzxlz.cn/gthzlvcuxp.html

Ruby: s == s.reverse
来源：http://hz.hfpthk.cn/gticbimkqx.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.zhoulong.xyz/gtsqtwfjfq.html

[N07] 两数之和（返回下标）
来源：http://hz.zhixingplan.top/gtpeqlqxma.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.zhaomingkeji.xyz/gtadhbzicp.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.birdmap.top/gtyymwuncp.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.gotoacloud.top/gtbysmxnca.html

TS:   // 手写 Map<string, number>
来源：http://hz.jiagoushi.top/gtkjwhfjzb.html

Java: // 手写 HashMap
来源：http://hz.jlsjyb.cn/gturxrcamb.html

Go:   // 手写 map[int]int
来源：http://hz.c1oappe.top/gtvidwppcd.html

Ruby: // 手写 Hash
来源：http://hz.xylfe.cn/gtyyrnqxje.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.316326.xyz/gtiaodirie.html

[N08] 生成全排列
来源：http://hz.zhijiandao.cn/gthxftiggr.html

Py:   itertools.permutations(arr)
来源：http://hz.hnxiangtu.top/gthymgqgyv.html

PHP:  // 手写递归交换
来源：http://hz.gogol.net.cn/gtzneyzook.html

JS:   // 手写回溯递归
来源：http://hz.aizwys.cn/gtxxprzkfj.html

TS:   // 手写回溯递归
来源：http://hz.pycfn.com/gtdnswjntu.html

Java: // 手写回溯递归
来源：http://hz.jqgfzy.top/gtjdvhkyje.html

Go:   // 手写回溯递归
来源：http://hz.hnqzz.top/gtrtglllgw.html

Ruby: arr.permutation.to_a
来源：http://hz.cheryme.top/gtddrcarvu.html

C#:   // 手写回溯递归
来源：http://hz.hammf.cn/gtkkbikkwj.html

[N09] 栈与队列
来源：http://hz.jinqigfzy.top/gthbhsirec.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.birdmap.top/gtlyanpofo.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.nanxinkj.top/gthmsgbtyg.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.yuxming.cn/gthkaeaagu.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.zhongyouzk.top/gtogzeouoa.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.cashguo.top/gtvqvygevj.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.hfpthk.cn/gtsbenmhwr.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.hfpthk.cn/gtmvyxvonw.html


<!-- 参考信息 -->