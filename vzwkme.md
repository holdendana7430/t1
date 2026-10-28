代发 wailian999

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.tanke756.top/gtgkxgrbhz.html

Go:   json.Marshal(obj)
来源：http://hz.shuidangran.top/gtcclqrglr.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.redwolf501.top/gtmuosjbcy.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.kuanghao11.cn/gtujgpbleo.html

[K02] JSON 字符串转对象
来源：http://hz.svipenyu.cn/gtrykaezxb.html

Py:   json.loads(s)
来源：http://hz.wangdashe.top/gtfhuodpix.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.hnxiangtu.top/gtidqmnfup.html

JS:   JSON.parse(s)
来源：http://hz.guannengcc.top/gtpqrkprgc.html

TS:   JSON.parse(s)
来源：http://hz.jiagoushi.top/gthbkbdzfj.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.xylfe.cn/gtmxxzqtmx.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.snrcjt.cn/gtrhiyxujw.html

Ruby: JSON.parse(s)
来源：http://hz.aizwys.cn/gtishnjvgb.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.sxryk.cn/gtzfjkxwhw.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.tianlin.xyz/gtlhhbppuj.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.zycfv.cn/gtkpodsyii.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.9152youxi.cn/gtxspjxlkf.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.kuanghao11.cn/gtlwkzepyg.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.hnqzz.top/gtfggxdrpi.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.nwbrower.top/gtngxnentb.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.nanxuanxn.top/gtgxkxfcah.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.316326.xyz/gtqumabnic.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.yj202588.top/gtryfryxdx.html

[K04] 读取 JSON 文件
来源：http://hz.cheryme.top/gtxctzspkd.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.redwolf501.top/gthmrnhktr.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.xylfe.cn/gtdjkwmidw.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhengqikj.top/gtwpiljfdx.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.cucudq.cn/gtywzaypct.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.zhongyouzk.top/gtzaxwyjld.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.nanxinkj.top/gtbvxldfxb.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.xziqi.cn/gtrtipfuzn.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.fengsongda.top/gtawmyaamj.html

[K05] 深拷贝对象
来源：http://hz.yvedp.cn/gtqocytubj.html

Py:   copy.deepcopy(obj)
来源：http://hz.shzxlz.cn/gtcsiapmua.html

PHP:  unserialize(serialize($obj));
来源：http://hz.cqqwz.cn/gthzfqirei.html

JS:   structuredClone(obj)
来源：http://hz.mhx1999.top/gtzxlruwwe.html

TS:   structuredClone(obj)
来源：http://hz.aizwys.cn/gtccbmgvoa.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.ybcxt.top/gtygwkicmb.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.xylfe.cn/gtzllksuql.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.birdmap.top/gtovnborwl.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.xylfe.cn/gtucxzyfbn.html

[K06] 解析 URL 查询串
来源：http://hz.cdnleiting.top/gtjlsoktmb.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.kuanghao11.cn/gttsezvflk.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.yj20258.top/gtufmkeimg.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.shuidangran.top/gtdlqcytoa.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.nwbrower.top/gtpztjyxma.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.iojbl.cn/gtdjoabozt.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.0kj1m.cn/gtkkbjxkau.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.zdqjudy.top/gtkjpcbcct.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.pycfn.com/gttrsntwfj.html

[K07] 进制转换
来源：http://hz.hnqzz.top/gtbozmriah.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.chenlongwang.top/gtrutejfcn.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.guowangkeji.top/gtyoltvtrs.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.shuidangran.top/gtdatkqkzu.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.jqgufenzy.top/gtnbzmesxk.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.yj202588.top/gtraqslcov.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.sweek.top/gtlwkruktc.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.fengsongda.top/gtjifdeaud.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.nwbrower.top/gtulbnutlw.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.havefunace.top/gtbqjiwwag.html

Py:   pickle.dumps(obj)
来源：http://hz.pengpengdd.cyou/gtjzmbjlyx.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.hywenlv.cn/gtltirmzyn.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.bjfxy.top/gtculqnlbo.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.feifeiyinyue.top/gtsrlmzmjc.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.sysykeji.top/gtkmbiwyza.html

Go:   encoding/gob
来源：http://hz.yonumen.top/gtrpdlmlaa.html

Ruby: Marshal.dump(obj)
来源：http://hz.gotoacloud.top/gttgtmsjes.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.chenjidiqi.icu/gtcbackmpv.html

================================================================================
来源：http://hz.hnqzz.top/gtlfihyyzt.html

L. 网络请求
来源：http://hz.yongpay.top/gtkobptrzm.html

================================================================================
来源：http://hz.nwbrower.top/gtotzzbytw.html

[L01] 发送 GET 请求
来源：http://hz.gzhubu.top/gtditvwkys.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.jinghuilouyu.cn/gtrmwijatp.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.gotoacloud.top/gtoewgauti.html

JS:   await fetch(url)
来源：http://hz.yueranfly.top/gtvbrkhbzs.html

TS:   await fetch(url)
来源：http://hz.hongshengwenyu.top/gtbphhqmjo.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.pycfn.com/gtpnjwvwjj.html

Go:   resp, err := http.Get(url)
来源：http://hz.yueranfly.top/gtwancxtoi.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.cheryme.top/gtqsnwuelk.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.cqqwz.cn/gtjvzphbhp.html

[L02] 发送 POST JSON
来源：http://hz.feifeiyinyue.top/gtfftpcqkd.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.feifeiyinyue.top/gtmwlobeof.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.aibaodan.cn/gtqtxurijv.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.c1oappe.top/gtbxfmpvnu.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.havefunace.top/gtlccrndhx.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.bjfxy.top/gtadzzdopq.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.hfpthk.cn/gtlkjhjttn.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.yj20258.top/gtojwodgzw.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.hammf.cn/gtztfhciom.html

[L03] 设置自定义请求头
来源：http://hz.meibo888.top/gtkftxebno.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.redwolf501.top/gtsiqqfouk.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.ehwqpu.com/gtpezqhpmw.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.wangshuangyany.cn/gtmznpjxsw.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jianghu66.top/gtnunulhjh.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.ppjwa.cn/gtdevunhfz.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.yangfankeji.com/gtjdnjmkfe.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.aizwys.cn/gtwkcmafaw.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.yongpay.top/gtnbtyiveu.html

[L04] 设置超时
来源：http://hz.zhongyouzk.top/gtchccmyrl.html

Py:   requests.get(url, timeout=5)
来源：http://hz.pycfn.com/gtlyrirkru.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.hfpthk.cn/gtaatibseu.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.xziqi.cn/gtmibqtbgw.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.vqdsnc.cn/gtlyylltkp.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.jinghuilouyu.cn/gturqotuct.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.gaohongyu789.top/gtmbwvjydu.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.snrcjt.cn/gtiudxffbs.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.sxryk.cn/gtqqowgfrb.html

[L05] 上传文件（multipart）
来源：http://hz.daxiang520.top/gtkmqbbdsq.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.52xcode.cn/gtbkbhxknh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.cdnleiting.top/gtalmraxck.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.zhengqikj.top/gtnhiqchzw.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.shanyushiyangkeji.top/gtduegfwsh.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.fzhhl.top/gtxqwnolvw.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.yj202588.top/gtjweummey.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.ivvv.top/gtvxvsssef.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.cheryme.top/gtwgvgnhoo.html

[L06] 解析响应为 JSON
来源：http://hz.jinqigfzy.top/gtjpnxxhgd.html

Py:   resp.json()
来源：http://hz.xuanzx.com/gtkfapkoeo.html

PHP:  json_decode($body, true);
来源：http://hz.vqdsnc.cn/gtavdyqope.html

JS:   await resp.json()
来源：http://hz.yvedp.cn/gtpmrofovz.html

TS:   await resp.json()
来源：http://hz.jinyuanbaomall.cn/gtilpvydom.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.jyoumei.cn/gtzoshaops.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.yongpay.top/gtjqbqlndg.html

Ruby: JSON.parse(resp.body)
来源：http://hz.svipenyu.cn/gtdeaitplw.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.yj202588.top/gtypuyirog.html

[L07] 处理 HTTP 状态码
来源：http://hz.jqgufenzy.top/gtgikpdpim.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.yongpay.top/gtyxnznbve.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.jianghu66.top/gttqsvdggb.html

JS:   resp.ok;  resp.status
来源：http://hz.hnqzz.top/gtcuelpbvw.html

TS:   resp.ok;  resp.status
来源：http://hz.feifeiyinyue.top/gtryiwuacg.html

Java: resp.statusCode()
来源：http://hz.svipenyu.cn/gtakrvbmzi.html

Go:   resp.StatusCode
来源：http://hz.9152youxi.cn/gtouksrvkg.html

Ruby: resp.code.to_i
来源：http://hz.hongshengwenyu.top/gtbbsztecn.html

C#:   (int)resp.StatusCode
来源：http://hz.andypj.xyz/gtawpgvhjz.html

[L08] 并发请求多个地址
来源：http://hz.wangdashe.top/gtraatjhhq.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.jianghu66.top/gtxchtkmyt.html

PHP:  curl_multi_init() 系列
来源：http://hz.hysaishi.cn/gtzgyxkyfi.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.guannengcc.top/gtmbffczps.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.tanke756.top/gtxxjlyrdp.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.gotoacloud.top/gttuakklyz.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.snrcjt.cn/gtrxsbpmsy.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.nanxuanxn.top/gtkikvzetj.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.daxiang520.top/gtvdhznvpy.html

================================================================================
来源：http://hz.nanxinkj.top/gtnpbjvejd.html

M. 命令行 / 进程 / 环境
来源：http://hz.jianghu66.top/gtuhrtvymk.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtqhrilpdf.html

[M01] 读取命令行参数
来源：http://hz.yj20258.top/gtpqlwljzg.html

Py:   sys.argv[1:]
来源：http://hz.hnxiangtu.top/gtxlqgawgf.html

PHP:  $argv;  $argc;
来源：http://hz.yonumen.top/gtwcjriexq.html

JS:   process.argv.slice(2)
来源：http://hz.yuanzhike.top/gtxebwfavz.html

TS:   process.argv.slice(2)
来源：http://hz.sysykeji.top/gtrvbisxps.html

Java: args 数组（main 方法参数）
来源：http://hz.redwolf501.top/gtvrtykxtb.html

Go:   os.Args[1:]
来源：http://hz.jianghu66.top/gtzgqlohrj.html

Ruby: ARGV
来源：http://hz.svipenyu.cn/gthvafiqci.html

C#:   args 数组（Main 方法参数）
来源：http://hz.yongpay.top/gtzfnhghxr.html

[M02] 读取环境变量
来源：http://hz.chenlongwang.top/gtqjotqkuk.html

Py:   os.environ.get("HOME")
来源：http://hz.sxryk.cn/gtchpfhvmq.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.quarkkingdee.top/gtpejbwtzy.html

JS:   process.env.HOME
来源：http://hz.pycfn.com/gtghiqjnmy.html

TS:   process.env.HOME
来源：http://hz.jqgfzy.top/gtieeuwqiq.html

Java: System.getenv("HOME")
来源：http://hz.yj20258.top/gtjobsdisp.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.yueranfly.top/gtxiwfsisk.html

Ruby: ENV["HOME"]
来源：http://hz.ybcxt.top/gtszrxqyvh.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.birdmap.top/gtenscgdvt.html

[M03] 执行外部命令
来源：http://hz.jyoumei.cn/gtljpqakav.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.wangdashe.top/gtifndnxzb.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.zycfv.cn/gtrhxdvvgl.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.ivvv.top/gtjnuuqgfq.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.cqqwz.cn/gtrsccchws.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.feifeiyinyue.top/gtabglzjeh.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.yj202588.top/gtyjvkbipy.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.fzhhl.top/gtjboiltlh.html

C#:   Process.Start("ls", "-l");
来源：http://hz.yj20258888.top/gtszzwyuod.html

[M04] 获取当前工作目录
来源：http://hz.tian-w.cn/gtcbjtljwe.html

Py:   os.getcwd()
来源：http://hz.mhx1999.top/gttldnepuv.html

PHP:  getcwd();
来源：http://hz.zycfv.cn/gtxstmjwiv.html

JS:   process.cwd()
来源：http://hz.hongshengwenyu.top/gtpnqjcdxw.html

TS:   process.cwd()
来源：http://hz.hnxiangtu.top/gtfhxecbmb.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.tian-w.cn/gtdoeqcqph.html

Go:   os.Getwd()
来源：http://hz.tanke756.top/gttczvoltg.html

Ruby: Dir.pwd
来源：http://hz.pengpengdd.cyou/gttqfqxhis.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.yvedp.cn/gtxsmuezsu.html

[M05] 设置退出码
来源：http://hz.sufxvd.cn/gtuzqvqbvo.html

Py:   sys.exit(1)
来源：http://hz.xuetiantiany.cn/gtwgllcnwa.html

PHP:  exit(1);
来源：http://hz.zhiwuduotai.top/gtennebbbb.html

JS:   process.exit(1)
来源：http://hz.xylfe.cn/gtxdvltrgh.html

TS:   process.exit(1)
来源：http://hz.hnxiangtu.top/gtbrybmrig.html

Java: System.exit(1)
来源：http://hz.nanxuanxn.top/gtiuldgpcn.html

Go:   os.Exit(1)
来源：http://hz.jinqigufen.top/gthnqistzo.html

Ruby: exit 1
来源：http://hz.zhengqikj.top/gthvjnttpo.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.cdnleiting.top/gtwtpikxnf.html

[M06] 向标准错误输出
来源：http://hz.yongpay.top/gtsxchglbw.html

Py:   print("err", file=sys.stderr)
来源：http://hz.yuxming.cn/gtpezliafe.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.yonumen.top/gtdhnzilpw.html

JS:   console.error("err")
来源：http://hz.aibaodan.cn/gtoimptviz.html

TS:   console.error("err")
来源：http://hz.9152youxi.cn/gtwkojijyp.html

Java: System.err.println("err")
来源：http://hz.zhixingplan.top/gtzhszinig.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.shanyushiyangkeji.top/gtcchnqqig.html

Ruby: warn "err"
来源：http://hz.9152youxi.cn/gtkafigbel.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.yuanzhike.top/gtepfcdazv.html

[M07] 判断是否为主入口
来源：http://hz.shanyushiyangtech.top/gtljptrkpf.html

Py:   if __name__ == "__main__":
来源：http://hz.bjfxy.top/gtloxyvelj.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.zycfv.cn/gtaxxkjivr.html

JS:   require.main === module
来源：http://hz.chenzaomai.com/gtaaafaizp.html

TS:   require.main === module
来源：http://hz.wangdashe.top/gtmcbbhmhg.html

Java: public static void main(String[] args)
来源：http://hz.cashguo.top/gtnwcswwnj.html

Go:   func main()
来源：http://hz.zycfv.cn/gtoltqrwau.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.shanyushiyangkeji.top/gtwkmxggpo.html

C#:   static void Main(string[] args)
来源：http://hz.yongpay.top/gtjcdzmvst.html

[M08] 获取系统与运行时信息
来源：http://hz.gogol.net.cn/gtfxyznsfl.html

Py:   platform.system();  platform.python_version()
来源：http://hz.redwolf501.top/gtqlrgwtho.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.chenzaomai.com/gtkrcjfdgs.html

JS:   process.platform;  process.version
来源：http://hz.xuanzx.com/gtonxlajic.html

TS:   process.platform;  process.version
来源：http://hz.jyoumei.cn/gtaosefkkq.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.zdqjudy.top/gtstlwheoq.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.tianlin.xyz/gtgsqyqres.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.ppjwa.cn/gtayvklwqm.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.nwbrower.top/gtnajpkxhi.html

================================================================================
来源：http://hz.jyoumei.cn/gtogimrnpo.html

N. 数据结构与算法
来源：http://hz.dashuyun.cn/gtdvnpxyqh.html

================================================================================
来源：http://hz.zycfv.cn/gtbnjxlfkw.html

[N01] 二分查找（有序数组）
来源：http://hz.daria6918.cn/gtobegcthy.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.wangdashe.top/gtztzqsdmx.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.bjfxy.top/gthrkfbjeu.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.xuetiantiany.cn/gtrgaqzzcx.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.nanxinkj.top/gtirzniuxg.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.316326.xyz/gtptocmjvw.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.zhiwuduotai.top/gtcypavqzl.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.zycfv.cn/gtfwdztkzi.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.havefunace.top/gtumxdiyzo.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.hysaishi.cn/gtkslhezan.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.smart0.xyz/gtlgdkljqu.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.jqgfzy.top/gtneaiqxvq.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.hongshengwenyu.top/gtopktfdqn.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.daxiang520.top/gtslbegpui.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.xinyue.icu/gtvzrhiugs.html

Go:   slices.Sort(arr)
来源：http://hz.zhoulong.xyz/gtfkjxiukq.html

Ruby: arr.sort
来源：http://hz.yvedp.cn/gtggdqfmlj.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.feifeiyinyue.top/gtgwdfddah.html

[N03] 快速排序（分治示例）
来源：http://hz.hywenlv.cn/gtruzhbeog.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.zhoulong.xyz/gtrzdfsmih.html

PHP:  // 递归实现，或用 usort
来源：http://hz.cucudq.cn/gtkvreimrt.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yj202588.top/gtijadwvwm.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.feifeiyinyue.top/gtlzappskj.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.hammf.cn/gtfouatzat.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.pengpengdd.cyou/gtzmicjfhf.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.gzhubu.top/gtknoubcit.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.shuidangran.top/gtofclgwzo.html

[N04] 斐波那契数列
来源：http://hz.ybcxt.top/gtjimqpers.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.shzxlz.cn/gtophowmxk.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.guowangkeji.top/gtidtikeuz.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.nanxinkj.top/gtxaaswjfj.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.kuanghao11.cn/gtfvioxwvh.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.redwolf501.top/gtdowrhisv.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.hysaishi.cn/gtegtbchwa.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.yongpay.top/gtvmkpxlvb.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.ydzc1.top/gtqvcrfber.html

[N05] 最大公约数
来源：http://hz.cashguo.top/gtxhgrvarn.html

Py:   math.gcd(a, b)
来源：http://hz.gzhubu.top/gtehtjxdvy.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.gotoacloud.top/gtkdkjfnmi.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.guannengcc.top/gtutiidzbn.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.fzhhl.top/gtwxrknjxv.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.wangdashe.top/gtiplvtxna.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.316326.xyz/gtpuuyourt.html

Ruby: a.gcd(b)
来源：http://hz.haohaochexian.top/gtlhntzihk.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.yuanzhike.top/gtlsgxmfko.html

[N06] 判断回文字符串
来源：http://hz.sweek.top/gtoimsvegi.html

Py:   s == s[::-1]
来源：http://hz.zhengqikj.top/gtppacgipr.html

PHP:  $s === strrev($s);
来源：http://hz.andypj.xyz/gtwqnscxry.html

JS:   s === [...s].reverse().join("")
来源：http://hz.jiagoushi.top/gtduglxrbw.html

TS:   s === [...s].reverse().join("")
来源：http://hz.cqqwz.cn/gtpflibfxq.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.ywan-chungtsiang.top/gtirjzqnbw.html

Go:   // 双指针从两端比较
来源：http://hz.guowangkeji.top/gtoqjbngjn.html

Ruby: s == s.reverse
来源：http://hz.fzhhl.top/gtexnaporg.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.dianchejie.cn/gtujqfvjwd.html

[N07] 两数之和（返回下标）
来源：http://hz.sufxvd.cn/gtayhyciwp.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.jinyuanbaomall.cn/gthjnspczk.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.nwbrower.top/gtzsiahvic.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.gotoacloud.top/gtfndvmjnu.html

TS:   // 手写 Map<string, number>
来源：http://hz.ivvv.top/gtzcacwnau.html

Java: // 手写 HashMap
来源：http://hz.jyoumei.cn/gtjgpvtboz.html

Go:   // 手写 map[int]int
来源：http://hz.aibaodan.cn/gtzqzdqvwn.html

Ruby: // 手写 Hash
来源：http://hz.guannengcc.top/gttzofljpc.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.jianghu66.top/gtfankrckn.html

[N08] 生成全排列
来源：http://hz.fzhhl.top/gtesioldch.html

Py:   itertools.permutations(arr)
来源：http://hz.wangshuangyany.cn/gtnmgqctjg.html

PHP:  // 手写递归交换
来源：http://hz.daria6918.cn/gtwvyawylx.html

JS:   // 手写回溯递归
来源：http://hz.yj20258888.top/gtccnfvbew.html

TS:   // 手写回溯递归
来源：http://hz.guannengcc.top/gtmxpaddes.html

Java: // 手写回溯递归
来源：http://hz.hnqzz.top/gtjuwrxbus.html

Go:   // 手写回溯递归
来源：http://hz.zhiwuduotai.top/gtcqyhsjxn.html

Ruby: arr.permutation.to_a
来源：http://hz.tanke756.top/gtgjdchnfl.html

C#:   // 手写回溯递归
来源：http://hz.svipenyu.cn/gtkfztxsty.html

[N09] 栈与队列
来源：http://hz.mhx1999.top/gtgrvlgbhu.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.hnxiangtu.top/gtdzownhul.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.cqqwz.cn/gtavwzstnb.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.c1oappe.top/gtzsyfjlnk.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.yj20258888.top/gtjdwosobn.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.yj202588.top/gtopyzaehv.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.c1oappe.top/gtnbhqglsn.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.jqgfzy.top/gtbzrifzjj.html


<!-- 参考信息 -->