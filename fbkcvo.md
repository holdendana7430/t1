代发 wailian999

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.dianchejie.cn/gtjxnurdlq.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.gzhubu.top/gtnzkupjzt.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.jinyuanbaomall.cn/gtatavocdz.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.chenjidiqi.icu/gtionzillh.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.zhoulong.xyz/gtvspgvgpf.html

[K07] 进制转换
来源：http://hz.daria6918.cn/gtpaghlgdz.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.ydjk.org.cn/gthkqmwgny.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.yj20258.top/gthinklmwk.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.9152youxi.cn/gtvkforgzb.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.havefunace.top/gtwwektsmu.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.aizwys.cn/gtulyzkhsv.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.xinyue.icu/gtipoprxgu.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.wangdashe.top/gtlckydhht.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.jqgfzy.top/gthkptcywp.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.zhongyouzk.top/gtqelitens.html

Py:   pickle.dumps(obj)
来源：http://hz.ydzc1.top/gtvtgovvwk.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.zycfv.cn/gtpepxxcqq.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.wangdashe.top/gtrzdnzfbr.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.9152youxi.cn/gtafvcyhot.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.hnxiangtu.top/gtclrweiij.html

Go:   encoding/gob
来源：http://hz.ywan-chungtsiang.top/gtzcszwinu.html

Ruby: Marshal.dump(obj)
来源：http://hz.mhx1999.top/gtdeolaiap.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.quarkkingdee.top/gthmtufskx.html

================================================================================
来源：http://hz.yonumen.top/gtfofgvalh.html

L. 网络请求
来源：http://hz.snrcjt.cn/gtybwklumk.html

================================================================================
来源：http://hz.gogol.net.cn/gtrzpzkfxy.html

[L01] 发送 GET 请求
来源：http://hz.sweek.top/gtrncqodsy.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.bjfxy.top/gtnisovdzq.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.aizwys.cn/gttycrlvse.html

JS:   await fetch(url)
来源：http://hz.yj202588.top/gttifmrczd.html

TS:   await fetch(url)
来源：http://hz.meibo888.top/gtjxfuqwxj.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.aibaodan.cn/gtrzlurwbg.html

Go:   resp, err := http.Get(url)
来源：http://hz.fengsongda.top/gtyncnnbkr.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.cdnleiting.top/gtclkkjmiw.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.9152youxi.cn/gtsvrsbhlk.html

[L02] 发送 POST JSON
来源：http://hz.smart0.xyz/gtykocutvm.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.xziqi.cn/gtqyzodfiu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.yj20258.top/gteacgxcxo.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.chenjidiqi.icu/gtbdjatkpe.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.ivvv.top/gtyeonhtsm.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.yj20258888.top/gtwszmgjrr.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.sxryk.cn/gtsxsotxgk.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.zdqjudy.top/gtezybsfmj.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.fzhhl.top/gteuqvoniz.html

[L03] 设置自定义请求头
来源：http://hz.jqgufenzy.top/gtiufxacwj.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.yvedp.cn/gtqohevxep.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.yangfankeji.com/gtctongdtk.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.nwbrower.top/gtnjzlzjkn.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jinyuanbaomall.cn/gtxxxvvpve.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.pengpengdd.cyou/gtnvdubodn.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.kuanghao11.cn/gteuwhadvv.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.zycfv.cn/gtqbhjkotp.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.xylfe.cn/gtgrurfeyi.html

[L04] 设置超时
来源：http://hz.zycfv.cn/gtlicdxiff.html

Py:   requests.get(url, timeout=5)
来源：http://hz.yanxiufei.cn/gtfgffuihx.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.yuxming.cn/gtkzvzzlry.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yuanzhike.top/gtszjeajwk.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zhiwuduotai.top/gtqyepbhlc.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.quarkkingdee.top/gtbtavphbd.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.tanke756.top/gtzctgsodz.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.guowangkeji.top/gttnwyuozj.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.svipenyu.cn/gtyljnqwhl.html

[L05] 上传文件（multipart）
来源：http://hz.guowangkeji.top/gtbzjsrxby.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.ivvv.top/gtbdziaqkz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.316326.xyz/gtjrvwluij.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.hysaishi.cn/gtdzyfbdxy.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.tianlin.xyz/gtbnsyvakn.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.dashuyun.cn/gtibhaejdp.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.cheryme.top/gtrzmerawb.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.yvedp.cn/gtgzlmcokh.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.xylfe.cn/gtqdjwcesx.html

[L06] 解析响应为 JSON
来源：http://hz.hywenlv.cn/gthqqhxjlp.html

Py:   resp.json()
来源：http://hz.havefunace.top/gtbdjxiilk.html

PHP:  json_decode($body, true);
来源：http://hz.yuxming.cn/gtmgjglihp.html

JS:   await resp.json()
来源：http://hz.havefunace.top/gtzbmcqxrq.html

TS:   await resp.json()
来源：http://hz.wangdashe.top/gtqlnjyduf.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.birdmap.top/gtwxhtccav.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.gzhubu.top/gtdvbxslfs.html

Ruby: JSON.parse(resp.body)
来源：http://hz.yanxiufei.cn/gtwdtilkuw.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.birdmap.top/gtaygkqcpq.html

[L07] 处理 HTTP 状态码
来源：http://hz.smart0.xyz/gtobtdbjog.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.jiagoushi.top/gtrxlhjpyn.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.gotoacloud.top/gteefoftsk.html

JS:   resp.ok;  resp.status
来源：http://hz.nanxinkj.top/gtkuwyqgyr.html

TS:   resp.ok;  resp.status
来源：http://hz.zhixingplan.top/gtzlmfzptp.html

Java: resp.statusCode()
来源：http://hz.kuanghao11.cn/gtbperinau.html

Go:   resp.StatusCode
来源：http://hz.ppjwa.cn/gtaqmvxvzm.html

Ruby: resp.code.to_i
来源：http://hz.sysykeji.top/gtosrxernl.html

C#:   (int)resp.StatusCode
来源：http://hz.hongshengwenyu.top/gtifdfjjlq.html

[L08] 并发请求多个地址
来源：http://hz.ehwqpu.com/gtyocihaor.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.316326.xyz/gtixbefeur.html

PHP:  curl_multi_init() 系列
来源：http://hz.sysykeji.top/gtibaolzgm.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.0kj1m.cn/gtwwnpoovy.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.gaohongyu789.top/gtbrliozkq.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.andypj.xyz/gtucwmfsug.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.quarkkingdee.top/gtxqhwhjrd.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.birdmap.top/gtykvhjtkg.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.tian-w.cn/gtsqphzmgc.html

================================================================================
来源：http://hz.quarkkingdee.top/gtkqkucrzr.html

M. 命令行 / 进程 / 环境
来源：http://hz.cqqwz.cn/gtjerncdjd.html

================================================================================
来源：http://hz.hysaishi.cn/gtabilegtz.html

[M01] 读取命令行参数
来源：http://hz.gaohongyu789.top/gtekdhmpmd.html

Py:   sys.argv[1:]
来源：http://hz.ehwqpu.com/gtngjcyjpg.html

PHP:  $argv;  $argc;
来源：http://hz.gogol.net.cn/gtguhykclw.html

JS:   process.argv.slice(2)
来源：http://hz.aibaodan.cn/gthnjrnnmp.html

TS:   process.argv.slice(2)
来源：http://hz.redwolf501.top/gthjbptaeu.html

Java: args 数组（main 方法参数）
来源：http://hz.zhengqikj.top/gttzwxiplf.html

Go:   os.Args[1:]
来源：http://hz.tian-w.cn/gtrsaasepc.html

Ruby: ARGV
来源：http://hz.hnqzz.top/gtgewmnoxl.html

C#:   args 数组（Main 方法参数）
来源：http://hz.hywenlv.cn/gtezjcgfwn.html

[M02] 读取环境变量
来源：http://hz.yvedp.cn/gtennicsgl.html

Py:   os.environ.get("HOME")
来源：http://hz.sufxvd.cn/gtwojyknrw.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.shuidangran.top/gtniuskxek.html

JS:   process.env.HOME
来源：http://hz.nwbrower.top/gtcovotslf.html

TS:   process.env.HOME
来源：http://hz.shzxlz.cn/gtcjwyfgpq.html

Java: System.getenv("HOME")
来源：http://hz.feifeiyinyue.top/gtilxpckwx.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.zhaomingkeji.xyz/gtbpdfiioa.html

Ruby: ENV["HOME"]
来源：http://hz.jlsjyb.cn/gtjxpvhebx.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.jinqigufen.top/gtdzusdytn.html

[M03] 执行外部命令
来源：http://hz.zhongyouzk.top/gtkbpgqjoe.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.dianchejie.cn/gtdcigxiny.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.tanke756.top/gtbxdgdfjr.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.tianlin.xyz/gtrrvvudwx.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.zhongyouzk.top/gtlordmvzs.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.yangfankeji.com/gtzirffgvs.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.andypj.xyz/gturgaiebw.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.xinyue.icu/gtjacwlzzx.html

C#:   Process.Start("ls", "-l");
来源：http://hz.mhx1999.top/gtnhoyaqai.html

[M04] 获取当前工作目录
来源：http://hz.mhx1999.top/gtrcfahmhx.html

Py:   os.getcwd()
来源：http://hz.wangdashe.top/gtxjulusut.html

PHP:  getcwd();
来源：http://hz.zycfv.cn/gtreeowlki.html

JS:   process.cwd()
来源：http://hz.vqdsnc.cn/gtfrbwsczi.html

TS:   process.cwd()
来源：http://hz.jianghu66.top/gtfbxqxxng.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.gogol.net.cn/gthmhtvwiy.html

Go:   os.Getwd()
来源：http://hz.zdqjudy.top/gtdwchdyid.html

Ruby: Dir.pwd
来源：http://hz.gaohongyu789.top/gtmearihwx.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.shanyushiyangkeji.top/gtygclbkxp.html

[M05] 设置退出码
来源：http://hz.zycfv.cn/gtuyftvflo.html

Py:   sys.exit(1)
来源：http://hz.redwolf501.top/gtfkkdpbny.html

PHP:  exit(1);
来源：http://hz.nanxinkj.top/gthsfxhlbd.html

JS:   process.exit(1)
来源：http://hz.wangdashe.top/gtpnvhrjkn.html

TS:   process.exit(1)
来源：http://hz.ywan-chungtsiang.top/gtqcdgntsm.html

Java: System.exit(1)
来源：http://hz.gzhubu.top/gtdvwosxuw.html

Go:   os.Exit(1)
来源：http://hz.jiagoushi.top/gtpyzgndro.html

Ruby: exit 1
来源：http://hz.zhixingplan.top/gtljzexfkv.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.smart0.xyz/gtvgjrgpvb.html

[M06] 向标准错误输出
来源：http://hz.aizwys.cn/gtmkisljic.html

Py:   print("err", file=sys.stderr)
来源：http://hz.shzxlz.cn/gtwogrinfn.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.zhijiandao.cn/gtewmibkjl.html

JS:   console.error("err")
来源：http://hz.jyoumei.cn/gtvrwjyrvs.html

TS:   console.error("err")
来源：http://hz.yvedp.cn/gtgrtgoowl.html

Java: System.err.println("err")
来源：http://hz.xylfe.cn/gttbebmppa.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.yj20258.top/gtflvitazr.html

Ruby: warn "err"
来源：http://hz.hnqzz.top/gtncirmitw.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.pengpengdd.cyou/gtfvgcgnld.html

[M07] 判断是否为主入口
来源：http://hz.zycfv.cn/gtfkjgcsoq.html

Py:   if __name__ == "__main__":
来源：http://hz.gaohongyu789.top/gtfofltrqi.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.aizwys.cn/gtqhnisgcl.html

JS:   require.main === module
来源：http://hz.zhaomingkeji.xyz/gtkclqoefx.html

TS:   require.main === module
来源：http://hz.zhixingplan.top/gtnolawagu.html

Java: public static void main(String[] args)
来源：http://hz.sufxvd.cn/gtostngxnu.html

Go:   func main()
来源：http://hz.cashguo.top/gtibuegtuc.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.jinyuanbaomall.cn/gtwdospyav.html

C#:   static void Main(string[] args)
来源：http://hz.316326.xyz/gtphzshyqd.html

[M08] 获取系统与运行时信息
来源：http://hz.nanxinkj.top/gtgmmzxtvi.html

Py:   platform.system();  platform.python_version()
来源：http://hz.jinyuanbaomall.cn/gtgmlupryy.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.zhengqikj.top/gtnimolbba.html

JS:   process.platform;  process.version
来源：http://hz.yueranfly.top/gtpopyqvir.html

TS:   process.platform;  process.version
来源：http://hz.316326.xyz/gtuqsbhkdf.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.ydjk.org.cn/gtzgvefogi.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.yonumen.top/gtreecptxw.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.zhongyouzk.top/gtvjucsqog.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.hysaishi.cn/gtylyzbpgi.html

================================================================================
来源：http://hz.9152youxi.cn/gtirplunqk.html

N. 数据结构与算法
来源：http://hz.xinyue.icu/gtntkrwpnk.html

================================================================================
来源：http://hz.xziqi.cn/gteqyoizge.html

[N01] 二分查找（有序数组）
来源：http://hz.yanxiufei.cn/gtpthobwgl.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.xuanzx.com/gtwjoizogv.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.sxryk.cn/gtwigrnymj.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.fengsongda.top/gtayycifbc.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.ivvv.top/gtizxqlqmg.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.svipenyu.cn/gtevddeiva.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.xingfuxueyuan.xyz/gtlwawcyfi.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.meibo888.top/gtzrdeaelx.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.jiagoushi.top/gtdreeeiug.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.aibaodan.cn/gtlbjjsuyz.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.meibo888.top/gtclvendbn.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.jyoumei.cn/gthqnwzynk.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.shanyushiyangkeji.top/gtsuesnqxg.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.svipenyu.cn/gtmckxovap.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.pycfn.com/gttmfejmrr.html

Go:   slices.Sort(arr)
来源：http://hz.meibo888.top/gtewcyyiet.html

Ruby: arr.sort
来源：http://hz.9152youxi.cn/gtavjxbfkn.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.feifeiyinyue.top/gtsisdymma.html

[N03] 快速排序（分治示例）
来源：http://hz.yj202588.top/gtksotbvnu.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.shanyushiyangkeji.top/gtrzljpuhq.html

PHP:  // 递归实现，或用 usort
来源：http://hz.jinqigufen.top/gthkrwbxma.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jqgfzy.top/gtcmiwifvt.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yonumen.top/gtyogoqbgs.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.xinyue.icu/gtcbkfykwl.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.zycfv.cn/gtsjubuinw.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.ydjk.org.cn/gtikuvewme.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.shangyingyoupin.top/gtftjkcwpn.html

[N04] 斐波那契数列
来源：http://hz.guannengcc.top/gtpzgemdit.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.dashuyun.cn/gtqttwnzqv.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.yangfankeji.com/gtdpvmjill.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.xingfuxueyuan.xyz/gtxeimtjzm.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.aizwys.cn/gtogobojqh.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.shanyushiyangtech.top/gtutaoksdo.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.sweek.top/gtbzzwyqwm.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.jqgfzy.top/gtbgtdwibi.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.yuxming.cn/gtmtcikeik.html

[N05] 最大公约数
来源：http://hz.yonumen.top/gtdkduwmep.html

Py:   math.gcd(a, b)
来源：http://hz.zhiwuduotai.top/gtcotkrvgf.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.chenjidiqi.icu/gtfedlpvzx.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.chenjidiqi.icu/gthsgukefa.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.pengpengdd.cyou/gtxovpvtde.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.yuanzhike.top/gtawcepksa.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.chenzaomai.com/gtvxnbtxre.html

Ruby: a.gcd(b)
来源：http://hz.zdqjudy.top/gtgjyrzvae.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.cqqwz.cn/gtnsscctby.html

[N06] 判断回文字符串
来源：http://hz.zhixingplan.top/gtjmlixhbc.html

Py:   s == s[::-1]
来源：http://hz.sweek.top/gteydknzuk.html

PHP:  $s === strrev($s);
来源：http://hz.birdmap.top/gtfptugjsv.html

JS:   s === [...s].reverse().join("")
来源：http://hz.dashuyun.cn/gtjsacpnnv.html

TS:   s === [...s].reverse().join("")
来源：http://hz.yj202588.top/gtjuprzoic.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.gogol.net.cn/gtpkldfubz.html

Go:   // 双指针从两端比较
来源：http://hz.kuanghao11.cn/gtvyxkavay.html

Ruby: s == s.reverse
来源：http://hz.yanxiufei.cn/gtftdtjfbn.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.hfpthk.cn/gtuagqwwhe.html

[N07] 两数之和（返回下标）
来源：http://hz.shangyingyoupin.top/gtkwuhixnz.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.ydzc1.top/gtcwsproaq.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.cucudq.cn/gtdaqvsmtn.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.gotoacloud.top/gtkjxrwmip.html

TS:   // 手写 Map<string, number>
来源：http://hz.dashuyun.cn/gtspafhgse.html

Java: // 手写 HashMap
来源：http://hz.pengpengdd.cyou/gtpmnhizpz.html

Go:   // 手写 map[int]int
来源：http://hz.dianchejie.cn/gtggczvytu.html

Ruby: // 手写 Hash
来源：http://hz.yuanzhike.top/gtzwtbedzi.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.jinqigfzy.top/gtceryyxgr.html

[N08] 生成全排列
来源：http://hz.hnxiangtu.top/gtespneuok.html

Py:   itertools.permutations(arr)
来源：http://hz.tianlin.xyz/gtrqfnawge.html

PHP:  // 手写递归交换
来源：http://hz.yj20258.top/gtwmmhimdy.html

JS:   // 手写回溯递归
来源：http://hz.ydjk.org.cn/gtsgnpftyk.html

TS:   // 手写回溯递归
来源：http://hz.nwbrower.top/gtfrlwpnid.html

Java: // 手写回溯递归
来源：http://hz.shuidangran.top/gtgmjascfu.html

Go:   // 手写回溯递归
来源：http://hz.cheryme.top/gtztcitkpf.html

Ruby: arr.permutation.to_a
来源：http://hz.cashguo.top/gtswybhdso.html

C#:   // 手写回溯递归
来源：http://hz.nanxinkj.top/gthjlwhtor.html

[N09] 栈与队列
来源：http://hz.dianchejie.cn/gtemasxsyw.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.yvedp.cn/gtewspuowf.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.tian-w.cn/gttmwmdzrj.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.xuetiantiany.cn/gtrrrweweh.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.hnxiangtu.top/gtotoahglf.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.yj20258.top/gtdckfmlfr.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.smart0.xyz/gtoqlumjna.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.fzhhl.top/gttztrucqr.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.hywenlv.cn/gtumnhtxnt.html

[N10] 链表节点定义
来源：http://hz.nwbrower.top/gtvqbzgncs.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.ehwqpu.com/gthlbgyyik.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.vqdsnc.cn/gtdozbhvia.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.sweek.top/gtewyxymce.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.gotoacloud.top/gtwlubfhit.html

Java: class Node { int v; Node next; }
来源：http://hz.c1oappe.top/gtotcxsfiz.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.xingfuxueyuan.xyz/gthjktscfc.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.jinqigufen.top/gtgohhwemr.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.vqdsnc.cn/gtwzatpdqy.html

[N11] 二叉树中序遍历
来源：http://hz.nanxuanxn.top/gtzqmyopdv.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.yj20258888.top/gthbgnklmh.html

PHP:  // 手写递归函数
来源：http://hz.pycfn.com/gtjdelhewj.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.bjfxy.top/gtgjnjnfdr.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.tian-w.cn/gthmpzeuff.html

Java: // 手写递归
来源：http://hz.zdqjudy.top/gtbrxoawfe.html

Go:   // 手写递归
来源：http://hz.ppjwa.cn/gtuuqcjcqv.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.cheryme.top/gtitfsjljr.html

C#:   // 手写递归
来源：http://hz.jinqigufen.top/gtqvpqdpea.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.jqgfzy.top/gtosiptxpp.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.sweek.top/gtzcnmyeax.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.andypj.xyz/gtugiqgncl.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.aibaodan.cn/gtgcsltybo.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.svipenyu.cn/gtwxzcziej.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.52xcode.cn/gtmpgohtkv.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.chenzaomai.com/gttmclobjc.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.bjfxy.top/gtxzsmmjrm.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.gotoacloud.top/gtqljfymaf.html

================================================================================
来源：http://hz.tanke756.top/gtgymtxihp.html

O. 并发与异步
来源：http://hz.hongshengwenyu.top/gtgcpjegji.html

================================================================================
来源：http://hz.yongpay.top/gteiwdnbtn.html

[O01] 启动一个线程
来源：http://hz.aizwys.cn/gteqrwkhkx.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.gogol.net.cn/gtaxbnzpcq.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.jinghuilouyu.cn/gtdoyqzkqv.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.shanyushiyangtech.top/gtpzdqlajr.html

TS:   // 同 JS
来源：http://hz.daxiang520.top/gtcnppivqj.html

Java: new Thread(() -> f()).start()
来源：http://hz.ehwqpu.com/gtlgoodidd.html

Go:   go f()
来源：http://hz.ehwqpu.com/gttlrrhyfx.html

Ruby: Thread.new { f }
来源：http://hz.xingfuxueyuan.xyz/gtfkzcueuj.html

C#:   Task.Run(() => F());
来源：http://hz.52xcode.cn/gtapwpotws.html

[O02] 使用线程池
来源：http://hz.gzhubu.top/gtrzeiimum.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.tian-w.cn/gtwnnjfmgk.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.cashguo.top/gtkaemoxdt.html

JS:   // worker_threads 线程池
来源：http://hz.iojbl.cn/gtodliedlw.html


<!-- 参考信息 -->