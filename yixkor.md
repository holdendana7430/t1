代发 wailian999

[E18] 模板占位符替换
来源：http://hz.0kj1m.cn/gtbzdpvepp.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.yonumen.top/gtsxbqodfd.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.haohaochexian.top/gtoaobwirn.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.feifeiyinyue.top/gthznnybmt.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.nanxuanxn.top/gtdofdefqw.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.jinqigufen.top/gtjughrgmt.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.iojbl.cn/gtffroyxgp.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.smart0.xyz/gtlftlqyfa.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.nanxinkj.top/gttkpxwbrr.html

[E19] 多行文本按行拆分
来源：http://hz.meibo888.top/gtzublzqmv.html

Py:   s.splitlines()
来源：http://hz.yongpay.top/gtujabxujs.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.shuidangran.top/gtodjmfmdf.html

JS:   s.split(/\r?\n/)
来源：http://hz.vqdsnc.cn/gtuhjuvnve.html

TS:   s.split(/\r?\n/)
来源：http://hz.zhiwuduotai.top/gtmapcorry.html

Java: s.lines().toList()
来源：http://hz.yuanzhike.top/gtkpqnyrzw.html

Go:   strings.Split(s, "\n")
来源：http://hz.cqqwz.cn/gtlzffvqij.html

Ruby: s.lines
来源：http://hz.sxryk.cn/gtasraxgnm.html

C#:   s.Split('\n')
来源：http://hz.mhx1999.top/gtzgqwlvzc.html

[E20] 判断字符串是否为空
来源：http://hz.yueranfly.top/gtuaoblfin.html

Py:   if not s:
来源：http://hz.jqgufenzy.top/gtwcsoeiel.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.52xcode.cn/gtstclgznn.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.shangyingyoupin.top/gtvrfbzfcf.html

TS:   if (s === "") {}
来源：http://hz.zhijiandao.cn/gtggivcwtg.html

Java: if (s.isEmpty()) {}
来源：http://hz.fengsongda.top/gtcljnrnvf.html

Go:   if s == "" {}
来源：http://hz.ydjk.org.cn/gtcsuwxwav.html

Ruby: if s.empty?
来源：http://hz.zhengqikj.top/gtjfazkjtd.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.kuanghao11.cn/gtpixdzvhk.html

[E21] 超长截断加省略号
来源：http://hz.xingfuxueyuan.xyz/gtofpxsdmf.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.iojbl.cn/gtopflxkcq.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.dashuyun.cn/gtarsnwgcu.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.sxryk.cn/gtwxfytbnh.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.shanyushiyangtech.top/gtehupghwe.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.quarkkingdee.top/gtuvrrzdsq.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.zycfv.cn/gtqfgvysoz.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.pengpengdd.cyou/gtoqtxemcn.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.bjfxy.top/gttozehuyy.html

[E22] 字节长度与字符长度
来源：http://hz.ywan-chungtsiang.top/gtuxowtkqb.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.hammf.cn/gtdnnodskh.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.hysaishi.cn/gtpbwfudbr.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.gaohongyu789.top/gtkcgwowie.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.xylfe.cn/gtgumheazn.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.zhoulong.xyz/gtwufjhojj.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.hnqzz.top/gtlynxgieb.html

Ruby: s.bytesize;  s.length
来源：http://hz.daria6918.cn/gtbosjcatl.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.gaohongyu789.top/gthhclfcst.html

================================================================================
来源：http://hz.jinqigfzy.top/gtjpujgxie.html

F. 文件与目录
来源：http://hz.snrcjt.cn/gtauspxblc.html

================================================================================
来源：http://hz.yangfankeji.com/gtcqvcbfna.html

[F01] 读取整个文件
来源：http://hz.xingfuxueyuan.xyz/gtvaxynnns.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.ydzc1.top/gtsfsvqtub.html

PHP:  file_get_contents("a.txt");
来源：http://hz.gotoacloud.top/gtefurqyic.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.cheryme.top/gtdyiuletl.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.yuanzhike.top/gtnyilbvuy.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.gotoacloud.top/gtyjylvpqu.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.jinghuilouyu.cn/gtnpnemokx.html

Ruby: File.read("a.txt")
来源：http://hz.yuanzhike.top/gtmpomncxv.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.chenjidiqi.icu/gtqtktsnel.html

[F02] 逐行读取文件
来源：http://hz.hfpthk.cn/gtaubwaukx.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.jinqigufen.top/gtxqjrukeh.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.xuanzx.com/gtfwnmfecr.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.ydzc1.top/gtftbcmris.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.aizwys.cn/gtuntnzjae.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.tian-w.cn/gticyepbeb.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.yangfankeji.com/gtckgegnpn.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.birdmap.top/gtxeuwykpc.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.daxiang520.top/gtmgxtvhnq.html

[F03] 写入文件（覆盖）
来源：http://hz.cucudq.cn/gtkugyjxiz.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.sysykeji.top/gteztzdxcc.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.jinyuanbaomall.cn/gtjzsnmhtl.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.cdnleiting.top/gtjmzlsjfs.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.zhoulong.xyz/gtabcuatck.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.yongpay.top/gtcrpzwtls.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.chenlongwang.top/gtmbgttztl.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.yangfankeji.com/gtjsfgxdrp.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.haohaochexian.top/gtccxicqme.html

[F04] 追加写入文件
来源：http://hz.nanxinkj.top/gtrdllvasa.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.xingfuxueyuan.xyz/gtgopfwjob.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.xuetiantiany.cn/gtwzukqomy.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.kuanghao11.cn/gtbnmexrcr.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zhixingplan.top/gtwnchfrxe.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.shanyushiyangkeji.top/gtjqczlrvg.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.wangdashe.top/gtkddjphga.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.hysaishi.cn/gtmqvahkss.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.jianghu66.top/gtrfzymzeg.html

[F05] 判断文件或目录是否存在
来源：http://hz.xuanzx.com/gtablftkcw.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.zhoulong.xyz/gtvggsckoj.html

PHP:  file_exists("a.txt");
来源：http://hz.andypj.xyz/gtoyhbekgb.html

JS:   fs.existsSync("a.txt")
来源：http://hz.sysykeji.top/gtsuhpuocg.html

TS:   fs.existsSync("a.txt")
来源：http://hz.cheryme.top/gtxmkeulnz.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.havefunace.top/gtctrevoxu.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.xingfuxueyuan.xyz/gtavzdgfwr.html

Ruby: File.exist?("a.txt")
来源：http://hz.daxiang520.top/gtgfpmzgel.html

C#:   File.Exists("a.txt")
来源：http://hz.dashuyun.cn/gtqgooxldi.html

[F06] 删除文件
来源：http://hz.mhx1999.top/gttvdpcdex.html

Py:   os.remove("a.txt")
来源：http://hz.zycfv.cn/gtzmbnavvu.html

PHP:  unlink("a.txt");
来源：http://hz.zdqjudy.top/gtufoocxkk.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.yj20258888.top/gtqsgpehnr.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.jinghuilouyu.cn/gtfoexhqyo.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.shanyushiyangtech.top/gtefvloipr.html

Go:   os.Remove("a.txt")
来源：http://hz.cqqwz.cn/gtmrbathlg.html

Ruby: File.delete("a.txt")
来源：http://hz.ehwqpu.com/gtruvvuctd.html

C#:   File.Delete("a.txt");
来源：http://hz.c1oappe.top/gtedtutuzu.html

[F07] 创建目录（含多级）
来源：http://hz.jinqigfzy.top/gtyhdurxnz.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.redwolf501.top/gtyvhflzuo.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.yj20258.top/gtztuvripn.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jinqigufen.top/gtpnnsmkjc.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.xingfuxueyuan.xyz/gtkjgducjk.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.jqgufenzy.top/gtdnsvpspn.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.hfpthk.cn/gtlqkscooo.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.aizwys.cn/gtygoukplu.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.jlsjyb.cn/gtvxzovauw.html

[F08] 遍历目录
来源：http://hz.wangshuangyany.cn/gtvgfikinp.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.shanyushiyangkeji.top/gtmaqatkif.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.9152youxi.cn/gtcuemkeue.html

JS:   fs.readdirSync("dir")
来源：http://hz.zhaomingkeji.xyz/gtxskvagzh.html

TS:   fs.readdirSync("dir")
来源：http://hz.kuanghao11.cn/gtxyprczdu.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.shanyushiyangkeji.top/gtqmginlzv.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.iojbl.cn/gtaeqngzsh.html

Ruby: Dir.children("dir")
来源：http://hz.svipenyu.cn/gterxaxixo.html

C#:   Directory.GetFiles("dir")
来源：http://hz.yangfankeji.com/gtvnlgwbwc.html

[F09] 获取文件大小
来源：http://hz.zhixingplan.top/gtzrnfdomg.html

Py:   os.path.getsize("a.txt")
来源：http://hz.yuanzhike.top/gtqjcsvczu.html

PHP:  filesize("a.txt");
来源：http://hz.guannengcc.top/gtzjhmkcdb.html

JS:   fs.statSync("a.txt").size
来源：http://hz.cucudq.cn/gtfapibjxc.html

TS:   fs.statSync("a.txt").size
来源：http://hz.yuxming.cn/gtzsaohxpv.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.ywan-chungtsiang.top/gtzihsiorh.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.zhiwuduotai.top/gtluwyybil.html

Ruby: File.size("a.txt")
来源：http://hz.yongpay.top/gtiotsyfjn.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.pengpengdd.cyou/gtdixckcqg.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.aibaodan.cn/gtxdqiqror.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.haohaochexian.top/gtnqgfrxoy.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.xinyue.icu/gtzmtgainq.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.zhijiandao.cn/gtktawxlwt.html

TS:   path.extname("a.txt")
来源：http://hz.jqgufenzy.top/gtnauzhgbl.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.quarkkingdee.top/gtdllukpvi.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.shangyingyoupin.top/gtavpqsxfs.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.ydjk.org.cn/gtibcznrzv.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.bjfxy.top/gtmejcavyv.html

[F11] 复制与移动文件
来源：http://hz.andypj.xyz/gtcxfqwzjn.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.aizwys.cn/gthghukeyw.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.cucudq.cn/gttqgwyngp.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.snrcjt.cn/gtrvfuhder.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.quarkkingdee.top/gtskhgdmta.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.andypj.xyz/gtowozdcpe.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.yanxiufei.cn/gtiigaiuaz.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.c1oappe.top/gtdhocyxgr.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.gogol.net.cn/gtdyneaxbj.html

[F12] CSV 读写
来源：http://hz.cashguo.top/gtbxsmrhkk.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.shzxlz.cn/gtsdhrqqvj.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.hammf.cn/gtjuvfbqnp.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.tian-w.cn/gtvomvgjqy.html

TS:   // 同上
来源：http://hz.shangyingyoupin.top/gtoryoefza.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.hammf.cn/gtngzvhuuy.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.jqgfzy.top/gtuexbsdfn.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.jqgfzy.top/gtcfxyyqaf.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.jinqigfzy.top/gtsoowqjao.html

================================================================================
来源：http://hz.quarkkingdee.top/gtqpwtwpmp.html

G. 面向对象
来源：http://hz.shanyushiyangtech.top/gtqfjwzjhj.html

================================================================================
来源：http://hz.52xcode.cn/gtszbdoduw.html

[G01] 定义类
来源：http://hz.ppjwa.cn/gtccslvrgn.html

Py:   class User: pass
来源：http://hz.jianghu66.top/gtrxiekydy.html

PHP:  class User {}
来源：http://hz.jianghu66.top/gtnrjbmnzs.html

JS:   class User {}
来源：http://hz.yueranfly.top/gtbwwqyjvs.html

TS:   class User { name: string = ""; }
来源：http://hz.redwolf501.top/gtigkanaak.html

Java: class User {}
来源：http://hz.ydzc1.top/gtwemykfgj.html

Go:   type User struct { Name string }
来源：http://hz.sufxvd.cn/gtmpdoxnog.html

Ruby: class User; end
来源：http://hz.shzxlz.cn/gtujuupyhu.html

C#:   class User {}
来源：http://hz.jianghu66.top/gtcnmsugvj.html

[G02] 构造函数
来源：http://hz.nanxinkj.top/gtrpijimkx.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.aizwys.cn/gtbepdpbmf.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.ybcxt.top/gtfkspehoh.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.nwbrower.top/gtzuzkulle.html

TS:   constructor(public name: string) {}
来源：http://hz.fengsongda.top/gttgokufjv.html

Java: User(String name) { this.name = name; }
来源：http://hz.daria6918.cn/gtqwwgftwx.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.zhoulong.xyz/gtduxedlwm.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.nwbrower.top/gtpftqaenn.html

C#:   public User(string name) { Name = name; }
来源：http://hz.yanxiufei.cn/gtbgfxmezj.html

[G03] 实例属性
来源：http://hz.gaohongyu789.top/gtwdzlaxnb.html

Py:   self.name = "x"
来源：http://hz.havefunace.top/gtouiowzad.html

PHP:  public string $name = "x";
来源：http://hz.jqgufenzy.top/gtxxmuzbup.html

JS:   this.name = "x";
来源：http://hz.yuxming.cn/gtrwldyjwn.html

TS:   name: string = "x";
来源：http://hz.zhiwuduotai.top/gtojlgqijd.html

Java: private String name;
来源：http://hz.dianchejie.cn/gtkwerblwv.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.zhoulong.xyz/gtgxvbwdhy.html

Ruby: @name = "x"
来源：http://hz.gogol.net.cn/gtgryycwta.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.svipenyu.cn/gtfcjfonac.html

[G04] 定义方法
来源：http://hz.snrcjt.cn/gtipixozlw.html

Py:   def greet(self): return self.name
来源：http://hz.sweek.top/gttexlykrj.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.gotoacloud.top/gtajfitkkd.html

JS:   greet() { return this.name; }
来源：http://hz.ivvv.top/gtkxhtdytc.html

TS:   greet(): string { return this.name; }
来源：http://hz.wangshuangyany.cn/gtrmzvyoyj.html

Java: String greet() { return name; }
来源：http://hz.jyoumei.cn/gtzeiayuej.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.cqqwz.cn/gtacmaoiif.html

Ruby: def greet; @name; end
来源：http://hz.zhoulong.xyz/gtvhoezuay.html

C#:   public string Greet() => Name;
来源：http://hz.shanyushiyangtech.top/gtiiwfezat.html

[G05] 继承
来源：http://hz.jinghuilouyu.cn/gtredyzspq.html

Py:   class Admin(User): pass
来源：http://hz.fzhhl.top/gtyvygstmx.html

PHP:  class Admin extends User {}
来源：http://hz.gaohongyu789.top/gtgjthxhea.html

JS:   class Admin extends User {}
来源：http://hz.kuanghao11.cn/gtituoqowy.html

TS:   class Admin extends User {}
来源：http://hz.nanxinkj.top/gteekflnfr.html

Java: class Admin extends User {}
来源：http://hz.cucudq.cn/gtqjmuucxi.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.jqgufenzy.top/gtttnaoeyo.html

Ruby: class Admin < User; end
来源：http://hz.ywan-chungtsiang.top/gtrogfodoe.html

C#:   class Admin : User {}
来源：http://hz.sufxvd.cn/gtqnsyuurx.html

[G06] 重写方法
来源：http://hz.jyoumei.cn/gtwntjzbfj.html

Py:   def greet(self): return "admin"
来源：http://hz.wangdashe.top/gtirqszeby.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.ydzc1.top/gtrooetwne.html

JS:   greet() { return "admin"; }
来源：http://hz.nanxuanxn.top/gttvzpluul.html

TS:   greet(): string { return "admin"; }
来源：http://hz.mhx1999.top/gtbasoqbye.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.xinyue.icu/gtwrmjnpaz.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.ppjwa.cn/gtqlhcorbo.html

Ruby: def greet; "admin"; end
来源：http://hz.fengsongda.top/gtvqppxwpl.html

C#:   public override string Greet() => "admin";
来源：http://hz.pengpengdd.cyou/gtstnfdndr.html

[G07] 调用父类方法
来源：http://hz.jqgufenzy.top/gtmkevqonq.html

Py:   super().greet()
来源：http://hz.shzxlz.cn/gtcamorymk.html

PHP:  parent::greet();
来源：http://hz.ybcxt.top/gtdrbngltt.html

JS:   super.greet();
来源：http://hz.yanxiufei.cn/gtlgxfuqpt.html

TS:   super.greet();
来源：http://hz.fzhhl.top/gtjklloazk.html

Java: super.greet();
来源：http://hz.chenlongwang.top/gtpjqchneb.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.yongpay.top/gtksgypclg.html

Ruby: super
来源：http://hz.shzxlz.cn/gtrkxlkazx.html

C#:   base.Greet();
来源：http://hz.xziqi.cn/gtjsycaeay.html

[G08] 静态方法与属性
来源：http://hz.zhiwuduotai.top/gtspdkpjdt.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.daxiang520.top/gtnwjccjfn.html

PHP:  public static function f() {}
来源：http://hz.ppjwa.cn/gteobrrimd.html

JS:   static f() {}
来源：http://hz.jinyuanbaomall.cn/gtfmdceskv.html

TS:   static f(): void {}
来源：http://hz.ehwqpu.com/gtpbpurfuo.html

Java: static void f() {}
来源：http://hz.zycfv.cn/gtxnppyrpr.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.jianghu66.top/gtoddpeakv.html

Ruby: def self.f; end
来源：http://hz.pengpengdd.cyou/gtluaaecet.html

C#:   public static void F() {}
来源：http://hz.hywenlv.cn/gtteislzas.html

[G09] 接口 / 抽象类
来源：http://hz.hysaishi.cn/gtdenvjsyz.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.nanxinkj.top/gtaxulneyy.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.yangfankeji.com/gtymedlvdb.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.yueranfly.top/gtylywtiyk.html

TS:   interface Shape { area(): number; }
来源：http://hz.chenjidiqi.icu/gtswironid.html

Java: interface Shape { double area(); }
来源：http://hz.jinyuanbaomall.cn/gtviishohk.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.wangdashe.top/gtywgshjes.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.yangfankeji.com/gtlfzjjosi.html

C#:   interface IShape { double Area(); }
来源：http://hz.redwolf501.top/gtjxoaixxm.html

[G10] 访问控制
来源：http://hz.quarkkingdee.top/gtwtrglnrh.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.shanyushiyangtech.top/gtvfeeqdeg.html

PHP:  public / protected / private
来源：http://hz.zhijiandao.cn/gtvdskricd.html

JS:   #private 字段；其余公开
来源：http://hz.yj20258.top/gtjzoesbgh.html

TS:   public / protected / private
来源：http://hz.aizwys.cn/gtdnlwcqpk.html

Java: public / protected / private / 默认包级
来源：http://hz.hfpthk.cn/gtjgarjaol.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.shangyingyoupin.top/gtatteetaa.html

Ruby: public / protected / private
来源：http://hz.iojbl.cn/gtjbxbtelt.html

C#:   public / protected / private / internal
来源：http://hz.nanxinkj.top/gttmpslmrq.html

[G11] getter / setter
来源：http://hz.tian-w.cn/gtzdneqxgo.html

Py:   @property 与 @x.setter
来源：http://hz.kuanghao11.cn/gtmgpgyecz.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.yj20258.top/gtffkoifda.html

JS:   get name() { return this._name; }
来源：http://hz.sweek.top/gtdvucbtxa.html

TS:   get name(): string { return this._name; }
来源：http://hz.sweek.top/gtsxixvkex.html

Java: public String getName() { return name; }
来源：http://hz.jinyuanbaomall.cn/gtinljvlmh.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.jyoumei.cn/gtuazqjxtv.html

Ruby: attr_accessor :name
来源：http://hz.ivvv.top/gtkfwwljeb.html

C#:   public string Name { get; set; }
来源：http://hz.zhengqikj.top/gtbnaflqdw.html

[G12] 对象转字符串
来源：http://hz.yvedp.cn/gtddjktvtl.html

Py:   def __str__(self): return self.name
来源：http://hz.tian-w.cn/gtnlrnwawj.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.mhx1999.top/gtlfetfhgl.html

JS:   toString() { return this.name; }
来源：http://hz.chenjidiqi.icu/gtqupepncc.html

TS:   toString(): string { return this.name; }
来源：http://hz.gogol.net.cn/gtubkqvcih.html

Java: @Override public String toString() { return name; }
来源：http://hz.gogol.net.cn/gtumcbxnmm.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.aizwys.cn/gtdjgiavhp.html

Ruby: def to_s; @name; end
来源：http://hz.havefunace.top/gtljiwdbtc.html

C#:   public override string ToString() => Name;
来源：http://hz.ybcxt.top/gtggxfajyz.html

[G13] 判断对象类型
来源：http://hz.jlsjyb.cn/gtppzzbiqd.html

Py:   isinstance(u, User)
来源：http://hz.ywan-chungtsiang.top/gtqqjjkvnf.html

PHP:  $u instanceof User
来源：http://hz.nwbrower.top/gtxwxfhnyi.html

JS:   u instanceof User
来源：http://hz.gzhubu.top/gtdsfvflyl.html

TS:   u instanceof User
来源：http://hz.guannengcc.top/gtcbaummla.html

Java: u instanceof User
来源：http://hz.chenzaomai.com/gttawhfnad.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.ybcxt.top/gtiowczxtq.html

Ruby: u.is_a?(User)
来源：http://hz.jqgufenzy.top/gtijhuhvfu.html

C#:   u is User
来源：http://hz.andypj.xyz/gtpyeyixyv.html

[G14] 数据类 / record
来源：http://hz.nanxuanxn.top/gtbpdqqkmq.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.svipenyu.cn/gtgzptzuxg.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.ywan-chungtsiang.top/gtcwcqctqk.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.snrcjt.cn/gtubttqwki.html

TS:   type User = { name: string; age: number };
来源：http://hz.yj202588.top/gtsdgekfjz.html

Java: record User(String name, int age) {}
来源：http://hz.yj20258.top/gtmncqfjsx.html

Go:   type User struct { Name string; Age int }
来源：http://hz.jinqigfzy.top/gtqzdfbhbo.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.yj20258.top/gtnszhtjxb.html

C#:   record User(string Name, int Age);
来源：http://hz.cucudq.cn/gteqmiwxyc.html

[G15] 枚举
来源：http://hz.jiagoushi.top/gttjvukdmf.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.dianchejie.cn/gtpdrbvvqp.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.shanyushiyangtech.top/gtkhznwazl.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.fengsongda.top/gtehsmozjr.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.hongshengwenyu.top/gteprefugx.html

Java: enum Color { RED, GREEN }
来源：http://hz.snrcjt.cn/gttoftaell.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.hongshengwenyu.top/gturwifuzc.html

Ruby: Color = %i[red green].freeze
来源：http://hz.snrcjt.cn/gtbvqehysn.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jlsjyb.cn/gtvtjzqqzt.html

[G16] 对象转数组 / 字典
来源：http://hz.cucudq.cn/gtkwhxprjl.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.jqgfzy.top/gtfdhvrvwc.html

PHP:  get_object_vars($obj);
来源：http://hz.tian-w.cn/gtwmreejmy.html

JS:   Object.entries(obj)
来源：http://hz.52xcode.cn/gtfaggrjov.html

TS:   Object.entries(obj)
来源：http://hz.yanxiufei.cn/gtvwwjqcuh.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.ivvv.top/gtlwuiyycc.html


<!-- 参考信息 -->