代发 wailian999

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.jinyuanbaomall.cn/gtxxuoiuij.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.cashguo.top/gtqpxchegw.html

Ruby: s.capitalize
来源：http://hz.gogol.net.cn/gtvzwcapvq.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.fengsongda.top/gttljzvitg.html

[E18] 模板占位符替换
来源：http://hz.zdqjudy.top/gtgxqvovde.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.hfpthk.cn/gtrdtvbdgm.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.shuidangran.top/gtoaylppej.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.quarkkingdee.top/gttnjrvqsf.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.guowangkeji.top/gtsygvkmlk.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.sysykeji.top/gtgpmrgbbf.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.smart0.xyz/gtxhkgvdqx.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.c1oappe.top/gtxrofoado.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.hfpthk.cn/gtycelqjuu.html

[E19] 多行文本按行拆分
来源：http://hz.hongshengwenyu.top/gtvjcbzlim.html

Py:   s.splitlines()
来源：http://hz.feifeiyinyue.top/gtejvbpzwp.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.quarkkingdee.top/gtkhnngqzs.html

JS:   s.split(/\r?\n/)
来源：http://hz.andypj.xyz/gtpjxmcgwo.html

TS:   s.split(/\r?\n/)
来源：http://hz.gotoacloud.top/gtxsgehdkn.html

Java: s.lines().toList()
来源：http://hz.ywan-chungtsiang.top/gtpebndtue.html

Go:   strings.Split(s, "\n")
来源：http://hz.sxryk.cn/gtlcomqxen.html

Ruby: s.lines
来源：http://hz.ydzc1.top/gtbxavglha.html

C#:   s.Split('\n')
来源：http://hz.pengpengdd.cyou/gtujdzwicw.html

[E20] 判断字符串是否为空
来源：http://hz.sysykeji.top/gttgnopjfq.html

Py:   if not s:
来源：http://hz.mhx1999.top/gtgvavkspo.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.gaohongyu789.top/gthzamdefw.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.feifeiyinyue.top/gtlprrvmdz.html

TS:   if (s === "") {}
来源：http://hz.ydjk.org.cn/gtrdmoxdqz.html

Java: if (s.isEmpty()) {}
来源：http://hz.shuidangran.top/gtfacrnnut.html

Go:   if s == "" {}
来源：http://hz.ywan-chungtsiang.top/gtfuzhnfsd.html

Ruby: if s.empty?
来源：http://hz.zhoulong.xyz/gtyffoqfpe.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.zycfv.cn/gttennvlgg.html

[E21] 超长截断加省略号
来源：http://hz.yj20258.top/gtebfgfzns.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.andypj.xyz/gthgtkqozf.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.vqdsnc.cn/gtlfgmozre.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.feifeiyinyue.top/gtgrcbmeqg.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.ywan-chungtsiang.top/gtwakztyuo.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.shuidangran.top/gtgqfamzdg.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.daria6918.cn/gtbfozzblu.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.guowangkeji.top/gtptpyrzwo.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.havefunace.top/gtlssjoppr.html

[E22] 字节长度与字符长度
来源：http://hz.xylfe.cn/gtoyksgmzw.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.daxiang520.top/gtlfzqzkic.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.ppjwa.cn/gtaczvwitx.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.zhiwuduotai.top/gtuimqeblk.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.316326.xyz/gtfjdiveuh.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.jiagoushi.top/gtzzbridpz.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.haohaochexian.top/gtshqtuubj.html

Ruby: s.bytesize;  s.length
来源：http://hz.nwbrower.top/gtbdpdxvqk.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.cdnleiting.top/gtcvzsjjjh.html

================================================================================
来源：http://hz.jlsjyb.cn/gtdnizmowv.html

F. 文件与目录
来源：http://hz.shzxlz.cn/gtlceivgbg.html

================================================================================
来源：http://hz.fzhhl.top/gtprmtvnia.html

[F01] 读取整个文件
来源：http://hz.nanxinkj.top/gthfekgjsi.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.bjfxy.top/gtljeljudn.html

PHP:  file_get_contents("a.txt");
来源：http://hz.dashuyun.cn/gtkgizvcjb.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.hnqzz.top/gtbcejbepi.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.yj202588.top/gtdglasszn.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.jianghu66.top/gtjzutxuwd.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.zdqjudy.top/gtzpxphmyy.html

Ruby: File.read("a.txt")
来源：http://hz.wangdashe.top/gtcholnifs.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.xziqi.cn/gtznkbcfty.html

[F02] 逐行读取文件
来源：http://hz.cqqwz.cn/gtgteodvax.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.jinqigfzy.top/gtzetxkaox.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.316326.xyz/gtgnslhgxf.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.tanke756.top/gtrqbznxwi.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.aibaodan.cn/gtvyhsgdpo.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.snrcjt.cn/gtkszzinfg.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.jinqigufen.top/gtsiazxboi.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.yj202588.top/gtzuolysns.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.aibaodan.cn/gtrobgzzwq.html

[F03] 写入文件（覆盖）
来源：http://hz.mhx1999.top/gtqorcbkka.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.aibaodan.cn/gtqxyafwly.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.xuetiantiany.cn/gtwnqdrliw.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.cucudq.cn/gtpevnyfyp.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.zdqjudy.top/gtcckcugod.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.ydjk.org.cn/gtaddgpvdm.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.jinghuilouyu.cn/gtahkpzdtv.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.c1oappe.top/gthktphjnq.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.svipenyu.cn/gtfpzitjit.html

[F04] 追加写入文件
来源：http://hz.zhaomingkeji.xyz/gtvpvtkvkd.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.bjfxy.top/gthqeyjspv.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.redwolf501.top/gtjuxshrkv.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yj202588.top/gtagwrqlwa.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.tanke756.top/gtwnqkkqud.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.sweek.top/gtyrwgywuc.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.dianchejie.cn/gtedwmbjxa.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.ehwqpu.com/gtnalloslh.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.yonumen.top/gtmltbsfvk.html

[F05] 判断文件或目录是否存在
来源：http://hz.sysykeji.top/gtumeliqzn.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.xziqi.cn/gtjzjvmhxf.html

PHP:  file_exists("a.txt");
来源：http://hz.meibo888.top/gtudqgtxll.html

JS:   fs.existsSync("a.txt")
来源：http://hz.hywenlv.cn/gtuwnjarck.html

TS:   fs.existsSync("a.txt")
来源：http://hz.jianghu66.top/gturqwloxj.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.nwbrower.top/gtvhiwitdn.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.zdqjudy.top/gttlquolqs.html

Ruby: File.exist?("a.txt")
来源：http://hz.svipenyu.cn/gttojzhtos.html

C#:   File.Exists("a.txt")
来源：http://hz.jiagoushi.top/gtihesbwwk.html

[F06] 删除文件
来源：http://hz.mhx1999.top/gtonrbguyz.html

Py:   os.remove("a.txt")
来源：http://hz.fengsongda.top/gtmwelumyu.html

PHP:  unlink("a.txt");
来源：http://hz.zycfv.cn/gtkpohrsev.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.xuetiantiany.cn/gtgijokach.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.gzhubu.top/gtlgazpsiq.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.0kj1m.cn/gtzhomhuwo.html

Go:   os.Remove("a.txt")
来源：http://hz.wangdashe.top/gtouqzdryd.html

Ruby: File.delete("a.txt")
来源：http://hz.ybcxt.top/gtodbwovfe.html

C#:   File.Delete("a.txt");
来源：http://hz.0kj1m.cn/gtjprkzpvs.html

[F07] 创建目录（含多级）
来源：http://hz.52xcode.cn/gtzpieuxhp.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.jinqigufen.top/gtfykkprdl.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.hysaishi.cn/gtynvjbzfl.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jqgfzy.top/gtrunoqjra.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.tian-w.cn/gtjtwytfpy.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.guowangkeji.top/gtjhwjcsbp.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.gotoacloud.top/gtjdpexema.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.yanxiufei.cn/gtsimpndgu.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.jqgfzy.top/gtfwymkrns.html

[F08] 遍历目录
来源：http://hz.ydjk.org.cn/gtujkzskfv.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.xylfe.cn/gtxrpqmuuz.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.zhongyouzk.top/gtzgbvwzwx.html

JS:   fs.readdirSync("dir")
来源：http://hz.feifeiyinyue.top/gtaiihbbqy.html

TS:   fs.readdirSync("dir")
来源：http://hz.chenlongwang.top/gtaolebcyv.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.yanxiufei.cn/gtcnbuoxag.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.tianlin.xyz/gtbqgrwhos.html

Ruby: Dir.children("dir")
来源：http://hz.hysaishi.cn/gtmyiloyha.html

C#:   Directory.GetFiles("dir")
来源：http://hz.chenjidiqi.icu/gtusprsocg.html

[F09] 获取文件大小
来源：http://hz.xuetiantiany.cn/gtrrabsnkk.html

Py:   os.path.getsize("a.txt")
来源：http://hz.wangdashe.top/gtqbrpepxo.html

PHP:  filesize("a.txt");
来源：http://hz.smart0.xyz/gtsqmlfrkl.html

JS:   fs.statSync("a.txt").size
来源：http://hz.chenjidiqi.icu/gterrecjvw.html

TS:   fs.statSync("a.txt").size
来源：http://hz.smart0.xyz/gthrqwhdoz.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.aizwys.cn/gtfoowiioy.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.zhengqikj.top/gthgqxmbwa.html

Ruby: File.size("a.txt")
来源：http://hz.zhiwuduotai.top/gtauigwfmm.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.xuetiantiany.cn/gtsadludit.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.feifeiyinyue.top/gtuxxgiizw.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.yuxming.cn/gtcbcsmbws.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.jinqigfzy.top/gtmxhbowcu.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.zhoulong.xyz/gtdnwltcdp.html

TS:   path.extname("a.txt")
来源：http://hz.jyoumei.cn/gtlywlrdww.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.ydzc1.top/gtzjqkzbnv.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.cqqwz.cn/gtucvwmbsq.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.gzhubu.top/gtqfnxdikq.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.ydzc1.top/gtctknzovf.html

[F11] 复制与移动文件
来源：http://hz.xylfe.cn/gtjfhvgcoe.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.wangdashe.top/gtnlgtmgbi.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.yongpay.top/gthvoaodrm.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.vqdsnc.cn/gtrfpawxhn.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.sweek.top/gtjhephnkr.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.hfpthk.cn/gtxhjwjkoc.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.meibo888.top/gtiuhoptox.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.ybcxt.top/gtsnqnhtkx.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.gogol.net.cn/gttisydtgn.html

[F12] CSV 读写
来源：http://hz.yj202588.top/gtpkvnpivo.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.chenjidiqi.icu/gtpkzlssns.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.zhixingplan.top/gtcimzwsog.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.zhixingplan.top/gtglmesnzh.html

TS:   // 同上
来源：http://hz.sxryk.cn/gtzllpulta.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.mhx1999.top/gtquynufoo.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.tianlin.xyz/gtuhopfnig.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.yuxming.cn/gtvdminzvc.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.haohaochexian.top/gtrbqomdvy.html

================================================================================
来源：http://hz.gaohongyu789.top/gtmwlzkspg.html

G. 面向对象
来源：http://hz.jinyuanbaomall.cn/gtdjiazxty.html

================================================================================
来源：http://hz.smart0.xyz/gtkatmdmhf.html

[G01] 定义类
来源：http://hz.dianchejie.cn/gtasbfimfg.html

Py:   class User: pass
来源：http://hz.jiagoushi.top/gtkymrzoxi.html

PHP:  class User {}
来源：http://hz.hysaishi.cn/gtvtsoinkw.html

JS:   class User {}
来源：http://hz.chenzaomai.com/gtoefttrcq.html

TS:   class User { name: string = ""; }
来源：http://hz.jinqigufen.top/gtsyyoenkw.html

Java: class User {}
来源：http://hz.guannengcc.top/gttrwtqcbe.html

Go:   type User struct { Name string }
来源：http://hz.fengsongda.top/gtwumsuqvn.html

Ruby: class User; end
来源：http://hz.meibo888.top/gtjgaanmql.html

C#:   class User {}
来源：http://hz.nwbrower.top/gtfnxqpfax.html

[G02] 构造函数
来源：http://hz.feifeiyinyue.top/gtqubejflk.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.zhongyouzk.top/gtgtigxfjk.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.vqdsnc.cn/gtepdahivf.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.yongpay.top/gtqvhkukpu.html

TS:   constructor(public name: string) {}
来源：http://hz.kuanghao11.cn/gtwlyzpgiy.html

Java: User(String name) { this.name = name; }
来源：http://hz.hysaishi.cn/gtyvbcdvtb.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.yonumen.top/gtbcukdlnu.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.dashuyun.cn/gtubplemfu.html

C#:   public User(string name) { Name = name; }
来源：http://hz.pengpengdd.cyou/gtqegsxirj.html

[G03] 实例属性
来源：http://hz.jianghu66.top/gtoldpgqyp.html

Py:   self.name = "x"
来源：http://hz.pycfn.com/gtmcykpryc.html

PHP:  public string $name = "x";
来源：http://hz.xuetiantiany.cn/gtztmprrze.html

JS:   this.name = "x";
来源：http://hz.dashuyun.cn/gtsrfsdafo.html

TS:   name: string = "x";
来源：http://hz.sysykeji.top/gtwkkbtotc.html

Java: private String name;
来源：http://hz.sufxvd.cn/gtcvsdhsce.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.feifeiyinyue.top/gtxuysukbg.html

Ruby: @name = "x"
来源：http://hz.hywenlv.cn/gtklvdkjqm.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.nanxinkj.top/gtanlsqrwx.html

[G04] 定义方法
来源：http://hz.gzhubu.top/gtwcqwcgus.html

Py:   def greet(self): return self.name
来源：http://hz.zhoulong.xyz/gtiylyqmkw.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.ybcxt.top/gtpspuivbt.html

JS:   greet() { return this.name; }
来源：http://hz.ywan-chungtsiang.top/gtenzlxsdp.html

TS:   greet(): string { return this.name; }
来源：http://hz.jinqigufen.top/gttdectxnm.html

Java: String greet() { return name; }
来源：http://hz.havefunace.top/gtkfmshuwy.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.gzhubu.top/gtfrobbpui.html

Ruby: def greet; @name; end
来源：http://hz.xziqi.cn/gtwaxdacju.html

C#:   public string Greet() => Name;
来源：http://hz.ydzc1.top/gtwukhnhzj.html

[G05] 继承
来源：http://hz.jqgfzy.top/gtmvdxdqcp.html

Py:   class Admin(User): pass
来源：http://hz.xuanzx.com/gtmtcjtfop.html

PHP:  class Admin extends User {}
来源：http://hz.dianchejie.cn/gtrkkzaviq.html

JS:   class Admin extends User {}
来源：http://hz.meibo888.top/gtxntnezij.html

TS:   class Admin extends User {}
来源：http://hz.guannengcc.top/gtpupilkho.html

Java: class Admin extends User {}
来源：http://hz.fzhhl.top/gtpksnawuw.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.vqdsnc.cn/gtuzwqvzaq.html

Ruby: class Admin < User; end
来源：http://hz.yongpay.top/gtoxnyabyo.html

C#:   class Admin : User {}
来源：http://hz.mhx1999.top/gtwwgojvwi.html

[G06] 重写方法
来源：http://hz.jinghuilouyu.cn/gtmhlhvnwt.html

Py:   def greet(self): return "admin"
来源：http://hz.hongshengwenyu.top/gtqusqabgw.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.jinqigfzy.top/gtgpihxgvy.html

JS:   greet() { return "admin"; }
来源：http://hz.jyoumei.cn/gtbtnikmrz.html

TS:   greet(): string { return "admin"; }
来源：http://hz.shanyushiyangkeji.top/gtlmeixptw.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.52xcode.cn/gthjjawpca.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.316326.xyz/gtuhyevjzc.html

Ruby: def greet; "admin"; end
来源：http://hz.havefunace.top/gthgbaazmb.html

C#:   public override string Greet() => "admin";
来源：http://hz.andypj.xyz/gthvbupisp.html

[G07] 调用父类方法
来源：http://hz.zhaomingkeji.xyz/gtxicqqyio.html

Py:   super().greet()
来源：http://hz.dashuyun.cn/gtvgwoxrgy.html

PHP:  parent::greet();
来源：http://hz.nanxinkj.top/gtdmwbwugh.html

JS:   super.greet();
来源：http://hz.316326.xyz/gtydylownj.html

TS:   super.greet();
来源：http://hz.kuanghao11.cn/gtoxvlbjwn.html

Java: super.greet();
来源：http://hz.shuidangran.top/gtlhkucodj.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.daria6918.cn/gttmxrnrvb.html

Ruby: super
来源：http://hz.jyoumei.cn/gtqlmfzwbi.html

C#:   base.Greet();
来源：http://hz.shanyushiyangkeji.top/gtqikzxlfd.html

[G08] 静态方法与属性
来源：http://hz.jqgfzy.top/gtawgznvrz.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.ybcxt.top/gtzjlijbgs.html

PHP:  public static function f() {}
来源：http://hz.zhoulong.xyz/gttixbtxne.html

JS:   static f() {}
来源：http://hz.sweek.top/gtasarxbxv.html

TS:   static f(): void {}
来源：http://hz.shanyushiyangtech.top/gthkvjpdam.html

Java: static void f() {}
来源：http://hz.sysykeji.top/gtumsqlmnv.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.zhongyouzk.top/gtqzvejkma.html

Ruby: def self.f; end
来源：http://hz.zdqjudy.top/gteppsvpxe.html

C#:   public static void F() {}
来源：http://hz.gotoacloud.top/gtkmalturd.html

[G09] 接口 / 抽象类
来源：http://hz.zhongyouzk.top/gtxobhbncp.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.yonumen.top/gtmjukkzkm.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.ehwqpu.com/gtogdfyksk.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.ehwqpu.com/gtsyarbafe.html

TS:   interface Shape { area(): number; }
来源：http://hz.yj20258.top/gthaclvsnz.html

Java: interface Shape { double area(); }
来源：http://hz.yuanzhike.top/gtcekaeezg.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.tian-w.cn/gtemcckuze.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.cucudq.cn/gtxjhxedwz.html

C#:   interface IShape { double Area(); }
来源：http://hz.yj20258.top/gtpsnebajn.html

[G10] 访问控制
来源：http://hz.jinqigfzy.top/gtskwtlqgz.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.nanxuanxn.top/gtqemaqdfs.html

PHP:  public / protected / private
来源：http://hz.xuetiantiany.cn/gtuowcmyfr.html

JS:   #private 字段；其余公开
来源：http://hz.jinyuanbaomall.cn/gtydtjpwrg.html

TS:   public / protected / private
来源：http://hz.pycfn.com/gtgyjsdiyr.html

Java: public / protected / private / 默认包级
来源：http://hz.sysykeji.top/gtxzxudxtf.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.zhaomingkeji.xyz/gttupkoyjr.html

Ruby: public / protected / private
来源：http://hz.shangyingyoupin.top/gtksnikehk.html

C#:   public / protected / private / internal
来源：http://hz.xinyue.icu/gtwnuhopft.html

[G11] getter / setter
来源：http://hz.cheryme.top/gtyaqxfxao.html

Py:   @property 与 @x.setter
来源：http://hz.zhiwuduotai.top/gtmtppxtfo.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.gogol.net.cn/gtpvmdsjgp.html

JS:   get name() { return this._name; }
来源：http://hz.vqdsnc.cn/gtelfiwapt.html

TS:   get name(): string { return this._name; }
来源：http://hz.gaohongyu789.top/gtdqztohsl.html

Java: public String getName() { return name; }
来源：http://hz.sweek.top/gtmtxkvlqv.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.daria6918.cn/gtbmpkxgwp.html

Ruby: attr_accessor :name
来源：http://hz.hysaishi.cn/gtrsvvujgu.html

C#:   public string Name { get; set; }
来源：http://hz.svipenyu.cn/gtniurbnli.html

[G12] 对象转字符串
来源：http://hz.ydzc1.top/gteukqdlmc.html

Py:   def __str__(self): return self.name
来源：http://hz.hongshengwenyu.top/gtkvsladpw.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.shzxlz.cn/gtrxfnyzif.html

JS:   toString() { return this.name; }
来源：http://hz.yongpay.top/gttjberusp.html

TS:   toString(): string { return this.name; }
来源：http://hz.jianghu66.top/gtuijjwkny.html

Java: @Override public String toString() { return name; }
来源：http://hz.wangshuangyany.cn/gtrynqjrlc.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.zhaomingkeji.xyz/gtbwhaijxo.html

Ruby: def to_s; @name; end
来源：http://hz.zhaomingkeji.xyz/gtxystglwy.html

C#:   public override string ToString() => Name;
来源：http://hz.jiagoushi.top/gthiqimkbw.html

[G13] 判断对象类型
来源：http://hz.yongpay.top/gtmiixfeyy.html

Py:   isinstance(u, User)
来源：http://hz.cucudq.cn/gtjhizbpdb.html

PHP:  $u instanceof User
来源：http://hz.wangshuangyany.cn/gtcpjyvoer.html

JS:   u instanceof User
来源：http://hz.wangshuangyany.cn/gtnmwzzeng.html

TS:   u instanceof User
来源：http://hz.ivvv.top/gthjfzmajj.html

Java: u instanceof User
来源：http://hz.shuidangran.top/gtpddcbkid.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.aizwys.cn/gtzyhyvosp.html

Ruby: u.is_a?(User)
来源：http://hz.birdmap.top/gtpgzxmkpl.html

C#:   u is User
来源：http://hz.nwbrower.top/gtlxqzlquf.html

[G14] 数据类 / record
来源：http://hz.ywan-chungtsiang.top/gtdcsntpav.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.aibaodan.cn/gtxmecjuzj.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.nanxuanxn.top/gtynivgccz.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.yuxming.cn/gtelertlmd.html

TS:   type User = { name: string; age: number };
来源：http://hz.jqgfzy.top/gtqncsttqi.html

Java: record User(String name, int age) {}
来源：http://hz.ivvv.top/gtytqwcwrx.html

Go:   type User struct { Name string; Age int }
来源：http://hz.daxiang520.top/gtysmhwfca.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.andypj.xyz/gtmjgmaqxf.html

C#:   record User(string Name, int Age);
来源：http://hz.zhengqikj.top/gtfoydkbrm.html

[G15] 枚举
来源：http://hz.svipenyu.cn/gtwjuneosj.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.tian-w.cn/gtosfjpxqg.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.vqdsnc.cn/gtrixygtyk.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.birdmap.top/gtgdcqtqmr.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.hammf.cn/gtwshicnul.html

Java: enum Color { RED, GREEN }
来源：http://hz.cheryme.top/gtuqkxxoga.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.zhengqikj.top/gtaelasdqh.html

Ruby: Color = %i[red green].freeze
来源：http://hz.quarkkingdee.top/gtiakdzzxj.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.quarkkingdee.top/gtisvzbpfw.html

[G16] 对象转数组 / 字典
来源：http://hz.yvedp.cn/gtgjaxqopr.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.pycfn.com/gtnfwgoquz.html


<!-- 参考信息 -->