代发 wailian999

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.yvedp.cn/gtnsyhvnwu.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.daxiang520.top/gtzoxdiurz.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.yangfankeji.com/gtzuzftulw.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.chenjidiqi.icu/gtgldpnpfi.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.hywenlv.cn/gtdhgpcvof.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.sufxvd.cn/gtroinxhyb.html

Ruby: s.capitalize
来源：http://hz.pycfn.com/gtxpdiuawy.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.jinyuanbaomall.cn/gthsqczsih.html

[E18] 模板占位符替换
来源：http://hz.xziqi.cn/gthzhadjlp.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.quarkkingdee.top/gtxluhypmd.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.cucudq.cn/gtkqbnjrll.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.shzxlz.cn/gtauqivcdj.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.haohaochexian.top/gtufmetwgs.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.hfpthk.cn/gtpmyqnfce.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.xylfe.cn/gtdgnhtldv.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.hnxiangtu.top/gttaufbamb.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.jinghuilouyu.cn/gtkydvmryw.html

[E19] 多行文本按行拆分
来源：http://hz.hywenlv.cn/gtmmbgtypl.html

Py:   s.splitlines()
来源：http://hz.redwolf501.top/gtszdimoey.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.shuidangran.top/gtrdaezjsf.html

JS:   s.split(/\r?\n/)
来源：http://hz.hfpthk.cn/gtkdugfqpm.html

TS:   s.split(/\r?\n/)
来源：http://hz.zhongyouzk.top/gtumvueevd.html

Java: s.lines().toList()
来源：http://hz.wangdashe.top/gtnqgqbamr.html

Go:   strings.Split(s, "\n")
来源：http://hz.xuanzx.com/gtketydaks.html

Ruby: s.lines
来源：http://hz.hammf.cn/gtympwwmdb.html

C#:   s.Split('\n')
来源：http://hz.gotoacloud.top/gtzowppykx.html

[E20] 判断字符串是否为空
来源：http://hz.fengsongda.top/gtrsoxelzh.html

Py:   if not s:
来源：http://hz.yj20258888.top/gtcsqqenhg.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.meibo888.top/gtkrmolbex.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.hongshengwenyu.top/gtpkycjjta.html

TS:   if (s === "") {}
来源：http://hz.shuidangran.top/gtbuzpbzje.html

Java: if (s.isEmpty()) {}
来源：http://hz.feifeiyinyue.top/gtkepjqqzz.html

Go:   if s == "" {}
来源：http://hz.quarkkingdee.top/gtwgmbiotm.html

Ruby: if s.empty?
来源：http://hz.zdqjudy.top/gturphxnfz.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.cqqwz.cn/gtutibnpxu.html

[E21] 超长截断加省略号
来源：http://hz.snrcjt.cn/gtlfijymzm.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.sysykeji.top/gtvyulqqeu.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.xinyue.icu/gtbzsbbrju.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.cashguo.top/gtnkrzsqnx.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.andypj.xyz/gtttszcuja.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.9152youxi.cn/gtqascyeev.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.xylfe.cn/gtabcqicho.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.feifeiyinyue.top/gtsdtfzfhy.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.iojbl.cn/gtwfqaeysw.html

[E22] 字节长度与字符长度
来源：http://hz.ydzc1.top/gtevzvfpvo.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.xziqi.cn/gthdgagaqt.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.52xcode.cn/gtcihvplez.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.birdmap.top/gtagovloat.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.ppjwa.cn/gtafusvmla.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.316326.xyz/gtnxtezzhj.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.jiagoushi.top/gtcddqznwi.html

Ruby: s.bytesize;  s.length
来源：http://hz.dianchejie.cn/gtsmdlynig.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.redwolf501.top/gtfddehoeg.html

================================================================================
来源：http://hz.hywenlv.cn/gtycemhtdt.html

F. 文件与目录
来源：http://hz.xuanzx.com/gtmygcexcp.html

================================================================================
来源：http://hz.jqgufenzy.top/gtjkzergtr.html

[F01] 读取整个文件
来源：http://hz.redwolf501.top/gtgbfneznk.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.aizwys.cn/gtgxfsbybo.html

PHP:  file_get_contents("a.txt");
来源：http://hz.shanyushiyangkeji.top/gtbvjunmno.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.vqdsnc.cn/gtwpumkxxe.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.yongpay.top/gtbnqpsawy.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.gzhubu.top/gtstrkgkdn.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.tianlin.xyz/gtejzlseyn.html

Ruby: File.read("a.txt")
来源：http://hz.yueranfly.top/gtyescfefe.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.hnqzz.top/gtswlqnjth.html

[F02] 逐行读取文件
来源：http://hz.nwbrower.top/gtzrdihbwp.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.52xcode.cn/gthckioqom.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.dashuyun.cn/gtseakdgih.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zhixingplan.top/gtdrmbyyyo.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.hammf.cn/gtfobiimxg.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.yuxming.cn/gtwsyjqvsz.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.hfpthk.cn/gtwxcteqcy.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.ppjwa.cn/gttlimezjb.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.dianchejie.cn/gtohmrqrdm.html

[F03] 写入文件（覆盖）
来源：http://hz.ivvv.top/gtsiibkpjv.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.aizwys.cn/gtfrigopsr.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.zhiwuduotai.top/gtepvyrjfc.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.svipenyu.cn/gtaqxmobrv.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.zhiwuduotai.top/gtcelfhzwl.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.cucudq.cn/gttqvpptqz.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.zhengqikj.top/gtekcwyaxc.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.meibo888.top/gtovpfmxkv.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.hongshengwenyu.top/gtjcrxdmst.html

[F04] 追加写入文件
来源：http://hz.9152youxi.cn/gttglcjtqc.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.iojbl.cn/gtdzuvritn.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.xingfuxueyuan.xyz/gtvfbiupxt.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.chenlongwang.top/gtfeeneabj.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.316326.xyz/gttuipjbvz.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.jinqigfzy.top/gtnvxshyev.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.jinqigfzy.top/gtbfcbdfmt.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.redwolf501.top/gtwjzqdctw.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.wangshuangyany.cn/gtuvekwtrm.html

[F05] 判断文件或目录是否存在
来源：http://hz.xingfuxueyuan.xyz/gtcunuyxcf.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.jinghuilouyu.cn/gtsyxochzy.html

PHP:  file_exists("a.txt");
来源：http://hz.yj202588.top/gtnawiiykj.html

JS:   fs.existsSync("a.txt")
来源：http://hz.yangfankeji.com/gtppthswwh.html

TS:   fs.existsSync("a.txt")
来源：http://hz.chenzaomai.com/gtcibmzilt.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.dashuyun.cn/gtitdfxibw.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.shanyushiyangkeji.top/gtbcvwpacp.html

Ruby: File.exist?("a.txt")
来源：http://hz.vqdsnc.cn/gtprrjigtg.html

C#:   File.Exists("a.txt")
来源：http://hz.jyoumei.cn/gtycaeqcki.html

[F06] 删除文件
来源：http://hz.jqgfzy.top/gtfmziuvfi.html

Py:   os.remove("a.txt")
来源：http://hz.yueranfly.top/gtyuiajavz.html

PHP:  unlink("a.txt");
来源：http://hz.ydjk.org.cn/gtxekydlcl.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.dianchejie.cn/gtuvjxlkig.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.dashuyun.cn/gtawedtwem.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.jinqigfzy.top/gtegtbaizk.html

Go:   os.Remove("a.txt")
来源：http://hz.yj20258.top/gtidabtjgs.html

Ruby: File.delete("a.txt")
来源：http://hz.shuidangran.top/gtgorwxutf.html

C#:   File.Delete("a.txt");
来源：http://hz.pycfn.com/gtagrhjwfe.html

[F07] 创建目录（含多级）
来源：http://hz.jinqigufen.top/gtvcwruvje.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.cucudq.cn/gtzjfhthev.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.iojbl.cn/gtyncensce.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.hysaishi.cn/gtsmsbdhju.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.vqdsnc.cn/gtaffemwgj.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.nanxuanxn.top/gtlfpdyyid.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.yueranfly.top/gtdwyxbzfh.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.quarkkingdee.top/gtzghyrnro.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.jinyuanbaomall.cn/gtldetuucq.html

[F08] 遍历目录
来源：http://hz.zhiwuduotai.top/gtguxzxsdp.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.meibo888.top/gtqgutpwjx.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.redwolf501.top/gtmqkvoecu.html

JS:   fs.readdirSync("dir")
来源：http://hz.mhx1999.top/gtwwymidso.html

TS:   fs.readdirSync("dir")
来源：http://hz.jinqigfzy.top/gtseokmlho.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.gotoacloud.top/gtblgdimgt.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.bjfxy.top/gtzdfoqzjf.html

Ruby: Dir.children("dir")
来源：http://hz.chenjidiqi.icu/gtulhlcioa.html

C#:   Directory.GetFiles("dir")
来源：http://hz.bjfxy.top/gtyjfcasfn.html

[F09] 获取文件大小
来源：http://hz.52xcode.cn/gtweqazaym.html

Py:   os.path.getsize("a.txt")
来源：http://hz.shzxlz.cn/gteaqoshbu.html

PHP:  filesize("a.txt");
来源：http://hz.nanxuanxn.top/gtwtjebyzi.html

JS:   fs.statSync("a.txt").size
来源：http://hz.kuanghao11.cn/gtntixhbjy.html

TS:   fs.statSync("a.txt").size
来源：http://hz.jyoumei.cn/gtvglnuosz.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.birdmap.top/gtcnkqxvpf.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.fzhhl.top/gtyfzbmzzq.html

Ruby: File.size("a.txt")
来源：http://hz.zhixingplan.top/gtpznmozou.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.yuanzhike.top/gtxkqowqjb.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.fzhhl.top/gtvocutbvp.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.xingfuxueyuan.xyz/gtjogxczpk.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.shanyushiyangkeji.top/gtqisibscz.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.xziqi.cn/gtawftdgtq.html

TS:   path.extname("a.txt")
来源：http://hz.shuidangran.top/gtqwwvcbvf.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.xuetiantiany.cn/gtcmzdrbkj.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.shanyushiyangtech.top/gteyrzknqj.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.quarkkingdee.top/gtdploxcgg.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.meibo888.top/gtqszcnpfj.html

[F11] 复制与移动文件
来源：http://hz.yuxming.cn/gtjggmkvku.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.haohaochexian.top/gtrinutbwh.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.yvedp.cn/gtdwardyju.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yueranfly.top/gtbeehgdwx.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.meibo888.top/gtyivlqbnm.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.jyoumei.cn/gtsyfydfbf.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.zhongyouzk.top/gtwoddckgh.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.nanxuanxn.top/gtfgpmkulj.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.havefunace.top/gtbsebgnjb.html

[F12] CSV 读写
来源：http://hz.yonumen.top/gtpmbuohwj.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.zhixingplan.top/gtsfvhykrv.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.316326.xyz/gtdicwcmfs.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.kuanghao11.cn/gtohmeedtb.html

TS:   // 同上
来源：http://hz.xingfuxueyuan.xyz/gtzwsrrxqs.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.aibaodan.cn/gturtjopbr.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.wangdashe.top/gtrvikgkhq.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.mhx1999.top/gtkbakkyxf.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.nanxinkj.top/gtlicwyhnz.html

================================================================================
来源：http://hz.tianlin.xyz/gtebkzfhhc.html

G. 面向对象
来源：http://hz.feifeiyinyue.top/gtxhoymozn.html

================================================================================
来源：http://hz.jinqigufen.top/gtmszpoyaf.html

[G01] 定义类
来源：http://hz.cheryme.top/gtlradkjjf.html

Py:   class User: pass
来源：http://hz.cqqwz.cn/gtnntfepvr.html

PHP:  class User {}
来源：http://hz.vqdsnc.cn/gtdsonsylk.html

JS:   class User {}
来源：http://hz.ivvv.top/gtpoeojmtw.html

TS:   class User { name: string = ""; }
来源：http://hz.smart0.xyz/gtzafhctta.html

Java: class User {}
来源：http://hz.52xcode.cn/gtczhcohdc.html

Go:   type User struct { Name string }
来源：http://hz.yonumen.top/gtwvstqpuj.html

Ruby: class User; end
来源：http://hz.zhiwuduotai.top/gtemmakkjc.html

C#:   class User {}
来源：http://hz.nwbrower.top/gtujlgtvbt.html

[G02] 构造函数
来源：http://hz.hongshengwenyu.top/gthmwbojco.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.yangfankeji.com/gthpzdutzm.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.yanxiufei.cn/gtpyybbqgr.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.gogol.net.cn/gtiaibqakb.html

TS:   constructor(public name: string) {}
来源：http://hz.gaohongyu789.top/gtynsnvzrb.html

Java: User(String name) { this.name = name; }
来源：http://hz.jinqigufen.top/gtzztvuitx.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.xziqi.cn/gtwegwvqsj.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.zhijiandao.cn/gtiveuyuzq.html

C#:   public User(string name) { Name = name; }
来源：http://hz.shzxlz.cn/gtzhblosqt.html

[G03] 实例属性
来源：http://hz.xuetiantiany.cn/gtffhugpdn.html

Py:   self.name = "x"
来源：http://hz.sweek.top/gthfgtxmhi.html

PHP:  public string $name = "x";
来源：http://hz.jinqigfzy.top/gtiwcbcuez.html

JS:   this.name = "x";
来源：http://hz.quarkkingdee.top/gtiiczrkeh.html

TS:   name: string = "x";
来源：http://hz.havefunace.top/gtlnljegwt.html

Java: private String name;
来源：http://hz.hammf.cn/gthbkkhuoj.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.jianghu66.top/gtoqupfzga.html

Ruby: @name = "x"
来源：http://hz.cheryme.top/gtrsxgxzkr.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.daxiang520.top/gtpzwzpslu.html

[G04] 定义方法
来源：http://hz.daria6918.cn/gtgdlvratw.html

Py:   def greet(self): return self.name
来源：http://hz.quarkkingdee.top/gtodehpfbz.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.nanxuanxn.top/gtnmdmmpxs.html

JS:   greet() { return this.name; }
来源：http://hz.hywenlv.cn/gtcnktlnup.html

TS:   greet(): string { return this.name; }
来源：http://hz.ehwqpu.com/gtmhftxqxe.html

Java: String greet() { return name; }
来源：http://hz.snrcjt.cn/gtlheyhfuh.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.jiagoushi.top/gtrbsvgwby.html

Ruby: def greet; @name; end
来源：http://hz.zhoulong.xyz/gttkdgktqj.html

C#:   public string Greet() => Name;
来源：http://hz.cdnleiting.top/gtgfkhponr.html

[G05] 继承
来源：http://hz.ydzc1.top/gtemjqiizc.html

Py:   class Admin(User): pass
来源：http://hz.tanke756.top/gthkddbelt.html

PHP:  class Admin extends User {}
来源：http://hz.ydjk.org.cn/gttwzexhff.html

JS:   class Admin extends User {}
来源：http://hz.9152youxi.cn/gtsvrwrlmz.html

TS:   class Admin extends User {}
来源：http://hz.jinqigufen.top/gtcdxdmaco.html

Java: class Admin extends User {}
来源：http://hz.wangshuangyany.cn/gtqwgofvnm.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.xylfe.cn/gtghnybscg.html

Ruby: class Admin < User; end
来源：http://hz.hysaishi.cn/gtekqjkmyo.html

C#:   class Admin : User {}
来源：http://hz.ehwqpu.com/gtciifeebe.html

[G06] 重写方法
来源：http://hz.jqgfzy.top/gtayprmerm.html

Py:   def greet(self): return "admin"
来源：http://hz.sweek.top/gtdtcfcpfi.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.wangshuangyany.cn/gtuczclzwu.html

JS:   greet() { return "admin"; }
来源：http://hz.nanxinkj.top/gtofijtrqh.html

TS:   greet(): string { return "admin"; }
来源：http://hz.xuetiantiany.cn/gtdneyepvp.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.yonumen.top/gtfyzyjtay.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.smart0.xyz/gtnirkfrut.html

Ruby: def greet; "admin"; end
来源：http://hz.yangfankeji.com/gtmoydvdmx.html

C#:   public override string Greet() => "admin";
来源：http://hz.iojbl.cn/gtdftvgpdf.html

[G07] 调用父类方法
来源：http://hz.xuanzx.com/gtfkcbawmm.html

Py:   super().greet()
来源：http://hz.sweek.top/gtjsinzlrp.html

PHP:  parent::greet();
来源：http://hz.ivvv.top/gtgehjpsui.html

JS:   super.greet();
来源：http://hz.jinqigufen.top/gtghlcovkx.html

TS:   super.greet();
来源：http://hz.redwolf501.top/gtysrotaeg.html

Java: super.greet();
来源：http://hz.kuanghao11.cn/gtpbckyawd.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.zhongyouzk.top/gtcujyjkod.html

Ruby: super
来源：http://hz.havefunace.top/gttpaymvgo.html

C#:   base.Greet();
来源：http://hz.xinyue.icu/gtdtylbqau.html

[G08] 静态方法与属性
来源：http://hz.jyoumei.cn/gtccvuqrgw.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.sweek.top/gtpsmbinna.html

PHP:  public static function f() {}
来源：http://hz.yvedp.cn/gtomovtxba.html

JS:   static f() {}
来源：http://hz.xuetiantiany.cn/gtuahfjvgq.html

TS:   static f(): void {}
来源：http://hz.0kj1m.cn/gtuwytbwbk.html

Java: static void f() {}
来源：http://hz.jinghuilouyu.cn/gtjcfubqul.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.hammf.cn/gthzxeytaq.html

Ruby: def self.f; end
来源：http://hz.chenlongwang.top/gtaekovoyi.html

C#:   public static void F() {}
来源：http://hz.wangshuangyany.cn/gtlbpezxhr.html

[G09] 接口 / 抽象类
来源：http://hz.vqdsnc.cn/gtwythxfef.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.yj20258888.top/gtjdudwkqe.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.yueranfly.top/gtzxpkmzmp.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.wangdashe.top/gtggznfeoy.html

TS:   interface Shape { area(): number; }
来源：http://hz.pengpengdd.cyou/gtdsyoaexe.html

Java: interface Shape { double area(); }
来源：http://hz.sufxvd.cn/gthbjorjum.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.pengpengdd.cyou/gtunjtnchq.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.quarkkingdee.top/gtlmrbdnta.html

C#:   interface IShape { double Area(); }
来源：http://hz.dianchejie.cn/gtvebxhrjl.html

[G10] 访问控制
来源：http://hz.zycfv.cn/gtzzgtmwhp.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.316326.xyz/gtqgawaclt.html

PHP:  public / protected / private
来源：http://hz.zhiwuduotai.top/gtakdjdrea.html

JS:   #private 字段；其余公开
来源：http://hz.yanxiufei.cn/gtfqijnwzr.html

TS:   public / protected / private
来源：http://hz.havefunace.top/gtzqwajmse.html

Java: public / protected / private / 默认包级
来源：http://hz.mhx1999.top/gtetruxobn.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.zhengqikj.top/gtbcqvjfud.html

Ruby: public / protected / private
来源：http://hz.shanyushiyangkeji.top/gtjucxcrwz.html

C#:   public / protected / private / internal
来源：http://hz.shzxlz.cn/gtagyjyiqg.html

[G11] getter / setter
来源：http://hz.ybcxt.top/gthifcjxwa.html

Py:   @property 与 @x.setter
来源：http://hz.hammf.cn/gtgrgciffu.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.guannengcc.top/gtstcicspp.html

JS:   get name() { return this._name; }
来源：http://hz.nwbrower.top/gtfqaykggs.html

TS:   get name(): string { return this._name; }
来源：http://hz.yuxming.cn/gttgpmkgwe.html

Java: public String getName() { return name; }
来源：http://hz.shanyushiyangtech.top/gtwuzvafkz.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.redwolf501.top/gtwlrudylg.html

Ruby: attr_accessor :name
来源：http://hz.smart0.xyz/gtkcuzmahe.html

C#:   public string Name { get; set; }
来源：http://hz.chenjidiqi.icu/gtaypiwbbk.html

[G12] 对象转字符串
来源：http://hz.xylfe.cn/gtiuragdtl.html

Py:   def __str__(self): return self.name
来源：http://hz.gaohongyu789.top/gtgzfxekir.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.nanxinkj.top/gtiyangfpz.html

JS:   toString() { return this.name; }
来源：http://hz.guannengcc.top/gtamvigchb.html

TS:   toString(): string { return this.name; }
来源：http://hz.cheryme.top/gtyyxdvllw.html

Java: @Override public String toString() { return name; }
来源：http://hz.xylfe.cn/gtuenwpglj.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.aibaodan.cn/gtyywlgzxl.html

Ruby: def to_s; @name; end
来源：http://hz.cucudq.cn/gtgzfvvuff.html

C#:   public override string ToString() => Name;
来源：http://hz.yj20258.top/gtudbomieh.html

[G13] 判断对象类型
来源：http://hz.yuxming.cn/gtprgtwbur.html

Py:   isinstance(u, User)
来源：http://hz.bjfxy.top/gtcbhcjosn.html

PHP:  $u instanceof User
来源：http://hz.wangshuangyany.cn/gtbvskvkxh.html

JS:   u instanceof User
来源：http://hz.zhongyouzk.top/gtbwzwxrut.html

TS:   u instanceof User
来源：http://hz.gotoacloud.top/gtjqesikda.html

Java: u instanceof User
来源：http://hz.ivvv.top/gtcdpudyfg.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.aibaodan.cn/gtknblilkv.html

Ruby: u.is_a?(User)
来源：http://hz.ydzc1.top/gtfnnpybdc.html

C#:   u is User
来源：http://hz.yueranfly.top/gtkqvbanqo.html

[G14] 数据类 / record
来源：http://hz.yongpay.top/gtvjbbhbmd.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.jqgfzy.top/gtockdrssv.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.jqgufenzy.top/gtiqchuzui.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.gzhubu.top/gtyuvsxduz.html

TS:   type User = { name: string; age: number };
来源：http://hz.guowangkeji.top/gtitlgrydu.html

Java: record User(String name, int age) {}
来源：http://hz.shangyingyoupin.top/gtpqxajvju.html

Go:   type User struct { Name string; Age int }
来源：http://hz.ywan-chungtsiang.top/gtlyauntdn.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.feifeiyinyue.top/gtvdjeokeq.html

C#:   record User(string Name, int Age);
来源：http://hz.jinyuanbaomall.cn/gtxxcloxcd.html

[G15] 枚举
来源：http://hz.xingfuxueyuan.xyz/gtozuilebr.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.cqqwz.cn/gttotavvdi.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.ydjk.org.cn/gtrcqzuryj.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.kuanghao11.cn/gtrfcygzxl.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zhongyouzk.top/gtrhpsnqux.html

Java: enum Color { RED, GREEN }
来源：http://hz.birdmap.top/gtqskcnjdx.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.jiagoushi.top/gtqgcwdonr.html


<!-- 参考信息 -->