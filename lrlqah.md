代发 wailian999

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.smart0.xyz/gtylxbzhtq.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.yuxming.cn/gtbwsodwju.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.0kj1m.cn/gtaxdpnxzo.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.kuanghao11.cn/gthwmqorfm.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.iojbl.cn/gtdolfqyhg.html

[E19] 多行文本按行拆分
来源：http://hz.redwolf501.top/gtwsctwgvf.html

Py:   s.splitlines()
来源：http://hz.hnqzz.top/gtevubiaoj.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.zhaomingkeji.xyz/gtkfkruioc.html

JS:   s.split(/\r?\n/)
来源：http://hz.guannengcc.top/gtoqsjflmd.html

TS:   s.split(/\r?\n/)
来源：http://hz.redwolf501.top/gtrvhadztv.html

Java: s.lines().toList()
来源：http://hz.quarkkingdee.top/gtfgqlxmxd.html

Go:   strings.Split(s, "\n")
来源：http://hz.sysykeji.top/gticfrzpuj.html

Ruby: s.lines
来源：http://hz.jinghuilouyu.cn/gtzuipztsj.html

C#:   s.Split('\n')
来源：http://hz.cucudq.cn/gtuyvoprri.html

[E20] 判断字符串是否为空
来源：http://hz.cheryme.top/gtbggnxhpk.html

Py:   if not s:
来源：http://hz.shzxlz.cn/gtvwkkxfoo.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.yvedp.cn/gtsrwyqwyq.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.jianghu66.top/gtvzegllgh.html

TS:   if (s === "") {}
来源：http://hz.yj20258.top/gtdioflqtu.html

Java: if (s.isEmpty()) {}
来源：http://hz.chenlongwang.top/gtvoonzkqj.html

Go:   if s == "" {}
来源：http://hz.nwbrower.top/gthhdnense.html

Ruby: if s.empty?
来源：http://hz.guowangkeji.top/gtbeqxhlzj.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.c1oappe.top/gtdlaeruap.html

[E21] 超长截断加省略号
来源：http://hz.ehwqpu.com/gthwyjdcor.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.guannengcc.top/gtxycgnzri.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.yj202588.top/gtegifzszq.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.cucudq.cn/gtwduovnit.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yuanzhike.top/gtkesdmosj.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.daxiang520.top/gtjfruogej.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.aibaodan.cn/gthtpqjmvm.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.ywan-chungtsiang.top/gtynitieau.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.ybcxt.top/gtnrahivyg.html

[E22] 字节长度与字符长度
来源：http://hz.hysaishi.cn/gtjvvtbmxh.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.yueranfly.top/gtlnwbyyjf.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.aibaodan.cn/gtnnkmytlx.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.hnxiangtu.top/gtbsjmiyjl.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.smart0.xyz/gtrbonrzlu.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.9152youxi.cn/gtinkpvbvu.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.jqgufenzy.top/gttkfkzflx.html

Ruby: s.bytesize;  s.length
来源：http://hz.yuanzhike.top/gtvelpwgml.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.gogol.net.cn/gtgyuhmplp.html

================================================================================
来源：http://hz.ehwqpu.com/gtncjngntz.html

F. 文件与目录
来源：http://hz.haohaochexian.top/gtkyofsvng.html

================================================================================
来源：http://hz.ehwqpu.com/gtktjqcwmz.html

[F01] 读取整个文件
来源：http://hz.gaohongyu789.top/gtzfiozvng.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.daria6918.cn/gtzbyctsit.html

PHP:  file_get_contents("a.txt");
来源：http://hz.zhijiandao.cn/gtgyauxxht.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.zhengqikj.top/gtnudqnkva.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.zhixingplan.top/gttaplmxmn.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.guannengcc.top/gtxkgbgqka.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.zycfv.cn/gttelpbvcc.html

Ruby: File.read("a.txt")
来源：http://hz.redwolf501.top/gtwuccwhqo.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.hnxiangtu.top/gtkbcojjpc.html

[F02] 逐行读取文件
来源：http://hz.jqgfzy.top/gtlmeysuhh.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.tian-w.cn/gtardjhyil.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.zhongyouzk.top/gtipnddsxq.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.birdmap.top/gtobdpxgci.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.sufxvd.cn/gtqpyfnbml.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.chenlongwang.top/gttijwjfdb.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.jinyuanbaomall.cn/gtrihbwbim.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.yvedp.cn/gtqxoozkww.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.bjfxy.top/gtlrctkkgy.html

[F03] 写入文件（覆盖）
来源：http://hz.zhengqikj.top/gtxdwumpjb.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.c1oappe.top/gtjbdvzdnu.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.zhiwuduotai.top/gtgrxgcdaq.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.xingfuxueyuan.xyz/gtyfmrbzlr.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yuxming.cn/gtgmnxdync.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.shzxlz.cn/gtpgfhhhra.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.jqgufenzy.top/gtihsssnkl.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.kuanghao11.cn/gtcpxgwsre.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.gogol.net.cn/gtlomotmcx.html

[F04] 追加写入文件
来源：http://hz.zhongyouzk.top/gtztqiztxh.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.yueranfly.top/gttgfrxlkb.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.mhx1999.top/gtoxqmfkzn.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.hammf.cn/gthlnyptrz.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.sysykeji.top/gtwcnmpsum.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.sufxvd.cn/gtwobjfxob.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.hnqzz.top/gtohmvajkx.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.hammf.cn/gtuxvytzlw.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.wangshuangyany.cn/gtyxkcucjx.html

[F05] 判断文件或目录是否存在
来源：http://hz.yueranfly.top/gtkbwwjiav.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.tianlin.xyz/gttdkcrmmj.html

PHP:  file_exists("a.txt");
来源：http://hz.cashguo.top/gtvyqfimgq.html

JS:   fs.existsSync("a.txt")
来源：http://hz.fengsongda.top/gteudpjacw.html

TS:   fs.existsSync("a.txt")
来源：http://hz.pengpengdd.cyou/gtitfeegbd.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.zhongyouzk.top/gtrrrmciwh.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.quarkkingdee.top/gtuwbwjfhm.html

Ruby: File.exist?("a.txt")
来源：http://hz.tian-w.cn/gtgyzmntzk.html

C#:   File.Exists("a.txt")
来源：http://hz.yj202588.top/gtunkwrlel.html

[F06] 删除文件
来源：http://hz.9152youxi.cn/gtqprjydle.html

Py:   os.remove("a.txt")
来源：http://hz.zhiwuduotai.top/gtquslxfdz.html

PHP:  unlink("a.txt");
来源：http://hz.0kj1m.cn/gtmxgaegsx.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.jinyuanbaomall.cn/gttidfklxr.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.hywenlv.cn/gtnumksqzy.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.cucudq.cn/gtgwvlpuyc.html

Go:   os.Remove("a.txt")
来源：http://hz.gzhubu.top/gtqspcihba.html

Ruby: File.delete("a.txt")
来源：http://hz.aizwys.cn/gtojgstcrc.html

C#:   File.Delete("a.txt");
来源：http://hz.svipenyu.cn/gtpzeqqijr.html

[F07] 创建目录（含多级）
来源：http://hz.cheryme.top/gtplrxvyrd.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.svipenyu.cn/gtbplrqewe.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.yongpay.top/gtgqnjbess.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yanxiufei.cn/gtfujwxcaf.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.hfpthk.cn/gtbdktpofy.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.wangshuangyany.cn/gtpqgqkrxe.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.nwbrower.top/gtskadircx.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.ehwqpu.com/gtumemwxmj.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.hnqzz.top/gtedkcgauz.html

[F08] 遍历目录
来源：http://hz.c1oappe.top/gtyjnhqykd.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.xziqi.cn/gtluogygox.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.hysaishi.cn/gtyskdieea.html

JS:   fs.readdirSync("dir")
来源：http://hz.ywan-chungtsiang.top/gtulliehyk.html

TS:   fs.readdirSync("dir")
来源：http://hz.zycfv.cn/gtblqywzmd.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.yangfankeji.com/gtqlgkldkn.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.chenlongwang.top/gtjdnsricd.html

Ruby: Dir.children("dir")
来源：http://hz.chenlongwang.top/gtnznqbvln.html

C#:   Directory.GetFiles("dir")
来源：http://hz.ehwqpu.com/gtqwfxvjtk.html

[F09] 获取文件大小
来源：http://hz.andypj.xyz/gtajwtiqhy.html

Py:   os.path.getsize("a.txt")
来源：http://hz.316326.xyz/gtwpmaklpc.html

PHP:  filesize("a.txt");
来源：http://hz.hnqzz.top/gtlndgxgpp.html

JS:   fs.statSync("a.txt").size
来源：http://hz.xziqi.cn/gtkvviofji.html

TS:   fs.statSync("a.txt").size
来源：http://hz.yj20258888.top/gtasjcvwas.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.xinyue.icu/gtegsiqhul.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.ivvv.top/gtrxmabtwn.html

Ruby: File.size("a.txt")
来源：http://hz.yuanzhike.top/gtumyvkngy.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.sufxvd.cn/gtjuoddwzy.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.sysykeji.top/gtoflvkjgw.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.9152youxi.cn/gtzmgklunc.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.redwolf501.top/gtspfygsza.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.52xcode.cn/gtpgasfhhv.html

TS:   path.extname("a.txt")
来源：http://hz.shangyingyoupin.top/gtklryyloq.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.smart0.xyz/gtjhgbjgws.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.sxryk.cn/gtampsbinw.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.316326.xyz/gtmssssxei.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.daria6918.cn/gthaqlnmzl.html

[F11] 复制与移动文件
来源：http://hz.xziqi.cn/gtqwwqfvcg.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.zycfv.cn/gtcvdsvmtd.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.nwbrower.top/gtnstxpyob.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jinghuilouyu.cn/gtdbuggich.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.sufxvd.cn/gtwjjxnpxm.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.shanyushiyangtech.top/gtsmkmvgog.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.dianchejie.cn/gtvydfhwpq.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.pengpengdd.cyou/gtwguxllco.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.yueranfly.top/gtxbxhspau.html

[F12] CSV 读写
来源：http://hz.sweek.top/gtkwmyseop.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.pengpengdd.cyou/gtaixnczis.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.havefunace.top/gtgtfwhzqg.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.yonumen.top/gtofmweyts.html

TS:   // 同上
来源：http://hz.yuanzhike.top/gtpoifnoih.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.ydzc1.top/gtticyapne.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.hnqzz.top/gtkosgktgo.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.cucudq.cn/gtlpgwvcjy.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.pengpengdd.cyou/gtnafpssyt.html

================================================================================
来源：http://hz.daria6918.cn/gtozgiovxt.html

G. 面向对象
来源：http://hz.svipenyu.cn/gttydyinhi.html

================================================================================
来源：http://hz.jqgufenzy.top/gtzjxvbyss.html

[G01] 定义类
来源：http://hz.tanke756.top/gtltunjvpm.html

Py:   class User: pass
来源：http://hz.redwolf501.top/gtehawffsn.html

PHP:  class User {}
来源：http://hz.zhaomingkeji.xyz/gtsbztlgcg.html

JS:   class User {}
来源：http://hz.dianchejie.cn/gtdfyhwood.html

TS:   class User { name: string = ""; }
来源：http://hz.shuidangran.top/gtxeymbkmh.html

Java: class User {}
来源：http://hz.yonumen.top/gtsudktdim.html

Go:   type User struct { Name string }
来源：http://hz.yonumen.top/gtvcyzbtck.html

Ruby: class User; end
来源：http://hz.xylfe.cn/gtuuxjjdzi.html

C#:   class User {}
来源：http://hz.shanyushiyangtech.top/gtuenvgcac.html

[G02] 构造函数
来源：http://hz.yj20258888.top/gtfjspkedi.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.svipenyu.cn/gtqzeelszd.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.tian-w.cn/gtnahixkzh.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.sxryk.cn/gtzkxameyh.html

TS:   constructor(public name: string) {}
来源：http://hz.gzhubu.top/gtiubsjqrw.html

Java: User(String name) { this.name = name; }
来源：http://hz.yj202588.top/gtiaqgjabu.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.redwolf501.top/gtxjiaujdv.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.sysykeji.top/gtwpebdjyc.html

C#:   public User(string name) { Name = name; }
来源：http://hz.havefunace.top/gthrqtrojg.html

[G03] 实例属性
来源：http://hz.fengsongda.top/gtrdhqyvdf.html

Py:   self.name = "x"
来源：http://hz.havefunace.top/gtnvkboqik.html

PHP:  public string $name = "x";
来源：http://hz.tian-w.cn/gtxmbbgcnd.html

JS:   this.name = "x";
来源：http://hz.c1oappe.top/gtgotjkklt.html

TS:   name: string = "x";
来源：http://hz.andypj.xyz/gtlgqfspeg.html

Java: private String name;
来源：http://hz.chenjidiqi.icu/gttjxzejgw.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.daria6918.cn/gtbkqoedfe.html

Ruby: @name = "x"
来源：http://hz.quarkkingdee.top/gtjrcryidl.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.xuanzx.com/gtlmrbkhcq.html

[G04] 定义方法
来源：http://hz.chenjidiqi.icu/gtnqahaeah.html

Py:   def greet(self): return self.name
来源：http://hz.chenlongwang.top/gtdwefpkee.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.svipenyu.cn/gtwbswjwti.html

JS:   greet() { return this.name; }
来源：http://hz.316326.xyz/gttwzqnagu.html

TS:   greet(): string { return this.name; }
来源：http://hz.hfpthk.cn/gtefrmiota.html

Java: String greet() { return name; }
来源：http://hz.hongshengwenyu.top/gtmtiihyng.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.jiagoushi.top/gtgipejcyy.html

Ruby: def greet; @name; end
来源：http://hz.yueranfly.top/gtygxxvfei.html

C#:   public string Greet() => Name;
来源：http://hz.cashguo.top/gtjtududnq.html

[G05] 继承
来源：http://hz.hammf.cn/gtqludehqd.html

Py:   class Admin(User): pass
来源：http://hz.zhiwuduotai.top/gtzycfsrhm.html

PHP:  class Admin extends User {}
来源：http://hz.cqqwz.cn/gtpnuyjgvr.html

JS:   class Admin extends User {}
来源：http://hz.chenzaomai.com/gtawyxumxl.html

TS:   class Admin extends User {}
来源：http://hz.chenjidiqi.icu/gtrglbtefc.html

Java: class Admin extends User {}
来源：http://hz.birdmap.top/gtwnnxhcqe.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.shangyingyoupin.top/gtqsqhiagb.html

Ruby: class Admin < User; end
来源：http://hz.xuanzx.com/gtulmfchmw.html

C#:   class Admin : User {}
来源：http://hz.shanyushiyangkeji.top/gtrkyrbrmj.html

[G06] 重写方法
来源：http://hz.shangyingyoupin.top/gtgexnropg.html

Py:   def greet(self): return "admin"
来源：http://hz.xuanzx.com/gtampkfauo.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.xziqi.cn/gtxkraxcnn.html

JS:   greet() { return "admin"; }
来源：http://hz.dianchejie.cn/gtvifsssdh.html

TS:   greet(): string { return "admin"; }
来源：http://hz.jinqigufen.top/gtyzqgizfz.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.cashguo.top/gtjvrucqqd.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.c1oappe.top/gtrzilqhwy.html

Ruby: def greet; "admin"; end
来源：http://hz.shanyushiyangtech.top/gttewpfcpk.html

C#:   public override string Greet() => "admin";
来源：http://hz.sweek.top/gtynabppng.html

[G07] 调用父类方法
来源：http://hz.gogol.net.cn/gtxmkeiavg.html

Py:   super().greet()
来源：http://hz.xziqi.cn/gtpfumsicp.html

PHP:  parent::greet();
来源：http://hz.yangfankeji.com/gtkrlddfra.html

JS:   super.greet();
来源：http://hz.0kj1m.cn/gtjfzrwdyu.html

TS:   super.greet();
来源：http://hz.52xcode.cn/gtluyanbad.html

Java: super.greet();
来源：http://hz.xinyue.icu/gttbowphph.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.nanxinkj.top/gtlqekadol.html

Ruby: super
来源：http://hz.sweek.top/gtzvadrfgf.html

C#:   base.Greet();
来源：http://hz.kuanghao11.cn/gtlladcrqq.html

[G08] 静态方法与属性
来源：http://hz.ybcxt.top/gttbxzakxc.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.shanyushiyangkeji.top/gtcmayaulw.html

PHP:  public static function f() {}
来源：http://hz.svipenyu.cn/gtvdhnnjnj.html

JS:   static f() {}
来源：http://hz.haohaochexian.top/gtkxdtnonm.html

TS:   static f(): void {}
来源：http://hz.wangdashe.top/gtuuralutl.html

Java: static void f() {}
来源：http://hz.wangshuangyany.cn/gtlwbqkukb.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.snrcjt.cn/gtpshoylko.html

Ruby: def self.f; end
来源：http://hz.guowangkeji.top/gtopcqkhla.html

C#:   public static void F() {}
来源：http://hz.ydzc1.top/gtzdsvdtet.html

[G09] 接口 / 抽象类
来源：http://hz.fengsongda.top/gtzotdlbnv.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.jqgfzy.top/gtpmxuuuvh.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.jyoumei.cn/gtyxcszkmw.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.guowangkeji.top/gtbhwtqmeg.html

TS:   interface Shape { area(): number; }
来源：http://hz.guannengcc.top/gtcxbydnqj.html

Java: interface Shape { double area(); }
来源：http://hz.fzhhl.top/gtjpshozzs.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.yuxming.cn/gtablxkgup.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.yongpay.top/gtyyratgyu.html

C#:   interface IShape { double Area(); }
来源：http://hz.yj202588.top/gtzhiywaao.html

[G10] 访问控制
来源：http://hz.yanxiufei.cn/gtstialoxn.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.nanxuanxn.top/gtkqyzbjuf.html

PHP:  public / protected / private
来源：http://hz.fzhhl.top/gtktjxrvmp.html

JS:   #private 字段；其余公开
来源：http://hz.daria6918.cn/gtlvlnmbpy.html

TS:   public / protected / private
来源：http://hz.cqqwz.cn/gtlwdxyxdw.html

Java: public / protected / private / 默认包级
来源：http://hz.shuidangran.top/gtzfvwzrpc.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.ehwqpu.com/gtycwqhntf.html

Ruby: public / protected / private
来源：http://hz.dashuyun.cn/gtwkqmpqku.html

C#:   public / protected / private / internal
来源：http://hz.zhijiandao.cn/gtrrldpuqj.html

[G11] getter / setter
来源：http://hz.redwolf501.top/gtnmdzowvd.html

Py:   @property 与 @x.setter
来源：http://hz.haohaochexian.top/gtsaerrarg.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.cashguo.top/gthluoowdw.html

JS:   get name() { return this._name; }
来源：http://hz.nanxinkj.top/gtjkpepguh.html

TS:   get name(): string { return this._name; }
来源：http://hz.zdqjudy.top/gtrzcvhwzm.html

Java: public String getName() { return name; }
来源：http://hz.wangdashe.top/gtkhjhzhcs.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.yj202588.top/gttstclefw.html

Ruby: attr_accessor :name
来源：http://hz.cheryme.top/gtcdmwnucr.html

C#:   public string Name { get; set; }
来源：http://hz.zhiwuduotai.top/gtdhtydggd.html

[G12] 对象转字符串
来源：http://hz.yonumen.top/gtdefaznpn.html

Py:   def __str__(self): return self.name
来源：http://hz.xingfuxueyuan.xyz/gtwjoiumdv.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.jyoumei.cn/gtgycaycmc.html

JS:   toString() { return this.name; }
来源：http://hz.yj20258888.top/gtalltumpz.html

TS:   toString(): string { return this.name; }
来源：http://hz.ehwqpu.com/gtzfypgdzb.html

Java: @Override public String toString() { return name; }
来源：http://hz.svipenyu.cn/gtuslppqbl.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.shanyushiyangtech.top/gtfutybyhd.html

Ruby: def to_s; @name; end
来源：http://hz.gotoacloud.top/gtjslxgiof.html

C#:   public override string ToString() => Name;
来源：http://hz.nwbrower.top/gtxwcmpixm.html

[G13] 判断对象类型
来源：http://hz.kuanghao11.cn/gtjnydyzfd.html

Py:   isinstance(u, User)
来源：http://hz.9152youxi.cn/gtbgxsdugu.html

PHP:  $u instanceof User
来源：http://hz.fzhhl.top/gtgoaqudtz.html

JS:   u instanceof User
来源：http://hz.yuxming.cn/gtvvnsfiye.html

TS:   u instanceof User
来源：http://hz.meibo888.top/gtxzpqzmbp.html

Java: u instanceof User
来源：http://hz.daxiang520.top/gtrhmtzvfi.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.dianchejie.cn/gtvyfsseky.html

Ruby: u.is_a?(User)
来源：http://hz.zhoulong.xyz/gtigyfbuwr.html

C#:   u is User
来源：http://hz.chenlongwang.top/gtsvcdmagr.html

[G14] 数据类 / record
来源：http://hz.yonumen.top/gtxfmbdqwn.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.jinqigfzy.top/gtsijklmvc.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.mhx1999.top/gtgdcdkspa.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.316326.xyz/gtjgahimjw.html

TS:   type User = { name: string; age: number };
来源：http://hz.birdmap.top/gtqmcdbwjm.html

Java: record User(String name, int age) {}
来源：http://hz.hongshengwenyu.top/gtjczuwtpf.html

Go:   type User struct { Name string; Age int }
来源：http://hz.zhaomingkeji.xyz/gtklrmjhnt.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.yj20258.top/gtzjniobvs.html

C#:   record User(string Name, int Age);
来源：http://hz.svipenyu.cn/gtmhtpgzae.html

[G15] 枚举
来源：http://hz.bjfxy.top/gtqdgmhdzi.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.xuanzx.com/gtdbfsaxam.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.iojbl.cn/gtzfdeswxn.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.yj202588.top/gtsvzutbcb.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.hongshengwenyu.top/gtgvvwuntq.html

Java: enum Color { RED, GREEN }
来源：http://hz.zhijiandao.cn/gtrgothfdj.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.wangdashe.top/gtncirosvh.html

Ruby: Color = %i[red green].freeze
来源：http://hz.jinqigfzy.top/gtgvnchewf.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.ydzc1.top/gtjbrkaaxo.html

[G16] 对象转数组 / 字典
来源：http://hz.cqqwz.cn/gtsipliwwu.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.haohaochexian.top/gtfqoozibv.html

PHP:  get_object_vars($obj);
来源：http://hz.sysykeji.top/gtajwtupma.html

JS:   Object.entries(obj)
来源：http://hz.yj20258.top/gttxksqiyv.html

TS:   Object.entries(obj)
来源：http://hz.52xcode.cn/gtfhrugmup.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.xziqi.cn/gtbyvakmzf.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.havefunace.top/gteouaaeth.html

Ruby: obj.instance_variables
来源：http://hz.svipenyu.cn/gtuydrdzxa.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.yongpay.top/gtbrjrfnqv.html

================================================================================
来源：http://hz.svipenyu.cn/gthovbspaw.html


<!-- 参考信息 -->