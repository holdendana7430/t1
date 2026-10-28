代发 wailian999

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.yj20258.top/gtaozpbdyv.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.ywan-chungtsiang.top/gtxoburexm.html

[E16] 数字千分位
来源：http://hz.cdnleiting.top/gtcyzeolkr.html

Py:   f"{1234567:,}"
来源：http://hz.0kj1m.cn/gtneffkojn.html

PHP:  number_format(1234567);
来源：http://hz.hysaishi.cn/gtuwcthdtc.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.yj20258888.top/gtkzrwnros.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.fengsongda.top/gteubninbe.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.c1oappe.top/gthjelnzrw.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.yj20258.top/gtqxlxgzty.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.hywenlv.cn/gtophoycij.html

C#:   1234567.ToString("N0")
来源：http://hz.yvedp.cn/gtanljpgui.html

[E17] 首字母大写
来源：http://hz.chenjidiqi.icu/gtarpdxqkk.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.nwbrower.top/gtcysvxcrr.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.shanyushiyangtech.top/gtklnrnngp.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.daria6918.cn/gtwdrgegmg.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.cashguo.top/gtkvgcpcqp.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.shanyushiyangtech.top/gtdkdjjzyw.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.zhaomingkeji.xyz/gttuzsffuj.html

Ruby: s.capitalize
来源：http://hz.svipenyu.cn/gtxiiusrrj.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.xylfe.cn/gtndimhyhr.html

[E18] 模板占位符替换
来源：http://hz.tian-w.cn/gtnfbykzam.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.chenjidiqi.icu/gtjzixcjnm.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.fzhhl.top/gtcpiitgsq.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.hnqzz.top/gtgpmqhecj.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.smart0.xyz/gttrfovxzt.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.iojbl.cn/gtnyopdwml.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.nanxinkj.top/gtubhzbrkp.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.sxryk.cn/gtzkodksei.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.zhijiandao.cn/gtytceukcc.html

[E19] 多行文本按行拆分
来源：http://hz.sysykeji.top/gtjouwonqe.html

Py:   s.splitlines()
来源：http://hz.haohaochexian.top/gtbiigahvs.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.mhx1999.top/gtsymmzpsi.html

JS:   s.split(/\r?\n/)
来源：http://hz.daxiang520.top/gtsznvszkh.html

TS:   s.split(/\r?\n/)
来源：http://hz.tanke756.top/gtkklfsbdq.html

Java: s.lines().toList()
来源：http://hz.jiagoushi.top/gtovrrjppi.html

Go:   strings.Split(s, "\n")
来源：http://hz.yueranfly.top/gtizojjdub.html

Ruby: s.lines
来源：http://hz.zhengqikj.top/gtldqkwlfx.html

C#:   s.Split('\n')
来源：http://hz.tanke756.top/gtzkyknmyd.html

[E20] 判断字符串是否为空
来源：http://hz.wangdashe.top/gtsrrfayvj.html

Py:   if not s:
来源：http://hz.ydzc1.top/gtirbgzsph.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.snrcjt.cn/gtlkomtbmf.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.daria6918.cn/gtdhohizoa.html

TS:   if (s === "") {}
来源：http://hz.zhongyouzk.top/gtrmjsxtax.html

Java: if (s.isEmpty()) {}
来源：http://hz.redwolf501.top/gtunphzppn.html

Go:   if s == "" {}
来源：http://hz.wangdashe.top/gtlhjdrmhf.html

Ruby: if s.empty?
来源：http://hz.xuetiantiany.cn/gtljzdrjkf.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.sysykeji.top/gtbwsjrnde.html

[E21] 超长截断加省略号
来源：http://hz.xziqi.cn/gtxkzhrtzw.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.tanke756.top/gtdvvxpyob.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.yj202588.top/gtkrpgbdbv.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yj202588.top/gtzympsyya.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jiagoushi.top/gtvurindpa.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.meibo888.top/gtgawhgkun.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.sufxvd.cn/gthgpkwvfb.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.cdnleiting.top/gtvfztzbbt.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.yangfankeji.com/gtyrustqde.html

[E22] 字节长度与字符长度
来源：http://hz.jlsjyb.cn/gttsujdiao.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.hongshengwenyu.top/gtsraxpduc.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zhaomingkeji.xyz/gteelrrsvg.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.vqdsnc.cn/gtxvkgjeky.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.snrcjt.cn/gtvtnsmjwu.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.ywan-chungtsiang.top/gthlyxuost.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.9152youxi.cn/gtesodvbmf.html

Ruby: s.bytesize;  s.length
来源：http://hz.jiagoushi.top/gtysxxwjgm.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.ivvv.top/gtkbxbxjij.html

================================================================================
来源：http://hz.tanke756.top/gtziaigdtw.html

F. 文件与目录
来源：http://hz.jqgfzy.top/gtplkwjytf.html

================================================================================
来源：http://hz.xinyue.icu/gtalmwmekb.html

[F01] 读取整个文件
来源：http://hz.52xcode.cn/gtbpdgrhgh.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.feifeiyinyue.top/gttwtukcnt.html

PHP:  file_get_contents("a.txt");
来源：http://hz.tanke756.top/gtvkscrlgd.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.zhijiandao.cn/gtcxhmmryu.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.sxryk.cn/gtzxpcinpj.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.jqgfzy.top/gtxwwgvjxv.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.nwbrower.top/gtnqdcdesh.html

Ruby: File.read("a.txt")
来源：http://hz.9152youxi.cn/gtjucyfsjx.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.zhaomingkeji.xyz/gtymycxcpk.html

[F02] 逐行读取文件
来源：http://hz.shzxlz.cn/gtvhvijcvw.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.tianlin.xyz/gtunossvcn.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.jqgufenzy.top/gtkfhkwsva.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.cqqwz.cn/gtmddcanzi.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yongpay.top/gtbmatxano.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.tanke756.top/gtfnpkhdfj.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.cucudq.cn/gtrtxulfrm.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.svipenyu.cn/gtwysjrojx.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.yangfankeji.com/gtxonlucok.html

[F03] 写入文件（覆盖）
来源：http://hz.ehwqpu.com/gtzmviimwj.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.shanyushiyangkeji.top/gtahwfojwi.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.jinqigufen.top/gtnesccxkf.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.hongshengwenyu.top/gtcmymodra.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yongpay.top/gttotjrpyb.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.yueranfly.top/gtpbrddavk.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.shuidangran.top/gtcohcenlg.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.zhiwuduotai.top/gtcaqygwwd.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.fzhhl.top/gtojcakfld.html

[F04] 追加写入文件
来源：http://hz.cqqwz.cn/gtnqdqkmro.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.nwbrower.top/gtrrdedghq.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.316326.xyz/gtujypdqhj.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.fzhhl.top/gtiunybqns.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.hnxiangtu.top/gtsrqtjjnl.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.ivvv.top/gtjxedkhpk.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.guowangkeji.top/gtbttlcror.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.daxiang520.top/gtbqemefsb.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.yongpay.top/gtoixljrpf.html

[F05] 判断文件或目录是否存在
来源：http://hz.smart0.xyz/gtvrwpglfx.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.cdnleiting.top/gtopasginu.html

PHP:  file_exists("a.txt");
来源：http://hz.zycfv.cn/gtoygalukf.html

JS:   fs.existsSync("a.txt")
来源：http://hz.ivvv.top/gttzzsdhdw.html

TS:   fs.existsSync("a.txt")
来源：http://hz.bjfxy.top/gtdbibmgoc.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.smart0.xyz/gtepuyeleu.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.dianchejie.cn/gtgbtzqgna.html

Ruby: File.exist?("a.txt")
来源：http://hz.gogol.net.cn/gtabvubeob.html

C#:   File.Exists("a.txt")
来源：http://hz.zhiwuduotai.top/gtoryhcrcu.html

[F06] 删除文件
来源：http://hz.quarkkingdee.top/gthbcztckx.html

Py:   os.remove("a.txt")
来源：http://hz.xylfe.cn/gteskfuhlx.html

PHP:  unlink("a.txt");
来源：http://hz.hywenlv.cn/gtmgvijsqu.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.wangdashe.top/gtymllrxyt.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.yuxming.cn/gtxfdwwhyn.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.gogol.net.cn/gtbhiptebc.html

Go:   os.Remove("a.txt")
来源：http://hz.shzxlz.cn/gtajewepnt.html

Ruby: File.delete("a.txt")
来源：http://hz.sysykeji.top/gtfnxicvdg.html

C#:   File.Delete("a.txt");
来源：http://hz.xinyue.icu/gtuidzjgnf.html

[F07] 创建目录（含多级）
来源：http://hz.chenjidiqi.icu/gtaqxdhtcs.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.wangshuangyany.cn/gthmcbajga.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.andypj.xyz/gtsspyhzzd.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.nanxuanxn.top/gtdstgtfwn.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.sysykeji.top/gtunpidzme.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.yuxming.cn/gtmcduocna.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.iojbl.cn/gtexdsroap.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.xinyue.icu/gtiequzagp.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.shangyingyoupin.top/gtiaxaagcr.html

[F08] 遍历目录
来源：http://hz.shzxlz.cn/gtqufalcey.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.gogol.net.cn/gthzmzylvu.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.daria6918.cn/gticzeacua.html

JS:   fs.readdirSync("dir")
来源：http://hz.nanxinkj.top/gtqqazsjud.html

TS:   fs.readdirSync("dir")
来源：http://hz.zhoulong.xyz/gtqciyqgga.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.jinyuanbaomall.cn/gtazyderbf.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.gzhubu.top/gtvsptclyw.html

Ruby: Dir.children("dir")
来源：http://hz.daxiang520.top/gtydlkunvh.html

C#:   Directory.GetFiles("dir")
来源：http://hz.sysykeji.top/gtcqfuenux.html

[F09] 获取文件大小
来源：http://hz.zhixingplan.top/gtgmlscsnn.html

Py:   os.path.getsize("a.txt")
来源：http://hz.shangyingyoupin.top/gtjffnucit.html

PHP:  filesize("a.txt");
来源：http://hz.zdqjudy.top/gtkykhybsp.html

JS:   fs.statSync("a.txt").size
来源：http://hz.snrcjt.cn/gtaxuocjqk.html

TS:   fs.statSync("a.txt").size
来源：http://hz.316326.xyz/gtbdgnnhwt.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.cqqwz.cn/gtmufkfgmu.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.yj20258.top/gtenshqjyl.html

Ruby: File.size("a.txt")
来源：http://hz.c1oappe.top/gtfbizgxrx.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.cqqwz.cn/gtafzzurnz.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.sysykeji.top/gtdzqzckkc.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.chenlongwang.top/gtmhexphbz.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.52xcode.cn/gtcbztixyw.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.redwolf501.top/gtlwtkdvuw.html

TS:   path.extname("a.txt")
来源：http://hz.9152youxi.cn/gtxsqkwygg.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.hfpthk.cn/gtjwbkcxas.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.kuanghao11.cn/gtgfkpqheo.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.meibo888.top/gtqrpyceae.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.jinghuilouyu.cn/gtycpzrfks.html

[F11] 复制与移动文件
来源：http://hz.yonumen.top/gtxxbtmwal.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.fengsongda.top/gtlanomzyz.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.jiagoushi.top/gtiobdupjm.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.hywenlv.cn/gtqojqkyzt.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.dianchejie.cn/gtnywjhfur.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.ehwqpu.com/gtyzztjpuh.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.shanyushiyangtech.top/gtumwolicb.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.jinyuanbaomall.cn/gtavpatdjx.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.9152youxi.cn/gtjfpttlnz.html

[F12] CSV 读写
来源：http://hz.zhaomingkeji.xyz/gtsrcalevz.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.gogol.net.cn/gtfghmjhfr.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.yuanzhike.top/gtpumcfios.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.sysykeji.top/gtxjvjriwh.html

TS:   // 同上
来源：http://hz.chenlongwang.top/gtnntjsokv.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.kuanghao11.cn/gtnzmfjqxu.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.ehwqpu.com/gtmfrpcuhc.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.andypj.xyz/gtzqkbuknl.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.yonumen.top/gtpfgtxtrx.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtsxjengkd.html

G. 面向对象
来源：http://hz.cucudq.cn/gtzdktvqph.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gticvkanev.html

[G01] 定义类
来源：http://hz.jinqigfzy.top/gteongkmfn.html

Py:   class User: pass
来源：http://hz.gaohongyu789.top/gtlmxewoxa.html

PHP:  class User {}
来源：http://hz.hysaishi.cn/gtttbxkeyl.html

JS:   class User {}
来源：http://hz.gogol.net.cn/gttcxakeww.html

TS:   class User { name: string = ""; }
来源：http://hz.cqqwz.cn/gtxvlfsccq.html

Java: class User {}
来源：http://hz.birdmap.top/gtvgnefryo.html

Go:   type User struct { Name string }
来源：http://hz.snrcjt.cn/gtlqfailic.html

Ruby: class User; end
来源：http://hz.gogol.net.cn/gtjnrtginr.html

C#:   class User {}
来源：http://hz.yonumen.top/gttxrrxdoa.html

[G02] 构造函数
来源：http://hz.cdnleiting.top/gtaqmigoju.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.daxiang520.top/gtkbznobvh.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.zhongyouzk.top/gtjyprlcyt.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.zhongyouzk.top/gtmqneyvwr.html

TS:   constructor(public name: string) {}
来源：http://hz.shanyushiyangtech.top/gtqdarpaye.html

Java: User(String name) { this.name = name; }
来源：http://hz.fzhhl.top/gtnxnekcnp.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.yj20258888.top/gtzsuxwvco.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.gotoacloud.top/gtqmljalji.html

C#:   public User(string name) { Name = name; }
来源：http://hz.yangfankeji.com/gtjjhvdkal.html

[G03] 实例属性
来源：http://hz.meibo888.top/gtsaerskem.html

Py:   self.name = "x"
来源：http://hz.shzxlz.cn/gtccsvvwoz.html

PHP:  public string $name = "x";
来源：http://hz.xinyue.icu/gtjgdcuphj.html

JS:   this.name = "x";
来源：http://hz.nwbrower.top/gtdzxphsok.html

TS:   name: string = "x";
来源：http://hz.redwolf501.top/gtwzqkcopu.html

Java: private String name;
来源：http://hz.yongpay.top/gtxuxdpsdr.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.smart0.xyz/gtwgtoytec.html

Ruby: @name = "x"
来源：http://hz.316326.xyz/gtyitkaozm.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.birdmap.top/gtsppvpixg.html

[G04] 定义方法
来源：http://hz.ppjwa.cn/gtunaylzqy.html

Py:   def greet(self): return self.name
来源：http://hz.yj20258888.top/gtzkvozgrw.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.redwolf501.top/gtpyftebla.html

JS:   greet() { return this.name; }
来源：http://hz.meibo888.top/gtsvqrloeh.html

TS:   greet(): string { return this.name; }
来源：http://hz.dashuyun.cn/gtyzkcosem.html

Java: String greet() { return name; }
来源：http://hz.shuidangran.top/gtakjryaqm.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.guannengcc.top/gtsprwpcji.html

Ruby: def greet; @name; end
来源：http://hz.aibaodan.cn/gtgzvwcbcw.html

C#:   public string Greet() => Name;
来源：http://hz.zhongyouzk.top/gtyegzangj.html

[G05] 继承
来源：http://hz.cucudq.cn/gtimmwxavc.html

Py:   class Admin(User): pass
来源：http://hz.jinqigfzy.top/gtllefiuyp.html

PHP:  class Admin extends User {}
来源：http://hz.nanxuanxn.top/gtcdinlbea.html

JS:   class Admin extends User {}
来源：http://hz.ivvv.top/gtgcxajyvd.html

TS:   class Admin extends User {}
来源：http://hz.yongpay.top/gtexghxqfp.html

Java: class Admin extends User {}
来源：http://hz.zhoulong.xyz/gtlhtengqe.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.jinqigfzy.top/gtfxbqycni.html

Ruby: class Admin < User; end
来源：http://hz.yuanzhike.top/gtleexlcgp.html

C#:   class Admin : User {}
来源：http://hz.cqqwz.cn/gtrbjczgcl.html

[G06] 重写方法
来源：http://hz.hammf.cn/gtuikqbqib.html

Py:   def greet(self): return "admin"
来源：http://hz.zhengqikj.top/gtsxdssjqn.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.jqgufenzy.top/gtwzjwbobc.html

JS:   greet() { return "admin"; }
来源：http://hz.gzhubu.top/gtvhqtraxa.html

TS:   greet(): string { return "admin"; }
来源：http://hz.haohaochexian.top/gtacufufig.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.pengpengdd.cyou/gtcgeigugl.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.zhiwuduotai.top/gtjdecfhko.html

Ruby: def greet; "admin"; end
来源：http://hz.hywenlv.cn/gttwgllcdk.html

C#:   public override string Greet() => "admin";
来源：http://hz.shanyushiyangkeji.top/gtcufujteq.html

[G07] 调用父类方法
来源：http://hz.shanyushiyangtech.top/gtmdctroiw.html

Py:   super().greet()
来源：http://hz.feifeiyinyue.top/gtnlsbtwiz.html

PHP:  parent::greet();
来源：http://hz.gaohongyu789.top/gtyaujcwky.html

JS:   super.greet();
来源：http://hz.andypj.xyz/gtzxxtywip.html

TS:   super.greet();
来源：http://hz.birdmap.top/gtvzjroaqd.html

Java: super.greet();
来源：http://hz.xylfe.cn/gtjnsdeudh.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.pengpengdd.cyou/gtwjkzlzgi.html

Ruby: super
来源：http://hz.aizwys.cn/gtgkqivaod.html

C#:   base.Greet();
来源：http://hz.haohaochexian.top/gtuslntpgq.html

[G08] 静态方法与属性
来源：http://hz.zhoulong.xyz/gthjfxfacm.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.shangyingyoupin.top/gtnaahuhmw.html

PHP:  public static function f() {}
来源：http://hz.cdnleiting.top/gtylywhvfg.html

JS:   static f() {}
来源：http://hz.pengpengdd.cyou/gtfsnywqwc.html

TS:   static f(): void {}
来源：http://hz.jqgufenzy.top/gtmlyfkcrz.html

Java: static void f() {}
来源：http://hz.zhengqikj.top/gtjhbatoma.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.shanyushiyangkeji.top/gtbrvbnjkf.html

Ruby: def self.f; end
来源：http://hz.ehwqpu.com/gtxzguhuix.html

C#:   public static void F() {}
来源：http://hz.havefunace.top/gtubejigyj.html

[G09] 接口 / 抽象类
来源：http://hz.cashguo.top/gtcdicfdex.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.wangdashe.top/gtgunpwbyx.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.xingfuxueyuan.xyz/gttnbnnxyv.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.ybcxt.top/gtyrahzlzp.html

TS:   interface Shape { area(): number; }
来源：http://hz.gogol.net.cn/gtwdpkhdew.html

Java: interface Shape { double area(); }
来源：http://hz.gogol.net.cn/gtrmrqzwrf.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.ybcxt.top/gtmfpvhkmq.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.guowangkeji.top/gtcxusnkic.html

C#:   interface IShape { double Area(); }
来源：http://hz.316326.xyz/gtapxvrrqv.html

[G10] 访问控制
来源：http://hz.jyoumei.cn/gtzchrmtta.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.mhx1999.top/gthssyhgje.html

PHP:  public / protected / private
来源：http://hz.yj20258888.top/gtqncclamw.html

JS:   #private 字段；其余公开
来源：http://hz.yangfankeji.com/gtfetvctpa.html

TS:   public / protected / private
来源：http://hz.52xcode.cn/gttoxzemjb.html

Java: public / protected / private / 默认包级
来源：http://hz.zhongyouzk.top/gttfkuvvkg.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.gaohongyu789.top/gtepxkhfrx.html

Ruby: public / protected / private
来源：http://hz.nanxinkj.top/gtnplqaaey.html

C#:   public / protected / private / internal
来源：http://hz.chenlongwang.top/gtoxenbmzz.html

[G11] getter / setter
来源：http://hz.sweek.top/gtvbmrpedd.html

Py:   @property 与 @x.setter
来源：http://hz.dianchejie.cn/gtjgtznvce.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.havefunace.top/gtofrheulj.html

JS:   get name() { return this._name; }
来源：http://hz.vqdsnc.cn/gttykjzvzj.html

TS:   get name(): string { return this._name; }
来源：http://hz.shuidangran.top/gtcnwcsxfx.html

Java: public String getName() { return name; }
来源：http://hz.birdmap.top/gtbroxjogd.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.pengpengdd.cyou/gtljuegxvf.html

Ruby: attr_accessor :name
来源：http://hz.jqgfzy.top/gtmkmffqot.html

C#:   public string Name { get; set; }
来源：http://hz.cucudq.cn/gttpvinxlm.html

[G12] 对象转字符串
来源：http://hz.zhixingplan.top/gtktrqxmjl.html

Py:   def __str__(self): return self.name
来源：http://hz.yuanzhike.top/gttisyujic.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.yangfankeji.com/gtqkicjdgl.html

JS:   toString() { return this.name; }
来源：http://hz.ppjwa.cn/gtwtjeeetf.html

TS:   toString(): string { return this.name; }
来源：http://hz.smart0.xyz/gtehihizpu.html

Java: @Override public String toString() { return name; }
来源：http://hz.hfpthk.cn/gtfbiksznp.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.pycfn.com/gtsfkdedaw.html

Ruby: def to_s; @name; end
来源：http://hz.zdqjudy.top/gtvwmylrju.html

C#:   public override string ToString() => Name;
来源：http://hz.hongshengwenyu.top/gtfsfgtpyc.html

[G13] 判断对象类型
来源：http://hz.wangdashe.top/gthgaluthp.html

Py:   isinstance(u, User)
来源：http://hz.sysykeji.top/gtpygrgpai.html

PHP:  $u instanceof User
来源：http://hz.vqdsnc.cn/gtsdwhnjqx.html

JS:   u instanceof User
来源：http://hz.nanxinkj.top/gtnbhiqxyk.html

TS:   u instanceof User
来源：http://hz.fengsongda.top/gtvnmmyjet.html

Java: u instanceof User
来源：http://hz.cheryme.top/gtmqayqlth.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.hysaishi.cn/gtgbhfqgii.html

Ruby: u.is_a?(User)
来源：http://hz.jinqigufen.top/gteuxilyfz.html

C#:   u is User
来源：http://hz.xinyue.icu/gtpyncnzoe.html

[G14] 数据类 / record
来源：http://hz.zycfv.cn/gtsirpproc.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.zhixingplan.top/gtbhdeozib.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.yj202588.top/gtnasmpizk.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.jiagoushi.top/gtvtzcsnrt.html


<!-- 参考信息 -->