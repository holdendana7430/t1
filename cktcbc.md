代发 wailian999

[K02] JSON 字符串转对象
来源：http://hz.xingfuxueyuan.xyz/gtciuehgzx.html

Py:   json.loads(s)
来源：http://hz.xuetiantiany.cn/gtkpdogtty.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.yj202588.top/gtarrufzfh.html

JS:   JSON.parse(s)
来源：http://hz.shzxlz.cn/gtcesukupo.html

TS:   JSON.parse(s)
来源：http://hz.ybcxt.top/gtwaaljprc.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.hammf.cn/gtkhmwctku.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.jinqigfzy.top/gtbactjmyg.html

Ruby: JSON.parse(s)
来源：http://hz.ydzc1.top/gtmzwrxbdv.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.0kj1m.cn/gtijjlrrgk.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.kuanghao11.cn/gtmrxvpxut.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.chenzaomai.com/gtabzooulf.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.yueranfly.top/gtqnueyenk.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.chenzaomai.com/gtrpntzvar.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.yongpay.top/gthuznsbgv.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.yuanzhike.top/gtsctgzgfg.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.sweek.top/gteneloxcl.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.zhengqikj.top/gtumstusca.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.zhixingplan.top/gtnaxqiipz.html

[K04] 读取 JSON 文件
来源：http://hz.guowangkeji.top/gtbxyeqvxd.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.ydjk.org.cn/gtyrrkvenc.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.yanxiufei.cn/gtkfuimqvn.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.smart0.xyz/gtvdijadfx.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.cqqwz.cn/gtweozjbrs.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.ydzc1.top/gtepzqaajl.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.xuanzx.com/gtrlzyjopt.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.ivvv.top/gtowtnfivc.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.hywenlv.cn/gtaxhpkbil.html

[K05] 深拷贝对象
来源：http://hz.chenjidiqi.icu/gtsikxpbvv.html

Py:   copy.deepcopy(obj)
来源：http://hz.xziqi.cn/gtqglesdbi.html

PHP:  unserialize(serialize($obj));
来源：http://hz.sysykeji.top/gtdqbadsrs.html

JS:   structuredClone(obj)
来源：http://hz.ehwqpu.com/gtprkkconk.html

TS:   structuredClone(obj)
来源：http://hz.gogol.net.cn/gtbrycjsuh.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.zhengqikj.top/gtffmprceb.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.zhaomingkeji.xyz/gtlgpiwmcr.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.c1oappe.top/gtazgvcybt.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.0kj1m.cn/gtalvcuvoq.html

[K06] 解析 URL 查询串
来源：http://hz.xylfe.cn/gtaaguvxjz.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.zhoulong.xyz/gtapqvxtft.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.jinqigufen.top/gtrecdlypq.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.quarkkingdee.top/gtttlngcxb.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.hongshengwenyu.top/gtzhumbfxg.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.shzxlz.cn/gtsmtzmwkn.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.haohaochexian.top/gtvgzpbhfh.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.sufxvd.cn/gtfhyxhubo.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.0kj1m.cn/gtrevlpexw.html

[K07] 进制转换
来源：http://hz.sweek.top/gtqdmmllfg.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.dianchejie.cn/gtrjjgossr.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.yongpay.top/gtchlyuqer.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.andypj.xyz/gtbhoyymbp.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.hongshengwenyu.top/gttpevaqkh.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.redwolf501.top/gtonludulr.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.guowangkeji.top/gtonjkqvfk.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.52xcode.cn/gtxlqfhdiu.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.aizwys.cn/gtxbajqfzl.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.pycfn.com/gtfvtgaild.html

Py:   pickle.dumps(obj)
来源：http://hz.havefunace.top/gthnkcxxot.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.zhoulong.xyz/gtmoqrlzns.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.yueranfly.top/gtbyuangyp.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.guannengcc.top/gtbahrmfai.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.jianghu66.top/gtsxjadwla.html

Go:   encoding/gob
来源：http://hz.0kj1m.cn/gtsgsbpibd.html

Ruby: Marshal.dump(obj)
来源：http://hz.bjfxy.top/gtujusgber.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.zycfv.cn/gtxifcarqz.html

================================================================================
来源：http://hz.yangfankeji.com/gtzkroyufh.html

L. 网络请求
来源：http://hz.xuetiantiany.cn/gtwjertxyt.html

================================================================================
来源：http://hz.shuidangran.top/gtzjlwddyz.html

[L01] 发送 GET 请求
来源：http://hz.havefunace.top/gtorjzgfus.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.xziqi.cn/gtcehilhtp.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.cashguo.top/gtvpbnjhah.html

JS:   await fetch(url)
来源：http://hz.svipenyu.cn/gtmgrkokvy.html

TS:   await fetch(url)
来源：http://hz.redwolf501.top/gtgtkhcjpv.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.guannengcc.top/gtcydeuahg.html

Go:   resp, err := http.Get(url)
来源：http://hz.chenlongwang.top/gtnuvchhry.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.cdnleiting.top/gtwwsilcwd.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.sufxvd.cn/gtfcbmvppt.html

[L02] 发送 POST JSON
来源：http://hz.gogol.net.cn/gtifhisric.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.shanyushiyangkeji.top/gtutrhyeaj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.0kj1m.cn/gtdqjowhqk.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.gotoacloud.top/gtlrhbdzmj.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.gogol.net.cn/gtokbekhqt.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.jinyuanbaomall.cn/gtxiiykezn.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.yvedp.cn/gtwfnzyttf.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.cashguo.top/gtbqvvrpwy.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.sufxvd.cn/gtdngruyhg.html

[L03] 设置自定义请求头
来源：http://hz.sxryk.cn/gtzsjxjval.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.aibaodan.cn/gtyvmrtdxr.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.haohaochexian.top/gtrjqjadix.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.aizwys.cn/gtaodfhdhf.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.cqqwz.cn/gtengwpobt.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.jinghuilouyu.cn/gthrzshftq.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.ehwqpu.com/gtajtuauuj.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.aizwys.cn/gtzvslfdmi.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.hysaishi.cn/gtzmnjrlrd.html

[L04] 设置超时
来源：http://hz.cucudq.cn/gtbyvaxame.html

Py:   requests.get(url, timeout=5)
来源：http://hz.yonumen.top/gtpykxzvhe.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.jinyuanbaomall.cn/gtsksbullc.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.guowangkeji.top/gtsnsrjqiv.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.iojbl.cn/gtkyxxosun.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.xuetiantiany.cn/gtelfucons.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.andypj.xyz/gthnvhlngl.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.guowangkeji.top/gtllbbysje.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.cucudq.cn/gtvkpvovsa.html

[L05] 上传文件（multipart）
来源：http://hz.jiagoushi.top/gtcujumrpx.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.9152youxi.cn/gtuprksxfy.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.gaohongyu789.top/gttvtwivbl.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.shanyushiyangkeji.top/gtjoyvrxaq.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.ydzc1.top/gtzlamydog.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.svipenyu.cn/gtowsnpjvv.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.sysykeji.top/gtqnisymmx.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.yonumen.top/gtlrwttrgp.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.9152youxi.cn/gthliztzyc.html

[L06] 解析响应为 JSON
来源：http://hz.aizwys.cn/gtybzqdxfe.html

Py:   resp.json()
来源：http://hz.yonumen.top/gtfpamrlst.html

PHP:  json_decode($body, true);
来源：http://hz.zhijiandao.cn/gtiagpthwj.html

JS:   await resp.json()
来源：http://hz.sysykeji.top/gtpqlufldo.html

TS:   await resp.json()
来源：http://hz.jianghu66.top/gtyefatyfp.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.guowangkeji.top/gtjccqbwtk.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.sufxvd.cn/gtwrgaefkx.html

Ruby: JSON.parse(resp.body)
来源：http://hz.quarkkingdee.top/gtzlngjsqj.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.jiagoushi.top/gtcfvojppo.html

[L07] 处理 HTTP 状态码
来源：http://hz.yanxiufei.cn/gtbjuvyzmi.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.meibo888.top/gtjfsrsqlz.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.shanyushiyangtech.top/gtkdoakatv.html

JS:   resp.ok;  resp.status
来源：http://hz.zhiwuduotai.top/gtbymkvyyp.html

TS:   resp.ok;  resp.status
来源：http://hz.guannengcc.top/gtadkeauge.html

Java: resp.statusCode()
来源：http://hz.jqgfzy.top/gtdwlyyrey.html

Go:   resp.StatusCode
来源：http://hz.hnqzz.top/gtkmqyuxvt.html

Ruby: resp.code.to_i
来源：http://hz.jinghuilouyu.cn/gtznmlxwqk.html

C#:   (int)resp.StatusCode
来源：http://hz.mhx1999.top/gthphbdmpa.html

[L08] 并发请求多个地址
来源：http://hz.jlsjyb.cn/gtalajkicu.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.yj20258.top/gtvqlhehzy.html

PHP:  curl_multi_init() 系列
来源：http://hz.zhiwuduotai.top/gtarafnjvt.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.ehwqpu.com/gtiiggpdzo.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.redwolf501.top/gtcvfbdufk.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.zhoulong.xyz/gtkptdhywz.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.jinqigfzy.top/gtceghlnia.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.nanxuanxn.top/gtwrvsxxph.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.gogol.net.cn/gtmmoaffzm.html

================================================================================
来源：http://hz.gotoacloud.top/gtgqkqruom.html

M. 命令行 / 进程 / 环境
来源：http://hz.c1oappe.top/gtmqmjsdjx.html

================================================================================
来源：http://hz.yongpay.top/gtcyygxsxy.html

[M01] 读取命令行参数
来源：http://hz.shzxlz.cn/gtcfmecefn.html

Py:   sys.argv[1:]
来源：http://hz.wangshuangyany.cn/gtcxudtfaa.html

PHP:  $argv;  $argc;
来源：http://hz.yj20258888.top/gtjexsbxcj.html

JS:   process.argv.slice(2)
来源：http://hz.quarkkingdee.top/gtdowawpwc.html

TS:   process.argv.slice(2)
来源：http://hz.pycfn.com/gthelsdwyz.html

Java: args 数组（main 方法参数）
来源：http://hz.shzxlz.cn/gtifcxdded.html

Go:   os.Args[1:]
来源：http://hz.nanxuanxn.top/gtwfrrpums.html

Ruby: ARGV
来源：http://hz.jyoumei.cn/gtmswxufnx.html

C#:   args 数组（Main 方法参数）
来源：http://hz.xingfuxueyuan.xyz/gtxxfwmdcd.html

[M02] 读取环境变量
来源：http://hz.sysykeji.top/gtakoyfrks.html

Py:   os.environ.get("HOME")
来源：http://hz.nanxuanxn.top/gtuecirbiu.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.tianlin.xyz/gtyxakisbk.html

JS:   process.env.HOME
来源：http://hz.chenlongwang.top/gtletljoio.html

TS:   process.env.HOME
来源：http://hz.tianlin.xyz/gtzcmdcvjt.html

Java: System.getenv("HOME")
来源：http://hz.cqqwz.cn/gtonzddfns.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.aibaodan.cn/gtksnfjrqp.html

Ruby: ENV["HOME"]
来源：http://hz.gzhubu.top/gthsanaogw.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.svipenyu.cn/gtrcskckxv.html

[M03] 执行外部命令
来源：http://hz.jinghuilouyu.cn/gtkerjjfvg.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.9152youxi.cn/gtsnxijaqg.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.daria6918.cn/gtranqfjbs.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.yonumen.top/gtemrjjxkj.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.jinqigfzy.top/gtfgvxnhex.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.sufxvd.cn/gtowamxvqp.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.pycfn.com/gtsdmbvcnf.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.jyoumei.cn/gtxmsabzqb.html

C#:   Process.Start("ls", "-l");
来源：http://hz.hongshengwenyu.top/gtxvinunnw.html

[M04] 获取当前工作目录
来源：http://hz.hnqzz.top/gtghjsrgtp.html

Py:   os.getcwd()
来源：http://hz.52xcode.cn/gtmejxbytf.html

PHP:  getcwd();
来源：http://hz.sysykeji.top/gtpifzrgrs.html

JS:   process.cwd()
来源：http://hz.jyoumei.cn/gtgknpfccd.html

TS:   process.cwd()
来源：http://hz.hnqzz.top/gtwxqkldcx.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.andypj.xyz/gtmbbrofpn.html

Go:   os.Getwd()
来源：http://hz.dashuyun.cn/gtumqjvrxq.html

Ruby: Dir.pwd
来源：http://hz.shangyingyoupin.top/gtnukrdzuk.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.zycfv.cn/gtpxlvmqbd.html

[M05] 设置退出码
来源：http://hz.hysaishi.cn/gteqzeeskm.html

Py:   sys.exit(1)
来源：http://hz.shuidangran.top/gtjdvirhww.html

PHP:  exit(1);
来源：http://hz.zhengqikj.top/gthaovbfix.html

JS:   process.exit(1)
来源：http://hz.yueranfly.top/gtrnzzgpnl.html

TS:   process.exit(1)
来源：http://hz.ehwqpu.com/gtaydpctng.html

Java: System.exit(1)
来源：http://hz.cdnleiting.top/gtcottislv.html

Go:   os.Exit(1)
来源：http://hz.fengsongda.top/gtqjipqliy.html

Ruby: exit 1
来源：http://hz.cqqwz.cn/gtcpkwcmdl.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.316326.xyz/gtthpfianu.html

[M06] 向标准错误输出
来源：http://hz.bjfxy.top/gtszvpazyy.html

Py:   print("err", file=sys.stderr)
来源：http://hz.andypj.xyz/gtraxkzypc.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.nwbrower.top/gtrdyxxtmx.html

JS:   console.error("err")
来源：http://hz.ybcxt.top/gtdluxbjox.html

TS:   console.error("err")
来源：http://hz.birdmap.top/gtdhiykkpx.html

Java: System.err.println("err")
来源：http://hz.xuetiantiany.cn/gtyhjadjfx.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.yvedp.cn/gtkoejmbll.html

Ruby: warn "err"
来源：http://hz.gogol.net.cn/gtkbnttlhn.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.nanxinkj.top/gtezloforr.html

[M07] 判断是否为主入口
来源：http://hz.smart0.xyz/gtwinrzvpb.html

Py:   if __name__ == "__main__":
来源：http://hz.hywenlv.cn/gtnmhluyxe.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.xziqi.cn/gtqxvylntq.html

JS:   require.main === module
来源：http://hz.vqdsnc.cn/gthasytgep.html

TS:   require.main === module
来源：http://hz.smart0.xyz/gtutpysesc.html

Java: public static void main(String[] args)
来源：http://hz.xuanzx.com/gtdpudztqf.html

Go:   func main()
来源：http://hz.nanxuanxn.top/gtftchsrlk.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.zhixingplan.top/gtmjwyubzm.html

C#:   static void Main(string[] args)
来源：http://hz.jinghuilouyu.cn/gtjecgdhyi.html

[M08] 获取系统与运行时信息
来源：http://hz.sxryk.cn/gtawfhtpza.html

Py:   platform.system();  platform.python_version()
来源：http://hz.guannengcc.top/gtwtwtjbuz.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.hywenlv.cn/gtyfrwwevi.html

JS:   process.platform;  process.version
来源：http://hz.jinqigufen.top/gtxwkssjnc.html

TS:   process.platform;  process.version
来源：http://hz.xingfuxueyuan.xyz/gtpfslsuau.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.haohaochexian.top/gteknquzbb.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.daxiang520.top/gtiupqkbkc.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.hfpthk.cn/gtnmgfaioz.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.ydzc1.top/gtmsnoxpiz.html

================================================================================
来源：http://hz.smart0.xyz/gthsymzgcu.html

N. 数据结构与算法
来源：http://hz.smart0.xyz/gtwjhvaoau.html

================================================================================
来源：http://hz.smart0.xyz/gthpawpmib.html

[N01] 二分查找（有序数组）
来源：http://hz.shanyushiyangkeji.top/gtgaohdaaa.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.gotoacloud.top/gtnyqyxoue.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.aibaodan.cn/gtcazfguko.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jinyuanbaomall.cn/gtspfshiva.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.hywenlv.cn/gtbamrxysx.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.hywenlv.cn/gtebctnsqm.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.hysaishi.cn/gttagdopkv.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.chenzaomai.com/gtkcqpchaf.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.yj202588.top/gteszvkfap.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.chenjidiqi.icu/gtgchdxawx.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.wangshuangyany.cn/gtuijjryvz.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.sweek.top/gtbhprfxud.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yuanzhike.top/gtcoawmpme.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.ybcxt.top/gtytalyzzp.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.daria6918.cn/gtgaqeidun.html

Go:   slices.Sort(arr)
来源：http://hz.jlsjyb.cn/gtzrlmslgs.html

Ruby: arr.sort
来源：http://hz.gotoacloud.top/gtetjoobgr.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.zhiwuduotai.top/gtoohcsfpl.html

[N03] 快速排序（分治示例）
来源：http://hz.vqdsnc.cn/gtwfomoazd.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.shanyushiyangtech.top/gtflzmbeir.html

PHP:  // 递归实现，或用 usort
来源：http://hz.jlsjyb.cn/gtpjxpkzmg.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.gotoacloud.top/gtcnysmmgw.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.wangshuangyany.cn/gtezatrphn.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.jqgufenzy.top/gthmwtjiur.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.xuanzx.com/gtqvigoffh.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.xziqi.cn/gtxdgyzzsp.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.haohaochexian.top/gtkyethshg.html

[N04] 斐波那契数列
来源：http://hz.guowangkeji.top/gtbkrzjurp.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.wangshuangyany.cn/gtndtuaudr.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.dianchejie.cn/gtzllyzsmy.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.ywan-chungtsiang.top/gtwyudycgz.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jianghu66.top/gtstpxoqvk.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.zhixingplan.top/gtglojwphq.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.yongpay.top/gtkdxpkedi.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.xziqi.cn/gtwktodqpc.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.cucudq.cn/gthecvivxb.html

[N05] 最大公约数
来源：http://hz.xingfuxueyuan.xyz/gtgmnpxtit.html

Py:   math.gcd(a, b)
来源：http://hz.nanxinkj.top/gtignnjbnb.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.xylfe.cn/gtmfhtfpyz.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.xuanzx.com/gttpdejnih.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yvedp.cn/gtrbmyamex.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.wangdashe.top/gtfzkwmvhn.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.iojbl.cn/gtuwlrmhga.html

Ruby: a.gcd(b)
来源：http://hz.zhaomingkeji.xyz/gtsyluuogs.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.andypj.xyz/gtdqaojiuk.html

[N06] 判断回文字符串
来源：http://hz.316326.xyz/gtpdvwbvhn.html

Py:   s == s[::-1]
来源：http://hz.yj20258.top/gtdsmbmkxt.html

PHP:  $s === strrev($s);
来源：http://hz.c1oappe.top/gttefjcsvd.html

JS:   s === [...s].reverse().join("")
来源：http://hz.xziqi.cn/gtxrkklmwx.html

TS:   s === [...s].reverse().join("")
来源：http://hz.yuxming.cn/gtbzsjfuak.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.cashguo.top/gtkvfdinoy.html

Go:   // 双指针从两端比较
来源：http://hz.jqgfzy.top/gtgpkrheib.html

Ruby: s == s.reverse
来源：http://hz.tianlin.xyz/gtiyyzgnsx.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.hfpthk.cn/gtkvxeuqmj.html

[N07] 两数之和（返回下标）
来源：http://hz.hammf.cn/gtdpluhwvy.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.aibaodan.cn/gtyvmnfnuv.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.cqqwz.cn/gtisxhrpeu.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.chenzaomai.com/gtptuuynep.html

TS:   // 手写 Map<string, number>
来源：http://hz.c1oappe.top/gtlnvmjrjv.html

Java: // 手写 HashMap
来源：http://hz.pycfn.com/gtjhalrddo.html

Go:   // 手写 map[int]int
来源：http://hz.jiagoushi.top/gtsmlpauue.html

Ruby: // 手写 Hash
来源：http://hz.cqqwz.cn/gtugcannfd.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.iojbl.cn/gtuflqadjh.html

[N08] 生成全排列
来源：http://hz.fzhhl.top/gtztevrsuo.html

Py:   itertools.permutations(arr)
来源：http://hz.hnqzz.top/gtkoajuhfd.html

PHP:  // 手写递归交换
来源：http://hz.xingfuxueyuan.xyz/gtrkvotdbv.html

JS:   // 手写回溯递归
来源：http://hz.iojbl.cn/gtmsnyghbr.html

TS:   // 手写回溯递归
来源：http://hz.daria6918.cn/gtkbukxnre.html

Java: // 手写回溯递归
来源：http://hz.ivvv.top/gtsznqxzmr.html

Go:   // 手写回溯递归
来源：http://hz.gzhubu.top/gthwzobhoo.html

Ruby: arr.permutation.to_a
来源：http://hz.zdqjudy.top/gtefinlppm.html

C#:   // 手写回溯递归
来源：http://hz.chenjidiqi.icu/gtvxprzxnh.html

[N09] 栈与队列
来源：http://hz.ywan-chungtsiang.top/gtbrpqpkag.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.sufxvd.cn/gtltopokhd.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.pengpengdd.cyou/gtufbutuww.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.havefunace.top/gtzwykdfoa.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.fzhhl.top/gtfvuqcdow.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.zycfv.cn/gtjvdkodpv.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.sufxvd.cn/gthocrhmkl.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.cqqwz.cn/gthtllgzzw.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.yj202588.top/gtmhzpdhrc.html

[N10] 链表节点定义
来源：http://hz.cheryme.top/gtdwdynfwi.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.zhongyouzk.top/gtqxpxpwvv.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.mhx1999.top/gtuuandont.html


<!-- 参考信息 -->