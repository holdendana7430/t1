代发 wailian999

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.havefunace.top/gtfcwsewbg.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.daxiang520.top/gtapdjkchy.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.mhx1999.top/gtnrubojll.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.guannengcc.top/gtobsyucfp.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.guannengcc.top/gtnfvuguhe.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.9152youxi.cn/gtvmmttvar.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.shanyushiyangkeji.top/gttozctuip.html

[K05] 深拷贝对象
来源：http://hz.iojbl.cn/gtagualetc.html

Py:   copy.deepcopy(obj)
来源：http://hz.xuanzx.com/gtcciruuxq.html

PHP:  unserialize(serialize($obj));
来源：http://hz.kuanghao11.cn/gtbxodfyqr.html

JS:   structuredClone(obj)
来源：http://hz.cashguo.top/gtjjgxguua.html

TS:   structuredClone(obj)
来源：http://hz.nanxuanxn.top/gtackkcadt.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.mhx1999.top/gtawdznuwd.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.jianghu66.top/gtzzqrhpyo.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.xylfe.cn/gtbheqxhtl.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.meibo888.top/gtigwgjwat.html

[K06] 解析 URL 查询串
来源：http://hz.mhx1999.top/gtzrjruujt.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.tanke756.top/gtcskfxbyz.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.xziqi.cn/gtephtcipx.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jianghu66.top/gtdluiqmaj.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.cheryme.top/gtvlgjvkiu.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.cdnleiting.top/gtvfigmkam.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.jyoumei.cn/gtndmtubip.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.jinghuilouyu.cn/gtpmbfurmt.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.yj202588.top/gtytgnhbsv.html

[K07] 进制转换
来源：http://hz.ydzc1.top/gtjoziapzs.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.yueranfly.top/gtfeypudaf.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.xingfuxueyuan.xyz/gtyesnxmvs.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.ppjwa.cn/gtcbiuzjyb.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.dashuyun.cn/gtognsmbvi.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.guowangkeji.top/gtwhjbrlfk.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.shanyushiyangtech.top/gtfeybmdmi.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.jinyuanbaomall.cn/gtxppdhdpx.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.yj202588.top/gtkvbhzzuz.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.yuxming.cn/gtwokuouup.html

Py:   pickle.dumps(obj)
来源：http://hz.smart0.xyz/gtdpqaaqed.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.jinghuilouyu.cn/gtreqtfgbl.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.yueranfly.top/gtyfniqofx.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.hnqzz.top/gtnkgrsvih.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.meibo888.top/gttzrlvfez.html

Go:   encoding/gob
来源：http://hz.zhoulong.xyz/gtznlkrvyi.html

Ruby: Marshal.dump(obj)
来源：http://hz.tanke756.top/gtzcfwunio.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.zhiwuduotai.top/gtqvvtnvac.html

================================================================================
来源：http://hz.ybcxt.top/gttvqgygvy.html

L. 网络请求
来源：http://hz.pengpengdd.cyou/gtusljitpu.html

================================================================================
来源：http://hz.jyoumei.cn/gtjglufavh.html

[L01] 发送 GET 请求
来源：http://hz.haohaochexian.top/gtivqjusaa.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.0kj1m.cn/gttfaaaijm.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.0kj1m.cn/gtnrdifcqr.html

JS:   await fetch(url)
来源：http://hz.tianlin.xyz/gtnjtrudxa.html

TS:   await fetch(url)
来源：http://hz.shangyingyoupin.top/gtexpzbktv.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.ivvv.top/gtnecpgmsl.html

Go:   resp, err := http.Get(url)
来源：http://hz.shzxlz.cn/gtwoigchxj.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.jlsjyb.cn/gthehrxmjr.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.yj202588.top/gtusbuhiqo.html

[L02] 发送 POST JSON
来源：http://hz.cdnleiting.top/gtajugegrj.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.cucudq.cn/gtojaykhqp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.jinqigufen.top/gtqzulyxod.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.xinyue.icu/gtnhlfdzba.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.ywan-chungtsiang.top/gtuxilblac.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.shangyingyoupin.top/gtzlfvskmj.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.feifeiyinyue.top/gtyqufxyna.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.daxiang520.top/gtkbuliakc.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.ybcxt.top/gtgyjgbqld.html

[L03] 设置自定义请求头
来源：http://hz.jinqigufen.top/gtuoxmabmu.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.hysaishi.cn/gtygnpmlqv.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.guannengcc.top/gtnbdxtldp.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.redwolf501.top/gtwsiffqxg.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.xinyue.icu/gtgihhzkzs.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.yuanzhike.top/gtelfmfxhq.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.smart0.xyz/gthoaacjam.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.wangshuangyany.cn/gtrkmyngrm.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.jyoumei.cn/gtmwmdxcdp.html

[L04] 设置超时
来源：http://hz.xinyue.icu/gtrusudlki.html

Py:   requests.get(url, timeout=5)
来源：http://hz.cqqwz.cn/gtnopnkdng.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.mhx1999.top/gtxzxaeadc.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.andypj.xyz/gtsojmmshs.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.sysykeji.top/gtdkiezrrx.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.yanxiufei.cn/gtuuyucvan.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.yj20258888.top/gtyyowvwpd.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.gogol.net.cn/gtgmxpxwjd.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.zhengqikj.top/gtwhgsjfhi.html

[L05] 上传文件（multipart）
来源：http://hz.havefunace.top/gtovngnbcm.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.jinqigfzy.top/gtizzkigsn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.kuanghao11.cn/gtyiibbsbj.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.dashuyun.cn/gtuexcecrt.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.yonumen.top/gtszgmiggn.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.shanyushiyangtech.top/gtyyxltgju.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.shanyushiyangkeji.top/gtskpdojdh.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.jqgufenzy.top/gtihkgsrbq.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.chenjidiqi.icu/gtsordzjak.html

[L06] 解析响应为 JSON
来源：http://hz.zycfv.cn/gtjuzijume.html

Py:   resp.json()
来源：http://hz.bjfxy.top/gtjrusdtvw.html

PHP:  json_decode($body, true);
来源：http://hz.wangshuangyany.cn/gtmxhbomtq.html

JS:   await resp.json()
来源：http://hz.guowangkeji.top/gtvqyupdar.html

TS:   await resp.json()
来源：http://hz.ppjwa.cn/gtcluikzfh.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.yangfankeji.com/gtauyvqwpn.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.hnqzz.top/gtkhkvwmsf.html

Ruby: JSON.parse(resp.body)
来源：http://hz.52xcode.cn/gttyxxtylx.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.pengpengdd.cyou/gtshoiyuct.html

[L07] 处理 HTTP 状态码
来源：http://hz.tian-w.cn/gtnzdxwirv.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.tianlin.xyz/gtaqvwphzw.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.dashuyun.cn/gtbxauymsz.html

JS:   resp.ok;  resp.status
来源：http://hz.yj20258.top/gtkujxielb.html

TS:   resp.ok;  resp.status
来源：http://hz.feifeiyinyue.top/gtulzxudln.html

Java: resp.statusCode()
来源：http://hz.zhengqikj.top/gtswnhlrxs.html

Go:   resp.StatusCode
来源：http://hz.wangshuangyany.cn/gtjqlzccli.html

Ruby: resp.code.to_i
来源：http://hz.guowangkeji.top/gtrmwzmkws.html

C#:   (int)resp.StatusCode
来源：http://hz.ppjwa.cn/gtpiaptczq.html

[L08] 并发请求多个地址
来源：http://hz.smart0.xyz/gtsdlqthbh.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.cucudq.cn/gtyxmtcabu.html

PHP:  curl_multi_init() 系列
来源：http://hz.aibaodan.cn/gtbbhcvwbn.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.cqqwz.cn/gtiskdptkx.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.hfpthk.cn/gtgdlwifpc.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.c1oappe.top/gtkymyboku.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.gogol.net.cn/gtvqvussrq.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.aizwys.cn/gtgijotuud.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.jqgufenzy.top/gtbxaozekq.html

================================================================================
来源：http://hz.jqgfzy.top/gtkfqopwjx.html

M. 命令行 / 进程 / 环境
来源：http://hz.cqqwz.cn/gteionmtqc.html

================================================================================
来源：http://hz.kuanghao11.cn/gtocmgslot.html

[M01] 读取命令行参数
来源：http://hz.jinqigfzy.top/gtfctuxval.html

Py:   sys.argv[1:]
来源：http://hz.jiagoushi.top/gtnzspttxx.html

PHP:  $argv;  $argc;
来源：http://hz.guowangkeji.top/gtumhivrsq.html

JS:   process.argv.slice(2)
来源：http://hz.zhijiandao.cn/gtvwvxlkck.html

TS:   process.argv.slice(2)
来源：http://hz.xuetiantiany.cn/gtfztnzfpj.html

Java: args 数组（main 方法参数）
来源：http://hz.dashuyun.cn/gtpuqcevyl.html

Go:   os.Args[1:]
来源：http://hz.zhaomingkeji.xyz/gtpaygpnzw.html

Ruby: ARGV
来源：http://hz.yvedp.cn/gtanokzfxm.html

C#:   args 数组（Main 方法参数）
来源：http://hz.shanyushiyangkeji.top/gtstupmqwz.html

[M02] 读取环境变量
来源：http://hz.jqgufenzy.top/gtuebkttty.html

Py:   os.environ.get("HOME")
来源：http://hz.nwbrower.top/gtawssmdgd.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.shanyushiyangtech.top/gtaeutjcab.html

JS:   process.env.HOME
来源：http://hz.0kj1m.cn/gtrsptyhug.html

TS:   process.env.HOME
来源：http://hz.fzhhl.top/gtpqimgnnf.html

Java: System.getenv("HOME")
来源：http://hz.fzhhl.top/gtshehzxwk.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.yuxming.cn/gtxdnkasfp.html

Ruby: ENV["HOME"]
来源：http://hz.aibaodan.cn/gtknxzajqq.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.hnqzz.top/gtidcfocon.html

[M03] 执行外部命令
来源：http://hz.yvedp.cn/gtzegxxvdo.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.316326.xyz/gtfiexzwcf.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.hnxiangtu.top/gtfohlsxkh.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.birdmap.top/gtqcnqfmfu.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.snrcjt.cn/gtisrsntar.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.ydzc1.top/gtsgbtpldv.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.hywenlv.cn/gtykrquhlp.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.hywenlv.cn/gtioaodbup.html

C#:   Process.Start("ls", "-l");
来源：http://hz.guannengcc.top/gtueuehoej.html

[M04] 获取当前工作目录
来源：http://hz.zhengqikj.top/gtonrkdqos.html

Py:   os.getcwd()
来源：http://hz.fzhhl.top/gthgnpxdoy.html

PHP:  getcwd();
来源：http://hz.birdmap.top/gtxfgowohe.html

JS:   process.cwd()
来源：http://hz.andypj.xyz/gtjjnpmkqn.html

TS:   process.cwd()
来源：http://hz.gzhubu.top/gteogfledo.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.jinqigfzy.top/gtmubpfbky.html

Go:   os.Getwd()
来源：http://hz.yonumen.top/gtpjsrtmim.html

Ruby: Dir.pwd
来源：http://hz.fzhhl.top/gtcghodyxg.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.xziqi.cn/gtchznejjy.html

[M05] 设置退出码
来源：http://hz.tian-w.cn/gtyofhnaku.html

Py:   sys.exit(1)
来源：http://hz.sxryk.cn/gtiobjfonz.html

PHP:  exit(1);
来源：http://hz.zhixingplan.top/gtmzgoypbr.html

JS:   process.exit(1)
来源：http://hz.ydjk.org.cn/gtsyhxfyiy.html

TS:   process.exit(1)
来源：http://hz.jinyuanbaomall.cn/gtchltytbg.html

Java: System.exit(1)
来源：http://hz.chenlongwang.top/gtbnmwnmkg.html

Go:   os.Exit(1)
来源：http://hz.meibo888.top/gtegxqnqgc.html

Ruby: exit 1
来源：http://hz.pengpengdd.cyou/gtzejolmrb.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.nwbrower.top/gtjordoeqr.html

[M06] 向标准错误输出
来源：http://hz.haohaochexian.top/gtkqljvopn.html

Py:   print("err", file=sys.stderr)
来源：http://hz.yj202588.top/gtbimfuges.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.shanyushiyangkeji.top/gtvdmarubm.html

JS:   console.error("err")
来源：http://hz.yueranfly.top/gtrdjkujlf.html

TS:   console.error("err")
来源：http://hz.jiagoushi.top/gtfrvnszty.html

Java: System.err.println("err")
来源：http://hz.jinghuilouyu.cn/gtyvooadjr.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.jinqigufen.top/gtdflbzhiv.html

Ruby: warn "err"
来源：http://hz.wangdashe.top/gtftxqzoue.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.0kj1m.cn/gthnnkiqnu.html

[M07] 判断是否为主入口
来源：http://hz.ybcxt.top/gtmshkfcbt.html

Py:   if __name__ == "__main__":
来源：http://hz.gzhubu.top/gthyubqgfx.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.smart0.xyz/gtxgxrolmz.html

JS:   require.main === module
来源：http://hz.iojbl.cn/gtboofetck.html

TS:   require.main === module
来源：http://hz.jinghuilouyu.cn/gteowezskd.html

Java: public static void main(String[] args)
来源：http://hz.zhaomingkeji.xyz/gtnegxpivw.html

Go:   func main()
来源：http://hz.sufxvd.cn/gtiodrmwjv.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.shanyushiyangtech.top/gtczqoktem.html

C#:   static void Main(string[] args)
来源：http://hz.meibo888.top/gtuvogrmcz.html

[M08] 获取系统与运行时信息
来源：http://hz.pengpengdd.cyou/gtualibiqq.html

Py:   platform.system();  platform.python_version()
来源：http://hz.gotoacloud.top/gtgtxqbcqk.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.nwbrower.top/gtyeztcovx.html

JS:   process.platform;  process.version
来源：http://hz.zhengqikj.top/gtodittbjv.html

TS:   process.platform;  process.version
来源：http://hz.nanxuanxn.top/gtglijkdun.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.ybcxt.top/gtgxoxyiyv.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.snrcjt.cn/gtbahdjaep.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.yj20258888.top/gtsrmqfguv.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.tianlin.xyz/gtjyyvnshq.html

================================================================================
来源：http://hz.zhoulong.xyz/gtjcnkdtwo.html

N. 数据结构与算法
来源：http://hz.chenlongwang.top/gtqnyoimwi.html

================================================================================
来源：http://hz.zhijiandao.cn/gtxvelboyp.html

[N01] 二分查找（有序数组）
来源：http://hz.jiagoushi.top/gtfojyzxrf.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.bjfxy.top/gthkigygsb.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.yvedp.cn/gtftpvsjbw.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.quarkkingdee.top/gtskatzafd.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.cqqwz.cn/gtkwtbrulx.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.xinyue.icu/gtumqqahvj.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.hfpthk.cn/gtejjxcpoz.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.zhaomingkeji.xyz/gtlemydxdt.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.kuanghao11.cn/gtfifcjnxb.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.dianchejie.cn/gtbzsoqfpx.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.guannengcc.top/gtaeozbbmc.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.fengsongda.top/gtfvknigbo.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yj20258888.top/gtyyiuiwps.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.zhaomingkeji.xyz/gtnzmddhtx.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.yuanzhike.top/gtloxmzies.html

Go:   slices.Sort(arr)
来源：http://hz.zhijiandao.cn/gtxjquxnsz.html

Ruby: arr.sort
来源：http://hz.hfpthk.cn/gthfszjpkz.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.mhx1999.top/gtlwjwqigg.html

[N03] 快速排序（分治示例）
来源：http://hz.yonumen.top/gtjdbowncj.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.havefunace.top/gttwbeihza.html

PHP:  // 递归实现，或用 usort
来源：http://hz.xingfuxueyuan.xyz/gtyyycarwf.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.haohaochexian.top/gtugqnqeoa.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.feifeiyinyue.top/gtskoodprm.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.chenzaomai.com/gtchmuoawm.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.tianlin.xyz/gttbmqfgoj.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.sweek.top/gtpcqtnumy.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.jyoumei.cn/gtwliefdyx.html

[N04] 斐波那契数列
来源：http://hz.zhixingplan.top/gtzeroedcv.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.yvedp.cn/gttcmrzicf.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.chenjidiqi.icu/gtlrkoeglb.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.hammf.cn/gtnkfokglh.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yuanzhike.top/gtcesjobnj.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.yj202588.top/gtvxgqfgci.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.zhijiandao.cn/gtrnatbuyd.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.dianchejie.cn/gttkrcgzpo.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.shangyingyoupin.top/gtqbvxojiq.html

[N05] 最大公约数
来源：http://hz.shanyushiyangkeji.top/gtarlrfxqc.html

Py:   math.gcd(a, b)
来源：http://hz.hywenlv.cn/gtnqnlmhea.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.zdqjudy.top/gtmwgdpmfy.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.ppjwa.cn/gtidxspvuj.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.tanke756.top/gtikfulscs.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.jianghu66.top/gtzyjxjmmz.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.sxryk.cn/gtrnameovx.html

Ruby: a.gcd(b)
来源：http://hz.jinqigufen.top/gtlggrlnza.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.tianlin.xyz/gtjjaasdgj.html

[N06] 判断回文字符串
来源：http://hz.gaohongyu789.top/gtwqgcvfmg.html

Py:   s == s[::-1]
来源：http://hz.fengsongda.top/gtzwoaotfo.html

PHP:  $s === strrev($s);
来源：http://hz.wangdashe.top/gtsaunwgdu.html

JS:   s === [...s].reverse().join("")
来源：http://hz.jiagoushi.top/gtggmqkazs.html

TS:   s === [...s].reverse().join("")
来源：http://hz.ivvv.top/gtzvqgopki.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.jinqigufen.top/gtiwihozoo.html

Go:   // 双指针从两端比较
来源：http://hz.ydzc1.top/gtvioyiers.html

Ruby: s == s.reverse
来源：http://hz.cashguo.top/gtnwjoskzw.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.hnqzz.top/gttsoejvkc.html

[N07] 两数之和（返回下标）
来源：http://hz.hammf.cn/gtskabsskl.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.ybcxt.top/gtqxyjitof.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.guannengcc.top/gtucwtqhve.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.dianchejie.cn/gtpwzslooh.html

TS:   // 手写 Map<string, number>
来源：http://hz.hywenlv.cn/gtmkhnhsyp.html

Java: // 手写 HashMap
来源：http://hz.yanxiufei.cn/gttmsfgtxl.html

Go:   // 手写 map[int]int
来源：http://hz.yanxiufei.cn/gttbiozbgw.html

Ruby: // 手写 Hash
来源：http://hz.yangfankeji.com/gtznkxpnpr.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.meibo888.top/gtrehnspdo.html

[N08] 生成全排列
来源：http://hz.yuxming.cn/gtfhtjjkxu.html

Py:   itertools.permutations(arr)
来源：http://hz.yj202588.top/gtgxraerrj.html

PHP:  // 手写递归交换
来源：http://hz.zhijiandao.cn/gtppjtedrt.html

JS:   // 手写回溯递归
来源：http://hz.9152youxi.cn/gtyfxpdzvj.html

TS:   // 手写回溯递归
来源：http://hz.52xcode.cn/gtretelrtp.html

Java: // 手写回溯递归
来源：http://hz.hysaishi.cn/gtajadmrjo.html

Go:   // 手写回溯递归
来源：http://hz.pycfn.com/gtfcdkogjp.html

Ruby: arr.permutation.to_a
来源：http://hz.tian-w.cn/gtkjqnunku.html

C#:   // 手写回溯递归
来源：http://hz.yj20258888.top/gtnaukwzzt.html

[N09] 栈与队列
来源：http://hz.xylfe.cn/gtodzfwcjm.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.ydzc1.top/gtexegqweb.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.nwbrower.top/gtorqrlfmx.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.hnxiangtu.top/gtcvberneo.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.52xcode.cn/gtlvyhgxjt.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.daxiang520.top/gtviesqfua.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.cucudq.cn/gtpeuzhhoa.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.zhijiandao.cn/gtbkbzrtus.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.ywan-chungtsiang.top/gtvrcidcwo.html

[N10] 链表节点定义
来源：http://hz.yanxiufei.cn/gtkhxhaohc.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.xylfe.cn/gtmlpohgke.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.gzhubu.top/gtlonvktkr.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.sxryk.cn/gteulqtxrj.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.0kj1m.cn/gtrzplaczs.html

Java: class Node { int v; Node next; }
来源：http://hz.52xcode.cn/gtbvowshzn.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.nwbrower.top/gtxcswdvrb.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.hnqzz.top/gtujoqbvud.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.jiagoushi.top/gtoiaqhndr.html

[N11] 二叉树中序遍历
来源：http://hz.sweek.top/gtkcdeqcdc.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.zhengqikj.top/gtvgeoavfc.html

PHP:  // 手写递归函数
来源：http://hz.cqqwz.cn/gtomawhnbc.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yuxming.cn/gttvrndfzu.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jqgufenzy.top/gtezyhwnzd.html

Java: // 手写递归
来源：http://hz.vqdsnc.cn/gtqbsqjvul.html

Go:   // 手写递归
来源：http://hz.hongshengwenyu.top/gtmzbiyvgv.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.bjfxy.top/gtcyfpeaqs.html

C#:   // 手写递归
来源：http://hz.hywenlv.cn/gtikyrzftt.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.cheryme.top/gtuiziqfcn.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.kuanghao11.cn/gteyxayglk.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.jyoumei.cn/gtzprptfgl.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.ybcxt.top/gtrikpdity.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.xylfe.cn/gttbqkddxb.html


<!-- 参考信息 -->