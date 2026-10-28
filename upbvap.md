代发 wailian999

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.mhx1999.top/gtrbcvumyu.html

[E19] 多行文本按行拆分
来源：http://hz.shzxlz.cn/gtbivzwgzn.html

Py:   s.splitlines()
来源：http://hz.zhongyouzk.top/gtwkwrvvrb.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.jianghu66.top/gtfnwwtiox.html

JS:   s.split(/\r?\n/)
来源：http://hz.yongpay.top/gtxwxwdegn.html

TS:   s.split(/\r?\n/)
来源：http://hz.shanyushiyangkeji.top/gtguwtzeyc.html

Java: s.lines().toList()
来源：http://hz.fzhhl.top/gtfaiinkji.html

Go:   strings.Split(s, "\n")
来源：http://hz.zhijiandao.cn/gtnqjrtgdj.html

Ruby: s.lines
来源：http://hz.sweek.top/gtljyczgtl.html

C#:   s.Split('\n')
来源：http://hz.tianlin.xyz/gtxbsbkfyh.html

[E20] 判断字符串是否为空
来源：http://hz.yongpay.top/gtvyxfmyhe.html

Py:   if not s:
来源：http://hz.yj20258888.top/gtnnokguqv.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.zhiwuduotai.top/gtrslnxbsf.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.aibaodan.cn/gtodppvshz.html

TS:   if (s === "") {}
来源：http://hz.zhaomingkeji.xyz/gtrqjrwsjl.html

Java: if (s.isEmpty()) {}
来源：http://hz.ydzc1.top/gtbeoidswx.html

Go:   if s == "" {}
来源：http://hz.xingfuxueyuan.xyz/gthlwpboif.html

Ruby: if s.empty?
来源：http://hz.shanyushiyangtech.top/gtxnftkdak.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.hammf.cn/gtxiktfkgt.html

[E21] 超长截断加省略号
来源：http://hz.chenzaomai.com/gthpfhlmcl.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.shanyushiyangtech.top/gtucceykwt.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.jiagoushi.top/gtulcefior.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.shuidangran.top/gtpdziegti.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.zhiwuduotai.top/gtjnlogatf.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.aibaodan.cn/gtwviqfzbs.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.yuanzhike.top/gtckmimddl.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.gzhubu.top/gtgqhurroe.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.gotoacloud.top/gtlvkykfpi.html

[E22] 字节长度与字符长度
来源：http://hz.gaohongyu789.top/gtvronojpv.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.cheryme.top/gtcyxgoudi.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.gotoacloud.top/gtgkntjmlx.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.feifeiyinyue.top/gtselplqzy.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.sysykeji.top/gtmihcxtgj.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.shuidangran.top/gtpfrrsqow.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.haohaochexian.top/gthspmufih.html

Ruby: s.bytesize;  s.length
来源：http://hz.jinyuanbaomall.cn/gtbnyelgie.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.chenzaomai.com/gteotkwhjo.html

================================================================================
来源：http://hz.ehwqpu.com/gtfxjdmlvm.html

F. 文件与目录
来源：http://hz.xuanzx.com/gtmknhciuk.html

================================================================================
来源：http://hz.yuanzhike.top/gtxephbrdn.html

[F01] 读取整个文件
来源：http://hz.tianlin.xyz/gtwiflweyo.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.hfpthk.cn/gtodxvejuo.html

PHP:  file_get_contents("a.txt");
来源：http://hz.cqqwz.cn/gtphcsuqfk.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.shuidangran.top/gtsunrowii.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.iojbl.cn/gtjmabhkjl.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.nanxuanxn.top/gtstciubov.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.0kj1m.cn/gtylqzbygk.html

Ruby: File.read("a.txt")
来源：http://hz.birdmap.top/gtqwwwmsdl.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.yanxiufei.cn/gtdzzyjwaf.html

[F02] 逐行读取文件
来源：http://hz.quarkkingdee.top/gtkhpwdoha.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.shangyingyoupin.top/gtelexrloa.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.birdmap.top/gthycyzibw.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.hysaishi.cn/gtdfvivtnx.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.chenlongwang.top/gtgqaiejvo.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.cdnleiting.top/gtwuwsaohh.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.zhongyouzk.top/gtbrwondip.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.hnxiangtu.top/gtjefexhet.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.jinqigufen.top/gtolzfhyqr.html

[F03] 写入文件（覆盖）
来源：http://hz.shanyushiyangkeji.top/gtvdbpyqcq.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.gogol.net.cn/gtcvqxsnrv.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.hnqzz.top/gtaqqhjuil.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.guannengcc.top/gtdodmndxm.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jqgufenzy.top/gtqqostrag.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.sxryk.cn/gtjioqvpog.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.jyoumei.cn/gttzcgfvzf.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.ydjk.org.cn/gtkbumnfey.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.sweek.top/gtugrddovd.html

[F04] 追加写入文件
来源：http://hz.cdnleiting.top/gtafruawul.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.jqgufenzy.top/gtemxbrsae.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.jinghuilouyu.cn/gtphgtywkt.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.snrcjt.cn/gtsgqyozfl.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jinyuanbaomall.cn/gtqnvruprw.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.hongshengwenyu.top/gtmoalpyal.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.xuetiantiany.cn/gtmawpodts.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.zhiwuduotai.top/gtokuntqyh.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.ydjk.org.cn/gtbtrabwkc.html

[F05] 判断文件或目录是否存在
来源：http://hz.hongshengwenyu.top/gtbuntitcv.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.sysykeji.top/gtxbjtseif.html

PHP:  file_exists("a.txt");
来源：http://hz.smart0.xyz/gtjaekuwos.html

JS:   fs.existsSync("a.txt")
来源：http://hz.nanxuanxn.top/gtzeksqcmu.html

TS:   fs.existsSync("a.txt")
来源：http://hz.yuxming.cn/gtjosmvoht.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.nanxinkj.top/gtarlgtjca.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.52xcode.cn/gtlmchrsdu.html

Ruby: File.exist?("a.txt")
来源：http://hz.zdqjudy.top/gtrrumpsbr.html

C#:   File.Exists("a.txt")
来源：http://hz.chenzaomai.com/gtrpguqxyn.html

[F06] 删除文件
来源：http://hz.ivvv.top/gtdobxzanx.html

Py:   os.remove("a.txt")
来源：http://hz.zhiwuduotai.top/gtxgbagenx.html

PHP:  unlink("a.txt");
来源：http://hz.daria6918.cn/gtbacbqyex.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.pengpengdd.cyou/gtdchxewqg.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.cdnleiting.top/gtwfpdgqru.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.pengpengdd.cyou/gthsgxinga.html

Go:   os.Remove("a.txt")
来源：http://hz.bjfxy.top/gtcfpoahai.html

Ruby: File.delete("a.txt")
来源：http://hz.cdnleiting.top/gtirdzgagv.html

C#:   File.Delete("a.txt");
来源：http://hz.hnqzz.top/gtwjiybvbq.html

[F07] 创建目录（含多级）
来源：http://hz.yangfankeji.com/gtkhviigcr.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.yj202588.top/gtxlbamrvv.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.jinghuilouyu.cn/gtwmvhfbyg.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.gotoacloud.top/gtjubywpjr.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.9152youxi.cn/gthisjycdg.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.cucudq.cn/gtqfealqop.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.andypj.xyz/gtgkgrqjbf.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.zdqjudy.top/gtfpohljda.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.jinqigufen.top/gturkhgoqm.html

[F08] 遍历目录
来源：http://hz.tian-w.cn/gtezmemksu.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.gogol.net.cn/gtbkipsqel.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.guannengcc.top/gtybsdkdth.html

JS:   fs.readdirSync("dir")
来源：http://hz.daxiang520.top/gtmqwyalnw.html

TS:   fs.readdirSync("dir")
来源：http://hz.dianchejie.cn/gtdwzstyti.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.bjfxy.top/gtvwknaouy.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.birdmap.top/gtjvagsvit.html

Ruby: Dir.children("dir")
来源：http://hz.jinqigufen.top/gtikxbzexe.html

C#:   Directory.GetFiles("dir")
来源：http://hz.kuanghao11.cn/gtorbnritg.html

[F09] 获取文件大小
来源：http://hz.quarkkingdee.top/gtvcizqzus.html

Py:   os.path.getsize("a.txt")
来源：http://hz.ehwqpu.com/gtmjutkyxc.html

PHP:  filesize("a.txt");
来源：http://hz.shzxlz.cn/gtilrreaew.html

JS:   fs.statSync("a.txt").size
来源：http://hz.chenjidiqi.icu/gtnglcssqa.html

TS:   fs.statSync("a.txt").size
来源：http://hz.xingfuxueyuan.xyz/gthfctzqsl.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.ywan-chungtsiang.top/gtyxeqnxbi.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.kuanghao11.cn/gtpndisszy.html

Ruby: File.size("a.txt")
来源：http://hz.tanke756.top/gthigakvpl.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.smart0.xyz/gtqpwfrsaz.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.yangfankeji.com/gtfjnjdpms.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.mhx1999.top/gtjegvwave.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.ydjk.org.cn/gtoqiqcqby.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.daria6918.cn/gtriurzbqu.html

TS:   path.extname("a.txt")
来源：http://hz.chenzaomai.com/gtdidetycs.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.zycfv.cn/gtjfhmkwbp.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.jinyuanbaomall.cn/gtwhsosnof.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.9152youxi.cn/gtdshiwibg.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.hnxiangtu.top/gtzotzucme.html

[F11] 复制与移动文件
来源：http://hz.sxryk.cn/gtopuemtha.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.xuetiantiany.cn/gtmdzfweks.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.cheryme.top/gtzosbqjmt.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.hnqzz.top/gtbkwzbrel.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.shzxlz.cn/gtcveibogz.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.yongpay.top/gtxrpidlnk.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.pengpengdd.cyou/gtpmkktqdm.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.chenjidiqi.icu/gtewygbvdz.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.wangshuangyany.cn/gtjgoehqmz.html

[F12] CSV 读写
来源：http://hz.yongpay.top/gtyrmrlquq.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.xuanzx.com/gtkeryqmbl.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.jqgufenzy.top/gtsoejtdxw.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.yuxming.cn/gtheddgwyv.html

TS:   // 同上
来源：http://hz.zhengqikj.top/gtpnzuuuhi.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.hysaishi.cn/gtkighutkd.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.yanxiufei.cn/gttjodkgro.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.hywenlv.cn/gtmmngraod.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.xinyue.icu/gtmrulnaxv.html

================================================================================
来源：http://hz.aibaodan.cn/gtxwjxbbpv.html

G. 面向对象
来源：http://hz.fengsongda.top/gtwgebsrsj.html

================================================================================
来源：http://hz.nanxuanxn.top/gtsayhrmva.html

[G01] 定义类
来源：http://hz.cashguo.top/gtehswcita.html

Py:   class User: pass
来源：http://hz.hysaishi.cn/gtyumnerdw.html

PHP:  class User {}
来源：http://hz.bjfxy.top/gtplxbbdmb.html

JS:   class User {}
来源：http://hz.feifeiyinyue.top/gtzgpbupqu.html

TS:   class User { name: string = ""; }
来源：http://hz.zdqjudy.top/gtcqivfany.html

Java: class User {}
来源：http://hz.yanxiufei.cn/gtgyzeuyve.html

Go:   type User struct { Name string }
来源：http://hz.ywan-chungtsiang.top/gtepeuqqtv.html

Ruby: class User; end
来源：http://hz.zhiwuduotai.top/gtofuvxeiw.html

C#:   class User {}
来源：http://hz.bjfxy.top/gtrecoaxha.html

[G02] 构造函数
来源：http://hz.pengpengdd.cyou/gtxyhhnrtg.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.dashuyun.cn/gtmlujrbsg.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.quarkkingdee.top/gtqjgjxhlx.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.pengpengdd.cyou/gtnnlormff.html

TS:   constructor(public name: string) {}
来源：http://hz.hfpthk.cn/gtbsyemapw.html

Java: User(String name) { this.name = name; }
来源：http://hz.havefunace.top/gtcilfwzdp.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.ppjwa.cn/gtrszbddih.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.ydzc1.top/gtotzhualo.html

C#:   public User(string name) { Name = name; }
来源：http://hz.gotoacloud.top/gtpliqlsla.html

[G03] 实例属性
来源：http://hz.jqgufenzy.top/gtbryjkoev.html

Py:   self.name = "x"
来源：http://hz.guowangkeji.top/gtjtwtopwu.html

PHP:  public string $name = "x";
来源：http://hz.zhongyouzk.top/gtyszcsqwo.html

JS:   this.name = "x";
来源：http://hz.zhixingplan.top/gtgobregmc.html

TS:   name: string = "x";
来源：http://hz.gotoacloud.top/gtnagprznu.html

Java: private String name;
来源：http://hz.hysaishi.cn/gtjumpuwbl.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.yvedp.cn/gtyhyniifo.html

Ruby: @name = "x"
来源：http://hz.daria6918.cn/gtzinpupux.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.jiagoushi.top/gtridbsekn.html

[G04] 定义方法
来源：http://hz.guowangkeji.top/gtyiegbpzx.html

Py:   def greet(self): return self.name
来源：http://hz.redwolf501.top/gtcihtqswm.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.ivvv.top/gtklqaiijs.html

JS:   greet() { return this.name; }
来源：http://hz.yuanzhike.top/gtmfdtgsse.html

TS:   greet(): string { return this.name; }
来源：http://hz.andypj.xyz/gtwdijggyg.html

Java: String greet() { return name; }
来源：http://hz.feifeiyinyue.top/gtcbdcijgc.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.hnqzz.top/gticrfzwrp.html

Ruby: def greet; @name; end
来源：http://hz.zhijiandao.cn/gtpdhcuptq.html

C#:   public string Greet() => Name;
来源：http://hz.zdqjudy.top/gtndqdjcol.html

[G05] 继承
来源：http://hz.zhongyouzk.top/gtwhbvzktg.html

Py:   class Admin(User): pass
来源：http://hz.c1oappe.top/gtcbkhrmct.html

PHP:  class Admin extends User {}
来源：http://hz.cdnleiting.top/gtcscucknu.html

JS:   class Admin extends User {}
来源：http://hz.316326.xyz/gtpcpgrevi.html

TS:   class Admin extends User {}
来源：http://hz.yanxiufei.cn/gtuiccvyxd.html

Java: class Admin extends User {}
来源：http://hz.zycfv.cn/gtjyugnxrb.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.chenzaomai.com/gtcaxrbgfj.html

Ruby: class Admin < User; end
来源：http://hz.zhaomingkeji.xyz/gtwopcdcxj.html

C#:   class Admin : User {}
来源：http://hz.haohaochexian.top/gtwrsnbacp.html

[G06] 重写方法
来源：http://hz.cqqwz.cn/gthquklcxo.html

Py:   def greet(self): return "admin"
来源：http://hz.jlsjyb.cn/gtmwmswuyu.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.hysaishi.cn/gtchhaqtpb.html

JS:   greet() { return "admin"; }
来源：http://hz.zhixingplan.top/gtnqjqdmvn.html

TS:   greet(): string { return "admin"; }
来源：http://hz.mhx1999.top/gtsmqtyzbz.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.bjfxy.top/gtdijiycev.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.snrcjt.cn/gtsctvqppi.html

Ruby: def greet; "admin"; end
来源：http://hz.shzxlz.cn/gtlrdzdwkw.html

C#:   public override string Greet() => "admin";
来源：http://hz.hysaishi.cn/gtcyquyztz.html

[G07] 调用父类方法
来源：http://hz.kuanghao11.cn/gtdklduhis.html

Py:   super().greet()
来源：http://hz.svipenyu.cn/gtjtaqoqhm.html

PHP:  parent::greet();
来源：http://hz.tian-w.cn/gtgxndjrhf.html

JS:   super.greet();
来源：http://hz.ydzc1.top/gtufzjmvlj.html

TS:   super.greet();
来源：http://hz.meibo888.top/gtpxckxfus.html

Java: super.greet();
来源：http://hz.ydzc1.top/gtplsnjqpm.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.cucudq.cn/gtamypicbu.html

Ruby: super
来源：http://hz.hysaishi.cn/gtwanstbtd.html

C#:   base.Greet();
来源：http://hz.pengpengdd.cyou/gthkzrzgrg.html

[G08] 静态方法与属性
来源：http://hz.haohaochexian.top/gtiohgckbm.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.kuanghao11.cn/gtyzjnqpqp.html

PHP:  public static function f() {}
来源：http://hz.fengsongda.top/gtaqczkhti.html

JS:   static f() {}
来源：http://hz.zycfv.cn/gtymxnmgmz.html

TS:   static f(): void {}
来源：http://hz.gzhubu.top/gtllsndclx.html

Java: static void f() {}
来源：http://hz.ivvv.top/gtplbzgfdu.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.ppjwa.cn/gtjykhavnv.html

Ruby: def self.f; end
来源：http://hz.zhaomingkeji.xyz/gtothqxvut.html

C#:   public static void F() {}
来源：http://hz.fengsongda.top/gtjkpizdvj.html

[G09] 接口 / 抽象类
来源：http://hz.daria6918.cn/gttyyjxkgp.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.meibo888.top/gtwjyppdiu.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.mhx1999.top/gtgtbwigxu.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.shanyushiyangkeji.top/gtziqanqek.html

TS:   interface Shape { area(): number; }
来源：http://hz.sufxvd.cn/gtweoxjshu.html

Java: interface Shape { double area(); }
来源：http://hz.xylfe.cn/gtypznbllz.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.feifeiyinyue.top/gtapquyldh.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.nanxuanxn.top/gtoegzawvx.html

C#:   interface IShape { double Area(); }
来源：http://hz.pengpengdd.cyou/gtomntfefh.html

[G10] 访问控制
来源：http://hz.cashguo.top/gthanlgbuj.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.cdnleiting.top/gtmofihpna.html

PHP:  public / protected / private
来源：http://hz.vqdsnc.cn/gtxtvggdhx.html

JS:   #private 字段；其余公开
来源：http://hz.xylfe.cn/gtpsbnlerx.html

TS:   public / protected / private
来源：http://hz.havefunace.top/gtotfzzucn.html

Java: public / protected / private / 默认包级
来源：http://hz.bjfxy.top/gtxiumhcoj.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.hysaishi.cn/gtojcbbovj.html

Ruby: public / protected / private
来源：http://hz.zdqjudy.top/gtekoewbro.html

C#:   public / protected / private / internal
来源：http://hz.yueranfly.top/gthcjvohch.html

[G11] getter / setter
来源：http://hz.gaohongyu789.top/gtttfcteji.html

Py:   @property 与 @x.setter
来源：http://hz.zhongyouzk.top/gtnatcruxs.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.guowangkeji.top/gtgmcwnoom.html

JS:   get name() { return this._name; }
来源：http://hz.daria6918.cn/gtqwermdjy.html

TS:   get name(): string { return this._name; }
来源：http://hz.aibaodan.cn/gtfhqbdpeh.html

Java: public String getName() { return name; }
来源：http://hz.sxryk.cn/gttadrcyuh.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.yongpay.top/gtcrfbhhje.html

Ruby: attr_accessor :name
来源：http://hz.shanyushiyangtech.top/gtlamorwfm.html

C#:   public string Name { get; set; }
来源：http://hz.cqqwz.cn/gtltqzdaud.html

[G12] 对象转字符串
来源：http://hz.quarkkingdee.top/gtkqcgecdr.html

Py:   def __str__(self): return self.name
来源：http://hz.cashguo.top/gttpsyqpdg.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.guannengcc.top/gtwnbptxei.html

JS:   toString() { return this.name; }
来源：http://hz.daxiang520.top/gtdebfgzpu.html

TS:   toString(): string { return this.name; }
来源：http://hz.hongshengwenyu.top/gtwehszgob.html

Java: @Override public String toString() { return name; }
来源：http://hz.zycfv.cn/gtiycfhdam.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.yj202588.top/gtqgpvmpxm.html

Ruby: def to_s; @name; end
来源：http://hz.c1oappe.top/gthdkwvtlc.html

C#:   public override string ToString() => Name;
来源：http://hz.xuanzx.com/gtwvwqxkoq.html

[G13] 判断对象类型
来源：http://hz.316326.xyz/gtitdhufhz.html

Py:   isinstance(u, User)
来源：http://hz.nanxuanxn.top/gtyinzvoal.html

PHP:  $u instanceof User
来源：http://hz.yvedp.cn/gtrfazxagj.html

JS:   u instanceof User
来源：http://hz.xziqi.cn/gtzcjvybpi.html

TS:   u instanceof User
来源：http://hz.bjfxy.top/gtbxnvjgam.html

Java: u instanceof User
来源：http://hz.andypj.xyz/gtfpljljwk.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.haohaochexian.top/gterpdzrzz.html

Ruby: u.is_a?(User)
来源：http://hz.sysykeji.top/gtjsegxirl.html

C#:   u is User
来源：http://hz.316326.xyz/gtigvqmylj.html

[G14] 数据类 / record
来源：http://hz.tianlin.xyz/gtghtgtsjs.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.andypj.xyz/gtodsrilen.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.cashguo.top/gtjiixqviw.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.jqgfzy.top/gtwjxtczfr.html

TS:   type User = { name: string; age: number };
来源：http://hz.sysykeji.top/gtulhakslj.html

Java: record User(String name, int age) {}
来源：http://hz.tanke756.top/gtxcpfftze.html

Go:   type User struct { Name string; Age int }
来源：http://hz.zdqjudy.top/gtcotiloyc.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.havefunace.top/gtdadthaib.html

C#:   record User(string Name, int Age);
来源：http://hz.gogol.net.cn/gtyhuweqfm.html

[G15] 枚举
来源：http://hz.cqqwz.cn/gtyrikyxaf.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.gogol.net.cn/gtzmakqgqr.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.fzhhl.top/gtkfqqkdvl.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.shangyingyoupin.top/gtkrhgsuli.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.ivvv.top/gtagrpxsqz.html

Java: enum Color { RED, GREEN }
来源：http://hz.havefunace.top/gttzlfwjof.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.jinyuanbaomall.cn/gtqkelqyul.html

Ruby: Color = %i[red green].freeze
来源：http://hz.c1oappe.top/gttegfqknf.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.tanke756.top/gtiwqwlnqa.html

[G16] 对象转数组 / 字典
来源：http://hz.yj20258.top/gttramrkqc.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.wangshuangyany.cn/gtsfcgglcz.html

PHP:  get_object_vars($obj);
来源：http://hz.jinghuilouyu.cn/gtttoohpzv.html

JS:   Object.entries(obj)
来源：http://hz.yj20258.top/gtnkotoedh.html

TS:   Object.entries(obj)
来源：http://hz.pycfn.com/gtnqmxrgfe.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.zycfv.cn/gtkdrnifeq.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.shzxlz.cn/gtctpocxfh.html

Ruby: obj.instance_variables
来源：http://hz.guowangkeji.top/gtkzuouoop.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.snrcjt.cn/gtgtdxoybs.html

================================================================================
来源：http://hz.yj202588.top/gtnpqvptjd.html

H. 异常与错误处理
来源：http://hz.smart0.xyz/gtrvkmwmte.html

================================================================================
来源：http://hz.guannengcc.top/gtuzytysus.html

[H01] try / catch 基础
来源：http://hz.bjfxy.top/gtxnjvnaim.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.cucudq.cn/gtkdyiabqq.html


<!-- 参考信息 -->