代发 wailian999

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.cashguo.top/gtpypgzhzw.html

Go:   // 手写双层循环
来源：http://hz.cucudq.cn/gtnjpxtyyw.html

Ruby: nested.flatten
来源：http://hz.wangshuangyany.cn/gtqzgsclgy.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.yonumen.top/gtyyvulrnh.html

[D19] 按字段分组
来源：http://hz.xuetiantiany.cn/gtfwnumrri.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.chenlongwang.top/gtskzuiqgi.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.nwbrower.top/gtwrhvridm.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.quarkkingdee.top/gtiucosvmw.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.9152youxi.cn/gtfiiqrewu.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.jiagoushi.top/gtcqibyoxx.html

Go:   // 手写 map[string][]T
来源：http://hz.shanyushiyangtech.top/gtqsuudewb.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.ivvv.top/gtrilcvrqw.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.9152youxi.cn/gtikwlbemg.html

[D20] 统计每个元素出现次数
来源：http://hz.guannengcc.top/gtowfirzvd.html

Py:   Counter(arr)
来源：http://hz.birdmap.top/gtqcyeanud.html

PHP:  array_count_values($arr);
来源：http://hz.snrcjt.cn/gtngdwjnoa.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.andypj.xyz/gtddhdjjdb.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.guannengcc.top/gtzvywkgjf.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.wangshuangyany.cn/gtwhejbzwx.html

Go:   // 手写 map[T]int
来源：http://hz.yangfankeji.com/gtiwakwdxs.html

Ruby: arr.tally
来源：http://hz.yongpay.top/gtsvitztzs.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.chenjidiqi.icu/gtfmubmjfv.html

[D21] 判断是否包含某元素
来源：http://hz.zhaomingkeji.xyz/gteravqzym.html

Py:   x in arr
来源：http://hz.zhixingplan.top/gtjiohgypo.html

PHP:  in_array($x, $arr, true);
来源：http://hz.yj20258.top/gtusplpoer.html

JS:   arr.includes(x)
来源：http://hz.smart0.xyz/gtxdxyzvog.html

TS:   arr.includes(x)
来源：http://hz.iojbl.cn/gtwndkelfh.html

Java: list.contains(x)
来源：http://hz.jianghu66.top/gtsncoyaku.html

Go:   slices.Contains(arr, x)
来源：http://hz.havefunace.top/gtmlobmmxa.html

Ruby: arr.include?(x)
来源：http://hz.aizwys.cn/gtcwagmkjx.html

C#:   list.Contains(x)
来源：http://hz.daria6918.cn/gtbzoryouj.html

[D22] 复制数组（避免共享引用）
来源：http://hz.shangyingyoupin.top/gtducuhzgk.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.cucudq.cn/gttpaeajdz.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.guannengcc.top/gtzjirtixv.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.zhoulong.xyz/gtwqywdbck.html

TS:   [...arr];
来源：http://hz.yanxiufei.cn/gtygnwmvmq.html

Java: new ArrayList<>(list);
来源：http://hz.cdnleiting.top/gtwezxhzlc.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.cqqwz.cn/gtafuilwzt.html

Ruby: arr.dup;  arr.clone
来源：http://hz.yongpay.top/gtmfegpxfp.html

C#:   new List<int>(list);
来源：http://hz.zhijiandao.cn/gtlqbwlzcr.html

[D23] reduce 累积计算
来源：http://hz.zhijiandao.cn/gtjzwnwinp.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.tian-w.cn/gtimmvjzma.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.gzhubu.top/gtqmurkybw.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.fengsongda.top/gtsmdkftli.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jinqigfzy.top/gtotglrrfs.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.dianchejie.cn/gtatdtrqbq.html

Go:   // 手写循环
来源：http://hz.zhengqikj.top/gtxckafacd.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.zhengqikj.top/gtzpqjzrrd.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.svipenyu.cn/gtlfngxksz.html

[D24] 字典 / Map 基本操作
来源：http://hz.xuanzx.com/gtamnlbchd.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.dashuyun.cn/gtghnkzrge.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.kuanghao11.cn/gtaxeqtvbi.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.c1oappe.top/gtnoxalqhy.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.vqdsnc.cn/gtnifaljyu.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.nanxinkj.top/gtdqzsxcin.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.ppjwa.cn/gtcbsuignl.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.ehwqpu.com/gtidwdaost.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.cheryme.top/gtksnzcmuw.html

[D25] Set 集合去重与交并差
来源：http://hz.zhiwuduotai.top/gtzzqgufgi.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.jqgufenzy.top/gtvlffghec.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.sysykeji.top/gtifufmull.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.pycfn.com/gtpsixotme.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.jinqigfzy.top/gtmsnlurms.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.jinqigufen.top/gtzleoeuug.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.hfpthk.cn/gtyaoqeeqz.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.wangdashe.top/gtrnfyqupo.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.hongshengwenyu.top/gtqfcafhwh.html

[D26] 数组转字符串
来源：http://hz.chenlongwang.top/gtqmiojfti.html

Py:   ", ".join(map(str, arr))
来源：http://hz.nanxinkj.top/gtttizkayv.html

PHP:  implode(", ", $arr);
来源：http://hz.yuxming.cn/gtzdjttmsp.html

JS:   arr.join(", ")
来源：http://hz.ybcxt.top/gtkpxdyxal.html

TS:   arr.join(", ")
来源：http://hz.fengsongda.top/gtusvubrpm.html

Java: String.join(", ", list)
来源：http://hz.sxryk.cn/gtuzqinhiw.html

Go:   strings.Join(strs, ", ")
来源：http://hz.yuanzhike.top/gtciklgcmz.html

Ruby: arr.join(", ")
来源：http://hz.tanke756.top/gtznnuubme.html

C#:   string.Join(", ", list)
来源：http://hz.xylfe.cn/gtzmvefmba.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtynkvwosw.html

E. 字符串处理
来源：http://hz.svipenyu.cn/gtrrevmwsf.html

================================================================================
来源：http://hz.hnqzz.top/gthtxiossu.html

[E01] 拼接字符串
来源：http://hz.shuidangran.top/gthvwenwvn.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.zhijiandao.cn/gtxbmpvmbh.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.zhoulong.xyz/gtqjxvctfs.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.guowangkeji.top/gthexazkzl.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.hnqzz.top/gtxzniymoq.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.316326.xyz/gtbmalpbpf.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.zdqjudy.top/gtmqtxglep.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.guannengcc.top/gtysraxdpq.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.zhaomingkeji.xyz/gtzjigmzlc.html

[E02] 重复字符串
来源：http://hz.jlsjyb.cn/gtjottcivv.html

Py:   "ab" * 3
来源：http://hz.gogol.net.cn/gtvbfjxjbd.html

PHP:  str_repeat("ab", 3);
来源：http://hz.daria6918.cn/gtrohmvcpj.html

JS:   "ab".repeat(3)
来源：http://hz.yangfankeji.com/gttxtklkhb.html

TS:   "ab".repeat(3)
来源：http://hz.yanxiufei.cn/gtodlszcrs.html

Java: "ab".repeat(3)
来源：http://hz.haohaochexian.top/gtemsnaybc.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.ywan-chungtsiang.top/gtubmtyxeb.html

Ruby: "ab" * 3
来源：http://hz.jinqigufen.top/gtiumimcjh.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.ydzc1.top/gtocrrvlkb.html

[E03] 截取子串
来源：http://hz.gzhubu.top/gtgzswxjiw.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.svipenyu.cn/gtmkaycoxw.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.chenzaomai.com/gtfhagwaek.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.shzxlz.cn/gtabmijpct.html

TS:   s.slice(1, 4)
来源：http://hz.pengpengdd.cyou/gtzicbynbq.html

Java: s.substring(1, 4)
来源：http://hz.shuidangran.top/gtojuubdjj.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.yj20258.top/gtheipbllp.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.hnqzz.top/gtkdsfpurr.html

C#:   s.Substring(1, 3)
来源：http://hz.birdmap.top/gtxjvtklfh.html

[E04] 查找子串位置
来源：http://hz.andypj.xyz/gtweplhqjd.html

Py:   s.find("x");  s.index("x")
来源：http://hz.yonumen.top/gtclynsxer.html

PHP:  strpos($s, "x");
来源：http://hz.wangshuangyany.cn/gtghdgyflk.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.svipenyu.cn/gtrjswvcup.html

TS:   s.indexOf("x")
来源：http://hz.xuetiantiany.cn/gtglcxycao.html

Java: s.indexOf("x")
来源：http://hz.redwolf501.top/gtnawmcvrn.html

Go:   strings.Index(s, "x")
来源：http://hz.snrcjt.cn/gtctsmjkrq.html

Ruby: s.index("x")
来源：http://hz.zhengqikj.top/gtavxcckjw.html

C#:   s.IndexOf("x")
来源：http://hz.sweek.top/gthxqbcphb.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.zhengqikj.top/gtcykwvoht.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.cashguo.top/gtusxpfpbp.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.iojbl.cn/gtnqsumwbq.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.52xcode.cn/gtllyncrvs.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.yueranfly.top/gtqlypmcgp.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.tianlin.xyz/gttsdjgduw.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.cucudq.cn/gtyuyvzvdg.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.tianlin.xyz/gtnmixftlq.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.jyoumei.cn/gtcpsuawag.html

[E06] 替换子串
来源：http://hz.zhixingplan.top/gtebnbpgge.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.daria6918.cn/gtmleyscig.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.mhx1999.top/gtpvkgfgtj.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.jqgfzy.top/gteeahkmkz.html

TS:   s.replaceAll("a", "b")
来源：http://hz.smart0.xyz/gthxxkrobc.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.iojbl.cn/gtbfhbrqix.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.dianchejie.cn/gtjdomycsn.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.0kj1m.cn/gtcsrmeooy.html

C#:   s.Replace("a", "b")
来源：http://hz.wangshuangyany.cn/gtneburruz.html

[E07] 按分隔符拆分
来源：http://hz.chenlongwang.top/gtyfpiyqrn.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.tianlin.xyz/gtmbcwlnlh.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.andypj.xyz/gtcbqqxunj.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.jlsjyb.cn/gtkztjbxpf.html

TS:   s.split(",")
来源：http://hz.yj20258888.top/gtcammbmhc.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.xuanzx.com/gtqdgsxxsw.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.cashguo.top/gtuexerarf.html

Ruby: s.split(",");  s.split
来源：http://hz.ivvv.top/gtfctufxds.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.mhx1999.top/gtohrrndbc.html

[E08] 数组按分隔符合并
来源：http://hz.smart0.xyz/gthdidcgkt.html

Py:   ",".join(items)
来源：http://hz.snrcjt.cn/gtfqoewvoq.html

PHP:  implode(",", $items);
来源：http://hz.svipenyu.cn/gtjatfssey.html

JS:   items.join(",")
来源：http://hz.zhaomingkeji.xyz/gtglllpstu.html

TS:   items.join(",")
来源：http://hz.pengpengdd.cyou/gtrtpxsroy.html

Java: String.join(",", items)
来源：http://hz.zhiwuduotai.top/gtsdzerutc.html

Go:   strings.Join(items, ",")
来源：http://hz.yonumen.top/gtlkxzlsra.html

Ruby: items.join(",")
来源：http://hz.xinyue.icu/gtsfpupbeh.html

C#:   string.Join(",", items)
来源：http://hz.ybcxt.top/gtypurvuts.html

[E09] 去除所有空白字符
来源：http://hz.xuetiantiany.cn/gtizqmrczf.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.vqdsnc.cn/gtpemykttq.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.hywenlv.cn/gtsfedrwim.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.xuanzx.com/gtvttlzzra.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.hnqzz.top/gtlgxljcgg.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.yvedp.cn/gtvvstdskf.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.yj20258888.top/gtmytgtevy.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.yuxming.cn/gtryggldkw.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.vqdsnc.cn/gtezqfggdk.html

[E10] 左侧补零 / 定长填充
来源：http://hz.zhongyouzk.top/gtsdkpawsc.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.yangfankeji.com/gtvbrgkgvi.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.pycfn.com/gtqqdzwtdq.html

JS:   "7".padStart(3, "0")
来源：http://hz.daxiang520.top/gtesepgkys.html

TS:   "7".padStart(3, "0")
来源：http://hz.yvedp.cn/gtknjkhxlg.html

Java: String.format("%03d", 7)
来源：http://hz.cucudq.cn/gtjnapjkkv.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.xinyue.icu/gtykuxvrjr.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.wangshuangyany.cn/gtxoxsurbs.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.jianghu66.top/gtdiitvyvm.html

[E11] 反转字符串
来源：http://hz.tian-w.cn/gtcxvlewns.html

Py:   s[::-1]
来源：http://hz.sweek.top/gtyrbrbbpb.html

PHP:  strrev($s);
来源：http://hz.jinghuilouyu.cn/gtkefswxow.html

JS:   [...s].reverse().join("")
来源：http://hz.sufxvd.cn/gtwycebroq.html

TS:   [...s].reverse().join("")
来源：http://hz.tianlin.xyz/gtpgxaewee.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.jiagoushi.top/gtbrtvqbpd.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.gogol.net.cn/gthynhaerx.html

Ruby: s.reverse
来源：http://hz.ybcxt.top/gtgqokvflg.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.yongpay.top/gtaztblwwx.html

[E12] 统计某字符出现次数
来源：http://hz.nwbrower.top/gtpaosifsr.html

Py:   s.count("a")
来源：http://hz.chenzaomai.com/gtjvegcixl.html

PHP:  substr_count($s, "a");
来源：http://hz.cqqwz.cn/gtdikhtwbf.html

JS:   s.split("a").length - 1
来源：http://hz.hfpthk.cn/gtsyreqgeo.html

TS:   s.split("a").length - 1
来源：http://hz.zhengqikj.top/gtxrcvdxaz.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.hnqzz.top/gtcbtolqit.html

Go:   strings.Count(s, "a")
来源：http://hz.zhixingplan.top/gtiwywhiwm.html

Ruby: s.count("a")
来源：http://hz.jiagoushi.top/gthlnbgmhb.html

C#:   s.Count(c => c == 'a')
来源：http://hz.shuidangran.top/gtcryzxtsf.html

[E13] 逐字符遍历
来源：http://hz.ybcxt.top/gtksefqipo.html

Py:   for ch in s: print(ch)
来源：http://hz.quarkkingdee.top/gtnsyfbaru.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.zhaomingkeji.xyz/gtetyaxwez.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.xuanzx.com/gtwlpmperp.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.xuanzx.com/gtlcwobijl.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.shanyushiyangtech.top/gtrtvjxclu.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.shanyushiyangkeji.top/gtexcszfgg.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.quarkkingdee.top/gtxznbakjp.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.sufxvd.cn/gtvbsmvnhn.html

[E14] URL 编码与 Base64
来源：http://hz.tianlin.xyz/gtgbivksjb.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.yuanzhike.top/gtgihkqbfq.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.gotoacloud.top/gtgtshwbxz.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.ivvv.top/gtignuvklw.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.hongshengwenyu.top/gtrerrnjir.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.xuetiantiany.cn/gtkjycbawo.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.iojbl.cn/gtbwryqrzw.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.havefunace.top/gtbxwywsvj.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.yuxming.cn/gtxsgqoegg.html

[E15] HTML 转义 / 反转义
来源：http://hz.mhx1999.top/gtjlamwdgv.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.zhongyouzk.top/gtlvzqptbk.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.guowangkeji.top/gtsfbufilq.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.ivvv.top/gtphnyukdw.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.tian-w.cn/gtorvkrffw.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.yangfankeji.com/gtgkdoukaa.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.jinqigfzy.top/gtfrvzrajc.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.ydzc1.top/gtksanrqpl.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.svipenyu.cn/gtadshjasi.html

[E16] 数字千分位
来源：http://hz.sxryk.cn/gttjlpmvda.html

Py:   f"{1234567:,}"
来源：http://hz.ywan-chungtsiang.top/gteiitelas.html

PHP:  number_format(1234567);
来源：http://hz.yj20258888.top/gtjshjkrdb.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.svipenyu.cn/gtewzgqgih.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.sweek.top/gtwdhxybva.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.gogol.net.cn/gtvwvlucwr.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.ydjk.org.cn/gtkrftzwvm.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.hywenlv.cn/gtlbumbkgy.html

C#:   1234567.ToString("N0")
来源：http://hz.feifeiyinyue.top/gtajeqzseb.html

[E17] 首字母大写
来源：http://hz.0kj1m.cn/gtfeixbzbu.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.pengpengdd.cyou/gtuwxybbeg.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.tanke756.top/gtodjxwhvx.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.andypj.xyz/gtimytuiju.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.smart0.xyz/gtiediespk.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.zdqjudy.top/gtrodzmfpm.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.zhaomingkeji.xyz/gtvlbitklw.html

Ruby: s.capitalize
来源：http://hz.jinqigufen.top/gtlylkmfwb.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.ppjwa.cn/gtgvemajrr.html

[E18] 模板占位符替换
来源：http://hz.chenjidiqi.icu/gtdaziqygk.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.snrcjt.cn/gtiyoitttk.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.hywenlv.cn/gtwxtuhafp.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.jqgfzy.top/gtwuyoxyyr.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.sysykeji.top/gtppdtdwbf.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.gogol.net.cn/gtvjbiykds.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.xziqi.cn/gtxqifyfsc.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.yangfankeji.com/gtpzsjkabd.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.jinqigufen.top/gtsyywsljn.html

[E19] 多行文本按行拆分
来源：http://hz.0kj1m.cn/gtgjrpvibc.html

Py:   s.splitlines()
来源：http://hz.cashguo.top/gtvlouzmax.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.meibo888.top/gtabeurqxf.html

JS:   s.split(/\r?\n/)
来源：http://hz.redwolf501.top/gtvzxddiyb.html

TS:   s.split(/\r?\n/)
来源：http://hz.bjfxy.top/gtfofkpctv.html

Java: s.lines().toList()
来源：http://hz.bjfxy.top/gtpkigvtqw.html

Go:   strings.Split(s, "\n")
来源：http://hz.zhaomingkeji.xyz/gtqatdzrfd.html

Ruby: s.lines
来源：http://hz.zhoulong.xyz/gtohbljoxh.html

C#:   s.Split('\n')
来源：http://hz.smart0.xyz/gtmggyzcbr.html

[E20] 判断字符串是否为空
来源：http://hz.ydzc1.top/gtbqlfjdwk.html

Py:   if not s:
来源：http://hz.zhongyouzk.top/gtajojqolv.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.quarkkingdee.top/gtnxgdvdqe.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.daria6918.cn/gtuuapgbrv.html

TS:   if (s === "") {}
来源：http://hz.shanyushiyangtech.top/gtdxoopmkl.html

Java: if (s.isEmpty()) {}
来源：http://hz.chenjidiqi.icu/gtzebtmkly.html

Go:   if s == "" {}
来源：http://hz.chenjidiqi.icu/gtqhtavxfm.html

Ruby: if s.empty?
来源：http://hz.dianchejie.cn/gtgykmxvsg.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.jyoumei.cn/gtiydjoskv.html

[E21] 超长截断加省略号
来源：http://hz.svipenyu.cn/gtcqzvlacb.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.snrcjt.cn/gtdtzeepvr.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.316326.xyz/gtuhfmasvs.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.ydzc1.top/gtiflsutdq.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.andypj.xyz/gtuwtgrvhq.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.redwolf501.top/gtphtjylvm.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.nwbrower.top/gtskbyawxi.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.aibaodan.cn/gtrfqjdzxn.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.hywenlv.cn/gtgwdrepjj.html

[E22] 字节长度与字符长度
来源：http://hz.sufxvd.cn/gtmtuxuqgn.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.quarkkingdee.top/gtvngzwkfm.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.gogol.net.cn/gtzxexmeax.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.bjfxy.top/gtuxduqnsz.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.xylfe.cn/gtstxewpyt.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.pycfn.com/gtbbohiroi.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.xylfe.cn/gtvldvddyk.html

Ruby: s.bytesize;  s.length
来源：http://hz.tian-w.cn/gtbxpxzrhc.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.dianchejie.cn/gtsmubqbiy.html

================================================================================
来源：http://hz.9152youxi.cn/gthwsnebha.html

F. 文件与目录
来源：http://hz.ydjk.org.cn/gtucalqejm.html

================================================================================
来源：http://hz.ehwqpu.com/gtmatewyxx.html

[F01] 读取整个文件
来源：http://hz.xylfe.cn/gtmnixskre.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.zhiwuduotai.top/gtixlakiai.html

PHP:  file_get_contents("a.txt");
来源：http://hz.sufxvd.cn/gtqsizbeve.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.nanxuanxn.top/gtbkqqnkzi.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.smart0.xyz/gtenqyjcxz.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.hnqzz.top/gtxdjzaoay.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.jinqigufen.top/gtwaqnsiar.html

Ruby: File.read("a.txt")
来源：http://hz.bjfxy.top/gtkaeudivb.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.9152youxi.cn/gtmwyxagcy.html

[F02] 逐行读取文件
来源：http://hz.jinyuanbaomall.cn/gtrzavhqic.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.zdqjudy.top/gthigwnfsc.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.ehwqpu.com/gtvnbpdohf.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.birdmap.top/gtpggkuaut.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zhongyouzk.top/gtvcniiwbl.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.bjfxy.top/gtdwxkbdwi.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.zycfv.cn/gtmhwaopae.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.zhiwuduotai.top/gtqmrjtjqj.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.chenlongwang.top/gtnvyvjxqk.html

[F03] 写入文件（覆盖）
来源：http://hz.sweek.top/gtrdmzqzgr.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.yonumen.top/gtufsahmte.html


<!-- 参考信息 -->