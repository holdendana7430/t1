代发 wailian999

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.zhiwuduotai.top/gtapzcduvl.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.feifeiyinyue.top/gtsdwqldjj.html

JS:   JSON.stringify(obj)
来源：http://hz.zhixingplan.top/gtxvanqvia.html

TS:   JSON.stringify(obj)
来源：http://hz.nanxinkj.top/gtvohvcubs.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.hongshengwenyu.top/gtubumyang.html

Go:   json.Marshal(obj)
来源：http://hz.yueranfly.top/gtvtlnwfmz.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.jlsjyb.cn/gtgagxwfba.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.shanyushiyangkeji.top/gtkrkubppz.html

[K02] JSON 字符串转对象
来源：http://hz.ivvv.top/gtvgkecbac.html

Py:   json.loads(s)
来源：http://hz.tanke756.top/gtydybtenk.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.9152youxi.cn/gtycwoueco.html

JS:   JSON.parse(s)
来源：http://hz.kuanghao11.cn/gtedkjuhju.html

TS:   JSON.parse(s)
来源：http://hz.gogol.net.cn/gtcjqchihc.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.sysykeji.top/gtcrmoleyn.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.hnqzz.top/gtdxjjwppp.html

Ruby: JSON.parse(s)
来源：http://hz.havefunace.top/gtowkmsfsb.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.gotoacloud.top/gtmacjhvpt.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.hnxiangtu.top/gtejbbrbct.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.aizwys.cn/gtiacuxmev.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.316326.xyz/gtfzwpllqo.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.ybcxt.top/gtqfzbfzij.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.quarkkingdee.top/gtcnqvanck.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.gogol.net.cn/gtncuhzzzy.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.shanyushiyangkeji.top/gtpachxsxy.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.jinqigufen.top/gtpbajgesu.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.gogol.net.cn/gtibgckdgz.html

[K04] 读取 JSON 文件
来源：http://hz.hfpthk.cn/gtneopirdc.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.shanyushiyangtech.top/gtzxszjsge.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.aibaodan.cn/gtensgjeel.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.hammf.cn/gtanllzupn.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.cashguo.top/gtmygqtbav.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.feifeiyinyue.top/gtcrrourph.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.jinghuilouyu.cn/gtpjdnydjf.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.feifeiyinyue.top/gtxwllqrrn.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.dashuyun.cn/gttmbfemkx.html

[K05] 深拷贝对象
来源：http://hz.jinqigufen.top/gtfwnxjext.html

Py:   copy.deepcopy(obj)
来源：http://hz.sysykeji.top/gtooatjorn.html

PHP:  unserialize(serialize($obj));
来源：http://hz.yuanzhike.top/gtohlsplxh.html

JS:   structuredClone(obj)
来源：http://hz.redwolf501.top/gtlodvmhvi.html

TS:   structuredClone(obj)
来源：http://hz.ywan-chungtsiang.top/gtstwargri.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.birdmap.top/gtjfizmtsu.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.jinqigfzy.top/gtvcmynsxc.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.ybcxt.top/gtaublmawd.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.jqgfzy.top/gthgjmrtpp.html

[K06] 解析 URL 查询串
来源：http://hz.jinyuanbaomall.cn/gtxglganhl.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.ydzc1.top/gtjwsnpdiq.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.zhijiandao.cn/gtguppjbou.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jiagoushi.top/gtycpxtmia.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jianghu66.top/gtolpggywt.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.xingfuxueyuan.xyz/gtdenkpfgy.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.zhengqikj.top/gtrzvjwums.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.haohaochexian.top/gtarvwlhji.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.cdnleiting.top/gtbptycggu.html

[K07] 进制转换
来源：http://hz.chenzaomai.com/gtyidmnysm.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.c1oappe.top/gtttfgqkhx.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.hongshengwenyu.top/gtqmrwmmhq.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.chenlongwang.top/gtlkibrdsx.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.ywan-chungtsiang.top/gtfjjrwoyh.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.ydzc1.top/gtmsqixhxm.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.aibaodan.cn/gtoljqcyys.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.tianlin.xyz/gtlltnbwio.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.yj20258.top/gtwnsqbusn.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.guannengcc.top/gtitqizvhj.html

Py:   pickle.dumps(obj)
来源：http://hz.fzhhl.top/gtvgabjpby.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.jinyuanbaomall.cn/gtaxttaqhx.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.meibo888.top/gtwsysonlq.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.316326.xyz/gtougbxaqt.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.yj20258888.top/gtdfegesxg.html

Go:   encoding/gob
来源：http://hz.zdqjudy.top/gtcnjdpbom.html

Ruby: Marshal.dump(obj)
来源：http://hz.9152youxi.cn/gtskmqerbv.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.snrcjt.cn/gtnuofoahq.html

================================================================================
来源：http://hz.aizwys.cn/gtpyxrnkya.html

L. 网络请求
来源：http://hz.yangfankeji.com/gtnqlvxdbj.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtpivmhyna.html

[L01] 发送 GET 请求
来源：http://hz.aizwys.cn/gtspnamcba.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.fzhhl.top/gtrrohhxfg.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.chenlongwang.top/gtwvimxzou.html

JS:   await fetch(url)
来源：http://hz.pycfn.com/gtdsaxhijd.html

TS:   await fetch(url)
来源：http://hz.nanxinkj.top/gtcbloewnq.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.tian-w.cn/gtzphhgwgp.html

Go:   resp, err := http.Get(url)
来源：http://hz.birdmap.top/gtlmfddjhr.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.gaohongyu789.top/gtifwuhdhw.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.xinyue.icu/gtantijkcc.html

[L02] 发送 POST JSON
来源：http://hz.meibo888.top/gtusostari.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.andypj.xyz/gtwweofvbe.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.kuanghao11.cn/gtalzhauyn.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.hammf.cn/gtmxepkinz.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jianghu66.top/gtenhpcdmr.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.haohaochexian.top/gtsswdmoxp.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.sysykeji.top/gtdhhazued.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.hnxiangtu.top/gtvbsgxzjp.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.aizwys.cn/gthgcnsdsc.html

[L03] 设置自定义请求头
来源：http://hz.cqqwz.cn/gtlqinntlw.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.yj202588.top/gtdnkxzrac.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.jinqigfzy.top/gttlmqtdsl.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zhengqikj.top/gthtvonzim.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.nwbrower.top/gtqkoybsvz.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.daxiang520.top/gtytbkoxhq.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.hnxiangtu.top/gtiwiuklya.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.feifeiyinyue.top/gtjjgdudlu.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.vqdsnc.cn/gtizqdfjnb.html

[L04] 设置超时
来源：http://hz.yuanzhike.top/gtjwaxendr.html

Py:   requests.get(url, timeout=5)
来源：http://hz.hnxiangtu.top/gtuzfkrfuy.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.tanke756.top/gtmvaexgid.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.daria6918.cn/gtgtufsqjk.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jqgfzy.top/gtznkxkwcn.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.xziqi.cn/gtidoviuuy.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.hnqzz.top/gtltbtigbp.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.yvedp.cn/gtjxixhlil.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.pycfn.com/gtvirzclwl.html

[L05] 上传文件（multipart）
来源：http://hz.jinghuilouyu.cn/gtexzdcrhw.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.c1oappe.top/gtkstntapz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.52xcode.cn/gtmzdwcxdf.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.gotoacloud.top/gtloigwimx.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.gogol.net.cn/gtspqdgusd.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.ivvv.top/gtdpmxevbn.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.zhoulong.xyz/gtqpbkcedr.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.tanke756.top/gtqcdllpoz.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.yongpay.top/gtgebahbzc.html

[L06] 解析响应为 JSON
来源：http://hz.jlsjyb.cn/gteosamzsd.html

Py:   resp.json()
来源：http://hz.hysaishi.cn/gtivbwfzlc.html

PHP:  json_decode($body, true);
来源：http://hz.xziqi.cn/gtybvwxalp.html

JS:   await resp.json()
来源：http://hz.bjfxy.top/gtksjfrhif.html

TS:   await resp.json()
来源：http://hz.zhengqikj.top/gtznftwyto.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.ehwqpu.com/gtjpznltmk.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.birdmap.top/gtwjftswmy.html

Ruby: JSON.parse(resp.body)
来源：http://hz.sweek.top/gttekulklq.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.ivvv.top/gtafgklmxc.html

[L07] 处理 HTTP 状态码
来源：http://hz.9152youxi.cn/gtisqghjel.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.gzhubu.top/gtfbsgfrts.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.vqdsnc.cn/gtadwrvrzi.html

JS:   resp.ok;  resp.status
来源：http://hz.cdnleiting.top/gtcjpmijwe.html

TS:   resp.ok;  resp.status
来源：http://hz.yuanzhike.top/gtxsxztmto.html

Java: resp.statusCode()
来源：http://hz.cqqwz.cn/gtgxhhcftk.html

Go:   resp.StatusCode
来源：http://hz.ehwqpu.com/gtoucnmuzr.html

Ruby: resp.code.to_i
来源：http://hz.316326.xyz/gtsuavdsiq.html

C#:   (int)resp.StatusCode
来源：http://hz.zhongyouzk.top/gtfdvnmtoq.html

[L08] 并发请求多个地址
来源：http://hz.316326.xyz/gtryylgmhv.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.chenzaomai.com/gtmujbrsxv.html

PHP:  curl_multi_init() 系列
来源：http://hz.cdnleiting.top/gtxrgxcqgc.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.316326.xyz/gtbwazyxxi.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.gogol.net.cn/gtyuorvlmv.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.hywenlv.cn/gtqfrdcigm.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.smart0.xyz/gtsuxyhxor.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.ydjk.org.cn/gtgjfojzvj.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.daxiang520.top/gttixvhbok.html

================================================================================
来源：http://hz.gogol.net.cn/gtypolyusd.html

M. 命令行 / 进程 / 环境
来源：http://hz.smart0.xyz/gtdxsjumlg.html

================================================================================
来源：http://hz.nanxinkj.top/gtuwwamnol.html

[M01] 读取命令行参数
来源：http://hz.hongshengwenyu.top/gtlzphppuz.html

Py:   sys.argv[1:]
来源：http://hz.gaohongyu789.top/gtdlescafy.html

PHP:  $argv;  $argc;
来源：http://hz.yj202588.top/gtgvkgrpuu.html

JS:   process.argv.slice(2)
来源：http://hz.cqqwz.cn/gthzcehzmx.html

TS:   process.argv.slice(2)
来源：http://hz.jinqigufen.top/gtisacuvlq.html

Java: args 数组（main 方法参数）
来源：http://hz.0kj1m.cn/gtqanphgng.html

Go:   os.Args[1:]
来源：http://hz.vqdsnc.cn/gtiqqcuqzv.html

Ruby: ARGV
来源：http://hz.birdmap.top/gtdnybhowe.html

C#:   args 数组（Main 方法参数）
来源：http://hz.birdmap.top/gtlcrsaoxz.html

[M02] 读取环境变量
来源：http://hz.cucudq.cn/gtdixqgtyo.html

Py:   os.environ.get("HOME")
来源：http://hz.dashuyun.cn/gtrylubkrd.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.guowangkeji.top/gtqvvmookw.html

JS:   process.env.HOME
来源：http://hz.yongpay.top/gthepgnmbq.html

TS:   process.env.HOME
来源：http://hz.aibaodan.cn/gtnknxpyhn.html

Java: System.getenv("HOME")
来源：http://hz.guowangkeji.top/gtkbwuqrbe.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.jqgfzy.top/gtlbaaigzr.html

Ruby: ENV["HOME"]
来源：http://hz.bjfxy.top/gtjbonxeiy.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.316326.xyz/gtdeamiprp.html

[M03] 执行外部命令
来源：http://hz.pycfn.com/gtzkguwbes.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.sysykeji.top/gtaehmwthn.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.mhx1999.top/gtikusloif.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.jiagoushi.top/gtgrodmljx.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.hammf.cn/gtvwjaoxqy.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.sufxvd.cn/gtzkwtmegf.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.yuxming.cn/gtlzthoefg.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.quarkkingdee.top/gtbjhngide.html

C#:   Process.Start("ls", "-l");
来源：http://hz.yangfankeji.com/gtzfnctgwv.html

[M04] 获取当前工作目录
来源：http://hz.yanxiufei.cn/gtypkyzmfo.html

Py:   os.getcwd()
来源：http://hz.zdqjudy.top/gtpeierbpo.html

PHP:  getcwd();
来源：http://hz.kuanghao11.cn/gtkffbanhz.html

JS:   process.cwd()
来源：http://hz.yangfankeji.com/gteeqdjxrd.html

TS:   process.cwd()
来源：http://hz.cheryme.top/gthgvancsl.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.fzhhl.top/gtxicxjgza.html

Go:   os.Getwd()
来源：http://hz.daxiang520.top/gtiaunpkya.html

Ruby: Dir.pwd
来源：http://hz.daxiang520.top/gteesufjfj.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.jinghuilouyu.cn/gthpaydtwj.html

[M05] 设置退出码
来源：http://hz.dianchejie.cn/gtolharwhn.html

Py:   sys.exit(1)
来源：http://hz.xinyue.icu/gtvlttqwfw.html

PHP:  exit(1);
来源：http://hz.chenlongwang.top/gtnfwwdnxt.html

JS:   process.exit(1)
来源：http://hz.cucudq.cn/gtssflgxfs.html

TS:   process.exit(1)
来源：http://hz.shanyushiyangkeji.top/gtstxkcuam.html

Java: System.exit(1)
来源：http://hz.xingfuxueyuan.xyz/gtpfltknna.html

Go:   os.Exit(1)
来源：http://hz.hfpthk.cn/gtvvpottbl.html

Ruby: exit 1
来源：http://hz.xziqi.cn/gtpijavxen.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.svipenyu.cn/gtzlddxilo.html

[M06] 向标准错误输出
来源：http://hz.shangyingyoupin.top/gtgifpqsws.html

Py:   print("err", file=sys.stderr)
来源：http://hz.ydjk.org.cn/gtdxgfbrhl.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.cashguo.top/gtbylcboha.html

JS:   console.error("err")
来源：http://hz.yanxiufei.cn/gtnbtliilx.html

TS:   console.error("err")
来源：http://hz.sufxvd.cn/gtleacjxul.html

Java: System.err.println("err")
来源：http://hz.jqgfzy.top/gtwjviqkwp.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.yj202588.top/gtgjhmzbxq.html

Ruby: warn "err"
来源：http://hz.sufxvd.cn/gtgohoolgg.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.haohaochexian.top/gtptskzkpl.html

[M07] 判断是否为主入口
来源：http://hz.xylfe.cn/gtxbhktsrd.html

Py:   if __name__ == "__main__":
来源：http://hz.9152youxi.cn/gtcsjthsrf.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.shzxlz.cn/gtahaqidiu.html

JS:   require.main === module
来源：http://hz.yj20258.top/gtkbniudny.html

TS:   require.main === module
来源：http://hz.xziqi.cn/gtvttgwjac.html

Java: public static void main(String[] args)
来源：http://hz.iojbl.cn/gtjuzepgme.html

Go:   func main()
来源：http://hz.guannengcc.top/gtmmwvjsdh.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.jyoumei.cn/gtbrnhxunp.html

C#:   static void Main(string[] args)
来源：http://hz.birdmap.top/gtszcqfosx.html

[M08] 获取系统与运行时信息
来源：http://hz.zhongyouzk.top/gtoecrhnvw.html

Py:   platform.system();  platform.python_version()
来源：http://hz.cucudq.cn/gtgapnugpn.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.sufxvd.cn/gtqqiczmni.html

JS:   process.platform;  process.version
来源：http://hz.yanxiufei.cn/gtuyvdwbfz.html

TS:   process.platform;  process.version
来源：http://hz.shuidangran.top/gtjxhwmsii.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.mhx1999.top/gtseljskyk.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.vqdsnc.cn/gtpltlsapx.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.ydzc1.top/gtzyxmbizb.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.tianlin.xyz/gtnxnmdoan.html

================================================================================
来源：http://hz.guowangkeji.top/gtixjkqjrs.html

N. 数据结构与算法
来源：http://hz.xinyue.icu/gttdbpeacp.html

================================================================================
来源：http://hz.haohaochexian.top/gtgtnivndj.html

[N01] 二分查找（有序数组）
来源：http://hz.bjfxy.top/gtzangvddh.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.svipenyu.cn/gtusjvjksp.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.cheryme.top/gtiwowphny.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.nanxuanxn.top/gttrvuaazg.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.quarkkingdee.top/gtaoqeuhjc.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.guannengcc.top/gtgcjdemph.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.daria6918.cn/gtxyztmxpe.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.0kj1m.cn/gtoymyzeto.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.nanxuanxn.top/gtzhwjmwuw.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.hfpthk.cn/gtujqbsial.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.cucudq.cn/gtcppruqos.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.tanke756.top/gtjjpjenut.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.aizwys.cn/gtvvzlwvxp.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.hywenlv.cn/gtnkqfsabv.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.316326.xyz/gtynrccvxh.html

Go:   slices.Sort(arr)
来源：http://hz.ppjwa.cn/gtsdabwclq.html

Ruby: arr.sort
来源：http://hz.zhijiandao.cn/gtkrnlbtmy.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.hfpthk.cn/gtxefcqoqz.html

[N03] 快速排序（分治示例）
来源：http://hz.0kj1m.cn/gturukveru.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.hywenlv.cn/gtbhxkmhbk.html

PHP:  // 递归实现，或用 usort
来源：http://hz.jqgfzy.top/gtcbaukkkt.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.gzhubu.top/gterhlvdxu.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.cqqwz.cn/gtbimbnuyz.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.cheryme.top/gtnvobpaeu.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.gaohongyu789.top/gtpqgyacta.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.smart0.xyz/gtejgkhwlq.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.jyoumei.cn/gtwjwnnnit.html

[N04] 斐波那契数列
来源：http://hz.cdnleiting.top/gtswpttcph.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.wangshuangyany.cn/gtznwkttzi.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.cucudq.cn/gtknhjhqpd.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.hongshengwenyu.top/gtuoddccni.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yuxming.cn/gtxksbcikz.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.ydjk.org.cn/gtjzwkkagw.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.jinqigufen.top/gtqsivoesz.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.sufxvd.cn/gtutbdzhna.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.0kj1m.cn/gtygfwczuy.html

[N05] 最大公约数
来源：http://hz.hnqzz.top/gtzfbjbgwk.html

Py:   math.gcd(a, b)
来源：http://hz.pengpengdd.cyou/gtchvvmmce.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.kuanghao11.cn/gtypspppzy.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.ywan-chungtsiang.top/gtzrmdlvjk.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.tanke756.top/gtmgsxwuri.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.shuidangran.top/gtusqpmdpw.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.tanke756.top/gthdzyxhxg.html

Ruby: a.gcd(b)
来源：http://hz.zhaomingkeji.xyz/gtfzedjuyd.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.9152youxi.cn/gtzfspanco.html

[N06] 判断回文字符串
来源：http://hz.chenzaomai.com/gtjtgxroxf.html

Py:   s == s[::-1]
来源：http://hz.jinqigufen.top/gtcrbcoied.html

PHP:  $s === strrev($s);
来源：http://hz.xziqi.cn/gtymncakhp.html

JS:   s === [...s].reverse().join("")
来源：http://hz.yj20258.top/gtvqxdqoir.html

TS:   s === [...s].reverse().join("")
来源：http://hz.yj20258888.top/gtiadtftds.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.shanyushiyangtech.top/gtijbbrpqt.html

Go:   // 双指针从两端比较
来源：http://hz.hfpthk.cn/gtiodtwtcx.html

Ruby: s == s.reverse
来源：http://hz.cucudq.cn/gtgqmgaoux.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.xuetiantiany.cn/gtsxumzidk.html

[N07] 两数之和（返回下标）
来源：http://hz.shanyushiyangkeji.top/gtfohbwwpr.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.ywan-chungtsiang.top/gthqzdyufa.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.zdqjudy.top/gtprrkyioa.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.chenlongwang.top/gtcsgkcvdx.html

TS:   // 手写 Map<string, number>
来源：http://hz.jinqigfzy.top/gttvsmahvo.html

Java: // 手写 HashMap
来源：http://hz.guannengcc.top/gtimrcfvtp.html

Go:   // 手写 map[int]int
来源：http://hz.c1oappe.top/gtqgrsuhnr.html

Ruby: // 手写 Hash
来源：http://hz.gotoacloud.top/gtocfiieio.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.daria6918.cn/gtcbojrioa.html

[N08] 生成全排列
来源：http://hz.andypj.xyz/gtjbipfods.html

Py:   itertools.permutations(arr)
来源：http://hz.tian-w.cn/gtxquxkhqb.html

PHP:  // 手写递归交换
来源：http://hz.c1oappe.top/gttrvpqcwj.html

JS:   // 手写回溯递归
来源：http://hz.svipenyu.cn/gtkclkvkhm.html

TS:   // 手写回溯递归
来源：http://hz.dashuyun.cn/gtaxkjftuo.html

Java: // 手写回溯递归
来源：http://hz.ywan-chungtsiang.top/gtduoedelk.html

Go:   // 手写回溯递归
来源：http://hz.guowangkeji.top/gtlagzubsw.html

Ruby: arr.permutation.to_a
来源：http://hz.guowangkeji.top/gtrqlyfeuh.html

C#:   // 手写回溯递归
来源：http://hz.gogol.net.cn/gtpqaiybki.html

[N09] 栈与队列
来源：http://hz.wangdashe.top/gttmyzhoch.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.hammf.cn/gtckhplsea.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.chenjidiqi.icu/gtfmyrsqyu.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.zhaomingkeji.xyz/gtyhyegval.html


<!-- 参考信息 -->