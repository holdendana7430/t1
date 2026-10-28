代发 wailian999

[K02] JSON 字符串转对象
来源：http://hz.tian-w.cn/gtfxrfkzgb.html

Py:   json.loads(s)
来源：http://hz.haohaochexian.top/gtjnrgojlj.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.yj20258888.top/gtjevbxgcf.html

JS:   JSON.parse(s)
来源：http://hz.sufxvd.cn/gtdosklxnp.html

TS:   JSON.parse(s)
来源：http://hz.cdnleiting.top/gtrvorvcih.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.gogol.net.cn/gtmadybaja.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.hnxiangtu.top/gtzrhstwwy.html

Ruby: JSON.parse(s)
来源：http://hz.hywenlv.cn/gthhyygtvz.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.andypj.xyz/gtdmcaxkzg.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.jianghu66.top/gtbeqcmzub.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.yonumen.top/gtuypniizw.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.zhongyouzk.top/gtgbpbfzff.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.ybcxt.top/gtkmzdixbq.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.chenlongwang.top/gttqkyzktd.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.jinqigufen.top/gtwbnjngul.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.sufxvd.cn/gtyuizxoiw.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.vqdsnc.cn/gtbuhmosbb.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.zhaomingkeji.xyz/gtmkkvejjb.html

[K04] 读取 JSON 文件
来源：http://hz.chenjidiqi.icu/gtsaadqgbq.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.meibo888.top/gttloalpiw.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.shzxlz.cn/gtczcvyjot.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.9152youxi.cn/gtxsuhnhqg.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.0kj1m.cn/gtktrokxkd.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.c1oappe.top/gtouklflbm.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.snrcjt.cn/gtfsrwomqt.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.cheryme.top/gtckslighb.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.yj20258.top/gtrevwxjbc.html

[K05] 深拷贝对象
来源：http://hz.jianghu66.top/gttvoopjfi.html

Py:   copy.deepcopy(obj)
来源：http://hz.nanxuanxn.top/gtnpayncjt.html

PHP:  unserialize(serialize($obj));
来源：http://hz.meibo888.top/gtnoedwtjv.html

JS:   structuredClone(obj)
来源：http://hz.jiagoushi.top/gtytpxohjs.html

TS:   structuredClone(obj)
来源：http://hz.guowangkeji.top/gtwohjaqdz.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.zhaomingkeji.xyz/gtjfjoqbvs.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.jqgfzy.top/gtmwxniltx.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.yj202588.top/gtuuayyxuj.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.hammf.cn/gtglwgwdrs.html

[K06] 解析 URL 查询串
来源：http://hz.zdqjudy.top/gtjnvvcjbl.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.hysaishi.cn/gtmxiqyppr.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.yangfankeji.com/gtjobsmylt.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.shangyingyoupin.top/gtomkkfquu.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.wangdashe.top/gtaixepqzz.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.zhixingplan.top/gtjvqkoris.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.cheryme.top/gtdeyzfvfe.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.quarkkingdee.top/gtoypuizyf.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.ybcxt.top/gtozcmyhvp.html

[K07] 进制转换
来源：http://hz.guowangkeji.top/gtcmxecqja.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.shanyushiyangtech.top/gtkommgata.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.chenjidiqi.icu/gtfupsfojf.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.wangdashe.top/gtldemlfow.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.xziqi.cn/gtalxpmwap.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.jinyuanbaomall.cn/gtyroanefy.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.zhengqikj.top/gtjcrqdjuk.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.yongpay.top/gtxghxtpvb.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.smart0.xyz/gtkybnqipe.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.smart0.xyz/gterbjjsuh.html

Py:   pickle.dumps(obj)
来源：http://hz.zdqjudy.top/gtrcislsql.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.vqdsnc.cn/gtkfuimoyj.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.havefunace.top/gttcczkmei.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.hnqzz.top/gtauoidmlh.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.dashuyun.cn/gtmaqjgdfi.html

Go:   encoding/gob
来源：http://hz.yanxiufei.cn/gtmwifpfdv.html

Ruby: Marshal.dump(obj)
来源：http://hz.hnqzz.top/gtxwskeyyd.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.jinqigfzy.top/gttacnkixz.html

================================================================================
来源：http://hz.jinqigfzy.top/gtcozulexs.html

L. 网络请求
来源：http://hz.gotoacloud.top/gtbwiaoebh.html

================================================================================
来源：http://hz.havefunace.top/gtjojqofnt.html

[L01] 发送 GET 请求
来源：http://hz.kuanghao11.cn/gtjkafrxbs.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.aizwys.cn/gtvflnmxsg.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.0kj1m.cn/gtzavxsfww.html

JS:   await fetch(url)
来源：http://hz.gaohongyu789.top/gtqrqylyge.html

TS:   await fetch(url)
来源：http://hz.cucudq.cn/gtnchksamc.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.vqdsnc.cn/gtqfyyefpq.html

Go:   resp, err := http.Get(url)
来源：http://hz.mhx1999.top/gttbzpefbp.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.guowangkeji.top/gtsunuvuto.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.hongshengwenyu.top/gtmevkplsb.html

[L02] 发送 POST JSON
来源：http://hz.gzhubu.top/gtbbpkrsuk.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.hysaishi.cn/gtybsslbom.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.vqdsnc.cn/gttbjecdgk.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.vqdsnc.cn/gtxynuqixf.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.gotoacloud.top/gtjhxilpkr.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.yanxiufei.cn/gtlfuxlgae.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.xinyue.icu/gtkuazplwq.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.svipenyu.cn/gtocnvabhr.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.tanke756.top/gtenyuopuc.html

[L03] 设置自定义请求头
来源：http://hz.cucudq.cn/gtrdramobr.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.xinyue.icu/gtncmljnfw.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.xuanzx.com/gtqgnkexfn.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.wangdashe.top/gthfyrkcar.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.xylfe.cn/gtmaojecph.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.cucudq.cn/gtpsrrdxsr.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.meibo888.top/gteutywjdo.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.shanyushiyangkeji.top/gtgxqsdeqz.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.jiagoushi.top/gtulbeaulw.html

[L04] 设置超时
来源：http://hz.dianchejie.cn/gtymlucdiq.html

Py:   requests.get(url, timeout=5)
来源：http://hz.svipenyu.cn/gtyyabzzhb.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.havefunace.top/gtaoggekvz.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.ydjk.org.cn/gtdpoyysem.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.wangshuangyany.cn/gtejmnxsll.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.dashuyun.cn/gtcetzuwdg.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.jinyuanbaomall.cn/gtiioncpuy.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.zhengqikj.top/gtekrpgxuw.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.jlsjyb.cn/gtpopwusui.html

[L05] 上传文件（multipart）
来源：http://hz.dianchejie.cn/gtshdkbahk.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.jianghu66.top/gtrinwbocp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.zhongyouzk.top/gtjgdqyhal.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.dashuyun.cn/gtrftmawem.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.smart0.xyz/gttwodojyn.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.birdmap.top/gtbhgfvwkq.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.cqqwz.cn/gtyjbnyftf.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.hongshengwenyu.top/gtyslvgyuv.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.zdqjudy.top/gteqwudmej.html

[L06] 解析响应为 JSON
来源：http://hz.chenlongwang.top/gtmtjivwit.html

Py:   resp.json()
来源：http://hz.zycfv.cn/gtvhmltcyf.html

PHP:  json_decode($body, true);
来源：http://hz.daria6918.cn/gtvdjhqsur.html

JS:   await resp.json()
来源：http://hz.xuanzx.com/gteprksdtd.html

TS:   await resp.json()
来源：http://hz.cheryme.top/gtqqyeqahf.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.zhongyouzk.top/gtgzocustn.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.chenjidiqi.icu/gtvzxicppo.html

Ruby: JSON.parse(resp.body)
来源：http://hz.shzxlz.cn/gtoikxgchu.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.shuidangran.top/gtysorzbsv.html

[L07] 处理 HTTP 状态码
来源：http://hz.dashuyun.cn/gtouvnqjwa.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.shanyushiyangkeji.top/gtjhspispg.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.yvedp.cn/gtkosxcbyu.html

JS:   resp.ok;  resp.status
来源：http://hz.52xcode.cn/gtnzlfzocb.html

TS:   resp.ok;  resp.status
来源：http://hz.bjfxy.top/gtpmqmglmm.html

Java: resp.statusCode()
来源：http://hz.pengpengdd.cyou/gtnojjcygg.html

Go:   resp.StatusCode
来源：http://hz.yongpay.top/gtekahrckh.html

Ruby: resp.code.to_i
来源：http://hz.chenzaomai.com/gtfvmutziw.html

C#:   (int)resp.StatusCode
来源：http://hz.guannengcc.top/gtzoqbfhmr.html

[L08] 并发请求多个地址
来源：http://hz.zhengqikj.top/gtwpkupwuu.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.daria6918.cn/gtbmhmsbii.html

PHP:  curl_multi_init() 系列
来源：http://hz.vqdsnc.cn/gtlgvahytv.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yongpay.top/gtdwpagpak.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.gogol.net.cn/gtizgjwujx.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.sxryk.cn/gtnsjitlhq.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.yueranfly.top/gtlgtocrqu.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.xuetiantiany.cn/gtftdpoonp.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.xinyue.icu/gtqrgiqikk.html

================================================================================
来源：http://hz.zdqjudy.top/gtczioafxu.html

M. 命令行 / 进程 / 环境
来源：http://hz.redwolf501.top/gtulklypsd.html

================================================================================
来源：http://hz.0kj1m.cn/gtriplclef.html

[M01] 读取命令行参数
来源：http://hz.0kj1m.cn/gtdclahvfu.html

Py:   sys.argv[1:]
来源：http://hz.birdmap.top/gtcjloyazg.html

PHP:  $argv;  $argc;
来源：http://hz.aibaodan.cn/gtxzmdluec.html

JS:   process.argv.slice(2)
来源：http://hz.birdmap.top/gtfmxayavc.html

TS:   process.argv.slice(2)
来源：http://hz.zycfv.cn/gtiezatqwl.html

Java: args 数组（main 方法参数）
来源：http://hz.jinqigufen.top/gtqfkcbidy.html

Go:   os.Args[1:]
来源：http://hz.dashuyun.cn/gtfeywwdjv.html

Ruby: ARGV
来源：http://hz.hongshengwenyu.top/gtorfzncqv.html

C#:   args 数组（Main 方法参数）
来源：http://hz.yuxming.cn/gtqczjeaft.html

[M02] 读取环境变量
来源：http://hz.jqgufenzy.top/gtaefimnay.html

Py:   os.environ.get("HOME")
来源：http://hz.ehwqpu.com/gtkrvzyjkh.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.jqgufenzy.top/gtthqtbsli.html

JS:   process.env.HOME
来源：http://hz.sufxvd.cn/gtzydenqwh.html

TS:   process.env.HOME
来源：http://hz.pengpengdd.cyou/gtjyzmjlyp.html

Java: System.getenv("HOME")
来源：http://hz.dashuyun.cn/gtmdfvjbda.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.zhongyouzk.top/gtsczsrpnh.html

Ruby: ENV["HOME"]
来源：http://hz.wangshuangyany.cn/gtafeplfir.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.xuanzx.com/gtbonkyqyi.html

[M03] 执行外部命令
来源：http://hz.andypj.xyz/gthavoqhra.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.hongshengwenyu.top/gtepujepwi.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.feifeiyinyue.top/gtleoccatg.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.jqgufenzy.top/gtvirqdmjs.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.yj20258.top/gtlbzfyoyj.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.tian-w.cn/gtupmgidru.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.nwbrower.top/gticbgqwng.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.yonumen.top/gtabkbonry.html

C#:   Process.Start("ls", "-l");
来源：http://hz.yuxming.cn/gtgubtoouo.html

[M04] 获取当前工作目录
来源：http://hz.fzhhl.top/gtigrnrumg.html

Py:   os.getcwd()
来源：http://hz.hfpthk.cn/gtsfjtspux.html

PHP:  getcwd();
来源：http://hz.hnxiangtu.top/gtlllwyptd.html

JS:   process.cwd()
来源：http://hz.zhongyouzk.top/gtrqdulazg.html

TS:   process.cwd()
来源：http://hz.zdqjudy.top/gttmxfomjp.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.ywan-chungtsiang.top/gtarzqlhhz.html

Go:   os.Getwd()
来源：http://hz.0kj1m.cn/gtvpopavcq.html

Ruby: Dir.pwd
来源：http://hz.gogol.net.cn/gtasppbtmv.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.yj202588.top/gtyzuqwirg.html

[M05] 设置退出码
来源：http://hz.gzhubu.top/gtpcfryila.html

Py:   sys.exit(1)
来源：http://hz.jinghuilouyu.cn/gthbhjxpph.html

PHP:  exit(1);
来源：http://hz.jlsjyb.cn/gtexarcmxq.html

JS:   process.exit(1)
来源：http://hz.daria6918.cn/gtbfzmltry.html

TS:   process.exit(1)
来源：http://hz.shanyushiyangtech.top/gtlpdxwvzo.html

Java: System.exit(1)
来源：http://hz.jqgfzy.top/gtvaremlap.html

Go:   os.Exit(1)
来源：http://hz.quarkkingdee.top/gthmwbenjz.html

Ruby: exit 1
来源：http://hz.pycfn.com/gtdbktoclj.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.guowangkeji.top/gtmuacotoq.html

[M06] 向标准错误输出
来源：http://hz.hongshengwenyu.top/gtwvhjkvmv.html

Py:   print("err", file=sys.stderr)
来源：http://hz.aibaodan.cn/gtskkrlwit.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.nwbrower.top/gtfjzmrfbk.html

JS:   console.error("err")
来源：http://hz.zhiwuduotai.top/gtbskabkhq.html

TS:   console.error("err")
来源：http://hz.hfpthk.cn/gthtpzthaw.html

Java: System.err.println("err")
来源：http://hz.shanyushiyangtech.top/gtllhnxvzv.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.jqgfzy.top/gtxdecxbpo.html

Ruby: warn "err"
来源：http://hz.c1oappe.top/gtpiicphsp.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.shangyingyoupin.top/gtufvgenst.html

[M07] 判断是否为主入口
来源：http://hz.svipenyu.cn/gtncblgcua.html

Py:   if __name__ == "__main__":
来源：http://hz.gotoacloud.top/gtyfsztamg.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.nanxinkj.top/gtduzulgry.html

JS:   require.main === module
来源：http://hz.zdqjudy.top/gtgvzaadih.html

TS:   require.main === module
来源：http://hz.xingfuxueyuan.xyz/gthwkdrzmh.html

Java: public static void main(String[] args)
来源：http://hz.ybcxt.top/gtgsgkmsup.html

Go:   func main()
来源：http://hz.ydzc1.top/gtkeoitrmo.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.andypj.xyz/gtfkebbast.html

C#:   static void Main(string[] args)
来源：http://hz.yueranfly.top/gthyxggxbn.html

[M08] 获取系统与运行时信息
来源：http://hz.pengpengdd.cyou/gtfcemhqna.html

Py:   platform.system();  platform.python_version()
来源：http://hz.shanyushiyangtech.top/gtyxbanppb.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.snrcjt.cn/gtnbwmlmps.html

JS:   process.platform;  process.version
来源：http://hz.fzhhl.top/gtqmymlqju.html

TS:   process.platform;  process.version
来源：http://hz.316326.xyz/gtyctpuwfz.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.jlsjyb.cn/gtylphrjte.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.jianghu66.top/gtenuffqdi.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.hammf.cn/gtaejvnail.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.shanyushiyangkeji.top/gtmidzeqkm.html

================================================================================
来源：http://hz.gotoacloud.top/gtfigtwotz.html

N. 数据结构与算法
来源：http://hz.yj20258.top/gtnitqqynf.html

================================================================================
来源：http://hz.fzhhl.top/gtbbekpjkm.html

[N01] 二分查找（有序数组）
来源：http://hz.zhixingplan.top/gtdvhbhzgb.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.andypj.xyz/gtzsnesnaa.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.ivvv.top/gtdcaufufe.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.0kj1m.cn/gtxmzkxxjd.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.dashuyun.cn/gtagoanlgr.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.gotoacloud.top/gtuxneoern.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.xziqi.cn/gtgcnodfvb.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.kuanghao11.cn/gtqgwqmsbz.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.zhongyouzk.top/gtngcmnakw.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.hysaishi.cn/gtljdueouh.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.shangyingyoupin.top/gturmtvruf.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.cheryme.top/gtxicpmech.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jinqigufen.top/gtiofjumeb.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.haohaochexian.top/gtxmkgyauk.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.jlsjyb.cn/gtdctboapv.html

Go:   slices.Sort(arr)
来源：http://hz.chenlongwang.top/gtcjpwjtzy.html

Ruby: arr.sort
来源：http://hz.redwolf501.top/gtellpjqxe.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.pycfn.com/gtlqxvhgum.html

[N03] 快速排序（分治示例）
来源：http://hz.quarkkingdee.top/gtzkqmiywc.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.jianghu66.top/gthlwofzbj.html

PHP:  // 递归实现，或用 usort
来源：http://hz.hnqzz.top/gtjirkmmwd.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.redwolf501.top/gthksptkro.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zhijiandao.cn/gtnfjjdrre.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.hysaishi.cn/gtogmubkxw.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.yj20258888.top/gtofhqzkbe.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.dashuyun.cn/gtjlpiyzca.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.tianlin.xyz/gtvtzawowx.html

[N04] 斐波那契数列
来源：http://hz.shzxlz.cn/gtodixinni.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.smart0.xyz/gtylpuvndq.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.smart0.xyz/gtipikkkwn.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.kuanghao11.cn/gttetrpmya.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.9152youxi.cn/gtevaqoprd.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.jiagoushi.top/gtepgcxgel.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.pengpengdd.cyou/gtvtqbxxib.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.xingfuxueyuan.xyz/gthdysvcsj.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.tian-w.cn/gtfbhjkpzw.html

[N05] 最大公约数
来源：http://hz.zhengqikj.top/gtsqpwqayw.html

Py:   math.gcd(a, b)
来源：http://hz.andypj.xyz/gtfmcxkwvw.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.fzhhl.top/gtsdsoqcju.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.havefunace.top/gtyeynyupj.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.gogol.net.cn/gtsdyawmev.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.tianlin.xyz/gtwkrhriya.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.gogol.net.cn/gtuomchkuh.html

Ruby: a.gcd(b)
来源：http://hz.cdnleiting.top/gtcyjepovq.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.ywan-chungtsiang.top/gtkwvniuvg.html

[N06] 判断回文字符串
来源：http://hz.zdqjudy.top/gtaguhbxms.html

Py:   s == s[::-1]
来源：http://hz.chenjidiqi.icu/gtrmqtyztu.html

PHP:  $s === strrev($s);
来源：http://hz.ppjwa.cn/gtnaupojlq.html

JS:   s === [...s].reverse().join("")
来源：http://hz.ywan-chungtsiang.top/gtqspmzoim.html

TS:   s === [...s].reverse().join("")
来源：http://hz.zhengqikj.top/gtqkfmvrdq.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.gaohongyu789.top/gtaxwwzxzx.html

Go:   // 双指针从两端比较
来源：http://hz.xuanzx.com/gttvikvijx.html

Ruby: s == s.reverse
来源：http://hz.cheryme.top/gtyuntryyi.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.xziqi.cn/gttehblklq.html

[N07] 两数之和（返回下标）
来源：http://hz.jyoumei.cn/gtidxrptns.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.aibaodan.cn/gtlztbmrih.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.wangdashe.top/gtbwmwwwsa.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.52xcode.cn/gtizltqees.html

TS:   // 手写 Map<string, number>
来源：http://hz.hfpthk.cn/gtunrezolf.html

Java: // 手写 HashMap
来源：http://hz.shanyushiyangkeji.top/gtruxmzhlj.html

Go:   // 手写 map[int]int
来源：http://hz.zdqjudy.top/gtynyantcg.html

Ruby: // 手写 Hash
来源：http://hz.tian-w.cn/gtqheuneqy.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.chenlongwang.top/gtjrkwpdcs.html

[N08] 生成全排列
来源：http://hz.xingfuxueyuan.xyz/gtriddtnft.html

Py:   itertools.permutations(arr)
来源：http://hz.guannengcc.top/gtzizomqoy.html

PHP:  // 手写递归交换
来源：http://hz.birdmap.top/gtvjwjfrbu.html

JS:   // 手写回溯递归
来源：http://hz.yj20258.top/gtcwunmnkd.html

TS:   // 手写回溯递归
来源：http://hz.shanyushiyangtech.top/gtkzkajfdc.html

Java: // 手写回溯递归
来源：http://hz.svipenyu.cn/gtvpmvbizg.html

Go:   // 手写回溯递归
来源：http://hz.hongshengwenyu.top/gthuabligr.html

Ruby: arr.permutation.to_a
来源：http://hz.pengpengdd.cyou/gtenhtrhrn.html

C#:   // 手写回溯递归
来源：http://hz.jinqigfzy.top/gtcndnzfvl.html

[N09] 栈与队列
来源：http://hz.yonumen.top/gtxiwfgdnf.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.daria6918.cn/gtxhqckxaw.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.ybcxt.top/gtlgmrhxft.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.ywan-chungtsiang.top/gtzjtflofw.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.gzhubu.top/gtusbodepr.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.sweek.top/gtmbaahuwi.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.shangyingyoupin.top/gtxbvmfnxd.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.bjfxy.top/gtvwtzrjbu.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.ehwqpu.com/gtaixcmsdm.html

[N10] 链表节点定义
来源：http://hz.yuxming.cn/gtqkqoqaxw.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.nanxinkj.top/gtlgezisqg.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.dianchejie.cn/gtpbhizoqe.html


<!-- 参考信息 -->