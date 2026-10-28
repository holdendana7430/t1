代发 wailian999

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.sufxvd.cn/gtiovxcrxy.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.yj202588.top/gtuwkykqkc.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.mhx1999.top/gtujblmitn.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.wangdashe.top/gtnlhbjnsp.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.hywenlv.cn/gtsddmqwia.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.yueranfly.top/gthefipjzd.html

[E16] 数字千分位
来源：http://hz.daxiang520.top/gtydcfadyp.html

Py:   f"{1234567:,}"
来源：http://hz.jqgufenzy.top/gtviyljkbl.html

PHP:  number_format(1234567);
来源：http://hz.nanxinkj.top/gthyjnaaaw.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.wangdashe.top/gtkmtavrbq.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.hywenlv.cn/gtqgtuaipq.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.jiagoushi.top/gtlhnhlssi.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.gogol.net.cn/gtgdoobvpr.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.yuxming.cn/gtqpzcjwvh.html

C#:   1234567.ToString("N0")
来源：http://hz.hongshengwenyu.top/gtlezshroq.html

[E17] 首字母大写
来源：http://hz.ydjk.org.cn/gtnjhgfsoy.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.yanxiufei.cn/gtolgjafur.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.daria6918.cn/gtlkjnfqxm.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.ivvv.top/gtesfvxcle.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.cucudq.cn/gtwrixrpgm.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.316326.xyz/gtaygcvaof.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.chenlongwang.top/gtipgfnjdo.html

Ruby: s.capitalize
来源：http://hz.jqgufenzy.top/gtpaphnxhx.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.ybcxt.top/gtocmiohph.html

[E18] 模板占位符替换
来源：http://hz.dashuyun.cn/gthrskrwrd.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.guannengcc.top/gtbfqgzsvi.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.zhaomingkeji.xyz/gtjzdamuhk.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.shanyushiyangtech.top/gtqlhyeqsx.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.shuidangran.top/gtqulrlgdp.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.guowangkeji.top/gtohrphuvx.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.fzhhl.top/gtfureyfkb.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.ywan-chungtsiang.top/gtjfocfzqn.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.fengsongda.top/gtjflacscv.html

[E19] 多行文本按行拆分
来源：http://hz.yj20258.top/gthdyodkkv.html

Py:   s.splitlines()
来源：http://hz.hongshengwenyu.top/gtadmdkcxz.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.xinyue.icu/gthcqgyvpo.html

JS:   s.split(/\r?\n/)
来源：http://hz.yangfankeji.com/gtwvbsrcxf.html

TS:   s.split(/\r?\n/)
来源：http://hz.hammf.cn/gtoyokgsma.html

Java: s.lines().toList()
来源：http://hz.jlsjyb.cn/gtimvuyrxy.html

Go:   strings.Split(s, "\n")
来源：http://hz.zhengqikj.top/gtbfjyuhal.html

Ruby: s.lines
来源：http://hz.dashuyun.cn/gtllwxjvtb.html

C#:   s.Split('\n')
来源：http://hz.shangyingyoupin.top/gtbgqhvcti.html

[E20] 判断字符串是否为空
来源：http://hz.xingfuxueyuan.xyz/gtvmpzvwnv.html

Py:   if not s:
来源：http://hz.redwolf501.top/gtafpcpvrx.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.kuanghao11.cn/gtlcbeiips.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.yvedp.cn/gtzcftghrs.html

TS:   if (s === "") {}
来源：http://hz.cashguo.top/gtpzubehpj.html

Java: if (s.isEmpty()) {}
来源：http://hz.birdmap.top/gtxlomoknf.html

Go:   if s == "" {}
来源：http://hz.jinghuilouyu.cn/gtdlucsfnf.html

Ruby: if s.empty?
来源：http://hz.gotoacloud.top/gtjnoavezy.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.sufxvd.cn/gtgpdjqmci.html

[E21] 超长截断加省略号
来源：http://hz.guannengcc.top/gtchrpcqgj.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.gzhubu.top/gtonttnmmy.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.jiagoushi.top/gtizewwhct.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yuxming.cn/gttgruerfj.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.nwbrower.top/gtjguppqrz.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.zhoulong.xyz/gtkqhefjjz.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.yj20258.top/gtmtdbkmbp.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.hfpthk.cn/gtceuxybkk.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.yangfankeji.com/gtvpewlxar.html

[E22] 字节长度与字符长度
来源：http://hz.ehwqpu.com/gtmxfmflku.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.ppjwa.cn/gttflcghuq.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.havefunace.top/gtokbwpmeb.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jinqigufen.top/gtevnrarqv.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jinghuilouyu.cn/gtdddnstjy.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.zhiwuduotai.top/gtxqbdsdor.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.tianlin.xyz/gtbytohokt.html

Ruby: s.bytesize;  s.length
来源：http://hz.9152youxi.cn/gttjcvbrbi.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.0kj1m.cn/gtynbgofnb.html

================================================================================
来源：http://hz.xziqi.cn/gtoxzegfmv.html

F. 文件与目录
来源：http://hz.nanxuanxn.top/gtpzcddpvr.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtyrxjmxwf.html

[F01] 读取整个文件
来源：http://hz.gotoacloud.top/gtzufzwojs.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.tianlin.xyz/gtvdrnzwlh.html

PHP:  file_get_contents("a.txt");
来源：http://hz.yonumen.top/gtezdndirz.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.9152youxi.cn/gtigdywagg.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.shanyushiyangkeji.top/gtngvfnvwk.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.zhijiandao.cn/gtlivgwozp.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.hnxiangtu.top/gtbnthcptd.html

Ruby: File.read("a.txt")
来源：http://hz.yvedp.cn/gtxliklczu.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.xinyue.icu/gtwhttoyxx.html

[F02] 逐行读取文件
来源：http://hz.guannengcc.top/gtrtjcjgay.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.cheryme.top/gtkxeofxvn.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.havefunace.top/gtvwppsapd.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.xziqi.cn/gttidudccm.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.wangshuangyany.cn/gtarjppqdd.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.fengsongda.top/gtkfisstzb.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.mhx1999.top/gtgegmemtr.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.c1oappe.top/gtdkupjckz.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.jlsjyb.cn/gttsbkhdva.html

[F03] 写入文件（覆盖）
来源：http://hz.andypj.xyz/gtblwfotxg.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.zhongyouzk.top/gtaohiltsh.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.tianlin.xyz/gtcyqkdjtm.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.tianlin.xyz/gtjwwwnwna.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.pycfn.com/gtpfxtjsie.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.feifeiyinyue.top/gtfptnzkrt.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.cheryme.top/gtacucuhxh.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.sweek.top/gtrzenvzfs.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.gaohongyu789.top/gtxkbhmock.html

[F04] 追加写入文件
来源：http://hz.havefunace.top/gtkrkdauvy.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.ywan-chungtsiang.top/gtbdcgzgpj.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.dianchejie.cn/gtyxufpkvr.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.daria6918.cn/gtdjookvuc.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.ivvv.top/gttnzxyyvm.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.yj202588.top/gtnejuxgio.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.zhixingplan.top/gtnjbatljz.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.gzhubu.top/gttfpwnzxm.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.tian-w.cn/gtmamgzcoc.html

[F05] 判断文件或目录是否存在
来源：http://hz.chenlongwang.top/gtftovwqns.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.gzhubu.top/gtiyarwvoa.html

PHP:  file_exists("a.txt");
来源：http://hz.mhx1999.top/gtnzruomey.html

JS:   fs.existsSync("a.txt")
来源：http://hz.ivvv.top/gtgtrrxcbc.html

TS:   fs.existsSync("a.txt")
来源：http://hz.xinyue.icu/gtpyihfvcx.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.hfpthk.cn/gtkueymlyu.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.xylfe.cn/gtpjywcnyz.html

Ruby: File.exist?("a.txt")
来源：http://hz.cucudq.cn/gtepmsxgma.html

C#:   File.Exists("a.txt")
来源：http://hz.yonumen.top/gtrdaexykp.html

[F06] 删除文件
来源：http://hz.gzhubu.top/gtmggarikv.html

Py:   os.remove("a.txt")
来源：http://hz.fzhhl.top/gtlzxgzydg.html

PHP:  unlink("a.txt");
来源：http://hz.andypj.xyz/gtdrhguxpw.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.wangshuangyany.cn/gtfgdinmyb.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.zdqjudy.top/gttnffoyex.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.ehwqpu.com/gttzrvcofx.html

Go:   os.Remove("a.txt")
来源：http://hz.sysykeji.top/gtixgxtgvp.html

Ruby: File.delete("a.txt")
来源：http://hz.chenjidiqi.icu/gtltoesloy.html

C#:   File.Delete("a.txt");
来源：http://hz.yj20258.top/gtzkamqxdm.html

[F07] 创建目录（含多级）
来源：http://hz.jlsjyb.cn/gtlbyuyptb.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.zhengqikj.top/gtvghyffjq.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.xingfuxueyuan.xyz/gtfqljdehr.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.c1oappe.top/gtizinwbsu.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.shangyingyoupin.top/gtevqhnqvq.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.jqgufenzy.top/gtatnqmkkq.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.yuanzhike.top/gtdtegmtpz.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.redwolf501.top/gtbaqjwxtc.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.52xcode.cn/gtqhhnyotx.html

[F08] 遍历目录
来源：http://hz.jqgfzy.top/gtrxxqmcuz.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.ybcxt.top/gtweqojzza.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.sxryk.cn/gtqabdrmbz.html

JS:   fs.readdirSync("dir")
来源：http://hz.meibo888.top/gtzttscpas.html

TS:   fs.readdirSync("dir")
来源：http://hz.fzhhl.top/gthjtmnkei.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.feifeiyinyue.top/gtfvdqlfmn.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.chenzaomai.com/gtjhunfnxd.html

Ruby: Dir.children("dir")
来源：http://hz.birdmap.top/gtouncsouc.html

C#:   Directory.GetFiles("dir")
来源：http://hz.gzhubu.top/gtdlrhnutw.html

[F09] 获取文件大小
来源：http://hz.9152youxi.cn/gtaxijjgiv.html

Py:   os.path.getsize("a.txt")
来源：http://hz.gotoacloud.top/gtjigsqbnk.html

PHP:  filesize("a.txt");
来源：http://hz.feifeiyinyue.top/gtfvxxcwxc.html

JS:   fs.statSync("a.txt").size
来源：http://hz.jyoumei.cn/gthrwyplpy.html

TS:   fs.statSync("a.txt").size
来源：http://hz.jiagoushi.top/gtipvzvvci.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.xingfuxueyuan.xyz/gtilyjqmxl.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.sweek.top/gtjjkscvcp.html

Ruby: File.size("a.txt")
来源：http://hz.kuanghao11.cn/gtlpblelyk.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.jinqigfzy.top/gtytwahrax.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.iojbl.cn/gtuppcrypz.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.yvedp.cn/gtabeltzwp.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.9152youxi.cn/gtbarjwhvt.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.52xcode.cn/gtcqbhjvjx.html

TS:   path.extname("a.txt")
来源：http://hz.kuanghao11.cn/gtkftuapho.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.zhaomingkeji.xyz/gtconlvpgk.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.pycfn.com/gtqbrqlnli.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.yonumen.top/gtuaypfyoy.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.gaohongyu789.top/gtdenclyze.html

[F11] 复制与移动文件
来源：http://hz.sysykeji.top/gtjxuydnoe.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.316326.xyz/gtndzuulrr.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.aibaodan.cn/gtszazuxzg.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.guannengcc.top/gttovwlmzg.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.fzhhl.top/gthqfgzcsj.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.cheryme.top/gtewwwsidr.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.chenlongwang.top/gtvooxqolb.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.cashguo.top/gtcsfspgsp.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.haohaochexian.top/gtqvqoomdu.html

[F12] CSV 读写
来源：http://hz.yvedp.cn/gtauihbols.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.zhiwuduotai.top/gtlypbjvzc.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.jyoumei.cn/gtbkyitntk.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.xylfe.cn/gtgisssnsw.html

TS:   // 同上
来源：http://hz.cheryme.top/gtjkavraxn.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.zdqjudy.top/gtzzweimrt.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.zdqjudy.top/gtjcdvwshv.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.jyoumei.cn/gtabtdasjy.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.zhaomingkeji.xyz/gtcslndggf.html

================================================================================
来源：http://hz.jyoumei.cn/gtcstkjexz.html

G. 面向对象
来源：http://hz.yuanzhike.top/gtalvaofdh.html

================================================================================
来源：http://hz.c1oappe.top/gtxggdtzpb.html

[G01] 定义类
来源：http://hz.haohaochexian.top/gtmwzyqszl.html

Py:   class User: pass
来源：http://hz.0kj1m.cn/gterkufpbx.html

PHP:  class User {}
来源：http://hz.yuxming.cn/gtqvmivdas.html

JS:   class User {}
来源：http://hz.jinyuanbaomall.cn/gtpquezfol.html

TS:   class User { name: string = ""; }
来源：http://hz.jqgfzy.top/gtbejlbqhv.html

Java: class User {}
来源：http://hz.aizwys.cn/gtwnooxijk.html

Go:   type User struct { Name string }
来源：http://hz.fzhhl.top/gtdkwijqrw.html

Ruby: class User; end
来源：http://hz.pengpengdd.cyou/gtsyddbndf.html

C#:   class User {}
来源：http://hz.hysaishi.cn/gtoxeebfnc.html

[G02] 构造函数
来源：http://hz.yonumen.top/gtydbfnohr.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.zhiwuduotai.top/gtfuklgkbw.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.wangdashe.top/gtgsjovykj.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.ppjwa.cn/gtqcqfspmh.html

TS:   constructor(public name: string) {}
来源：http://hz.ydzc1.top/gtihxneewn.html

Java: User(String name) { this.name = name; }
来源：http://hz.redwolf501.top/gttukqhonz.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.hywenlv.cn/gtlwuexrne.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.redwolf501.top/gtvjvycxku.html

C#:   public User(string name) { Name = name; }
来源：http://hz.jinqigfzy.top/gtijpiznba.html

[G03] 实例属性
来源：http://hz.snrcjt.cn/gtavofschp.html

Py:   self.name = "x"
来源：http://hz.52xcode.cn/gtsozkxyrm.html

PHP:  public string $name = "x";
来源：http://hz.shuidangran.top/gtpfcxwurz.html

JS:   this.name = "x";
来源：http://hz.birdmap.top/gtvyczadsn.html

TS:   name: string = "x";
来源：http://hz.dianchejie.cn/gtvuonqwqm.html

Java: private String name;
来源：http://hz.jianghu66.top/gtuepjwqra.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.redwolf501.top/gtymtphajv.html

Ruby: @name = "x"
来源：http://hz.cucudq.cn/gtjzuxagil.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.mhx1999.top/gtipbbqfpm.html

[G04] 定义方法
来源：http://hz.cashguo.top/gttwbbttzl.html

Py:   def greet(self): return self.name
来源：http://hz.andypj.xyz/gtbpzjakti.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.nwbrower.top/gtcxmnswft.html

JS:   greet() { return this.name; }
来源：http://hz.jinqigfzy.top/gtivtxhwxq.html

TS:   greet(): string { return this.name; }
来源：http://hz.guannengcc.top/gtqkyihwkk.html

Java: String greet() { return name; }
来源：http://hz.hnxiangtu.top/gtxueengsb.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.svipenyu.cn/gteptllkpo.html

Ruby: def greet; @name; end
来源：http://hz.dianchejie.cn/gtxpgtzdyo.html

C#:   public string Greet() => Name;
来源：http://hz.haohaochexian.top/gtvxfkmatj.html

[G05] 继承
来源：http://hz.zycfv.cn/gtwkxmzrtp.html

Py:   class Admin(User): pass
来源：http://hz.fengsongda.top/gtgwhzlpkr.html

PHP:  class Admin extends User {}
来源：http://hz.jqgufenzy.top/gtmiwdgeqx.html

JS:   class Admin extends User {}
来源：http://hz.dashuyun.cn/gtpgbjacbl.html

TS:   class Admin extends User {}
来源：http://hz.dianchejie.cn/gtftplgiwe.html

Java: class Admin extends User {}
来源：http://hz.tianlin.xyz/gtrjtcuvji.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.chenjidiqi.icu/gtqxnxcjcj.html

Ruby: class Admin < User; end
来源：http://hz.tanke756.top/gtxidnkwlz.html

C#:   class Admin : User {}
来源：http://hz.guowangkeji.top/gtuhcjtivm.html

[G06] 重写方法
来源：http://hz.iojbl.cn/gtwzonmbht.html

Py:   def greet(self): return "admin"
来源：http://hz.jqgfzy.top/gtodcdgtkn.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.0kj1m.cn/gtzzbrvoya.html

JS:   greet() { return "admin"; }
来源：http://hz.zhoulong.xyz/gtknqvhoju.html

TS:   greet(): string { return "admin"; }
来源：http://hz.yuxming.cn/gtpmiuktnw.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.xuetiantiany.cn/gtakzahpoz.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.ydjk.org.cn/gtqapuhpub.html

Ruby: def greet; "admin"; end
来源：http://hz.xuanzx.com/gtswijbeiu.html

C#:   public override string Greet() => "admin";
来源：http://hz.quarkkingdee.top/gtyhoxhzxy.html

[G07] 调用父类方法
来源：http://hz.yj202588.top/gtqtawocqx.html

Py:   super().greet()
来源：http://hz.tanke756.top/gtqgxotldw.html

PHP:  parent::greet();
来源：http://hz.birdmap.top/gtqrqkjhwi.html

JS:   super.greet();
来源：http://hz.ehwqpu.com/gttdomdjex.html

TS:   super.greet();
来源：http://hz.haohaochexian.top/gtajxrrrra.html

Java: super.greet();
来源：http://hz.aizwys.cn/gtnlkkmcph.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.cdnleiting.top/gtrextsvha.html

Ruby: super
来源：http://hz.feifeiyinyue.top/gtnjkmzbkc.html

C#:   base.Greet();
来源：http://hz.jinghuilouyu.cn/gtulywrhde.html

[G08] 静态方法与属性
来源：http://hz.aizwys.cn/gtdhqbeceq.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.chenzaomai.com/gtvbdscgdn.html

PHP:  public static function f() {}
来源：http://hz.hfpthk.cn/gtozezgqao.html

JS:   static f() {}
来源：http://hz.zhiwuduotai.top/gtcyhscubl.html

TS:   static f(): void {}
来源：http://hz.yj202588.top/gtjbxktbmc.html

Java: static void f() {}
来源：http://hz.hammf.cn/gtflpnxqfo.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.aizwys.cn/gtjwlqgiml.html

Ruby: def self.f; end
来源：http://hz.zhaomingkeji.xyz/gtcmvgvhds.html

C#:   public static void F() {}
来源：http://hz.yangfankeji.com/gtsfwsdtvt.html

[G09] 接口 / 抽象类
来源：http://hz.sysykeji.top/gtinredvgw.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.zdqjudy.top/gtxontracd.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.shzxlz.cn/gtxpbfvhbp.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.meibo888.top/gtcywtuonz.html

TS:   interface Shape { area(): number; }
来源：http://hz.zhoulong.xyz/gtvifyzjun.html

Java: interface Shape { double area(); }
来源：http://hz.cucudq.cn/gtfvrbhujz.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.shangyingyoupin.top/gtwitsikrg.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.jlsjyb.cn/gtcphhbuiw.html

C#:   interface IShape { double Area(); }
来源：http://hz.quarkkingdee.top/gttfamoyqo.html

[G10] 访问控制
来源：http://hz.shuidangran.top/gtrwlxuntd.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.sweek.top/gtsbqltcmu.html

PHP:  public / protected / private
来源：http://hz.smart0.xyz/gtugcymnci.html

JS:   #private 字段；其余公开
来源：http://hz.shanyushiyangtech.top/gtscijyjml.html

TS:   public / protected / private
来源：http://hz.nwbrower.top/gtanziczlk.html

Java: public / protected / private / 默认包级
来源：http://hz.andypj.xyz/gteyvsgbqg.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.daria6918.cn/gttporzmmo.html

Ruby: public / protected / private
来源：http://hz.jinqigufen.top/gtonxratjf.html

C#:   public / protected / private / internal
来源：http://hz.0kj1m.cn/gtftehoawb.html

[G11] getter / setter
来源：http://hz.yuxming.cn/gtczqynroo.html

Py:   @property 与 @x.setter
来源：http://hz.hywenlv.cn/gtwsazdbyl.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.ehwqpu.com/gteqfmhrja.html

JS:   get name() { return this._name; }
来源：http://hz.gaohongyu789.top/gtuvvxkzeq.html

TS:   get name(): string { return this._name; }
来源：http://hz.zdqjudy.top/gtrnnxrshj.html

Java: public String getName() { return name; }
来源：http://hz.zhiwuduotai.top/gtsafohlej.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.daria6918.cn/gtihgmxapm.html

Ruby: attr_accessor :name
来源：http://hz.ydjk.org.cn/gtbswmntte.html

C#:   public string Name { get; set; }
来源：http://hz.nwbrower.top/gtztmvcbxv.html

[G12] 对象转字符串
来源：http://hz.hammf.cn/gtsejkznfa.html

Py:   def __str__(self): return self.name
来源：http://hz.fengsongda.top/gturcchxoc.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.shangyingyoupin.top/gtcphmfizf.html

JS:   toString() { return this.name; }
来源：http://hz.zhijiandao.cn/gtxzrshtgx.html

TS:   toString(): string { return this.name; }
来源：http://hz.zhiwuduotai.top/gtfmhzbiyv.html

Java: @Override public String toString() { return name; }
来源：http://hz.cheryme.top/gtkonkckqh.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.c1oappe.top/gtkwglmfgt.html

Ruby: def to_s; @name; end
来源：http://hz.jianghu66.top/gtjgtyzsab.html

C#:   public override string ToString() => Name;
来源：http://hz.hongshengwenyu.top/gtpcuurtil.html

[G13] 判断对象类型
来源：http://hz.hysaishi.cn/gtvhfopohi.html

Py:   isinstance(u, User)
来源：http://hz.52xcode.cn/gtahsmtvmw.html

PHP:  $u instanceof User
来源：http://hz.hysaishi.cn/gtozpwnfhi.html

JS:   u instanceof User
来源：http://hz.quarkkingdee.top/gtecadxhji.html

TS:   u instanceof User
来源：http://hz.zycfv.cn/gtoogiaqpu.html

Java: u instanceof User
来源：http://hz.mhx1999.top/gtihibwbty.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.pengpengdd.cyou/gtfbzdahvs.html

Ruby: u.is_a?(User)
来源：http://hz.daxiang520.top/gtzifaevdd.html

C#:   u is User
来源：http://hz.feifeiyinyue.top/gtyfgwjlxd.html


<!-- 参考信息 -->