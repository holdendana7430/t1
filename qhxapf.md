代发 wailian999

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.jqgufenzy.top/gtnhhwysyn.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.tianlin.xyz/gtrnjnbmzg.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.cashguo.top/gtrlmznidn.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.cucudq.cn/gtftwbupcs.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.52xcode.cn/gtbgxjmhtz.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.wangdashe.top/gtylsjisxz.html

Ruby: s.capitalize
来源：http://hz.xuetiantiany.cn/gthyzaarqs.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.meibo888.top/gtffkutdck.html

[E18] 模板占位符替换
来源：http://hz.ydzc1.top/gtojizgsop.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.xuetiantiany.cn/gtrqyznmcg.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.haohaochexian.top/gtikxzenht.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.jyoumei.cn/gtrsiekvau.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.ehwqpu.com/gtltbnzjng.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.aizwys.cn/gtatgixdme.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.jinghuilouyu.cn/gtgnhiobep.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.fzhhl.top/gtyvykvulv.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.jlsjyb.cn/gtahxamrud.html

[E19] 多行文本按行拆分
来源：http://hz.jinghuilouyu.cn/gtpyqnjxvw.html

Py:   s.splitlines()
来源：http://hz.jqgufenzy.top/gtpjxmtqhf.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.sxryk.cn/gtcnmfrlip.html

JS:   s.split(/\r?\n/)
来源：http://hz.snrcjt.cn/gtblrdgqcc.html

TS:   s.split(/\r?\n/)
来源：http://hz.sxryk.cn/gtdjqoilcl.html

Java: s.lines().toList()
来源：http://hz.jlsjyb.cn/gtkqljxzsf.html

Go:   strings.Split(s, "\n")
来源：http://hz.fengsongda.top/gtsxvklswl.html

Ruby: s.lines
来源：http://hz.jyoumei.cn/gtsbcqbriz.html

C#:   s.Split('\n')
来源：http://hz.yj20258888.top/gteixasscl.html

[E20] 判断字符串是否为空
来源：http://hz.c1oappe.top/gtasaddjna.html

Py:   if not s:
来源：http://hz.yvedp.cn/gtnxrfpegi.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.zhijiandao.cn/gtkytlakpt.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.chenzaomai.com/gtikerosij.html

TS:   if (s === "") {}
来源：http://hz.jyoumei.cn/gtjcoyidvd.html

Java: if (s.isEmpty()) {}
来源：http://hz.shzxlz.cn/gternkbqxp.html

Go:   if s == "" {}
来源：http://hz.tian-w.cn/gtjfrrftmv.html

Ruby: if s.empty?
来源：http://hz.316326.xyz/gtpduyttqy.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.hnxiangtu.top/gtaphtfwhi.html

[E21] 超长截断加省略号
来源：http://hz.jiagoushi.top/gtwbacrmoq.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.chenjidiqi.icu/gtqlepopav.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.hongshengwenyu.top/gtxebubrgx.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.shanyushiyangkeji.top/gtsmifwbvw.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.zhengqikj.top/gtpjetyovb.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.aizwys.cn/gtktkrtwkx.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.xuetiantiany.cn/gtrsroqxfa.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.feifeiyinyue.top/gtlwaxljbj.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.shanyushiyangtech.top/gtcxclvwoq.html

[E22] 字节长度与字符长度
来源：http://hz.52xcode.cn/gtgqwxnzzp.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.zhiwuduotai.top/gtvkfufejv.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yangfankeji.com/gtamguxktf.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jinyuanbaomall.cn/gthkecugkt.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.sweek.top/gtnbygzjbs.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.shuidangran.top/gtcbdwsouu.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.zhongyouzk.top/gtydbytfou.html

Ruby: s.bytesize;  s.length
来源：http://hz.cqqwz.cn/gtrorljool.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.jinghuilouyu.cn/gtprjckhdr.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtcttdbzao.html

F. 文件与目录
来源：http://hz.c1oappe.top/gtwnqhlumk.html

================================================================================
来源：http://hz.fzhhl.top/gtzwoadknb.html

[F01] 读取整个文件
来源：http://hz.0kj1m.cn/gtpmujelvh.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.quarkkingdee.top/gtugwgdvrr.html

PHP:  file_get_contents("a.txt");
来源：http://hz.gotoacloud.top/gtjnmlujtl.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.gogol.net.cn/gtrfaknmph.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.sxryk.cn/gtegxdxhhx.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.yj20258888.top/gtdlkwqhbu.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.zhongyouzk.top/gtbyeudrgs.html

Ruby: File.read("a.txt")
来源：http://hz.hfpthk.cn/gtkoizjmdl.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.meibo888.top/gtwglggmnn.html

[F02] 逐行读取文件
来源：http://hz.gaohongyu789.top/gtmshqvqew.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.shanyushiyangtech.top/gtdzxutjnt.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.zhengqikj.top/gtmtivwxjd.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zhoulong.xyz/gtbykbkvqt.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.hammf.cn/gtpsspuahk.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.yj20258.top/gtbjneieek.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.pycfn.com/gtkqvvmudk.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.tianlin.xyz/gtyikykmrv.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.vqdsnc.cn/gtpnpcytsk.html

[F03] 写入文件（覆盖）
来源：http://hz.hywenlv.cn/gtwbwoakwz.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.xuanzx.com/gtvinpknwp.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.jinqigufen.top/gtmzzebiyp.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.tianlin.xyz/gtuhoisvpb.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.shanyushiyangkeji.top/gtswpcdgpr.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.gaohongyu789.top/gterishlhc.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.xingfuxueyuan.xyz/gtozbzdhrb.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.tian-w.cn/gtfydeixyl.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.daria6918.cn/gtkxtvqzxu.html

[F04] 追加写入文件
来源：http://hz.aizwys.cn/gtzjidjqxi.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.xingfuxueyuan.xyz/gtwjtxymac.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.nanxinkj.top/gtmeltvkck.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.hfpthk.cn/gtfuhebxrj.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.9152youxi.cn/gtroctnwkp.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.aibaodan.cn/gticankpwn.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.zhongyouzk.top/gtiimbnupb.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.nanxinkj.top/gtiuoduxoi.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.jqgfzy.top/gtkwrxfxpm.html

[F05] 判断文件或目录是否存在
来源：http://hz.meibo888.top/gtdiejxems.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.guannengcc.top/gtgvaqlsul.html

PHP:  file_exists("a.txt");
来源：http://hz.quarkkingdee.top/gtkybvccen.html

JS:   fs.existsSync("a.txt")
来源：http://hz.yonumen.top/gtyoqjfmen.html

TS:   fs.existsSync("a.txt")
来源：http://hz.yueranfly.top/gtgrhoyeqe.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.fengsongda.top/gtcayjqokd.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.xuanzx.com/gtvbdixhyb.html

Ruby: File.exist?("a.txt")
来源：http://hz.ppjwa.cn/gtyiqkiwfq.html

C#:   File.Exists("a.txt")
来源：http://hz.jlsjyb.cn/gtbzbamshn.html

[F06] 删除文件
来源：http://hz.dashuyun.cn/gtywxgdzeo.html

Py:   os.remove("a.txt")
来源：http://hz.vqdsnc.cn/gtkglpavlm.html

PHP:  unlink("a.txt");
来源：http://hz.sysykeji.top/gtobhqlcie.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.xylfe.cn/gtfqowabkp.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.shangyingyoupin.top/gtuhlzywmx.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.gotoacloud.top/gtvfyrigky.html

Go:   os.Remove("a.txt")
来源：http://hz.cucudq.cn/gtgsrznimu.html

Ruby: File.delete("a.txt")
来源：http://hz.wangdashe.top/gttdbbfmzj.html

C#:   File.Delete("a.txt");
来源：http://hz.haohaochexian.top/gtrnfzvkcm.html

[F07] 创建目录（含多级）
来源：http://hz.yj20258888.top/gtqwbmsrrr.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.zhijiandao.cn/gtdnarnkmz.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.cheryme.top/gtgrlyflyo.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zhengqikj.top/gtvxnhvmph.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.bjfxy.top/gtmcmglowt.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.haohaochexian.top/gtpxeujrwy.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.gaohongyu789.top/gtyzkovxac.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.jinqigfzy.top/gtgyezpwkb.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.ivvv.top/gtjbwnuoeg.html

[F08] 遍历目录
来源：http://hz.xuanzx.com/gtbmfbgdns.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.aizwys.cn/gtgecmjlzf.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.nanxuanxn.top/gtdvcnpybk.html

JS:   fs.readdirSync("dir")
来源：http://hz.zhoulong.xyz/gtzouxjzbu.html

TS:   fs.readdirSync("dir")
来源：http://hz.havefunace.top/gthoalkkzn.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.daria6918.cn/gtafsorqjg.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.svipenyu.cn/gtejaicguf.html

Ruby: Dir.children("dir")
来源：http://hz.9152youxi.cn/gtatbayxeo.html

C#:   Directory.GetFiles("dir")
来源：http://hz.chenlongwang.top/gttahyhdca.html

[F09] 获取文件大小
来源：http://hz.chenjidiqi.icu/gtvnksptzt.html

Py:   os.path.getsize("a.txt")
来源：http://hz.guannengcc.top/gtdpnibpfe.html

PHP:  filesize("a.txt");
来源：http://hz.gogol.net.cn/gtgtehkxav.html

JS:   fs.statSync("a.txt").size
来源：http://hz.yvedp.cn/gtfydlmwna.html

TS:   fs.statSync("a.txt").size
来源：http://hz.zhixingplan.top/gtgpgktanr.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.cheryme.top/gtprzvfkoz.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.zhixingplan.top/gtzozgdytz.html

Ruby: File.size("a.txt")
来源：http://hz.yueranfly.top/gtrmpiesdr.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.redwolf501.top/gtmuweiwxu.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.ydjk.org.cn/gtmyaypboz.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.daxiang520.top/gtsbwxsswu.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.vqdsnc.cn/gtpnmpmxma.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.meibo888.top/gtmsxeommr.html

TS:   path.extname("a.txt")
来源：http://hz.sysykeji.top/gtaszntxyy.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.aibaodan.cn/gtxjzfhnfb.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.gaohongyu789.top/gtoufdqklo.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.cheryme.top/gthcfovxzy.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.fengsongda.top/gtjgrudyjv.html

[F11] 复制与移动文件
来源：http://hz.yuxming.cn/gtshlwrxmq.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.xuetiantiany.cn/gtmappuugg.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.zycfv.cn/gtqzfhasnj.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.fzhhl.top/gtqrfhnmbc.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.9152youxi.cn/gtswunhwmu.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.gaohongyu789.top/gtrijtckpo.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.cdnleiting.top/gtrrhnfzki.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.nanxuanxn.top/gtpuhiihuu.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.sysykeji.top/gtwqddsfyo.html

[F12] CSV 读写
来源：http://hz.guannengcc.top/gtpsepajud.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.sxryk.cn/gtyafjfqpa.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.ydzc1.top/gtihfysmrd.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.nanxinkj.top/gtjylyogqs.html

TS:   // 同上
来源：http://hz.gotoacloud.top/gtpsrkylvx.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.chenzaomai.com/gtrbrabulu.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.jlsjyb.cn/gtacbaejhq.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.zycfv.cn/gtzfrgkcuv.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.jinyuanbaomall.cn/gtkvuvqhnq.html

================================================================================
来源：http://hz.yj202588.top/gtumouxhxv.html

G. 面向对象
来源：http://hz.xinyue.icu/gtwppkhxfs.html

================================================================================
来源：http://hz.hfpthk.cn/gtoipcfuyt.html

[G01] 定义类
来源：http://hz.guowangkeji.top/gtoibvdjic.html

Py:   class User: pass
来源：http://hz.zhengqikj.top/gtyfwvdvzz.html

PHP:  class User {}
来源：http://hz.aibaodan.cn/gtntiomxuc.html

JS:   class User {}
来源：http://hz.xylfe.cn/gtzmaldqfp.html

TS:   class User { name: string = ""; }
来源：http://hz.yj20258.top/gtjjazpbch.html

Java: class User {}
来源：http://hz.kuanghao11.cn/gtuhwvuhlh.html

Go:   type User struct { Name string }
来源：http://hz.wangdashe.top/gtevletqah.html

Ruby: class User; end
来源：http://hz.hnxiangtu.top/gtbhckxpjn.html

C#:   class User {}
来源：http://hz.sxryk.cn/gtqjaxzaan.html

[G02] 构造函数
来源：http://hz.cheryme.top/gtpnntuokb.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.wangdashe.top/gtzudzvuqd.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.snrcjt.cn/gtyiotqhfl.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.aibaodan.cn/gtyrnsugsk.html

TS:   constructor(public name: string) {}
来源：http://hz.xuetiantiany.cn/gthfmbdhcv.html

Java: User(String name) { this.name = name; }
来源：http://hz.feifeiyinyue.top/gtlosbenid.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.shuidangran.top/gtuxgornij.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.0kj1m.cn/gtnmytthik.html

C#:   public User(string name) { Name = name; }
来源：http://hz.daria6918.cn/gtyhjemzkv.html

[G03] 实例属性
来源：http://hz.jiagoushi.top/gtzgdwrewx.html

Py:   self.name = "x"
来源：http://hz.xuanzx.com/gtmqpfqlyq.html

PHP:  public string $name = "x";
来源：http://hz.yj202588.top/gttdlcomnl.html

JS:   this.name = "x";
来源：http://hz.ydjk.org.cn/gtdcpprsgo.html

TS:   name: string = "x";
来源：http://hz.pycfn.com/gtxmtmmduk.html

Java: private String name;
来源：http://hz.bjfxy.top/gtpgnkmfvs.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.aizwys.cn/gtfjrvryqw.html

Ruby: @name = "x"
来源：http://hz.hysaishi.cn/gtrpueelua.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.aibaodan.cn/gtedpeqtoi.html

[G04] 定义方法
来源：http://hz.jqgfzy.top/gtrjsvrqfr.html

Py:   def greet(self): return self.name
来源：http://hz.dashuyun.cn/gtuzdtqqqo.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.shanyushiyangtech.top/gtlliujzlx.html

JS:   greet() { return this.name; }
来源：http://hz.zhiwuduotai.top/gticfvefcm.html

TS:   greet(): string { return this.name; }
来源：http://hz.tianlin.xyz/gtaarcxbst.html

Java: String greet() { return name; }
来源：http://hz.zhongyouzk.top/gtukgemrfl.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.ppjwa.cn/gtmrxvyfdd.html

Ruby: def greet; @name; end
来源：http://hz.feifeiyinyue.top/gtowrjzaad.html

C#:   public string Greet() => Name;
来源：http://hz.gogol.net.cn/gtwmxoymns.html

[G05] 继承
来源：http://hz.hnqzz.top/gthlnepuuy.html

Py:   class Admin(User): pass
来源：http://hz.tian-w.cn/gtxgbqhjip.html

PHP:  class Admin extends User {}
来源：http://hz.shanyushiyangtech.top/gtlwmpsgxg.html

JS:   class Admin extends User {}
来源：http://hz.yj20258888.top/gtstoeougv.html

TS:   class Admin extends User {}
来源：http://hz.zhongyouzk.top/gtyrtmypfb.html

Java: class Admin extends User {}
来源：http://hz.hammf.cn/gtqjhoxzbh.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.ivvv.top/gtcsfijzbd.html

Ruby: class Admin < User; end
来源：http://hz.pycfn.com/gtuoxkvvmz.html

C#:   class Admin : User {}
来源：http://hz.jlsjyb.cn/gthjmzdioa.html

[G06] 重写方法
来源：http://hz.jinghuilouyu.cn/gtojobqpye.html

Py:   def greet(self): return "admin"
来源：http://hz.316326.xyz/gtcknrhasv.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.cheryme.top/gtrtkkmpoe.html

JS:   greet() { return "admin"; }
来源：http://hz.jinyuanbaomall.cn/gttlmctabi.html

TS:   greet(): string { return "admin"; }
来源：http://hz.guowangkeji.top/gtlrymqado.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.hongshengwenyu.top/gtfmvyzkzx.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.9152youxi.cn/gtqyeszaqv.html

Ruby: def greet; "admin"; end
来源：http://hz.aizwys.cn/gtnhwppwba.html

C#:   public override string Greet() => "admin";
来源：http://hz.hongshengwenyu.top/gtceihjrhs.html

[G07] 调用父类方法
来源：http://hz.tianlin.xyz/gtunsqgxdw.html

Py:   super().greet()
来源：http://hz.9152youxi.cn/gtsqdbwxfr.html

PHP:  parent::greet();
来源：http://hz.yanxiufei.cn/gtawjogerg.html

JS:   super.greet();
来源：http://hz.smart0.xyz/gtttqpymvk.html

TS:   super.greet();
来源：http://hz.redwolf501.top/gtecigfpaw.html

Java: super.greet();
来源：http://hz.guowangkeji.top/gtfwapmsrf.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.sysykeji.top/gtpfvzwyxv.html

Ruby: super
来源：http://hz.gaohongyu789.top/gtpglrzvor.html

C#:   base.Greet();
来源：http://hz.chenjidiqi.icu/gttzwcsnrt.html

[G08] 静态方法与属性
来源：http://hz.ivvv.top/gtjvgyimyf.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.aizwys.cn/gtdlwtpxeb.html

PHP:  public static function f() {}
来源：http://hz.jinyuanbaomall.cn/gtcdimdhfu.html

JS:   static f() {}
来源：http://hz.cqqwz.cn/gtaycefawe.html

TS:   static f(): void {}
来源：http://hz.yueranfly.top/gtmqrtnryi.html

Java: static void f() {}
来源：http://hz.hywenlv.cn/gtqqxorutz.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.jlsjyb.cn/gtlurfmnye.html

Ruby: def self.f; end
来源：http://hz.aizwys.cn/gtqpyjccjm.html

C#:   public static void F() {}
来源：http://hz.svipenyu.cn/gttcufbayy.html

[G09] 接口 / 抽象类
来源：http://hz.jqgfzy.top/gtzpihogrw.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.cheryme.top/gtjmlermcs.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.gotoacloud.top/gtzanawnrt.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.gaohongyu789.top/gtstndteko.html

TS:   interface Shape { area(): number; }
来源：http://hz.sysykeji.top/gtwnkuyzzx.html

Java: interface Shape { double area(); }
来源：http://hz.ehwqpu.com/gtzbltsvsr.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.sweek.top/gtlxgyrsai.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.yuxming.cn/gtxcgaiahy.html

C#:   interface IShape { double Area(); }
来源：http://hz.jianghu66.top/gtnodwawxb.html

[G10] 访问控制
来源：http://hz.sufxvd.cn/gtqcxcygei.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.c1oappe.top/gtylkfqsig.html

PHP:  public / protected / private
来源：http://hz.sxryk.cn/gtnerfrfve.html

JS:   #private 字段；其余公开
来源：http://hz.aibaodan.cn/gtfyuenhyc.html

TS:   public / protected / private
来源：http://hz.cashguo.top/gtpauolgrk.html

Java: public / protected / private / 默认包级
来源：http://hz.cucudq.cn/gtwarimbki.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.tanke756.top/gtonxasrec.html

Ruby: public / protected / private
来源：http://hz.ppjwa.cn/gtgfwjiwam.html

C#:   public / protected / private / internal
来源：http://hz.sysykeji.top/gtbdfhhmrj.html

[G11] getter / setter
来源：http://hz.yuanzhike.top/gtsiehqyso.html

Py:   @property 与 @x.setter
来源：http://hz.meibo888.top/gtmgqvjuxi.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.chenjidiqi.icu/gtrqzbiisu.html

JS:   get name() { return this._name; }
来源：http://hz.ydzc1.top/gtcuhbbfze.html

TS:   get name(): string { return this._name; }
来源：http://hz.gzhubu.top/gtjhvhqltq.html

Java: public String getName() { return name; }
来源：http://hz.zycfv.cn/gtyizatfoh.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.yonumen.top/gtuitnuuen.html

Ruby: attr_accessor :name
来源：http://hz.chenjidiqi.icu/gtvittyyhm.html

C#:   public string Name { get; set; }
来源：http://hz.pengpengdd.cyou/gtfjzbzfbq.html

[G12] 对象转字符串
来源：http://hz.zhongyouzk.top/gtixstxkff.html

Py:   def __str__(self): return self.name
来源：http://hz.vqdsnc.cn/gtrpyqdcgb.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.chenjidiqi.icu/gtmjdfmazh.html

JS:   toString() { return this.name; }
来源：http://hz.zhiwuduotai.top/gtwrhojlro.html

TS:   toString(): string { return this.name; }
来源：http://hz.nanxuanxn.top/gtyilphvmm.html

Java: @Override public String toString() { return name; }
来源：http://hz.zdqjudy.top/gtuhlpuyzx.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.jianghu66.top/gtfgserunu.html

Ruby: def to_s; @name; end
来源：http://hz.dianchejie.cn/gtekoowivz.html

C#:   public override string ToString() => Name;
来源：http://hz.redwolf501.top/gtefliytku.html

[G13] 判断对象类型
来源：http://hz.xuanzx.com/gtlbxcbecc.html

Py:   isinstance(u, User)
来源：http://hz.yueranfly.top/gtschjwogt.html

PHP:  $u instanceof User
来源：http://hz.pycfn.com/gtnbaqdibq.html

JS:   u instanceof User
来源：http://hz.yangfankeji.com/gtjkqeojjq.html

TS:   u instanceof User
来源：http://hz.jiagoushi.top/gtyrzasquz.html

Java: u instanceof User
来源：http://hz.dashuyun.cn/gtxzvfugam.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.zhijiandao.cn/gtrftgdwzl.html

Ruby: u.is_a?(User)
来源：http://hz.pycfn.com/gtjgqteqqt.html

C#:   u is User
来源：http://hz.shzxlz.cn/gtqoisusbu.html

[G14] 数据类 / record
来源：http://hz.hongshengwenyu.top/gtciwmeutl.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.xuetiantiany.cn/gtdpipkebg.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.jqgfzy.top/gtjbbqkjny.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.dashuyun.cn/gtjbjuiejo.html

TS:   type User = { name: string; age: number };
来源：http://hz.zhaomingkeji.xyz/gtkpvpblqy.html

Java: record User(String name, int age) {}
来源：http://hz.bjfxy.top/gtqsdcilgz.html

Go:   type User struct { Name string; Age int }
来源：http://hz.yj20258888.top/gtrcgostpe.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.zhaomingkeji.xyz/gtkqtmddrm.html

C#:   record User(string Name, int Age);
来源：http://hz.birdmap.top/gtdavmkxkq.html

[G15] 枚举
来源：http://hz.zhaomingkeji.xyz/gtofgxuknp.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.cheryme.top/gtbskigcnu.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.zhaomingkeji.xyz/gtjbhmweir.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.ydzc1.top/gtbynoqjhw.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.xuanzx.com/gthoddflwc.html

Java: enum Color { RED, GREEN }
来源：http://hz.cqqwz.cn/gtcdedmres.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.xingfuxueyuan.xyz/gtwryzkorx.html


<!-- 参考信息 -->