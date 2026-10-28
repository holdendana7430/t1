代发 wailian999

TS:   JSON.parse(s)
来源：http://hz.shanyushiyangtech.top/gtdqhjetot.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.hnqzz.top/gtvufaiwvn.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.cashguo.top/gtmfcdbgrg.html

Ruby: JSON.parse(s)
来源：http://hz.dashuyun.cn/gtytgdsimq.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.zhiwuduotai.top/gtfwvqmkbp.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.jqgufenzy.top/gtbmkhwgip.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.dashuyun.cn/gtfzyypwdy.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.zhaomingkeji.xyz/gttlllzpex.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.jinghuilouyu.cn/gtjoagadql.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.316326.xyz/gtenorvgze.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.yuxming.cn/gtkmktiilf.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.jinghuilouyu.cn/gtslsacezj.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.gaohongyu789.top/gthoolwnwo.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.sysykeji.top/gtazgdxmbc.html

[K04] 读取 JSON 文件
来源：http://hz.quarkkingdee.top/gtfclehjhu.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.pycfn.com/gtqeanqqpr.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.birdmap.top/gtmnxuzesh.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.hnxiangtu.top/gtsofdbgtl.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.shanyushiyangtech.top/gtmtyurqbj.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.fzhhl.top/gtqcgqayzf.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.jinqigfzy.top/gtsywzvigk.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.kuanghao11.cn/gtztytmhyg.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.tian-w.cn/gtcjnkhqkd.html

[K05] 深拷贝对象
来源：http://hz.iojbl.cn/gtcwutiwlc.html

Py:   copy.deepcopy(obj)
来源：http://hz.zdqjudy.top/gtcnxxcreb.html

PHP:  unserialize(serialize($obj));
来源：http://hz.gotoacloud.top/gtvhpicmpp.html

JS:   structuredClone(obj)
来源：http://hz.ppjwa.cn/gtsmyyenji.html

TS:   structuredClone(obj)
来源：http://hz.zhixingplan.top/gtqcddyrss.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.fzhhl.top/gtaxryntjh.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.gaohongyu789.top/gtmecoipjo.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.yuanzhike.top/gtheyewmgr.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.andypj.xyz/gtbseykcjx.html

[K06] 解析 URL 查询串
来源：http://hz.fengsongda.top/gtqyivuufc.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.jqgfzy.top/gtkzklhwtk.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.9152youxi.cn/gtgetominz.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.andypj.xyz/gtebmettfg.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.andypj.xyz/gtlcpoblkw.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.yueranfly.top/gtlcpcijuu.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.cheryme.top/gttvhdmzrj.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.cqqwz.cn/gtjbbzqbxq.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.xinyue.icu/gtwhbhurwb.html

[K07] 进制转换
来源：http://hz.316326.xyz/gtfyueapcx.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.sweek.top/gtvhpcgqtd.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.zhiwuduotai.top/gtkdjatjox.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.cashguo.top/gtscnhfkfe.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.hammf.cn/gtdoegvotp.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.cheryme.top/gtgzsjwaux.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.daxiang520.top/gtwqdplavu.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.andypj.xyz/gtpinpbdyw.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.iojbl.cn/gtsysicpcm.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.nwbrower.top/gtbckclxes.html

Py:   pickle.dumps(obj)
来源：http://hz.xziqi.cn/gtkuscwsaw.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.meibo888.top/gthhlnlqof.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.zycfv.cn/gttxhkapuo.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.zhoulong.xyz/gtpolvfikl.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.aibaodan.cn/gtahkppyhv.html

Go:   encoding/gob
来源：http://hz.0kj1m.cn/gtmpmgcfpq.html

Ruby: Marshal.dump(obj)
来源：http://hz.snrcjt.cn/gtwzpgogvd.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.daria6918.cn/gtnhmmalbh.html

================================================================================
来源：http://hz.jiagoushi.top/gtxxozdmft.html

L. 网络请求
来源：http://hz.jyoumei.cn/gtszebeyii.html

================================================================================
来源：http://hz.birdmap.top/gtwhpnmaey.html

[L01] 发送 GET 请求
来源：http://hz.jqgfzy.top/gtcaeguqks.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.yongpay.top/gtypjsisty.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.cdnleiting.top/gtfklthvde.html

JS:   await fetch(url)
来源：http://hz.smart0.xyz/gtyflwdwxa.html

TS:   await fetch(url)
来源：http://hz.ybcxt.top/gtihlxcvdb.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.jqgfzy.top/gtipqozhtc.html

Go:   resp, err := http.Get(url)
来源：http://hz.hysaishi.cn/gtkqhsifvt.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.guowangkeji.top/gtozqjqdop.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.hammf.cn/gtpvuevqrw.html

[L02] 发送 POST JSON
来源：http://hz.hywenlv.cn/gtqvpglohb.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.dianchejie.cn/gtrxupcbge.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.cqqwz.cn/gtwjsyzigs.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.xuetiantiany.cn/gtgqcwyqoa.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.meibo888.top/gtpuajdsaw.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.andypj.xyz/gtsvmyfsgy.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.kuanghao11.cn/gtrsbsdwpj.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.sufxvd.cn/gtlrrblbxc.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.zhixingplan.top/gtxlqpzpya.html

[L03] 设置自定义请求头
来源：http://hz.jiagoushi.top/gtaytoeola.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.hnxiangtu.top/gttnbsbwjj.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.feifeiyinyue.top/gtbcdioavj.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.0kj1m.cn/gtpdvfkpis.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yangfankeji.com/gtqniqgeci.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.jlsjyb.cn/gttyfoknnn.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.yvedp.cn/gteckvpvyy.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.iojbl.cn/gtnznvcxwr.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.aizwys.cn/gttefgefsu.html

[L04] 设置超时
来源：http://hz.shangyingyoupin.top/gtzyhzsqnd.html

Py:   requests.get(url, timeout=5)
来源：http://hz.ehwqpu.com/gtycbkstmu.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.c1oappe.top/gtyiyibuhb.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.xuetiantiany.cn/gtfwcppzel.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.sweek.top/gthxnzzdso.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.ehwqpu.com/gtlfvhjnlb.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.hywenlv.cn/gtcmgtcbtb.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.hongshengwenyu.top/gtekxkppji.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.jyoumei.cn/gtlraesmdx.html

[L05] 上传文件（multipart）
来源：http://hz.haohaochexian.top/gtustdwurf.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.sysykeji.top/gtsmragzel.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.zycfv.cn/gtsgvpeluj.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.sysykeji.top/gtirwdiqhz.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.shanyushiyangtech.top/gtaxmnhzls.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.snrcjt.cn/gtrsiiaqct.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.fengsongda.top/gtfijvsyoi.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.yueranfly.top/gtkhwbndfs.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.chenzaomai.com/gtyiukzevf.html

[L06] 解析响应为 JSON
来源：http://hz.tian-w.cn/gthgcpfxcj.html

Py:   resp.json()
来源：http://hz.yvedp.cn/gtvxitbuwd.html

PHP:  json_decode($body, true);
来源：http://hz.ppjwa.cn/gtuynvghkg.html

JS:   await resp.json()
来源：http://hz.xuetiantiany.cn/gtmrfvbhnv.html

TS:   await resp.json()
来源：http://hz.redwolf501.top/gtnvtzeqvh.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.svipenyu.cn/gtxxsmkume.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.chenlongwang.top/gtdmybyubh.html

Ruby: JSON.parse(resp.body)
来源：http://hz.kuanghao11.cn/gtklnvktnn.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.snrcjt.cn/gtxjnwvoyv.html

[L07] 处理 HTTP 状态码
来源：http://hz.yueranfly.top/gtdftgbvwi.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.52xcode.cn/gtkpbwqzhg.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.kuanghao11.cn/gtjpfeeqkz.html

JS:   resp.ok;  resp.status
来源：http://hz.hysaishi.cn/gtzkknqtrd.html

TS:   resp.ok;  resp.status
来源：http://hz.haohaochexian.top/gtmemchrbz.html

Java: resp.statusCode()
来源：http://hz.quarkkingdee.top/gthaddtpys.html

Go:   resp.StatusCode
来源：http://hz.kuanghao11.cn/gtsnhpsttr.html

Ruby: resp.code.to_i
来源：http://hz.xingfuxueyuan.xyz/gtdincrwil.html

C#:   (int)resp.StatusCode
来源：http://hz.chenlongwang.top/gtdhfalsfi.html

[L08] 并发请求多个地址
来源：http://hz.guowangkeji.top/gtrtgghzkj.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.snrcjt.cn/gtyvtzpshi.html

PHP:  curl_multi_init() 系列
来源：http://hz.yj20258888.top/gtrcrcbljn.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jqgfzy.top/gtgknsgpok.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.gogol.net.cn/gtrkiwvdvw.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.yangfankeji.com/gtfazkpwmf.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.ybcxt.top/gtydynqone.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.hongshengwenyu.top/gtgxsbwvrr.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.yuxming.cn/gtmplagvuo.html

================================================================================
来源：http://hz.jlsjyb.cn/gtmnuzrkib.html

M. 命令行 / 进程 / 环境
来源：http://hz.jqgfzy.top/gtqfmdqcjk.html

================================================================================
来源：http://hz.cashguo.top/gtjnncyojz.html

[M01] 读取命令行参数
来源：http://hz.daxiang520.top/gtflyticdl.html

Py:   sys.argv[1:]
来源：http://hz.nanxuanxn.top/gtpivxbfbt.html

PHP:  $argv;  $argc;
来源：http://hz.chenzaomai.com/gtroltyusp.html

JS:   process.argv.slice(2)
来源：http://hz.dashuyun.cn/gtzwfdneyu.html

TS:   process.argv.slice(2)
来源：http://hz.yvedp.cn/gtgytdhaej.html

Java: args 数组（main 方法参数）
来源：http://hz.yuanzhike.top/gtucjcuayf.html

Go:   os.Args[1:]
来源：http://hz.jianghu66.top/gtgarrjkem.html

Ruby: ARGV
来源：http://hz.fengsongda.top/gtodsruuiq.html

C#:   args 数组（Main 方法参数）
来源：http://hz.mhx1999.top/gtubdhvwzf.html

[M02] 读取环境变量
来源：http://hz.jinqigfzy.top/gtpqsppeis.html

Py:   os.environ.get("HOME")
来源：http://hz.jinqigufen.top/gtzzjhqahj.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.zhijiandao.cn/gtfqspkwec.html

JS:   process.env.HOME
来源：http://hz.zdqjudy.top/gtvccwznrm.html

TS:   process.env.HOME
来源：http://hz.yonumen.top/gtfqlvyixq.html

Java: System.getenv("HOME")
来源：http://hz.hysaishi.cn/gtddfijggv.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.meibo888.top/gtzmvonhgd.html

Ruby: ENV["HOME"]
来源：http://hz.jyoumei.cn/gtgdrwycmy.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.cdnleiting.top/gtboldxgyn.html

[M03] 执行外部命令
来源：http://hz.xylfe.cn/gtbxaaszvn.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.gogol.net.cn/gttaztdhml.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.chenzaomai.com/gtsiyvcora.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.xingfuxueyuan.xyz/gtiwsokydp.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.zdqjudy.top/gtekmdceij.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.havefunace.top/gtpsxucyjb.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.daria6918.cn/gtmmhpfbwi.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.dashuyun.cn/gtcdtwuhyb.html

C#:   Process.Start("ls", "-l");
来源：http://hz.shzxlz.cn/gtmnbbgxnh.html

[M04] 获取当前工作目录
来源：http://hz.zycfv.cn/gteaxmmehk.html

Py:   os.getcwd()
来源：http://hz.gzhubu.top/gtzupxzfzy.html

PHP:  getcwd();
来源：http://hz.wangdashe.top/gtczlijqir.html

JS:   process.cwd()
来源：http://hz.gzhubu.top/gtcowgbsza.html

TS:   process.cwd()
来源：http://hz.jinghuilouyu.cn/gtfavaqzri.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.zdqjudy.top/gtctcgouyh.html

Go:   os.Getwd()
来源：http://hz.yj20258888.top/gtxqlcwcbb.html

Ruby: Dir.pwd
来源：http://hz.9152youxi.cn/gticyiwgan.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.hfpthk.cn/gtrbvvramf.html

[M05] 设置退出码
来源：http://hz.shanyushiyangkeji.top/gtubvlrpid.html

Py:   sys.exit(1)
来源：http://hz.feifeiyinyue.top/gtlirtlzvc.html

PHP:  exit(1);
来源：http://hz.ydjk.org.cn/gtlrnypraz.html

JS:   process.exit(1)
来源：http://hz.nanxinkj.top/gtoffpjzna.html

TS:   process.exit(1)
来源：http://hz.ywan-chungtsiang.top/gtseizbxwi.html

Java: System.exit(1)
来源：http://hz.chenlongwang.top/gtdamgdhiv.html

Go:   os.Exit(1)
来源：http://hz.c1oappe.top/gtxeczvzqx.html

Ruby: exit 1
来源：http://hz.xinyue.icu/gtqagrjwcp.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.52xcode.cn/gtegdcbqso.html

[M06] 向标准错误输出
来源：http://hz.cqqwz.cn/gtkmdgxkyx.html

Py:   print("err", file=sys.stderr)
来源：http://hz.jinyuanbaomall.cn/gttpfplksj.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.xylfe.cn/gtevwzwiqj.html

JS:   console.error("err")
来源：http://hz.yuanzhike.top/gthglyzwfl.html

TS:   console.error("err")
来源：http://hz.zhixingplan.top/gtpbqqfrvd.html

Java: System.err.println("err")
来源：http://hz.zycfv.cn/gtgjatnulj.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.yj20258888.top/gtcdnxaize.html

Ruby: warn "err"
来源：http://hz.yonumen.top/gtapiaxays.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.jlsjyb.cn/gtsuoajeje.html

[M07] 判断是否为主入口
来源：http://hz.xinyue.icu/gtarfafakb.html

Py:   if __name__ == "__main__":
来源：http://hz.andypj.xyz/gtwbtpbkzh.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.jqgufenzy.top/gtxwobpdvz.html

JS:   require.main === module
来源：http://hz.shuidangran.top/gtacrcsuhx.html

TS:   require.main === module
来源：http://hz.shanyushiyangkeji.top/gtsrxkrljg.html

Java: public static void main(String[] args)
来源：http://hz.ybcxt.top/gtopzenqno.html

Go:   func main()
来源：http://hz.zhaomingkeji.xyz/gtuiapbjwq.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.yangfankeji.com/gtyxndyzee.html

C#:   static void Main(string[] args)
来源：http://hz.dianchejie.cn/gtxqxnpkga.html

[M08] 获取系统与运行时信息
来源：http://hz.xinyue.icu/gtihotvdpu.html

Py:   platform.system();  platform.python_version()
来源：http://hz.jianghu66.top/gteoimwaln.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.cashguo.top/gtjorstxqz.html

JS:   process.platform;  process.version
来源：http://hz.wangshuangyany.cn/gtdczzuahm.html

TS:   process.platform;  process.version
来源：http://hz.jqgufenzy.top/gtaoecgqyv.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.yj20258888.top/gtxzqurvcn.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.guannengcc.top/gtcyyfxnwr.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.cashguo.top/gtwyajgchn.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.quarkkingdee.top/gtkufajsvq.html

================================================================================
来源：http://hz.daria6918.cn/gthnfkevbt.html

N. 数据结构与算法
来源：http://hz.zhaomingkeji.xyz/gtgdzevpuw.html

================================================================================
来源：http://hz.c1oappe.top/gtqqcdrazd.html

[N01] 二分查找（有序数组）
来源：http://hz.jinqigufen.top/gtjaioeykj.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.sysykeji.top/gtlyinedth.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.guannengcc.top/gtyftgkpnr.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.dashuyun.cn/gtqalcgdnu.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.tian-w.cn/gtnxrdjwmc.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.hfpthk.cn/gteskgzhdh.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.chenzaomai.com/gtrkqfnuvf.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.jyoumei.cn/gtugrcgzrx.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.chenzaomai.com/gtibpjghkn.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.tanke756.top/gtsnxlqwls.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.wangdashe.top/gtyzrsoepz.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.tian-w.cn/gtrpofovkm.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jqgfzy.top/gthshivrnz.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.xingfuxueyuan.xyz/gtyzlsjskh.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.c1oappe.top/gtagfhiorz.html

Go:   slices.Sort(arr)
来源：http://hz.zhixingplan.top/gtrjfpammt.html

Ruby: arr.sort
来源：http://hz.hfpthk.cn/gtbjkrltwz.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.jiagoushi.top/gtriiwndju.html

[N03] 快速排序（分治示例）
来源：http://hz.cheryme.top/gtiwejfqpz.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.xuanzx.com/gtjnedoecw.html

PHP:  // 递归实现，或用 usort
来源：http://hz.xylfe.cn/gtmgfwtqev.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.redwolf501.top/gtwvcmpblx.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zhoulong.xyz/gthqojlrqp.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.tian-w.cn/gtivrvjdmp.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.yj20258.top/gtakpysshb.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.pycfn.com/gtpdfzwkbl.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.shanyushiyangtech.top/gtvlbebxrt.html

[N04] 斐波那契数列
来源：http://hz.hfpthk.cn/gtkilldxrg.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.ehwqpu.com/gtmbyjdjsj.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.aibaodan.cn/gtrrvnjzlp.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.svipenyu.cn/gtdvnqdnaf.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jlsjyb.cn/gthigicghj.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.shangyingyoupin.top/gtuwzfztev.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.ivvv.top/gtknpxinmc.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.xylfe.cn/gteutpnsnx.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.sxryk.cn/gtypyodudh.html

[N05] 最大公约数
来源：http://hz.yueranfly.top/gtakjdbcgl.html

Py:   math.gcd(a, b)
来源：http://hz.xziqi.cn/gttbjjxvvq.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.cheryme.top/gtgdqdhgqv.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yvedp.cn/gtzxllpung.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.xylfe.cn/gtmlgdrood.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.zdqjudy.top/gtbfwepbje.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.cheryme.top/gtctpjfzrv.html

Ruby: a.gcd(b)
来源：http://hz.hnqzz.top/gtltibppzi.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.c1oappe.top/gtfqrohsie.html

[N06] 判断回文字符串
来源：http://hz.cqqwz.cn/gtefrgqjwb.html

Py:   s == s[::-1]
来源：http://hz.316326.xyz/gtjyycdnps.html

PHP:  $s === strrev($s);
来源：http://hz.chenzaomai.com/gtcyreywkj.html

JS:   s === [...s].reverse().join("")
来源：http://hz.quarkkingdee.top/gtuhnwehos.html

TS:   s === [...s].reverse().join("")
来源：http://hz.zycfv.cn/gtrxybcgzl.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.shuidangran.top/gtowotixdm.html

Go:   // 双指针从两端比较
来源：http://hz.aibaodan.cn/gthxqliikz.html

Ruby: s == s.reverse
来源：http://hz.jinqigfzy.top/gthwefzzxl.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.zhaomingkeji.xyz/gtylsccftw.html

[N07] 两数之和（返回下标）
来源：http://hz.sysykeji.top/gtdtravxkf.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.nanxuanxn.top/gtxwxvkixm.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.cheryme.top/gtqqcfxeve.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.nanxinkj.top/gtmiicoxsu.html

TS:   // 手写 Map<string, number>
来源：http://hz.sysykeji.top/gtdwfnizga.html

Java: // 手写 HashMap
来源：http://hz.svipenyu.cn/gtovqrfvus.html

Go:   // 手写 map[int]int
来源：http://hz.hongshengwenyu.top/gtcljdhspz.html

Ruby: // 手写 Hash
来源：http://hz.tian-w.cn/gthgokcsra.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.yongpay.top/gtzsomumwa.html

[N08] 生成全排列
来源：http://hz.52xcode.cn/gtcuyewhqi.html

Py:   itertools.permutations(arr)
来源：http://hz.chenzaomai.com/gthyzvypsp.html

PHP:  // 手写递归交换
来源：http://hz.feifeiyinyue.top/gtcimajpmx.html

JS:   // 手写回溯递归
来源：http://hz.yj20258.top/gtjnikapyx.html

TS:   // 手写回溯递归
来源：http://hz.ehwqpu.com/gtpejqkuqk.html

Java: // 手写回溯递归
来源：http://hz.c1oappe.top/gtzcvzyplt.html

Go:   // 手写回溯递归
来源：http://hz.chenlongwang.top/gtgywklxuv.html

Ruby: arr.permutation.to_a
来源：http://hz.fzhhl.top/gtjkfrulpp.html

C#:   // 手写回溯递归
来源：http://hz.gotoacloud.top/gthtelkpon.html

[N09] 栈与队列
来源：http://hz.pengpengdd.cyou/gtqapoyjdk.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.sufxvd.cn/gtiasnffky.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.316326.xyz/gtzcnzxvmp.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.yueranfly.top/gtbvmpqytt.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.jiagoushi.top/gthwxnlvvw.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.shuidangran.top/gtxllaocrw.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.zycfv.cn/gthwwciypf.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.yueranfly.top/gtmetgauwz.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.xziqi.cn/gtfxxqvnis.html

[N10] 链表节点定义
来源：http://hz.zhiwuduotai.top/gtjachjwwt.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.zycfv.cn/gtoufxlvav.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.gzhubu.top/gtijrrchqm.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.sxryk.cn/gteexpfsha.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.haohaochexian.top/gtmpmpvbne.html

Java: class Node { int v; Node next; }
来源：http://hz.xinyue.icu/gtfupnaogj.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.aibaodan.cn/gtkszupncq.html


<!-- 参考信息 -->