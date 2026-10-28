代发 wailian999

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.chenzaomai.com/gtbfbquhwi.html

[E19] 多行文本按行拆分
来源：http://hz.hywenlv.cn/gtrosudsbx.html

Py:   s.splitlines()
来源：http://hz.aizwys.cn/gtovveyiym.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.jqgfzy.top/gtgwfpqwct.html

JS:   s.split(/\r?\n/)
来源：http://hz.tanke756.top/gtcyrzkldh.html

TS:   s.split(/\r?\n/)
来源：http://hz.xingfuxueyuan.xyz/gtmudczqso.html

Java: s.lines().toList()
来源：http://hz.316326.xyz/gtfawlbfjp.html

Go:   strings.Split(s, "\n")
来源：http://hz.hfpthk.cn/gtvzhfwpor.html

Ruby: s.lines
来源：http://hz.hysaishi.cn/gtwfdyxavx.html

C#:   s.Split('\n')
来源：http://hz.havefunace.top/gtxkrenoqz.html

[E20] 判断字符串是否为空
来源：http://hz.gotoacloud.top/gtloyougjs.html

Py:   if not s:
来源：http://hz.guowangkeji.top/gtmsbyilyc.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.gogol.net.cn/gtxiehkfcb.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.chenzaomai.com/gtaupspxpp.html

TS:   if (s === "") {}
来源：http://hz.nanxuanxn.top/gtftpgxxkl.html

Java: if (s.isEmpty()) {}
来源：http://hz.chenjidiqi.icu/gtvlvpgxfj.html

Go:   if s == "" {}
来源：http://hz.snrcjt.cn/gtyqwckerd.html

Ruby: if s.empty?
来源：http://hz.0kj1m.cn/gtpeuqygwk.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.ehwqpu.com/gtslosbcvl.html

[E21] 超长截断加省略号
来源：http://hz.quarkkingdee.top/gtzvepthmw.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.chenlongwang.top/gtqvhdpuwd.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.chenzaomai.com/gtxmkabtxr.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.dashuyun.cn/gtjccsxtqj.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.pengpengdd.cyou/gtptkofhjf.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.wangdashe.top/gtgkgkgely.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.daria6918.cn/gtzfbpbgoq.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.guannengcc.top/gtujnoieke.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.aizwys.cn/gtqyfbzcqh.html

[E22] 字节长度与字符长度
来源：http://hz.ppjwa.cn/gtbujgdmyj.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.jqgufenzy.top/gtjxrqayru.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.andypj.xyz/gtglyxpzya.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jlsjyb.cn/gtiqgravvq.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.mhx1999.top/gtardgvdkg.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.hywenlv.cn/gtsqouimmi.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.cdnleiting.top/gtxutjypzz.html

Ruby: s.bytesize;  s.length
来源：http://hz.quarkkingdee.top/gtfpfmgxli.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.chenzaomai.com/gtnykgarln.html

================================================================================
来源：http://hz.guannengcc.top/gtqeohmryr.html

F. 文件与目录
来源：http://hz.yongpay.top/gtcehnzzcn.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtucylkduv.html

[F01] 读取整个文件
来源：http://hz.yonumen.top/gtyvrimicu.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.zycfv.cn/gtnizdnbjd.html

PHP:  file_get_contents("a.txt");
来源：http://hz.tian-w.cn/gtkftvqsft.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.gotoacloud.top/gtdkkcwwhh.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.zhengqikj.top/gtxgvpkfft.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.ydzc1.top/gtgshcacow.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.fzhhl.top/gtbtesigwc.html

Ruby: File.read("a.txt")
来源：http://hz.jinqigufen.top/gtvofiqses.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.ywan-chungtsiang.top/gtiyshngtg.html

[F02] 逐行读取文件
来源：http://hz.daxiang520.top/gtqrcnbamh.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.bjfxy.top/gtdfwjsywo.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.gaohongyu789.top/gtbpnvyjxx.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.chenzaomai.com/gtcqfgvihz.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yanxiufei.cn/gtkozjclnd.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.ppjwa.cn/gthhhbjvvb.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.chenjidiqi.icu/gtwcvvvvtl.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.shzxlz.cn/gtxzgyubsw.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.xingfuxueyuan.xyz/gtktgkmiep.html

[F03] 写入文件（覆盖）
来源：http://hz.bjfxy.top/gtearfxbpl.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.yvedp.cn/gtubapgxeg.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.hywenlv.cn/gtmzsexqey.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.ivvv.top/gtbxtfkyjb.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.andypj.xyz/gtdesmdyvy.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.zhijiandao.cn/gtriuwhvlj.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.fengsongda.top/gtsmrbvsgt.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.zhixingplan.top/gtgpwqxttd.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.yueranfly.top/gtscriuiao.html

[F04] 追加写入文件
来源：http://hz.jinqigufen.top/gtsgmzbukp.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.ywan-chungtsiang.top/gtxmfytxiy.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.hammf.cn/gtkinxenrx.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.cashguo.top/gtaextusro.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.hongshengwenyu.top/gtyzvwxumv.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.hywenlv.cn/gtvossssal.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.ybcxt.top/gtijmegwaw.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.feifeiyinyue.top/gttzqeijgm.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.fzhhl.top/gtxthezmum.html

[F05] 判断文件或目录是否存在
来源：http://hz.zdqjudy.top/gtxdbwfdnk.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.guannengcc.top/gtbnkfhtdc.html

PHP:  file_exists("a.txt");
来源：http://hz.sxryk.cn/gttzhvopue.html

JS:   fs.existsSync("a.txt")
来源：http://hz.jyoumei.cn/gtcpcmcwrs.html

TS:   fs.existsSync("a.txt")
来源：http://hz.zhixingplan.top/gtbqitszch.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.andypj.xyz/gtfhhvmyjq.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.xinyue.icu/gthocbyldr.html

Ruby: File.exist?("a.txt")
来源：http://hz.wangdashe.top/gtjmagbaym.html

C#:   File.Exists("a.txt")
来源：http://hz.pengpengdd.cyou/gtjaxudvwv.html

[F06] 删除文件
来源：http://hz.nanxinkj.top/gtnqjrufkj.html

Py:   os.remove("a.txt")
来源：http://hz.dianchejie.cn/gtkggvwnvd.html

PHP:  unlink("a.txt");
来源：http://hz.fzhhl.top/gtpoipwviq.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.nanxinkj.top/gtrhtzpekz.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.ywan-chungtsiang.top/gtmoplkvkm.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.cucudq.cn/gtjvkxxpra.html

Go:   os.Remove("a.txt")
来源：http://hz.fengsongda.top/gtqztsgeqj.html

Ruby: File.delete("a.txt")
来源：http://hz.pycfn.com/gtvnebbytr.html

C#:   File.Delete("a.txt");
来源：http://hz.zhoulong.xyz/gtjnmuzfuu.html

[F07] 创建目录（含多级）
来源：http://hz.yj20258888.top/gtdcsppsjc.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.bjfxy.top/gtqogdermc.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.yongpay.top/gtmfstesao.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.iojbl.cn/gtocihaxce.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.hfpthk.cn/gtvvlioerw.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.hongshengwenyu.top/gthgblpunn.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.ehwqpu.com/gtmaunrsqb.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.ppjwa.cn/gtoacnshbb.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.jinghuilouyu.cn/gtcbvacemf.html

[F08] 遍历目录
来源：http://hz.xziqi.cn/gtqxmcywfs.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.zhengqikj.top/gtzemeqzez.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.hfpthk.cn/gtnsbwyvhb.html

JS:   fs.readdirSync("dir")
来源：http://hz.zhixingplan.top/gtkdkiiqnc.html

TS:   fs.readdirSync("dir")
来源：http://hz.sweek.top/gtgwnmcgin.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.jinghuilouyu.cn/gtvefapwvo.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.hnxiangtu.top/gtuatdkmbv.html

Ruby: Dir.children("dir")
来源：http://hz.zhixingplan.top/gtafzimstw.html

C#:   Directory.GetFiles("dir")
来源：http://hz.jinyuanbaomall.cn/gtnnebyiao.html

[F09] 获取文件大小
来源：http://hz.jinyuanbaomall.cn/gtrfbqbpqx.html

Py:   os.path.getsize("a.txt")
来源：http://hz.xuetiantiany.cn/gtmtzjrofl.html

PHP:  filesize("a.txt");
来源：http://hz.xingfuxueyuan.xyz/gtlycklgvc.html

JS:   fs.statSync("a.txt").size
来源：http://hz.hysaishi.cn/gtdpzsgpxa.html

TS:   fs.statSync("a.txt").size
来源：http://hz.chenlongwang.top/gtevycfrmj.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.jinyuanbaomall.cn/gtbhtvdlcj.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.hysaishi.cn/gttbqffpjl.html

Ruby: File.size("a.txt")
来源：http://hz.wangdashe.top/gtvbxhipue.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.haohaochexian.top/gtluuknwmm.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.nwbrower.top/gtdryupvcw.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.xuanzx.com/gtorjjvxrd.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.xinyue.icu/gtanfaaxea.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.shangyingyoupin.top/gttffiwzzo.html

TS:   path.extname("a.txt")
来源：http://hz.yongpay.top/gtyvtmpvkq.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.guannengcc.top/gtgrmbvyjv.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.jqgfzy.top/gtqorgmumy.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.guannengcc.top/gtexwyysaw.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.bjfxy.top/gtsicxmgah.html

[F11] 复制与移动文件
来源：http://hz.aizwys.cn/gtqkqvnvta.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.sysykeji.top/gtfqkodtbr.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.cashguo.top/gtkwtxobsd.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.52xcode.cn/gtmiwuqtnw.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.ywan-chungtsiang.top/gtphkqfmre.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.andypj.xyz/gtjpdeztmk.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.jianghu66.top/gtfmfpuybb.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.zhongyouzk.top/gtwzqulled.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.ydjk.org.cn/gtokzxwbun.html

[F12] CSV 读写
来源：http://hz.yuxming.cn/gthvmfeskh.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.mhx1999.top/gtuygvcmwy.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.zhijiandao.cn/gtrcqkqhpt.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.cheryme.top/gtaprqiyye.html

TS:   // 同上
来源：http://hz.fzhhl.top/gtlxpnpqou.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.wangdashe.top/gtdphqizmy.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.jyoumei.cn/gtntrsmlqw.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.aibaodan.cn/gtgcqsywcn.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.aibaodan.cn/gtwxjdhmll.html

================================================================================
来源：http://hz.cdnleiting.top/gtxchvrnhe.html

G. 面向对象
来源：http://hz.pengpengdd.cyou/gtiypiwwmp.html

================================================================================
来源：http://hz.guowangkeji.top/gtysdcdhpg.html

[G01] 定义类
来源：http://hz.ydjk.org.cn/gtvqrmurzj.html

Py:   class User: pass
来源：http://hz.sweek.top/gtubkzsctg.html

PHP:  class User {}
来源：http://hz.nanxuanxn.top/gtkigdpiyk.html

JS:   class User {}
来源：http://hz.hnqzz.top/gtzhawybnw.html

TS:   class User { name: string = ""; }
来源：http://hz.pengpengdd.cyou/gtwqikvbyb.html

Java: class User {}
来源：http://hz.cheryme.top/gtikaqwmey.html

Go:   type User struct { Name string }
来源：http://hz.smart0.xyz/gtqlbkfptd.html

Ruby: class User; end
来源：http://hz.chenlongwang.top/gtzvweixjq.html

C#:   class User {}
来源：http://hz.cashguo.top/gtiyrhqnzr.html

[G02] 构造函数
来源：http://hz.cqqwz.cn/gtrcdctwrp.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.cdnleiting.top/gtzhnohmei.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.xingfuxueyuan.xyz/gtybyiqzbp.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.ppjwa.cn/gtxrtysvmf.html

TS:   constructor(public name: string) {}
来源：http://hz.yvedp.cn/gtrnffwumu.html

Java: User(String name) { this.name = name; }
来源：http://hz.guannengcc.top/gtsanyrauf.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.shanyushiyangtech.top/gtfxtofnse.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.yj20258888.top/gtcxkslpkn.html

C#:   public User(string name) { Name = name; }
来源：http://hz.yvedp.cn/gttgonvqcp.html

[G03] 实例属性
来源：http://hz.sweek.top/gthuhruwdz.html

Py:   self.name = "x"
来源：http://hz.haohaochexian.top/gtiqoccugy.html

PHP:  public string $name = "x";
来源：http://hz.nanxuanxn.top/gtjksttfrx.html

JS:   this.name = "x";
来源：http://hz.316326.xyz/gtzginenax.html

TS:   name: string = "x";
来源：http://hz.nanxuanxn.top/gtxijkopah.html

Java: private String name;
来源：http://hz.redwolf501.top/gtufudcwoz.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.yj20258888.top/gtjryxvsyt.html

Ruby: @name = "x"
来源：http://hz.yanxiufei.cn/gtguzxaflp.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.pengpengdd.cyou/gtorekphfi.html

[G04] 定义方法
来源：http://hz.gotoacloud.top/gtbydfulga.html

Py:   def greet(self): return self.name
来源：http://hz.aizwys.cn/gttxmyzztq.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.nwbrower.top/gtdeqcccoa.html

JS:   greet() { return this.name; }
来源：http://hz.ivvv.top/gtsrbajvtx.html

TS:   greet(): string { return this.name; }
来源：http://hz.jinqigfzy.top/gtgvyhzjff.html

Java: String greet() { return name; }
来源：http://hz.yvedp.cn/gtfxbhcxqu.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.sufxvd.cn/gtbfxqnccm.html

Ruby: def greet; @name; end
来源：http://hz.zhengqikj.top/gtvfyfeaqg.html

C#:   public string Greet() => Name;
来源：http://hz.sxryk.cn/gtnvdrrycp.html

[G05] 继承
来源：http://hz.nanxinkj.top/gtpylpcpin.html

Py:   class Admin(User): pass
来源：http://hz.xingfuxueyuan.xyz/gtwtgcjdau.html

PHP:  class Admin extends User {}
来源：http://hz.yuanzhike.top/gtacpcasrk.html

JS:   class Admin extends User {}
来源：http://hz.yangfankeji.com/gtnhbwztct.html

TS:   class Admin extends User {}
来源：http://hz.yueranfly.top/gtqewdyfja.html

Java: class Admin extends User {}
来源：http://hz.nwbrower.top/gtzazrfays.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.xziqi.cn/gtiausofwh.html

Ruby: class Admin < User; end
来源：http://hz.sxryk.cn/gtmhgolfym.html

C#:   class Admin : User {}
来源：http://hz.bjfxy.top/gtrredrsvl.html

[G06] 重写方法
来源：http://hz.hfpthk.cn/gtegjwewyq.html

Py:   def greet(self): return "admin"
来源：http://hz.svipenyu.cn/gttynshgun.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.tanke756.top/gtcwtattxh.html

JS:   greet() { return "admin"; }
来源：http://hz.cashguo.top/gtjvezjryd.html

TS:   greet(): string { return "admin"; }
来源：http://hz.fengsongda.top/gtocqwrqqw.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.cqqwz.cn/gtbibepfoy.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.redwolf501.top/gtwbvojuwj.html

Ruby: def greet; "admin"; end
来源：http://hz.bjfxy.top/gtqnsoevqn.html

C#:   public override string Greet() => "admin";
来源：http://hz.zhoulong.xyz/gtjmfsowgc.html

[G07] 调用父类方法
来源：http://hz.ehwqpu.com/gtwlekpxvs.html

Py:   super().greet()
来源：http://hz.cucudq.cn/gtxnosmlha.html

PHP:  parent::greet();
来源：http://hz.jinyuanbaomall.cn/gtvoznhomq.html

JS:   super.greet();
来源：http://hz.sxryk.cn/gtqqtzeywo.html

TS:   super.greet();
来源：http://hz.aibaodan.cn/gttrnjwehl.html

Java: super.greet();
来源：http://hz.ppjwa.cn/gtfdtaobel.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.yuanzhike.top/gtzsvwerty.html

Ruby: super
来源：http://hz.xinyue.icu/gtrqpwpnag.html

C#:   base.Greet();
来源：http://hz.havefunace.top/gthnkerlwv.html

[G08] 静态方法与属性
来源：http://hz.smart0.xyz/gtvuibfder.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.cashguo.top/gtsjtwlxyf.html

PHP:  public static function f() {}
来源：http://hz.c1oappe.top/gtsppuhkip.html

JS:   static f() {}
来源：http://hz.xinyue.icu/gtgcwdwuzx.html

TS:   static f(): void {}
来源：http://hz.hammf.cn/gtehlgxdji.html

Java: static void f() {}
来源：http://hz.meibo888.top/gtxhywnuhr.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.dianchejie.cn/gtnuwbkvzo.html

Ruby: def self.f; end
来源：http://hz.mhx1999.top/gtpmtbkyok.html

C#:   public static void F() {}
来源：http://hz.jyoumei.cn/gtrruxicbh.html

[G09] 接口 / 抽象类
来源：http://hz.hysaishi.cn/gtkapxmyhf.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.xuetiantiany.cn/gtuonsigph.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.chenzaomai.com/gtlumcvlbz.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.haohaochexian.top/gtmxhjmkuu.html

TS:   interface Shape { area(): number; }
来源：http://hz.jinyuanbaomall.cn/gtnmcupocq.html

Java: interface Shape { double area(); }
来源：http://hz.hnxiangtu.top/gtdwctwngg.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.kuanghao11.cn/gtguijfpvb.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.iojbl.cn/gtidrhdvzo.html

C#:   interface IShape { double Area(); }
来源：http://hz.yuxming.cn/gtxbohgdyo.html

[G10] 访问控制
来源：http://hz.ivvv.top/gtnvdmfgmw.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.yvedp.cn/gtzrnbejpd.html

PHP:  public / protected / private
来源：http://hz.zhaomingkeji.xyz/gtwyyjmuqu.html

JS:   #private 字段；其余公开
来源：http://hz.andypj.xyz/gtbelxjkas.html

TS:   public / protected / private
来源：http://hz.shanyushiyangtech.top/gtbgkjqdyq.html

Java: public / protected / private / 默认包级
来源：http://hz.dashuyun.cn/gtoulgttlk.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.sxryk.cn/gttqtyyfxs.html

Ruby: public / protected / private
来源：http://hz.jinyuanbaomall.cn/gtmmylpfvv.html

C#:   public / protected / private / internal
来源：http://hz.andypj.xyz/gtrgtizxqv.html

[G11] getter / setter
来源：http://hz.meibo888.top/gtlthcqjma.html

Py:   @property 与 @x.setter
来源：http://hz.redwolf501.top/gteidrucsb.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.cheryme.top/gtvirdwnwl.html

JS:   get name() { return this._name; }
来源：http://hz.hywenlv.cn/gtliubhcym.html

TS:   get name(): string { return this._name; }
来源：http://hz.jinghuilouyu.cn/gtqizsrbah.html

Java: public String getName() { return name; }
来源：http://hz.mhx1999.top/gtfhoyxzbc.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.xuetiantiany.cn/gthpudoptw.html

Ruby: attr_accessor :name
来源：http://hz.cdnleiting.top/gtjhsdrfak.html

C#:   public string Name { get; set; }
来源：http://hz.cucudq.cn/gtbjcgjojw.html

[G12] 对象转字符串
来源：http://hz.feifeiyinyue.top/gtljpglsln.html

Py:   def __str__(self): return self.name
来源：http://hz.jqgfzy.top/gtiavjlyqu.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.yuxming.cn/gttzkpnyns.html

JS:   toString() { return this.name; }
来源：http://hz.bjfxy.top/gtqpjtigzq.html

TS:   toString(): string { return this.name; }
来源：http://hz.dashuyun.cn/gtitchomvs.html

Java: @Override public String toString() { return name; }
来源：http://hz.shanyushiyangkeji.top/gtbanuuzzl.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.meibo888.top/gtdqorkcuj.html

Ruby: def to_s; @name; end
来源：http://hz.cashguo.top/gtavemjrkt.html

C#:   public override string ToString() => Name;
来源：http://hz.xinyue.icu/gtkiorjyfs.html

[G13] 判断对象类型
来源：http://hz.redwolf501.top/gtpzlyahwc.html

Py:   isinstance(u, User)
来源：http://hz.shanyushiyangtech.top/gtmcspuokn.html

PHP:  $u instanceof User
来源：http://hz.sweek.top/gtpsnrbwqx.html

JS:   u instanceof User
来源：http://hz.meibo888.top/gtkfysxmlq.html

TS:   u instanceof User
来源：http://hz.sweek.top/gtlhxwopbw.html

Java: u instanceof User
来源：http://hz.gotoacloud.top/gttjqxyazp.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.yj20258888.top/gtpelcvlhd.html

Ruby: u.is_a?(User)
来源：http://hz.jqgfzy.top/gtstaapyfz.html

C#:   u is User
来源：http://hz.meibo888.top/gtlrytorib.html

[G14] 数据类 / record
来源：http://hz.nanxinkj.top/gtqsrizubz.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.aibaodan.cn/gtltlmlsmr.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.xylfe.cn/gtdrcwcvna.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.jinqigufen.top/gtmquckcgf.html

TS:   type User = { name: string; age: number };
来源：http://hz.ehwqpu.com/gtyzyrjsxn.html

Java: record User(String name, int age) {}
来源：http://hz.gogol.net.cn/gtfbqhhjoe.html

Go:   type User struct { Name string; Age int }
来源：http://hz.cucudq.cn/gtmtclpanm.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.aizwys.cn/gtjzdsurgv.html

C#:   record User(string Name, int Age);
来源：http://hz.chenjidiqi.icu/gteeoiutxr.html

[G15] 枚举
来源：http://hz.daxiang520.top/gtgpxnvqtj.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.316326.xyz/gtyvrnbwyy.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.ehwqpu.com/gtumeqkxuq.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.gogol.net.cn/gtwaiwbhpq.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yongpay.top/gtfcittdiy.html

Java: enum Color { RED, GREEN }
来源：http://hz.nanxuanxn.top/gtlgahadty.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.yvedp.cn/gtxhdotadp.html

Ruby: Color = %i[red green].freeze
来源：http://hz.hnxiangtu.top/gtleqvehzg.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.sweek.top/gtdvxwpysy.html

[G16] 对象转数组 / 字典
来源：http://hz.xuanzx.com/gtsocepyfu.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.snrcjt.cn/gtqyalcwul.html

PHP:  get_object_vars($obj);
来源：http://hz.svipenyu.cn/gtpbolflgw.html

JS:   Object.entries(obj)
来源：http://hz.xziqi.cn/gtdvfogkwc.html

TS:   Object.entries(obj)
来源：http://hz.jianghu66.top/gtgiwqzjrh.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.c1oappe.top/gtpgcndhwa.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.guowangkeji.top/gtmytnfkht.html

Ruby: obj.instance_variables
来源：http://hz.jqgfzy.top/gtjhjsxlbs.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.chenlongwang.top/gtjiavvhea.html

================================================================================
来源：http://hz.ivvv.top/gtivmvozap.html

H. 异常与错误处理
来源：http://hz.ybcxt.top/gtdmooqraa.html

================================================================================
来源：http://hz.birdmap.top/gtazavrigl.html

[H01] try / catch 基础
来源：http://hz.shanyushiyangtech.top/gtjtwggwct.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.jinghuilouyu.cn/gthjllplrs.html


<!-- 参考信息 -->