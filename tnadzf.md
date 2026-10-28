代发 wailian999

JS:   s.split(/\r?\n/)
来源：http://hz.shzxlz.cn/gtlvxjqexf.html

TS:   s.split(/\r?\n/)
来源：http://hz.hywenlv.cn/gttqnrwrkq.html

Java: s.lines().toList()
来源：http://hz.0kj1m.cn/gtizbteauq.html

Go:   strings.Split(s, "\n")
来源：http://hz.hfpthk.cn/gtwqzbfmin.html

Ruby: s.lines
来源：http://hz.yj20258888.top/gtllcwkbyl.html

C#:   s.Split('\n')
来源：http://hz.tanke756.top/gtryfmqnnr.html

[E20] 判断字符串是否为空
来源：http://hz.snrcjt.cn/gthkkddqqf.html

Py:   if not s:
来源：http://hz.wangdashe.top/gtdjacavjg.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.iojbl.cn/gtvafrwlng.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.gogol.net.cn/gtjpxhepqu.html

TS:   if (s === "") {}
来源：http://hz.sweek.top/gthuehllpx.html

Java: if (s.isEmpty()) {}
来源：http://hz.zhongyouzk.top/gtootyuksb.html

Go:   if s == "" {}
来源：http://hz.316326.xyz/gtuivuqhyz.html

Ruby: if s.empty?
来源：http://hz.zdqjudy.top/gtvltiwpsr.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.shanyushiyangkeji.top/gtchrtknwn.html

[E21] 超长截断加省略号
来源：http://hz.zhiwuduotai.top/gtisnptzfm.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.mhx1999.top/gtaqkjjtem.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.sysykeji.top/gtvmpvknft.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.wangshuangyany.cn/gtrepzcoxl.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jqgfzy.top/gtceihxqlq.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.ivvv.top/gtieroqccg.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.zhijiandao.cn/gtpnvwisud.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.daria6918.cn/gtebosqzcx.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.zhaomingkeji.xyz/gtztoygafa.html

[E22] 字节长度与字符长度
来源：http://hz.jiagoushi.top/gtpyywuljk.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.gaohongyu789.top/gtimkmngye.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jianghu66.top/gtxxkqxvjo.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.smart0.xyz/gtpwirhmsk.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.iojbl.cn/gtecfpujyp.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.guannengcc.top/gtntewdclp.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.yangfankeji.com/gteqetwgub.html

Ruby: s.bytesize;  s.length
来源：http://hz.nanxuanxn.top/gtjabuowkf.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.quarkkingdee.top/gtrastcjal.html

================================================================================
来源：http://hz.tian-w.cn/gteosuaegq.html

F. 文件与目录
来源：http://hz.sufxvd.cn/gtyjiuykhz.html

================================================================================
来源：http://hz.nanxuanxn.top/gtsmileasc.html

[F01] 读取整个文件
来源：http://hz.zhixingplan.top/gtfbjatsqc.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.yonumen.top/gtjupgzknu.html

PHP:  file_get_contents("a.txt");
来源：http://hz.hnxiangtu.top/gtevsiviwu.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.quarkkingdee.top/gtpsuawikx.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.hnxiangtu.top/gtpflkydne.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.zhoulong.xyz/gtfebflnel.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.fzhhl.top/gtxxsiwzgo.html

Ruby: File.read("a.txt")
来源：http://hz.dashuyun.cn/gttwqfpfnd.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.cashguo.top/gtafvdmifa.html

[F02] 逐行读取文件
来源：http://hz.tanke756.top/gtufhtowwt.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.yangfankeji.com/gtrkrndnjy.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.nanxinkj.top/gtxkemstui.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.ybcxt.top/gtzevidfio.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yvedp.cn/gtlnwsetrl.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.yongpay.top/gtgpmauzyw.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.316326.xyz/gtyhjvrnad.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.pycfn.com/gtulkzytdt.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.ydjk.org.cn/gtedrhblze.html

[F03] 写入文件（覆盖）
来源：http://hz.gogol.net.cn/gtbqhtmmwf.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.yuanzhike.top/gtweuffzzn.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.jinyuanbaomall.cn/gtvzeshfxq.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.c1oappe.top/gtjoethkrh.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.chenjidiqi.icu/gtzttgvhfl.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.sufxvd.cn/gtfskmsfdc.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.shanyushiyangkeji.top/gtialgsbsh.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.c1oappe.top/gtjkwedlsn.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.cqqwz.cn/gteypszlig.html

[F04] 追加写入文件
来源：http://hz.zhijiandao.cn/gtkmkacdpe.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.hammf.cn/gthsadqbyx.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.chenzaomai.com/gtjyigmebm.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.0kj1m.cn/gtyooohqhi.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.birdmap.top/gtxeuyvonx.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.ydzc1.top/gtzbytxgdz.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.nanxuanxn.top/gtwgrvcviu.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.yuxming.cn/gtyfkrmwkz.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.guannengcc.top/gtzcmuffna.html

[F05] 判断文件或目录是否存在
来源：http://hz.tian-w.cn/gtguxjyhbu.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.shanyushiyangtech.top/gtjpeaqxeq.html

PHP:  file_exists("a.txt");
来源：http://hz.zhoulong.xyz/gtqmnrwlno.html

JS:   fs.existsSync("a.txt")
来源：http://hz.mhx1999.top/gtjvccmfvj.html

TS:   fs.existsSync("a.txt")
来源：http://hz.ydzc1.top/gtijynqzuq.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.jqgufenzy.top/gtwoqezrxw.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.cashguo.top/gtctqhiuqo.html

Ruby: File.exist?("a.txt")
来源：http://hz.zhiwuduotai.top/gtiatcujuq.html

C#:   File.Exists("a.txt")
来源：http://hz.yvedp.cn/gtkvgybqgp.html

[F06] 删除文件
来源：http://hz.hywenlv.cn/gtfftqomys.html

Py:   os.remove("a.txt")
来源：http://hz.smart0.xyz/gtaomdrtgp.html

PHP:  unlink("a.txt");
来源：http://hz.fzhhl.top/gtxbxnxajo.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.52xcode.cn/gtbymuxnbq.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.bjfxy.top/gtmajqhyrj.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.tian-w.cn/gtlqtiwdvf.html

Go:   os.Remove("a.txt")
来源：http://hz.haohaochexian.top/gtjqkzjzue.html

Ruby: File.delete("a.txt")
来源：http://hz.yonumen.top/gtjysyzmnn.html

C#:   File.Delete("a.txt");
来源：http://hz.jqgfzy.top/gtxrpocbzu.html

[F07] 创建目录（含多级）
来源：http://hz.smart0.xyz/gtwyvvsaoz.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.daria6918.cn/gtizmuaivz.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.guowangkeji.top/gtzliihwwd.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.wangshuangyany.cn/gtvtzjlgll.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.svipenyu.cn/gtdewgsxcc.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.sweek.top/gtuvekljcv.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.shuidangran.top/gtnxoivfqy.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.cucudq.cn/gtzclvgvjm.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.zhengqikj.top/gthqosdvnt.html

[F08] 遍历目录
来源：http://hz.zycfv.cn/gtbbantczu.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.iojbl.cn/gtdgegzinm.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.meibo888.top/gtxzasmymw.html

JS:   fs.readdirSync("dir")
来源：http://hz.meibo888.top/gtnurronhu.html

TS:   fs.readdirSync("dir")
来源：http://hz.yuanzhike.top/gtarpwumyl.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.vqdsnc.cn/gtxrizipst.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.andypj.xyz/gthzlyjrmk.html

Ruby: Dir.children("dir")
来源：http://hz.chenjidiqi.icu/gtwfotrcbu.html

C#:   Directory.GetFiles("dir")
来源：http://hz.jinghuilouyu.cn/gtlstahnaw.html

[F09] 获取文件大小
来源：http://hz.zhiwuduotai.top/gtdgukthog.html

Py:   os.path.getsize("a.txt")
来源：http://hz.yuxming.cn/gtgkpqcszu.html

PHP:  filesize("a.txt");
来源：http://hz.shanyushiyangtech.top/gtbpzhqeij.html

JS:   fs.statSync("a.txt").size
来源：http://hz.jqgufenzy.top/gtqdndhqvu.html

TS:   fs.statSync("a.txt").size
来源：http://hz.jinghuilouyu.cn/gtdhflfllg.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.cashguo.top/gtpjytmzvu.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.shangyingyoupin.top/gtiknykydh.html

Ruby: File.size("a.txt")
来源：http://hz.daxiang520.top/gtutoqbbpa.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.pycfn.com/gtaoyugrsm.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.aizwys.cn/gtifdgnwql.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.xingfuxueyuan.xyz/gtzlvjhmqu.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.zhengqikj.top/gtbymicadh.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.yangfankeji.com/gtzpevkxhf.html

TS:   path.extname("a.txt")
来源：http://hz.aizwys.cn/gtqljfrmmd.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.ydjk.org.cn/gtskpzjhcm.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.tianlin.xyz/gtoanqphun.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.wangdashe.top/gtggfiaynv.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.yanxiufei.cn/gthpnupqfe.html

[F11] 复制与移动文件
来源：http://hz.hammf.cn/gtghmiixge.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.shzxlz.cn/gtfrtxvlor.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.xuetiantiany.cn/gtjcljfkfa.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.xingfuxueyuan.xyz/gtzngdwysl.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.xingfuxueyuan.xyz/gtrkrqfsqf.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.svipenyu.cn/gtjtthadbd.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.aibaodan.cn/gtpzddxxse.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.shzxlz.cn/gtabwkgiul.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.316326.xyz/gtqrbtiryw.html

[F12] CSV 读写
来源：http://hz.jinqigfzy.top/gtgvnjwypt.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.ehwqpu.com/gtzlnqmqmo.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.kuanghao11.cn/gtotjnrtsm.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.tian-w.cn/gtchrrrtec.html

TS:   // 同上
来源：http://hz.xuetiantiany.cn/gtishuujyd.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.xinyue.icu/gtapgulggr.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.iojbl.cn/gthfnfsdqp.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.zhixingplan.top/gtraodadhr.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.chenlongwang.top/gtnynlkqzd.html

================================================================================
来源：http://hz.meibo888.top/gterzooaxk.html

G. 面向对象
来源：http://hz.yongpay.top/gtwtasdxtj.html

================================================================================
来源：http://hz.c1oappe.top/gtscsztsal.html

[G01] 定义类
来源：http://hz.sysykeji.top/gtmxhorwff.html

Py:   class User: pass
来源：http://hz.9152youxi.cn/gtaxjrwfup.html

PHP:  class User {}
来源：http://hz.ppjwa.cn/gtcmrfiwmx.html

JS:   class User {}
来源：http://hz.fengsongda.top/gtepkrtlzm.html

TS:   class User { name: string = ""; }
来源：http://hz.jinghuilouyu.cn/gturkjuurm.html

Java: class User {}
来源：http://hz.havefunace.top/gtgltshnge.html

Go:   type User struct { Name string }
来源：http://hz.nanxuanxn.top/gtpdakvcgt.html

Ruby: class User; end
来源：http://hz.sxryk.cn/gtchziontm.html

C#:   class User {}
来源：http://hz.0kj1m.cn/gtxlxsizox.html

[G02] 构造函数
来源：http://hz.ydzc1.top/gtqqnajbsb.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.zhongyouzk.top/gtcoijxdhi.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.daria6918.cn/gtujfhtrfv.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.kuanghao11.cn/gtsxdqqnnl.html

TS:   constructor(public name: string) {}
来源：http://hz.yueranfly.top/gtzyjtnpxd.html

Java: User(String name) { this.name = name; }
来源：http://hz.andypj.xyz/gtiwcgaquf.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.fengsongda.top/gtwctvcwpx.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.ydzc1.top/gttgvasspo.html

C#:   public User(string name) { Name = name; }
来源：http://hz.smart0.xyz/gtfecttevg.html

[G03] 实例属性
来源：http://hz.tianlin.xyz/gtuyijegzk.html

Py:   self.name = "x"
来源：http://hz.zhiwuduotai.top/gtvjslqvoe.html

PHP:  public string $name = "x";
来源：http://hz.xylfe.cn/gtbuwssxvw.html

JS:   this.name = "x";
来源：http://hz.shzxlz.cn/gtmjnogcqr.html

TS:   name: string = "x";
来源：http://hz.yj20258.top/gtjpdpqrlh.html

Java: private String name;
来源：http://hz.zhijiandao.cn/gtdfhnmdst.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.hammf.cn/gtstxihuoy.html

Ruby: @name = "x"
来源：http://hz.nanxuanxn.top/gtxkbtzijr.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.mhx1999.top/gtrnoxaehj.html

[G04] 定义方法
来源：http://hz.birdmap.top/gtyqqamkqr.html

Py:   def greet(self): return self.name
来源：http://hz.cucudq.cn/gtphydizae.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.jinqigufen.top/gtawzetsbq.html

JS:   greet() { return this.name; }
来源：http://hz.yj20258888.top/gtnxgpqhxz.html

TS:   greet(): string { return this.name; }
来源：http://hz.mhx1999.top/gtyydjporb.html

Java: String greet() { return name; }
来源：http://hz.redwolf501.top/gtmbqjoeqk.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.yvedp.cn/gtbmquihzj.html

Ruby: def greet; @name; end
来源：http://hz.aibaodan.cn/gtilxwmesy.html

C#:   public string Greet() => Name;
来源：http://hz.wangshuangyany.cn/gtooayknrw.html

[G05] 继承
来源：http://hz.ivvv.top/gtblhcjjyy.html

Py:   class Admin(User): pass
来源：http://hz.9152youxi.cn/gtrkpobvxr.html

PHP:  class Admin extends User {}
来源：http://hz.yonumen.top/gtulpyvwmn.html

JS:   class Admin extends User {}
来源：http://hz.aizwys.cn/gtupddfdrv.html

TS:   class Admin extends User {}
来源：http://hz.yj20258888.top/gtdwjgiqgx.html

Java: class Admin extends User {}
来源：http://hz.zycfv.cn/gtajpixful.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.yanxiufei.cn/gtwngfgpks.html

Ruby: class Admin < User; end
来源：http://hz.kuanghao11.cn/gtqqxxnhsz.html

C#:   class Admin : User {}
来源：http://hz.ppjwa.cn/gtvayvhgxm.html

[G06] 重写方法
来源：http://hz.smart0.xyz/gtwtaeqfju.html

Py:   def greet(self): return "admin"
来源：http://hz.gzhubu.top/gtwhttnzly.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.jinyuanbaomall.cn/gtbxbwvkvy.html

JS:   greet() { return "admin"; }
来源：http://hz.nanxinkj.top/gtoezbtgzg.html

TS:   greet(): string { return "admin"; }
来源：http://hz.dashuyun.cn/gtkrnujwce.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.smart0.xyz/gtuhyilckz.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.zhengqikj.top/gtlrijolkb.html

Ruby: def greet; "admin"; end
来源：http://hz.jinghuilouyu.cn/gtxtelauky.html

C#:   public override string Greet() => "admin";
来源：http://hz.zhaomingkeji.xyz/gttmgwuvys.html

[G07] 调用父类方法
来源：http://hz.gogol.net.cn/gtzsjieyqv.html

Py:   super().greet()
来源：http://hz.daxiang520.top/gtnrqlutiz.html

PHP:  parent::greet();
来源：http://hz.chenlongwang.top/gtmmerqows.html

JS:   super.greet();
来源：http://hz.yuanzhike.top/gtakhrytpn.html

TS:   super.greet();
来源：http://hz.yuanzhike.top/gttqwicwbo.html

Java: super.greet();
来源：http://hz.jyoumei.cn/gtndwwrtcz.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.sxryk.cn/gtdbqwufue.html

Ruby: super
来源：http://hz.meibo888.top/gtijcdvoxm.html

C#:   base.Greet();
来源：http://hz.gzhubu.top/gtczqwtirh.html

[G08] 静态方法与属性
来源：http://hz.cqqwz.cn/gtsfdrxoaz.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.gaohongyu789.top/gtnghkudwm.html

PHP:  public static function f() {}
来源：http://hz.daxiang520.top/gtjvmpycyk.html

JS:   static f() {}
来源：http://hz.tianlin.xyz/gtwleqzfay.html

TS:   static f(): void {}
来源：http://hz.cqqwz.cn/gtdnmkbzuy.html

Java: static void f() {}
来源：http://hz.c1oappe.top/gtollcurpx.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.jqgfzy.top/gtermkisxv.html

Ruby: def self.f; end
来源：http://hz.daria6918.cn/gtajvhpmnf.html

C#:   public static void F() {}
来源：http://hz.yangfankeji.com/gtcnbwcnvc.html

[G09] 接口 / 抽象类
来源：http://hz.vqdsnc.cn/gtdkwitfex.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.zhixingplan.top/gtvofjmzzs.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.ivvv.top/gtfgkriuhs.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.feifeiyinyue.top/gtwjugixne.html

TS:   interface Shape { area(): number; }
来源：http://hz.yangfankeji.com/gtedavcmdz.html

Java: interface Shape { double area(); }
来源：http://hz.xingfuxueyuan.xyz/gtdqlqerxe.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.mhx1999.top/gtngtpufzq.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.sweek.top/gtxzqwiqjf.html

C#:   interface IShape { double Area(); }
来源：http://hz.tanke756.top/gtgwixrwrq.html

[G10] 访问控制
来源：http://hz.ppjwa.cn/gtrqfakltw.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.zhixingplan.top/gtgjbwtfqd.html

PHP:  public / protected / private
来源：http://hz.kuanghao11.cn/gtlxejmqlj.html

JS:   #private 字段；其余公开
来源：http://hz.cdnleiting.top/gtghnfqdop.html

TS:   public / protected / private
来源：http://hz.cheryme.top/gtdvndhfzn.html

Java: public / protected / private / 默认包级
来源：http://hz.pycfn.com/gtkovgdibp.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.cucudq.cn/gtgiqrkhtj.html

Ruby: public / protected / private
来源：http://hz.yj202588.top/gtfknuumax.html

C#:   public / protected / private / internal
来源：http://hz.hongshengwenyu.top/gtlrtkytva.html

[G11] getter / setter
来源：http://hz.jinyuanbaomall.cn/gtxidhydlz.html

Py:   @property 与 @x.setter
来源：http://hz.aizwys.cn/gtviwcanfs.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.fzhhl.top/gtjrfmidwq.html

JS:   get name() { return this._name; }
来源：http://hz.9152youxi.cn/gttqxysggk.html

TS:   get name(): string { return this._name; }
来源：http://hz.pycfn.com/gtvtnppyoj.html

Java: public String getName() { return name; }
来源：http://hz.tian-w.cn/gtksoguieq.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.ydzc1.top/gtrxgxross.html

Ruby: attr_accessor :name
来源：http://hz.ybcxt.top/gtsxaazdlx.html

C#:   public string Name { get; set; }
来源：http://hz.xuetiantiany.cn/gtieceozdz.html

[G12] 对象转字符串
来源：http://hz.ppjwa.cn/gtwajudrsc.html

Py:   def __str__(self): return self.name
来源：http://hz.xziqi.cn/gtwemlgbir.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.ybcxt.top/gtbukkixda.html

JS:   toString() { return this.name; }
来源：http://hz.0kj1m.cn/gtnnyhepwy.html

TS:   toString(): string { return this.name; }
来源：http://hz.smart0.xyz/gtrfgwnvtt.html

Java: @Override public String toString() { return name; }
来源：http://hz.shanyushiyangtech.top/gtfiboyrqh.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.mhx1999.top/gtvjfvboij.html

Ruby: def to_s; @name; end
来源：http://hz.316326.xyz/gtegsujbmi.html

C#:   public override string ToString() => Name;
来源：http://hz.guannengcc.top/gtknzivzdh.html

[G13] 判断对象类型
来源：http://hz.snrcjt.cn/gtewnvknkd.html

Py:   isinstance(u, User)
来源：http://hz.xziqi.cn/gtfcotcjvc.html

PHP:  $u instanceof User
来源：http://hz.quarkkingdee.top/gtllmzvrxw.html

JS:   u instanceof User
来源：http://hz.gogol.net.cn/gtlpmdyzkd.html

TS:   u instanceof User
来源：http://hz.ydjk.org.cn/gtqwiannov.html

Java: u instanceof User
来源：http://hz.yonumen.top/gtbpswbdji.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.316326.xyz/gtodmuklxf.html

Ruby: u.is_a?(User)
来源：http://hz.xingfuxueyuan.xyz/gtjhmvtija.html

C#:   u is User
来源：http://hz.aibaodan.cn/gtoubfzlqk.html

[G14] 数据类 / record
来源：http://hz.xylfe.cn/gtzwqfzxhs.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.kuanghao11.cn/gtupinxnox.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.shzxlz.cn/gtpadpapbp.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.meibo888.top/gtkzvbakkg.html

TS:   type User = { name: string; age: number };
来源：http://hz.zhengqikj.top/gtblbuskzv.html

Java: record User(String name, int age) {}
来源：http://hz.ydjk.org.cn/gtflxpnosy.html

Go:   type User struct { Name string; Age int }
来源：http://hz.yj20258888.top/gtyfrwchfv.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.ehwqpu.com/gtjkczrqqo.html

C#:   record User(string Name, int Age);
来源：http://hz.jqgufenzy.top/gtkcecrcwo.html

[G15] 枚举
来源：http://hz.dashuyun.cn/gtnqlvztdd.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.nwbrower.top/gtmaibtwix.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.jlsjyb.cn/gttpgsucof.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.cucudq.cn/gtifemgbbq.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.xingfuxueyuan.xyz/gtpxdtedjl.html

Java: enum Color { RED, GREEN }
来源：http://hz.quarkkingdee.top/gtzhwpuexp.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.zhixingplan.top/gtaygtbukp.html

Ruby: Color = %i[red green].freeze
来源：http://hz.hnxiangtu.top/gtbhfodwbf.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.sweek.top/gtowoouvag.html

[G16] 对象转数组 / 字典
来源：http://hz.316326.xyz/gtdqexgspr.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.shanyushiyangkeji.top/gteldhjcgq.html

PHP:  get_object_vars($obj);
来源：http://hz.hywenlv.cn/gtneauptsw.html

JS:   Object.entries(obj)
来源：http://hz.dashuyun.cn/gtzjkbavvk.html

TS:   Object.entries(obj)
来源：http://hz.zhengqikj.top/gtpsejwktk.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.hysaishi.cn/gtzxxsjdat.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.tianlin.xyz/gtvzgsuvzi.html

Ruby: obj.instance_variables
来源：http://hz.zdqjudy.top/gtaciuhhah.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.sxryk.cn/gtmopagwia.html

================================================================================
来源：http://hz.jqgufenzy.top/gtdapbptku.html

H. 异常与错误处理
来源：http://hz.pycfn.com/gtsuabotwb.html

================================================================================
来源：http://hz.ehwqpu.com/gtovtlloow.html

[H01] try / catch 基础
来源：http://hz.jqgufenzy.top/gtwbebaelm.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.snrcjt.cn/gtbgkqewtp.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.jqgfzy.top/gtyoawtfql.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.haohaochexian.top/gtexuyzypo.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.hnqzz.top/gtytqziemi.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.daxiang520.top/gtoowvmvkh.html


<!-- 参考信息 -->