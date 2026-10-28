代发 wailian999

Ruby: JSON.pretty_generate(obj)
来源：http://hz.nwbrower.top/gtsblzzupl.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.yuanzhike.top/gtxbzflfmq.html

[K04] 读取 JSON 文件
来源：http://hz.gotoacloud.top/gtpwfwkyme.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.ywan-chungtsiang.top/gtzcblfnsj.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.zhixingplan.top/gtwuxbailf.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.smart0.xyz/gtxvzsrybv.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.0kj1m.cn/gtxwyrjqep.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.tanke756.top/gtcyuxhwgp.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.iojbl.cn/gtdndosuro.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.shanyushiyangkeji.top/gtmgrvwsoq.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.zhiwuduotai.top/gtfxbrwitx.html

[K05] 深拷贝对象
来源：http://hz.dianchejie.cn/gtfpvbkrez.html

Py:   copy.deepcopy(obj)
来源：http://hz.wangdashe.top/gtrudyjyoa.html

PHP:  unserialize(serialize($obj));
来源：http://hz.vqdsnc.cn/gtrcrastpa.html

JS:   structuredClone(obj)
来源：http://hz.yueranfly.top/gtrkphgwgk.html

TS:   structuredClone(obj)
来源：http://hz.svipenyu.cn/gtwkqbwksg.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.tianlin.xyz/gtlufrajuu.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.cucudq.cn/gtqgvzhezo.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.ehwqpu.com/gtoeqdnurn.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.jiagoushi.top/gthzixgvmv.html

[K06] 解析 URL 查询串
来源：http://hz.zdqjudy.top/gtxdcnjrtk.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.mhx1999.top/gtkqceveoz.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.jyoumei.cn/gtytdlnvsk.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.mhx1999.top/gtjmccpxmw.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.bjfxy.top/gtfnxfplyf.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.sysykeji.top/gtlfosvdwq.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.guannengcc.top/gtgobvtayi.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.yj20258888.top/gtlxhgatsd.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.dashuyun.cn/gtjlphecfa.html

[K07] 进制转换
来源：http://hz.pycfn.com/gtpvuajrfg.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.hnqzz.top/gthpuhmcud.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.tianlin.xyz/gtucksiyhp.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.ppjwa.cn/gtuvkpwhpb.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.andypj.xyz/gtqptrhbig.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.dashuyun.cn/gtfenezcfh.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.shanyushiyangkeji.top/gtgdzicejf.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.yj20258888.top/gtvvrvlkla.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.shanyushiyangkeji.top/gtmkwotsrm.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.guannengcc.top/gttdkjziiw.html

Py:   pickle.dumps(obj)
来源：http://hz.chenzaomai.com/gtmtuyhklg.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.tian-w.cn/gtxpqaxmlf.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.fengsongda.top/gtqtzdtpsp.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.daria6918.cn/gtafwqoyvz.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.shanyushiyangtech.top/gtgrmldbpd.html

Go:   encoding/gob
来源：http://hz.havefunace.top/gtbiguddpy.html

Ruby: Marshal.dump(obj)
来源：http://hz.ybcxt.top/gtcksodawq.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.yongpay.top/gtmsjquzmy.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtaibfpnjb.html

L. 网络请求
来源：http://hz.hywenlv.cn/gttpspcfgo.html

================================================================================
来源：http://hz.yvedp.cn/gthyzbahtm.html

[L01] 发送 GET 请求
来源：http://hz.jiagoushi.top/gtkrfdkcnp.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.cdnleiting.top/gtlpxkfowm.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.nwbrower.top/gtzgshxzei.html

JS:   await fetch(url)
来源：http://hz.hfpthk.cn/gtfwqjejhb.html

TS:   await fetch(url)
来源：http://hz.aibaodan.cn/gtlshzgtcx.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.yonumen.top/gtxvomhart.html

Go:   resp, err := http.Get(url)
来源：http://hz.ydzc1.top/gtkbhgoobz.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.kuanghao11.cn/gtnzliaizw.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.wangshuangyany.cn/gtplcjlazy.html

[L02] 发送 POST JSON
来源：http://hz.tanke756.top/gtslnlohsy.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.xingfuxueyuan.xyz/gtkicmnulw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.jinqigufen.top/gtvthuwliu.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.shanyushiyangtech.top/gthzikfvef.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.hammf.cn/gtayxboich.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.xziqi.cn/gtgogbbimw.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.yongpay.top/gtroajzmcu.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.cashguo.top/gtfmiolvyd.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.jqgfzy.top/gtexdramwd.html

[L03] 设置自定义请求头
来源：http://hz.wangshuangyany.cn/gtuivdlnnf.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.quarkkingdee.top/gtvyvtzzqc.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.ydjk.org.cn/gtqsnbzfrw.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jlsjyb.cn/gtiwuquwtl.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zhaomingkeji.xyz/gtrivywaeb.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.hfpthk.cn/gtulbxitdq.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.shanyushiyangkeji.top/gtnhlrzbji.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.jiagoushi.top/gttajvocef.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.0kj1m.cn/gtghjgbjyw.html

[L04] 设置超时
来源：http://hz.yanxiufei.cn/gtmiesxwru.html

Py:   requests.get(url, timeout=5)
来源：http://hz.gzhubu.top/gtyjgdrbzb.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.shangyingyoupin.top/gtkofevqlh.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.hongshengwenyu.top/gtzfrnjkhn.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.cdnleiting.top/gteuuiriop.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.meibo888.top/gtqphtzaov.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.shanyushiyangtech.top/gtwnvikfoy.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.ehwqpu.com/gthnegqhsn.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.hammf.cn/gtbyekqjjq.html

[L05] 上传文件（multipart）
来源：http://hz.tian-w.cn/gtenogvdpi.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.ybcxt.top/gtxsllmbza.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.yuanzhike.top/gtuzoitjhb.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.shuidangran.top/gtdapuiyiu.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.kuanghao11.cn/gtkwkbtaep.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.zhijiandao.cn/gtvmsbwfdg.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.havefunace.top/gthkfeneux.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.pycfn.com/gtijciujoe.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.iojbl.cn/gtumpixknz.html

[L06] 解析响应为 JSON
来源：http://hz.ppjwa.cn/gtcjemklco.html

Py:   resp.json()
来源：http://hz.cashguo.top/gtgxwvbult.html

PHP:  json_decode($body, true);
来源：http://hz.redwolf501.top/gtuqkakkvs.html

JS:   await resp.json()
来源：http://hz.zhengqikj.top/gtjzffdmtk.html

TS:   await resp.json()
来源：http://hz.yj20258888.top/gtyhexhszn.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.yangfankeji.com/gtcrddamew.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.vqdsnc.cn/gtlgkpfwkn.html

Ruby: JSON.parse(resp.body)
来源：http://hz.yj20258.top/gtvhmmkhmr.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.zhengqikj.top/gtfhhyrnoy.html

[L07] 处理 HTTP 状态码
来源：http://hz.yuanzhike.top/gtehoiltiv.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.vqdsnc.cn/gtifpsqwad.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.shanyushiyangtech.top/gttmrovqky.html

JS:   resp.ok;  resp.status
来源：http://hz.andypj.xyz/gtwtygrjjq.html

TS:   resp.ok;  resp.status
来源：http://hz.shzxlz.cn/gtrutytmpd.html

Java: resp.statusCode()
来源：http://hz.cheryme.top/gtmdtuajph.html

Go:   resp.StatusCode
来源：http://hz.yj20258.top/gtkbdiztbg.html

Ruby: resp.code.to_i
来源：http://hz.jinghuilouyu.cn/gtyfsmwebc.html

C#:   (int)resp.StatusCode
来源：http://hz.0kj1m.cn/gtlpkzmlhi.html

[L08] 并发请求多个地址
来源：http://hz.shanyushiyangkeji.top/gtcztrqtbt.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.gogol.net.cn/gtrbzndxdw.html

PHP:  curl_multi_init() 系列
来源：http://hz.haohaochexian.top/gtlnvrpjrv.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.gzhubu.top/gtrxzizijn.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.dianchejie.cn/gtihaieguw.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.cucudq.cn/gtuudrhoyt.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.xylfe.cn/gtlzfxjboo.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.316326.xyz/gtobakfvxv.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.jlsjyb.cn/gtnzlkopto.html

================================================================================
来源：http://hz.jianghu66.top/gtajmbzjsk.html

M. 命令行 / 进程 / 环境
来源：http://hz.ppjwa.cn/gtolotxmwn.html

================================================================================
来源：http://hz.ivvv.top/gttsgjcdkl.html

[M01] 读取命令行参数
来源：http://hz.yangfankeji.com/gtvtuuxntx.html

Py:   sys.argv[1:]
来源：http://hz.birdmap.top/gtexoiprwe.html

PHP:  $argv;  $argc;
来源：http://hz.aizwys.cn/gtyzynjdmp.html

JS:   process.argv.slice(2)
来源：http://hz.gzhubu.top/gtawwtzxdk.html

TS:   process.argv.slice(2)
来源：http://hz.zhengqikj.top/gtuyrpzkbs.html

Java: args 数组（main 方法参数）
来源：http://hz.9152youxi.cn/gtqvwnsefh.html

Go:   os.Args[1:]
来源：http://hz.yj20258.top/gtlzphdyfm.html

Ruby: ARGV
来源：http://hz.0kj1m.cn/gttxediiiw.html

C#:   args 数组（Main 方法参数）
来源：http://hz.bjfxy.top/gtlbhwlczg.html

[M02] 读取环境变量
来源：http://hz.aizwys.cn/gtvvoyeaav.html

Py:   os.environ.get("HOME")
来源：http://hz.gaohongyu789.top/gtxkngfqxs.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.yanxiufei.cn/gthsrnkitp.html

JS:   process.env.HOME
来源：http://hz.zhixingplan.top/gtzhrvtmvo.html

TS:   process.env.HOME
来源：http://hz.vqdsnc.cn/gtyklxcwvc.html

Java: System.getenv("HOME")
来源：http://hz.shanyushiyangkeji.top/gtbzoecrqj.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.yuxming.cn/gtbwnyeega.html

Ruby: ENV["HOME"]
来源：http://hz.ydjk.org.cn/gtcxahpqnz.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.aizwys.cn/gtzjfdmemi.html

[M03] 执行外部命令
来源：http://hz.0kj1m.cn/gtusskpulb.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.havefunace.top/gtpucuxhvk.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.52xcode.cn/gtvqoihmqe.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.hammf.cn/gtvfmcfzeb.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.zhijiandao.cn/gttanbwmmd.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.316326.xyz/gtxqglqvea.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.zhengqikj.top/gtbmlqrmji.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.316326.xyz/gtetgoprtt.html

C#:   Process.Start("ls", "-l");
来源：http://hz.ybcxt.top/gtjgchkdep.html

[M04] 获取当前工作目录
来源：http://hz.shuidangran.top/gtomogryob.html

Py:   os.getcwd()
来源：http://hz.gogol.net.cn/gtphdcrnue.html

PHP:  getcwd();
来源：http://hz.jiagoushi.top/gtpnvqpncy.html

JS:   process.cwd()
来源：http://hz.zhiwuduotai.top/gtiysxjuer.html

TS:   process.cwd()
来源：http://hz.cucudq.cn/gtkveplwjo.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.yj202588.top/gtuozboqmf.html

Go:   os.Getwd()
来源：http://hz.meibo888.top/gtrrwwkwfu.html

Ruby: Dir.pwd
来源：http://hz.chenlongwang.top/gtttpfbjgh.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.redwolf501.top/gtpceuayia.html

[M05] 设置退出码
来源：http://hz.sxryk.cn/gtalemdqsy.html

Py:   sys.exit(1)
来源：http://hz.hongshengwenyu.top/gthrbthmow.html

PHP:  exit(1);
来源：http://hz.hywenlv.cn/gtrowweyql.html

JS:   process.exit(1)
来源：http://hz.shanyushiyangkeji.top/gtnfbsadvq.html

TS:   process.exit(1)
来源：http://hz.yj20258888.top/gtmelnvojk.html

Java: System.exit(1)
来源：http://hz.zhijiandao.cn/gtbsifdhyd.html

Go:   os.Exit(1)
来源：http://hz.shanyushiyangtech.top/gtlceqmbsm.html

Ruby: exit 1
来源：http://hz.jinqigfzy.top/gtadlrsija.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.tian-w.cn/gtkqdxapea.html

[M06] 向标准错误输出
来源：http://hz.bjfxy.top/gtjpbjluae.html

Py:   print("err", file=sys.stderr)
来源：http://hz.zhongyouzk.top/gtsvjasjyg.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.xylfe.cn/gtwbxqglvd.html

JS:   console.error("err")
来源：http://hz.haohaochexian.top/gtpsavhtrb.html

TS:   console.error("err")
来源：http://hz.nanxuanxn.top/gtsdqxsqhv.html

Java: System.err.println("err")
来源：http://hz.zhiwuduotai.top/gtxkjoascn.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.c1oappe.top/gtokhsbqyg.html

Ruby: warn "err"
来源：http://hz.ybcxt.top/gtvwaxgfki.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.yonumen.top/gtqsplxjki.html

[M07] 判断是否为主入口
来源：http://hz.c1oappe.top/gtvtitgkbj.html

Py:   if __name__ == "__main__":
来源：http://hz.daria6918.cn/gtrstwrsaq.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.pengpengdd.cyou/gtmznkzyuf.html

JS:   require.main === module
来源：http://hz.yanxiufei.cn/gtdjkahmrc.html

TS:   require.main === module
来源：http://hz.gogol.net.cn/gtiwcaasni.html

Java: public static void main(String[] args)
来源：http://hz.zhongyouzk.top/gtoqotyjpu.html

Go:   func main()
来源：http://hz.jinyuanbaomall.cn/gtgenywgpy.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.c1oappe.top/gtbddgfkmo.html

C#:   static void Main(string[] args)
来源：http://hz.dianchejie.cn/gtxlemtudo.html

[M08] 获取系统与运行时信息
来源：http://hz.meibo888.top/gtpoggrdwg.html

Py:   platform.system();  platform.python_version()
来源：http://hz.0kj1m.cn/gtxjuemdyx.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.jiagoushi.top/gtoxfwdxyl.html

JS:   process.platform;  process.version
来源：http://hz.sweek.top/gtoytlctmy.html

TS:   process.platform;  process.version
来源：http://hz.redwolf501.top/gtigvzhpce.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.yj20258.top/gtjzrnlevo.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.xylfe.cn/gtzxhvyipg.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.bjfxy.top/gtrivgmnwg.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.xuanzx.com/gthnkdlqan.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtyhdsaprz.html

N. 数据结构与算法
来源：http://hz.xingfuxueyuan.xyz/gtsbltxiab.html

================================================================================
来源：http://hz.meibo888.top/gtowikfwkm.html

[N01] 二分查找（有序数组）
来源：http://hz.guowangkeji.top/gtgauyavfr.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.kuanghao11.cn/gtzizmjmea.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.c1oappe.top/gtgmgffjpt.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.guannengcc.top/gtkovdhnle.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zdqjudy.top/gtuutahbsw.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.yuxming.cn/gtjqzemcrz.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.cqqwz.cn/gtwerozsox.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.sysykeji.top/gteykzkkdr.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.0kj1m.cn/gtzbkkkbld.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.zhaomingkeji.xyz/gtgwfopddu.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.ywan-chungtsiang.top/gtqmzdfsxn.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.jqgfzy.top/gtlbpywuke.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.daria6918.cn/gtuotanllt.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.chenjidiqi.icu/gtsqptfzgx.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.gaohongyu789.top/gthbrnbapg.html

Go:   slices.Sort(arr)
来源：http://hz.yvedp.cn/gtpwecdmlz.html

Ruby: arr.sort
来源：http://hz.52xcode.cn/gtefmggiqj.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.xingfuxueyuan.xyz/gtgssdiayz.html

[N03] 快速排序（分治示例）
来源：http://hz.sweek.top/gtbbblfwkw.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.aizwys.cn/gtgdyzadhw.html

PHP:  // 递归实现，或用 usort
来源：http://hz.zycfv.cn/gtidcsknvc.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zhiwuduotai.top/gtfabokgti.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yuxming.cn/gtwzedhyzv.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.chenzaomai.com/gtuwisbaqw.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.tanke756.top/gtvzpzklml.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.yuxming.cn/gtigbnilht.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.daria6918.cn/gtenyapmpl.html

[N04] 斐波那契数列
来源：http://hz.redwolf501.top/gtyfuiogca.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.yueranfly.top/gtywqhgosm.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.yvedp.cn/gtzdgabfbx.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.dianchejie.cn/gtjqydpwjx.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yj202588.top/gtzonboerr.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.iojbl.cn/gtqfnfgmqo.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.ywan-chungtsiang.top/gtwojfonwt.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.zhengqikj.top/gtcwlldtmz.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.tian-w.cn/gtjfkuwctg.html

[N05] 最大公约数
来源：http://hz.daria6918.cn/gtvqdwiltm.html

Py:   math.gcd(a, b)
来源：http://hz.nwbrower.top/gtqdiqvipe.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.ybcxt.top/gtewvthrew.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.ydzc1.top/gtksoatjlm.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.hammf.cn/gtjyrzptby.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.wangdashe.top/gtgvyhnxzf.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.xingfuxueyuan.xyz/gtzrbhqhpy.html

Ruby: a.gcd(b)
来源：http://hz.zhengqikj.top/gtshannehg.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.yuxming.cn/gtohlzqiwp.html

[N06] 判断回文字符串
来源：http://hz.cheryme.top/gtyikcrwkj.html

Py:   s == s[::-1]
来源：http://hz.gzhubu.top/gtzyvjfxbr.html

PHP:  $s === strrev($s);
来源：http://hz.jqgufenzy.top/gtjpqgrunm.html

JS:   s === [...s].reverse().join("")
来源：http://hz.aibaodan.cn/gtvsigowwx.html

TS:   s === [...s].reverse().join("")
来源：http://hz.sweek.top/gtdpxxxaii.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.cqqwz.cn/gtqxookoal.html

Go:   // 双指针从两端比较
来源：http://hz.bjfxy.top/gtluvpakyy.html

Ruby: s == s.reverse
来源：http://hz.aizwys.cn/gtbialxbis.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.zhoulong.xyz/gtdyhxienl.html

[N07] 两数之和（返回下标）
来源：http://hz.yvedp.cn/gtctjwbcqz.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.hywenlv.cn/gtireukijr.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.hysaishi.cn/gtfqndjcnk.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.316326.xyz/gtockabdxq.html

TS:   // 手写 Map<string, number>
来源：http://hz.smart0.xyz/gtcijtkbin.html

Java: // 手写 HashMap
来源：http://hz.zhongyouzk.top/gtrxxqowlz.html

Go:   // 手写 map[int]int
来源：http://hz.hnqzz.top/gtzodkjywb.html

Ruby: // 手写 Hash
来源：http://hz.zhiwuduotai.top/gtrxrbzxcf.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.hnqzz.top/gtbqponfws.html

[N08] 生成全排列
来源：http://hz.aibaodan.cn/gtqgspmokt.html

Py:   itertools.permutations(arr)
来源：http://hz.52xcode.cn/gtinokbnso.html

PHP:  // 手写递归交换
来源：http://hz.jyoumei.cn/gtdxxsyzah.html

JS:   // 手写回溯递归
来源：http://hz.hywenlv.cn/gtfzqdjltp.html

TS:   // 手写回溯递归
来源：http://hz.shanyushiyangtech.top/gtmbzjpzms.html

Java: // 手写回溯递归
来源：http://hz.yj202588.top/gtqaidacmg.html

Go:   // 手写回溯递归
来源：http://hz.jlsjyb.cn/gtetikarhq.html

Ruby: arr.permutation.to_a
来源：http://hz.yj202588.top/gtuoaeburn.html

C#:   // 手写回溯递归
来源：http://hz.yanxiufei.cn/gtheigwfpm.html

[N09] 栈与队列
来源：http://hz.pengpengdd.cyou/gtsuhwxdkk.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.ydzc1.top/gtakkfknbv.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.yuanzhike.top/gtwcrgdnkh.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.xziqi.cn/gtpwyxicmj.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.c1oappe.top/gtuldoimgh.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.jinqigfzy.top/gtoslwweim.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.yj20258.top/gtlatrhtha.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.jqgfzy.top/gtnjadriem.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.ybcxt.top/gtatidweru.html

[N10] 链表节点定义
来源：http://hz.daxiang520.top/gtjeyxglga.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.redwolf501.top/gtnzhzcshi.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.jinqigfzy.top/gtcfsbwkqs.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.yanxiufei.cn/gteozpixiv.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.yueranfly.top/gtvfshifxj.html

Java: class Node { int v; Node next; }
来源：http://hz.fzhhl.top/gtlcqolixk.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.tian-w.cn/gtkimetuvs.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.pycfn.com/gtnbvpjqsp.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.52xcode.cn/gtsmhvytkg.html

[N11] 二叉树中序遍历
来源：http://hz.sweek.top/gtqvjxkurc.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.zhaomingkeji.xyz/gtzpzakkva.html

PHP:  // 手写递归函数
来源：http://hz.jyoumei.cn/gtjlcqekkg.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.hywenlv.cn/gtohlfhgxx.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jinqigufen.top/gtcwmiqzps.html

Java: // 手写递归
来源：http://hz.pengpengdd.cyou/gtoskuhjah.html

Go:   // 手写递归
来源：http://hz.meibo888.top/gtihgcapqz.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.daria6918.cn/gtpaonzghw.html

C#:   // 手写递归
来源：http://hz.nanxuanxn.top/gttibtbsze.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.c1oappe.top/gtidywuaqs.html


<!-- 参考信息 -->