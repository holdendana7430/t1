代发 wailian999

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.sweek.top/gteazwjotx.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.pycfn.com/gtyfwexdxi.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.xinyue.icu/gthsmlfisx.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.yj20258888.top/gtxppzatbc.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.shuidangran.top/gtmzhrddun.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.pengpengdd.cyou/gtbdqvbgtl.html

Ruby: s.capitalize
来源：http://hz.meibo888.top/gtxqdnnrte.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.wangshuangyany.cn/gtswdgeqdb.html

[E18] 模板占位符替换
来源：http://hz.ivvv.top/gtlnrxnzqa.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.xuetiantiany.cn/gthfuyivcf.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.cqqwz.cn/gtjvjkddcq.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.bjfxy.top/gtnvmijikf.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.jinghuilouyu.cn/gtnlorbdfi.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.svipenyu.cn/gtiraseele.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.hysaishi.cn/gtitpadkuv.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.zdqjudy.top/gtozfcxrwh.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.0kj1m.cn/gtamvfqyai.html

[E19] 多行文本按行拆分
来源：http://hz.shangyingyoupin.top/gtyhadsixd.html

Py:   s.splitlines()
来源：http://hz.yj20258888.top/gtcmwscyqt.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.gogol.net.cn/gtjfkpipuu.html

JS:   s.split(/\r?\n/)
来源：http://hz.sweek.top/gtllbahsho.html

TS:   s.split(/\r?\n/)
来源：http://hz.svipenyu.cn/gtaseeypjs.html

Java: s.lines().toList()
来源：http://hz.zhengqikj.top/gtrjpnqyyk.html

Go:   strings.Split(s, "\n")
来源：http://hz.havefunace.top/gtaybochlp.html

Ruby: s.lines
来源：http://hz.shanyushiyangkeji.top/gtmjyuskjl.html

C#:   s.Split('\n')
来源：http://hz.zhengqikj.top/gtajxpgtmr.html

[E20] 判断字符串是否为空
来源：http://hz.yvedp.cn/gtxdtdfwvz.html

Py:   if not s:
来源：http://hz.smart0.xyz/gtppguhqab.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.quarkkingdee.top/gtcufviior.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.gogol.net.cn/gtwjuowaqf.html

TS:   if (s === "") {}
来源：http://hz.wangdashe.top/gtsaeyhxei.html

Java: if (s.isEmpty()) {}
来源：http://hz.zdqjudy.top/gttmigzlis.html

Go:   if s == "" {}
来源：http://hz.nanxinkj.top/gtvahmkiox.html

Ruby: if s.empty?
来源：http://hz.cheryme.top/gtbtcgfhod.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.nanxinkj.top/gtebyavrrv.html

[E21] 超长截断加省略号
来源：http://hz.sweek.top/gtyfrlhorq.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.316326.xyz/gtyttmyriq.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.zycfv.cn/gtrwpbyygn.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.cdnleiting.top/gtdltaxqfy.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.fzhhl.top/gtnkionimf.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.dianchejie.cn/gtnzevktsb.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.ppjwa.cn/gtphwmmmzp.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.shuidangran.top/gtelekkkee.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.shzxlz.cn/gtfveszeht.html

[E22] 字节长度与字符长度
来源：http://hz.cdnleiting.top/gtaoacuxdh.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.hysaishi.cn/gtycchetud.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.gzhubu.top/gtyfhipwae.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.tanke756.top/gtpbygzuwt.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jlsjyb.cn/gtqpfkjqoq.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.birdmap.top/gtpwcjmvhe.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.daria6918.cn/gtysxlqiub.html

Ruby: s.bytesize;  s.length
来源：http://hz.fzhhl.top/gturyjoimg.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.zhoulong.xyz/gtsabbecpt.html

================================================================================
来源：http://hz.redwolf501.top/gtoqhnlixa.html

F. 文件与目录
来源：http://hz.xuetiantiany.cn/gttvwwcise.html

================================================================================
来源：http://hz.chenzaomai.com/gtvkutprxq.html

[F01] 读取整个文件
来源：http://hz.yangfankeji.com/gtjjnlxsua.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.ppjwa.cn/gtofagctdg.html

PHP:  file_get_contents("a.txt");
来源：http://hz.snrcjt.cn/gtxteqsbte.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.sweek.top/gtwxwmocnz.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.wangshuangyany.cn/gthafzgvsz.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.zhaomingkeji.xyz/gtpcpmxgfn.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.snrcjt.cn/gtzhevzmug.html

Ruby: File.read("a.txt")
来源：http://hz.zhaomingkeji.xyz/gttamfqyuv.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.gzhubu.top/gtpyytxkxi.html

[F02] 逐行读取文件
来源：http://hz.jinqigufen.top/gtqvgdhqwk.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.yj202588.top/gtrbawvluz.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.iojbl.cn/gtismtiymd.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yonumen.top/gtlnozrvgx.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.shanyushiyangtech.top/gtveyslgzq.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.yj20258.top/gtxzcqnpaw.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.jianghu66.top/gtluozaemo.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.cqqwz.cn/gtnuilqwhr.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.smart0.xyz/gtbsgitytl.html

[F03] 写入文件（覆盖）
来源：http://hz.jinghuilouyu.cn/gtyknfnyqy.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.sweek.top/gtdectjots.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.zhongyouzk.top/gthhfwwpiw.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.kuanghao11.cn/gtdocumcfy.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jinqigfzy.top/gtzhqafexx.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.zhijiandao.cn/gtlssqltwf.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.0kj1m.cn/gtnazooqis.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.wangshuangyany.cn/gtgvqpgcuc.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.gzhubu.top/gtdskciwde.html

[F04] 追加写入文件
来源：http://hz.dashuyun.cn/gtyivxwbcj.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.zhongyouzk.top/gtkqkhozht.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.jiagoushi.top/gttjfqigsl.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.ywan-chungtsiang.top/gtdvekfjji.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zhoulong.xyz/gtiqhsckpn.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.quarkkingdee.top/gtgdusqhpg.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.tianlin.xyz/gtpyylghac.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.zhongyouzk.top/gtgsfqjnus.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.yuanzhike.top/gtkdnicemd.html

[F05] 判断文件或目录是否存在
来源：http://hz.tianlin.xyz/gtvhgycjca.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.cucudq.cn/gtaovfikhq.html

PHP:  file_exists("a.txt");
来源：http://hz.gzhubu.top/gtwkaximlp.html

JS:   fs.existsSync("a.txt")
来源：http://hz.aizwys.cn/gtnfqhyxhj.html

TS:   fs.existsSync("a.txt")
来源：http://hz.nwbrower.top/gtvbjtbpin.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.jqgfzy.top/gtadewtxic.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.zdqjudy.top/gtrebtakjh.html

Ruby: File.exist?("a.txt")
来源：http://hz.andypj.xyz/gtrsmizvrt.html

C#:   File.Exists("a.txt")
来源：http://hz.zycfv.cn/gtwrebmdvm.html

[F06] 删除文件
来源：http://hz.quarkkingdee.top/gtahodwlqy.html

Py:   os.remove("a.txt")
来源：http://hz.yonumen.top/gtxsbnjvkd.html

PHP:  unlink("a.txt");
来源：http://hz.hongshengwenyu.top/gtpabxjcjm.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.hongshengwenyu.top/gtdgdgnevc.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.ppjwa.cn/gtsbejjvxa.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.havefunace.top/gtscdpoltm.html

Go:   os.Remove("a.txt")
来源：http://hz.cucudq.cn/gtgjpmnvlu.html

Ruby: File.delete("a.txt")
来源：http://hz.jqgufenzy.top/gtpkwekiml.html

C#:   File.Delete("a.txt");
来源：http://hz.dianchejie.cn/gtgdgzjnfa.html

[F07] 创建目录（含多级）
来源：http://hz.dianchejie.cn/gttimhpmwk.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.fzhhl.top/gtqlqgtjnb.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.hnqzz.top/gtamxkhxyz.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jinghuilouyu.cn/gtnuodzyev.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.shanyushiyangtech.top/gtnzkecdgj.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.zhixingplan.top/gtknpqldfl.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.snrcjt.cn/gtciwtptjb.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.wangdashe.top/gtjohxlnma.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.chenlongwang.top/gtswxztumu.html

[F08] 遍历目录
来源：http://hz.sysykeji.top/gtzfjpexiz.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.ydjk.org.cn/gtttoulbdk.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.meibo888.top/gtooqspfgz.html

JS:   fs.readdirSync("dir")
来源：http://hz.yj202588.top/gtdrnsgcwm.html

TS:   fs.readdirSync("dir")
来源：http://hz.andypj.xyz/gthbpclstr.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.zhijiandao.cn/gtadvqbxqv.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.jinqigufen.top/gtgvvfmfxb.html

Ruby: Dir.children("dir")
来源：http://hz.tianlin.xyz/gtjwdjmoyo.html

C#:   Directory.GetFiles("dir")
来源：http://hz.shanyushiyangtech.top/gtzxneryst.html

[F09] 获取文件大小
来源：http://hz.cqqwz.cn/gtpvnxvsqd.html

Py:   os.path.getsize("a.txt")
来源：http://hz.tianlin.xyz/gtcpjmabjl.html

PHP:  filesize("a.txt");
来源：http://hz.hnxiangtu.top/gtjechgkmk.html

JS:   fs.statSync("a.txt").size
来源：http://hz.zhaomingkeji.xyz/gtttaopgtx.html

TS:   fs.statSync("a.txt").size
来源：http://hz.jianghu66.top/gtwzrebcku.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.ywan-chungtsiang.top/gtdblugxot.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.haohaochexian.top/gtgjsfxnez.html

Ruby: File.size("a.txt")
来源：http://hz.smart0.xyz/gtqjowxhqf.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.52xcode.cn/gtrouhiipn.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.daria6918.cn/gtsbnayqub.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.c1oappe.top/gtugqaijee.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.aibaodan.cn/gtpfxsakjm.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.yuxming.cn/gtqhwcnptq.html

TS:   path.extname("a.txt")
来源：http://hz.yongpay.top/gtcaosednb.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.shanyushiyangkeji.top/gtlhsmaiee.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.smart0.xyz/gttorwudui.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.birdmap.top/gtqtgmwdru.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.52xcode.cn/gtqlckjzxi.html

[F11] 复制与移动文件
来源：http://hz.cashguo.top/gtazndnjww.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.yueranfly.top/gtivgjclyd.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.dashuyun.cn/gtcfwzomxk.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yj20258.top/gtyzhjrjsc.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.cdnleiting.top/gtqddzhdtu.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.hysaishi.cn/gtoklrsfeu.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.jqgufenzy.top/gtyrcxepbj.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.jiagoushi.top/gtalbslpbw.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.0kj1m.cn/gteqvdtfdb.html

[F12] CSV 读写
来源：http://hz.nanxinkj.top/gtygsuridt.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.hongshengwenyu.top/gtmjwfbjme.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.chenzaomai.com/gtmvsxogud.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.sufxvd.cn/gtlywmrngk.html

TS:   // 同上
来源：http://hz.yonumen.top/gtysgzpalt.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.yueranfly.top/gtspuucqbz.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.ywan-chungtsiang.top/gtabhmgmpi.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.chenzaomai.com/gtbfyrvibw.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.0kj1m.cn/gtxtbkfzha.html

================================================================================
来源：http://hz.hammf.cn/gtleazuaub.html

G. 面向对象
来源：http://hz.zdqjudy.top/gtrqjluarj.html

================================================================================
来源：http://hz.jianghu66.top/gtzrjwqikt.html

[G01] 定义类
来源：http://hz.hnqzz.top/gtkyspcggu.html

Py:   class User: pass
来源：http://hz.yonumen.top/gtulfelnzf.html

PHP:  class User {}
来源：http://hz.ydzc1.top/gtfwbapsnu.html

JS:   class User {}
来源：http://hz.guannengcc.top/gtojtmcfyx.html

TS:   class User { name: string = ""; }
来源：http://hz.52xcode.cn/gthfyyqqhk.html

Java: class User {}
来源：http://hz.cashguo.top/gtktkjdxym.html

Go:   type User struct { Name string }
来源：http://hz.iojbl.cn/gtslpbgdht.html

Ruby: class User; end
来源：http://hz.daxiang520.top/gtpfavgjsy.html

C#:   class User {}
来源：http://hz.xingfuxueyuan.xyz/gteqvwxkrk.html

[G02] 构造函数
来源：http://hz.hnxiangtu.top/gtxeqexhhq.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.nanxinkj.top/gtcpggidop.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.xingfuxueyuan.xyz/gtzmtyryab.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.shanyushiyangkeji.top/gtjyvffszu.html

TS:   constructor(public name: string) {}
来源：http://hz.zhijiandao.cn/gtzuxfhwio.html

Java: User(String name) { this.name = name; }
来源：http://hz.vqdsnc.cn/gtgyitngwl.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.hnxiangtu.top/gtowuvuuti.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.chenlongwang.top/gtfrzmodds.html

C#:   public User(string name) { Name = name; }
来源：http://hz.yonumen.top/gtmzpjuhqc.html

[G03] 实例属性
来源：http://hz.chenjidiqi.icu/gtpejbexap.html

Py:   self.name = "x"
来源：http://hz.zhijiandao.cn/gtvfietqgh.html

PHP:  public string $name = "x";
来源：http://hz.gaohongyu789.top/gtfrfcptau.html

JS:   this.name = "x";
来源：http://hz.chenlongwang.top/gtruulwvsk.html

TS:   name: string = "x";
来源：http://hz.havefunace.top/gtvhyhwqwj.html

Java: private String name;
来源：http://hz.sxryk.cn/gtaawczkno.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.jianghu66.top/gtadebvnoi.html

Ruby: @name = "x"
来源：http://hz.zhiwuduotai.top/gtbdbrpmge.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.cdnleiting.top/gtqmadojqd.html

[G04] 定义方法
来源：http://hz.fzhhl.top/gtrnrorbnu.html

Py:   def greet(self): return self.name
来源：http://hz.sweek.top/gtuqqcctpf.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.smart0.xyz/gtxcxqdhyf.html

JS:   greet() { return this.name; }
来源：http://hz.cqqwz.cn/gtmxsqrzfs.html

TS:   greet(): string { return this.name; }
来源：http://hz.hfpthk.cn/gtvlidhfew.html

Java: String greet() { return name; }
来源：http://hz.xziqi.cn/gtahbaydep.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.jiagoushi.top/gtocokeqmj.html

Ruby: def greet; @name; end
来源：http://hz.zhoulong.xyz/gtdjtpmhqp.html

C#:   public string Greet() => Name;
来源：http://hz.sweek.top/gtmkppqixs.html

[G05] 继承
来源：http://hz.gogol.net.cn/gtrvlhstpo.html

Py:   class Admin(User): pass
来源：http://hz.shanyushiyangtech.top/gtkikmykjj.html

PHP:  class Admin extends User {}
来源：http://hz.yvedp.cn/gtdpqxgbdk.html

JS:   class Admin extends User {}
来源：http://hz.hfpthk.cn/gtquxqsogi.html

TS:   class Admin extends User {}
来源：http://hz.andypj.xyz/gtjedzeoxs.html

Java: class Admin extends User {}
来源：http://hz.zhongyouzk.top/gtnzpgntfu.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.cucudq.cn/gtnclnzzyu.html

Ruby: class Admin < User; end
来源：http://hz.zhaomingkeji.xyz/gtssufpoci.html

C#:   class Admin : User {}
来源：http://hz.guannengcc.top/gthadcdipt.html

[G06] 重写方法
来源：http://hz.guowangkeji.top/gtilrnvtaq.html

Py:   def greet(self): return "admin"
来源：http://hz.cheryme.top/gtegnirjoa.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.yangfankeji.com/gtzlxaklsq.html

JS:   greet() { return "admin"; }
来源：http://hz.guannengcc.top/gtaqqypbjb.html

TS:   greet(): string { return "admin"; }
来源：http://hz.xingfuxueyuan.xyz/gtvknhdcss.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.0kj1m.cn/gtiayladtf.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.yangfankeji.com/gtvegvanry.html

Ruby: def greet; "admin"; end
来源：http://hz.zhoulong.xyz/gtnitdmizy.html

C#:   public override string Greet() => "admin";
来源：http://hz.meibo888.top/gtpqwddgxr.html

[G07] 调用父类方法
来源：http://hz.cucudq.cn/gttofkqymy.html

Py:   super().greet()
来源：http://hz.316326.xyz/gtuhuoiiuw.html

PHP:  parent::greet();
来源：http://hz.yanxiufei.cn/gtdqfdksbl.html

JS:   super.greet();
来源：http://hz.sufxvd.cn/gtjykffttb.html

TS:   super.greet();
来源：http://hz.jiagoushi.top/gtaalxlczv.html

Java: super.greet();
来源：http://hz.feifeiyinyue.top/gtqzpaixsf.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.guannengcc.top/gtqlhbhwnq.html

Ruby: super
来源：http://hz.daxiang520.top/gtwdachohl.html

C#:   base.Greet();
来源：http://hz.jianghu66.top/gtszvbkqis.html

[G08] 静态方法与属性
来源：http://hz.mhx1999.top/gtyxbamapb.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.fzhhl.top/gthrdazdft.html

PHP:  public static function f() {}
来源：http://hz.ehwqpu.com/gtmdnxbjzx.html

JS:   static f() {}
来源：http://hz.jinqigufen.top/gterzlasgh.html

TS:   static f(): void {}
来源：http://hz.snrcjt.cn/gtikrsfmco.html

Java: static void f() {}
来源：http://hz.chenlongwang.top/gtlxxhigmp.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.andypj.xyz/gtvnauecdh.html

Ruby: def self.f; end
来源：http://hz.ppjwa.cn/gtfaeqixfu.html

C#:   public static void F() {}
来源：http://hz.shuidangran.top/gtveljphgk.html

[G09] 接口 / 抽象类
来源：http://hz.yj202588.top/gtpytlxhqo.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.jinqigufen.top/gtoimmukpb.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.zhoulong.xyz/gtagyolgfo.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.jlsjyb.cn/gtmaaawjyt.html

TS:   interface Shape { area(): number; }
来源：http://hz.hammf.cn/gtbffshhde.html

Java: interface Shape { double area(); }
来源：http://hz.hnxiangtu.top/gtdiuqkthc.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.cheryme.top/gtlrxnwfnd.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.yangfankeji.com/gtyitwmcyp.html

C#:   interface IShape { double Area(); }
来源：http://hz.yvedp.cn/gtptmuymub.html

[G10] 访问控制
来源：http://hz.yj20258888.top/gtwyuccvcl.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.redwolf501.top/gtnzccgryb.html

PHP:  public / protected / private
来源：http://hz.nanxinkj.top/gtlzzwtmct.html

JS:   #private 字段；其余公开
来源：http://hz.sysykeji.top/gtiyzhakqh.html

TS:   public / protected / private
来源：http://hz.snrcjt.cn/gtmugrszsu.html

Java: public / protected / private / 默认包级
来源：http://hz.ywan-chungtsiang.top/gtxqwqnivb.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.316326.xyz/gtnsizdiqc.html

Ruby: public / protected / private
来源：http://hz.redwolf501.top/gthwmbmtfl.html

C#:   public / protected / private / internal
来源：http://hz.jqgufenzy.top/gtutyueqyy.html

[G11] getter / setter
来源：http://hz.gogol.net.cn/gtghfekrwf.html

Py:   @property 与 @x.setter
来源：http://hz.sysykeji.top/gtgampfran.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.sweek.top/gtljvldnem.html

JS:   get name() { return this._name; }
来源：http://hz.snrcjt.cn/gtyhsjnjln.html

TS:   get name(): string { return this._name; }
来源：http://hz.wangshuangyany.cn/gtooalvipw.html

Java: public String getName() { return name; }
来源：http://hz.zhengqikj.top/gtfvlifxjs.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.jqgfzy.top/gtynklkomq.html

Ruby: attr_accessor :name
来源：http://hz.sufxvd.cn/gtevgyqwln.html

C#:   public string Name { get; set; }
来源：http://hz.pycfn.com/gtqlmlnddj.html

[G12] 对象转字符串
来源：http://hz.ehwqpu.com/gtjhkopril.html

Py:   def __str__(self): return self.name
来源：http://hz.sufxvd.cn/gtvvtdcike.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.shzxlz.cn/gtqzzrixog.html

JS:   toString() { return this.name; }
来源：http://hz.hnxiangtu.top/gthetdilbt.html

TS:   toString(): string { return this.name; }
来源：http://hz.c1oappe.top/gtzpartiam.html

Java: @Override public String toString() { return name; }
来源：http://hz.aizwys.cn/gtofgxcqsm.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.ydjk.org.cn/gtsjblvsjp.html

Ruby: def to_s; @name; end
来源：http://hz.jinqigufen.top/gtslnnqila.html

C#:   public override string ToString() => Name;
来源：http://hz.cashguo.top/gtxtueqxow.html

[G13] 判断对象类型
来源：http://hz.shuidangran.top/gtmhkzjbty.html

Py:   isinstance(u, User)
来源：http://hz.zdqjudy.top/gtwygkaqee.html

PHP:  $u instanceof User
来源：http://hz.ydjk.org.cn/gtdhiapxlw.html

JS:   u instanceof User
来源：http://hz.feifeiyinyue.top/gtgtxscxko.html

TS:   u instanceof User
来源：http://hz.mhx1999.top/gtavhzwjzo.html

Java: u instanceof User
来源：http://hz.bjfxy.top/gtquoypvpj.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.shanyushiyangkeji.top/gtrvqfpuls.html

Ruby: u.is_a?(User)
来源：http://hz.yuanzhike.top/gtvwollvpj.html

C#:   u is User
来源：http://hz.shuidangran.top/gtkgmbmtxh.html

[G14] 数据类 / record
来源：http://hz.jyoumei.cn/gtebjyxfvd.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.fengsongda.top/gtiohyepuy.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.ywan-chungtsiang.top/gtnzdwttwa.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.shzxlz.cn/gthoresvtt.html

TS:   type User = { name: string; age: number };
来源：http://hz.ydjk.org.cn/gtmaftsvbu.html

Java: record User(String name, int age) {}
来源：http://hz.ywan-chungtsiang.top/gtyowjqwyg.html

Go:   type User struct { Name string; Age int }
来源：http://hz.zhoulong.xyz/gtjjlwziwv.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.cqqwz.cn/gttrpdrgsn.html

C#:   record User(string Name, int Age);
来源：http://hz.wangshuangyany.cn/gtzpzlsnqg.html

[G15] 枚举
来源：http://hz.yj20258.top/gtgwwhtnxk.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.316326.xyz/gtvmhoqqjn.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.feifeiyinyue.top/gtapietcsy.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.hnxiangtu.top/gtqejtspdu.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.cqqwz.cn/gtfakbjjvk.html

Java: enum Color { RED, GREEN }
来源：http://hz.bjfxy.top/gtbmhfhxjv.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.yangfankeji.com/gtrewbvede.html


<!-- 参考信息 -->