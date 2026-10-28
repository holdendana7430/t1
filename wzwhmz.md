代发 wailian999

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.yueranfly.top/gtumccjtus.html

Go:   // 手写双层循环
来源：http://hz.cheryme.top/gtnjzvlatr.html

Ruby: nested.flatten
来源：http://hz.quarkkingdee.top/gtxnvtrdbz.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.dianchejie.cn/gtdqgddlem.html

[D19] 按字段分组
来源：http://hz.gzhubu.top/gttrjzgyjx.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.gotoacloud.top/gteqnocrby.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.fzhhl.top/gtmvknocsn.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.hnxiangtu.top/gtknbtfcad.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.svipenyu.cn/gtwjzxhiqf.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.xingfuxueyuan.xyz/gtpjqlacak.html

Go:   // 手写 map[string][]T
来源：http://hz.shuidangran.top/gtymwonyfc.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.tianlin.xyz/gtkfzwocsc.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.yangfankeji.com/gtilyyygyk.html

[D20] 统计每个元素出现次数
来源：http://hz.svipenyu.cn/gtrnqumpds.html

Py:   Counter(arr)
来源：http://hz.jinyuanbaomall.cn/gtuqnhbeax.html

PHP:  array_count_values($arr);
来源：http://hz.ydzc1.top/gtjymxshmk.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.xuanzx.com/gtzpfhyqkc.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.daria6918.cn/gtopotwxfu.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.zhengqikj.top/gthbmfpbst.html

Go:   // 手写 map[T]int
来源：http://hz.sweek.top/gtzcxuzzza.html

Ruby: arr.tally
来源：http://hz.yangfankeji.com/gtofqapgxm.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.pycfn.com/gteprjmiiw.html

[D21] 判断是否包含某元素
来源：http://hz.yuxming.cn/gtrtfqmhah.html

Py:   x in arr
来源：http://hz.xylfe.cn/gtaadjpxnu.html

PHP:  in_array($x, $arr, true);
来源：http://hz.ydzc1.top/gtwtxzbezx.html

JS:   arr.includes(x)
来源：http://hz.cashguo.top/gtjlzpjqiz.html

TS:   arr.includes(x)
来源：http://hz.dashuyun.cn/gtltxppjjo.html

Java: list.contains(x)
来源：http://hz.fzhhl.top/gtmlxhwemz.html

Go:   slices.Contains(arr, x)
来源：http://hz.daria6918.cn/gtrwgvtsgo.html

Ruby: arr.include?(x)
来源：http://hz.hfpthk.cn/gtzuqypbnb.html

C#:   list.Contains(x)
来源：http://hz.jianghu66.top/gtzihkzjqa.html

[D22] 复制数组（避免共享引用）
来源：http://hz.shanyushiyangtech.top/gtomvxccve.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.quarkkingdee.top/gtxgcfncyx.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.yongpay.top/gtssmzsdcf.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.jyoumei.cn/gtermsieis.html

TS:   [...arr];
来源：http://hz.yuanzhike.top/gtztqzufyy.html

Java: new ArrayList<>(list);
来源：http://hz.jinqigufen.top/gtploktzlp.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.jinghuilouyu.cn/gtzwdzvbho.html

Ruby: arr.dup;  arr.clone
来源：http://hz.jinqigufen.top/gtlofklppd.html

C#:   new List<int>(list);
来源：http://hz.wangshuangyany.cn/gtpunfpmwp.html

[D23] reduce 累积计算
来源：http://hz.ivvv.top/gtlotbiong.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.jlsjyb.cn/gtqzuwvmcz.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.zhengqikj.top/gtyziwibvb.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.xuetiantiany.cn/gtximuhibz.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.guannengcc.top/gtmxfjsozp.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.chenlongwang.top/gtzivjymsc.html

Go:   // 手写循环
来源：http://hz.shuidangran.top/gtptpdjqqs.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.cqqwz.cn/gtlqkfwtkz.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.zhengqikj.top/gtwwnhnxdh.html

[D24] 字典 / Map 基本操作
来源：http://hz.gzhubu.top/gtgnnnawiz.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.vqdsnc.cn/gtuhpkrkii.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.yj20258888.top/gtdlflurff.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.shuidangran.top/gtmrkoqacc.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.jyoumei.cn/gthervkmma.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.sufxvd.cn/gtfhifzxfc.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.nanxinkj.top/gtwublaybq.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.tian-w.cn/gtpriynyin.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.cashguo.top/gtuhrrnohf.html

[D25] Set 集合去重与交并差
来源：http://hz.wangdashe.top/gtypyaoexx.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.316326.xyz/gtdnzoedxm.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.hnxiangtu.top/gtzzeamgxq.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.ppjwa.cn/gtovssmaoy.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.zhengqikj.top/gthurbkanv.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.chenzaomai.com/gtsaxjpdqn.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.0kj1m.cn/gtskepkjfc.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.ybcxt.top/gtaaqmflsd.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.xuetiantiany.cn/gtrdudbbhn.html

[D26] 数组转字符串
来源：http://hz.zdqjudy.top/gtunybjbfk.html

Py:   ", ".join(map(str, arr))
来源：http://hz.cqqwz.cn/gtfnoxdhbh.html

PHP:  implode(", ", $arr);
来源：http://hz.gogol.net.cn/gtyxijqlqd.html

JS:   arr.join(", ")
来源：http://hz.quarkkingdee.top/gtvdnszyyh.html

TS:   arr.join(", ")
来源：http://hz.andypj.xyz/gtxgzgqswb.html

Java: String.join(", ", list)
来源：http://hz.wangdashe.top/gtjmnayxby.html

Go:   strings.Join(strs, ", ")
来源：http://hz.yj20258888.top/gtzsfsyikb.html

Ruby: arr.join(", ")
来源：http://hz.sufxvd.cn/gteqlpevdc.html

C#:   string.Join(", ", list)
来源：http://hz.jqgfzy.top/gtounzfkvi.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtswmnjokt.html

E. 字符串处理
来源：http://hz.mhx1999.top/gtvrpgxkoh.html

================================================================================
来源：http://hz.c1oappe.top/gtcqhryrnm.html

[E01] 拼接字符串
来源：http://hz.yj20258.top/gtwttifglr.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.yvedp.cn/gtcxbwekrg.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.ywan-chungtsiang.top/gtrylqrdfm.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yueranfly.top/gtmjjhzktz.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jinqigfzy.top/gtqqaddvjw.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.cucudq.cn/gtxtcecskb.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.xylfe.cn/gtssyfxdhz.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.ybcxt.top/gtyglcmhqm.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.pycfn.com/gtivrjanvu.html

[E02] 重复字符串
来源：http://hz.sufxvd.cn/gtohjrvkjx.html

Py:   "ab" * 3
来源：http://hz.sysykeji.top/gtxywmlsej.html

PHP:  str_repeat("ab", 3);
来源：http://hz.yanxiufei.cn/gtpiosbggh.html

JS:   "ab".repeat(3)
来源：http://hz.hfpthk.cn/gtkfdxudsp.html

TS:   "ab".repeat(3)
来源：http://hz.9152youxi.cn/gtuacftmvm.html

Java: "ab".repeat(3)
来源：http://hz.chenjidiqi.icu/gtougvbetc.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.ydjk.org.cn/gtxqvrmgvg.html

Ruby: "ab" * 3
来源：http://hz.gogol.net.cn/gtyuizlmac.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.zycfv.cn/gtlmmampdw.html

[E03] 截取子串
来源：http://hz.daxiang520.top/gtncqnecfu.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.tian-w.cn/gttiwpbzal.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.ydzc1.top/gtmdoeycnt.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.yangfankeji.com/gtfophervh.html

TS:   s.slice(1, 4)
来源：http://hz.iojbl.cn/gtmowbjhep.html

Java: s.substring(1, 4)
来源：http://hz.cqqwz.cn/gtnsrpbjbr.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.andypj.xyz/gtdxvpbpim.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.jinyuanbaomall.cn/gtnxevyqzg.html

C#:   s.Substring(1, 3)
来源：http://hz.fzhhl.top/gttrdaoohv.html

[E04] 查找子串位置
来源：http://hz.ppjwa.cn/gthuhyoqtl.html

Py:   s.find("x");  s.index("x")
来源：http://hz.jinqigfzy.top/gthtnzkuqo.html

PHP:  strpos($s, "x");
来源：http://hz.yuxming.cn/gtdvlalxww.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.jinyuanbaomall.cn/gtcyjqmqct.html

TS:   s.indexOf("x")
来源：http://hz.hysaishi.cn/gtmhayjyds.html

Java: s.indexOf("x")
来源：http://hz.gzhubu.top/gtdddkoxqi.html

Go:   strings.Index(s, "x")
来源：http://hz.jqgufenzy.top/gtdrgvzjjp.html

Ruby: s.index("x")
来源：http://hz.xinyue.icu/gtospapitc.html

C#:   s.IndexOf("x")
来源：http://hz.zhongyouzk.top/gtrigihjel.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.yj20258.top/gtcrhavbky.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.ydzc1.top/gtazrovwzj.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.pengpengdd.cyou/gtcmbyxfve.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.tanke756.top/gtatjyvotm.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.guowangkeji.top/gtcvsyqqur.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.nanxuanxn.top/gtsdkezzvh.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.meibo888.top/gtgfzpckyg.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.yj20258.top/gtcuhgiwel.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.tianlin.xyz/gtihrqmpna.html

[E06] 替换子串
来源：http://hz.guannengcc.top/gtimyimvms.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.guannengcc.top/gtebgtjaex.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.sxryk.cn/gtyaqeexsi.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.ivvv.top/gtgqgzhggb.html

TS:   s.replaceAll("a", "b")
来源：http://hz.hfpthk.cn/gtunsrogzl.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.xinyue.icu/gtxvidnsqx.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.wangdashe.top/gtynbihtnu.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.zhijiandao.cn/gttcfomnts.html

C#:   s.Replace("a", "b")
来源：http://hz.cqqwz.cn/gtocaawuvn.html

[E07] 按分隔符拆分
来源：http://hz.sufxvd.cn/gtwvwxgfvc.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.sysykeji.top/gtvskpqikr.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.316326.xyz/gtnsgxeipw.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.iojbl.cn/gtltlfokvr.html

TS:   s.split(",")
来源：http://hz.shangyingyoupin.top/gtgqpxbbia.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.cucudq.cn/gtycluipyj.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.tanke756.top/gtdjjqteql.html

Ruby: s.split(",");  s.split
来源：http://hz.cqqwz.cn/gtapbvmbpb.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.shanyushiyangtech.top/gtxgtwskna.html

[E08] 数组按分隔符合并
来源：http://hz.cheryme.top/gtiquupxnn.html

Py:   ",".join(items)
来源：http://hz.hywenlv.cn/gtsbbcbzro.html

PHP:  implode(",", $items);
来源：http://hz.yuxming.cn/gtqpuuiwxr.html

JS:   items.join(",")
来源：http://hz.wangdashe.top/gtwxsosycx.html

TS:   items.join(",")
来源：http://hz.shanyushiyangtech.top/gtyfjqxqxe.html

Java: String.join(",", items)
来源：http://hz.xylfe.cn/gtmqlbnxyy.html

Go:   strings.Join(items, ",")
来源：http://hz.snrcjt.cn/gtcvzaxnol.html

Ruby: items.join(",")
来源：http://hz.c1oappe.top/gtovwsozmm.html

C#:   string.Join(",", items)
来源：http://hz.daxiang520.top/gtrsnlvvth.html

[E09] 去除所有空白字符
来源：http://hz.cheryme.top/gtsgnbqcjl.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.zhongyouzk.top/gtwjbyhfkb.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.sysykeji.top/gtacnwtwia.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.aibaodan.cn/gtxgdwimsx.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.shanyushiyangtech.top/gtqzeoitxv.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.yj202588.top/gtenieugtz.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.xuanzx.com/gtnxgkmcgs.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.jinqigufen.top/gtjqkrtdsk.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.jlsjyb.cn/gtpvbnikjj.html

[E10] 左侧补零 / 定长填充
来源：http://hz.pengpengdd.cyou/gtaygqcgnc.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.vqdsnc.cn/gtwlwlyumx.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.redwolf501.top/gtppzsbymn.html

JS:   "7".padStart(3, "0")
来源：http://hz.ivvv.top/gtchferynz.html

TS:   "7".padStart(3, "0")
来源：http://hz.quarkkingdee.top/gtrbnvfptd.html

Java: String.format("%03d", 7)
来源：http://hz.zdqjudy.top/gtxshspqmb.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.snrcjt.cn/gtupcbbinv.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.ivvv.top/gtuinhtgpj.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.cqqwz.cn/gtgfdcuxoq.html

[E11] 反转字符串
来源：http://hz.hongshengwenyu.top/gtrawqeawy.html

Py:   s[::-1]
来源：http://hz.shanyushiyangtech.top/gtwqzzxhwy.html

PHP:  strrev($s);
来源：http://hz.xingfuxueyuan.xyz/gtiphbuuki.html

JS:   [...s].reverse().join("")
来源：http://hz.xuanzx.com/gtoamsdykn.html

TS:   [...s].reverse().join("")
来源：http://hz.guowangkeji.top/gtlvdlunyi.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.cucudq.cn/gtzajkesar.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.tanke756.top/gtxmqpkyem.html

Ruby: s.reverse
来源：http://hz.kuanghao11.cn/gtqenslnxh.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.jinyuanbaomall.cn/gtrxukvpak.html

[E12] 统计某字符出现次数
来源：http://hz.jyoumei.cn/gtyiaasojd.html

Py:   s.count("a")
来源：http://hz.cdnleiting.top/gthwdcxnvr.html

PHP:  substr_count($s, "a");
来源：http://hz.redwolf501.top/gtbvznnegw.html

JS:   s.split("a").length - 1
来源：http://hz.smart0.xyz/gtnkrtkgru.html

TS:   s.split("a").length - 1
来源：http://hz.hywenlv.cn/gtumrrzzhu.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.zhaomingkeji.xyz/gtzmivoazh.html

Go:   strings.Count(s, "a")
来源：http://hz.gzhubu.top/gtkelzaqnr.html

Ruby: s.count("a")
来源：http://hz.ppjwa.cn/gtihfzgigt.html

C#:   s.Count(c => c == 'a')
来源：http://hz.vqdsnc.cn/gtfzwzapnn.html

[E13] 逐字符遍历
来源：http://hz.pycfn.com/gtksrreibz.html

Py:   for ch in s: print(ch)
来源：http://hz.yangfankeji.com/gtzmuqudgd.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.svipenyu.cn/gtiavknrjd.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.zycfv.cn/gtkuffjcnj.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.aibaodan.cn/gtspnakhxb.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.fengsongda.top/gtuakxzbrq.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.smart0.xyz/gtyjxbwuzx.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.hywenlv.cn/gtlkzsxosv.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.ydzc1.top/gtxleusdtu.html

[E14] URL 编码与 Base64
来源：http://hz.316326.xyz/gtgmculkpr.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.haohaochexian.top/gtpmsozphd.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.gogol.net.cn/gtzsyydgny.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.andypj.xyz/gtwzuidxym.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.feifeiyinyue.top/gtdwujdrxp.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.hywenlv.cn/gtpeaicrvn.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.yj202588.top/gtblyqbliy.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.shangyingyoupin.top/gtaegpbegc.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.shangyingyoupin.top/gtysbudwxd.html

[E15] HTML 转义 / 反转义
来源：http://hz.daria6918.cn/gtcnrtuuim.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.jyoumei.cn/gtqrwyqbqh.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.meibo888.top/gtdphqrweg.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.yuanzhike.top/gtzopnpimn.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.meibo888.top/gtbdegxvqd.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.dashuyun.cn/gtelmalake.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.fengsongda.top/gtrxybajtk.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.meibo888.top/gtqwvjvcct.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.nanxuanxn.top/gtpmunxydm.html

[E16] 数字千分位
来源：http://hz.tian-w.cn/gtejkioilc.html

Py:   f"{1234567:,}"
来源：http://hz.yj202588.top/gtympmjdvu.html

PHP:  number_format(1234567);
来源：http://hz.havefunace.top/gtnmeuzten.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.yj20258888.top/gtqynevrar.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.shanyushiyangtech.top/gttgjfrjeu.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.ppjwa.cn/gtzprrlwku.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.zhijiandao.cn/gtnnfmwjdo.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.yueranfly.top/gteauznuxz.html

C#:   1234567.ToString("N0")
来源：http://hz.jlsjyb.cn/gttdqllnwu.html

[E17] 首字母大写
来源：http://hz.redwolf501.top/gtqlbnhxma.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.nanxuanxn.top/gthrbdzvnj.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.daxiang520.top/gtomclezjb.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.xuanzx.com/gtqatyeuvh.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.zhaomingkeji.xyz/gtuybuilow.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.chenjidiqi.icu/gtwbmuqcdt.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.shanyushiyangkeji.top/gtbmlgdoxv.html

Ruby: s.capitalize
来源：http://hz.gzhubu.top/gttnmvchxt.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.yj20258.top/gtiztktwiw.html

[E18] 模板占位符替换
来源：http://hz.zdqjudy.top/gtgadbrtfl.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.vqdsnc.cn/gtsonxkljf.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.haohaochexian.top/gtqeeypawn.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.c1oappe.top/gtagzgukjo.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.shanyushiyangkeji.top/gtczphfmll.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.zycfv.cn/gtxkkixeas.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.sxryk.cn/gtdyvpyuit.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.hongshengwenyu.top/gtxkyjydcv.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.cashguo.top/gtojpkpujq.html

[E19] 多行文本按行拆分
来源：http://hz.yj20258888.top/gtbtiaojqr.html

Py:   s.splitlines()
来源：http://hz.hongshengwenyu.top/gtkxlvdsux.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.zhixingplan.top/gtlkyhhqrx.html

JS:   s.split(/\r?\n/)
来源：http://hz.yuanzhike.top/gtjgyhpiao.html

TS:   s.split(/\r?\n/)
来源：http://hz.yongpay.top/gtzcohpnys.html

Java: s.lines().toList()
来源：http://hz.hysaishi.cn/gtumjfffje.html

Go:   strings.Split(s, "\n")
来源：http://hz.hnxiangtu.top/gtbmfgdcxr.html

Ruby: s.lines
来源：http://hz.yanxiufei.cn/gthyogripz.html

C#:   s.Split('\n')
来源：http://hz.shangyingyoupin.top/gtducuavya.html

[E20] 判断字符串是否为空
来源：http://hz.jyoumei.cn/gtjvblefjc.html

Py:   if not s:
来源：http://hz.ehwqpu.com/gtsaoprwuu.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.shanyushiyangkeji.top/gtqezviufj.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.chenjidiqi.icu/gtnmdlxtjt.html

TS:   if (s === "") {}
来源：http://hz.birdmap.top/gtwasuftfa.html

Java: if (s.isEmpty()) {}
来源：http://hz.cqqwz.cn/gtlkgyxraw.html

Go:   if s == "" {}
来源：http://hz.mhx1999.top/gtllnrouik.html

Ruby: if s.empty?
来源：http://hz.ivvv.top/gtaugzhjdc.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.pengpengdd.cyou/gtdtztagxq.html

[E21] 超长截断加省略号
来源：http://hz.sufxvd.cn/gtwbexkblo.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.redwolf501.top/gtmpdcufjm.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.zhijiandao.cn/gtpseqfycn.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.haohaochexian.top/gtnoywcttf.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.vqdsnc.cn/gtdtfbdgga.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.pycfn.com/gtqqjbejbe.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.feifeiyinyue.top/gtrkttzkoy.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.jinqigfzy.top/gtgmkdwqqb.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.feifeiyinyue.top/gtphdgujpg.html

[E22] 字节长度与字符长度
来源：http://hz.nwbrower.top/gtrlaxeqti.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.ydjk.org.cn/gtkdulucur.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jyoumei.cn/gtqnmymcmn.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.gaohongyu789.top/gtpezyhhfj.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.meibo888.top/gtqtizonah.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.yongpay.top/gtktramqay.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.nanxinkj.top/gtdkvayytp.html

Ruby: s.bytesize;  s.length
来源：http://hz.zycfv.cn/gtkzainhpk.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.nwbrower.top/gtwfyrlrdh.html

================================================================================
来源：http://hz.316326.xyz/gtvmrlwpup.html

F. 文件与目录
来源：http://hz.jinyuanbaomall.cn/gtiqrbuwgh.html

================================================================================
来源：http://hz.redwolf501.top/gteamvsweh.html

[F01] 读取整个文件
来源：http://hz.vqdsnc.cn/gttackznyu.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.meibo888.top/gtlbrjmptf.html

PHP:  file_get_contents("a.txt");
来源：http://hz.dianchejie.cn/gtcgjhhwox.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.chenjidiqi.icu/gtzkydvitw.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.zhongyouzk.top/gtiwtaxkvz.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.zycfv.cn/gtzfesbwum.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.birdmap.top/gtrtizjkep.html

Ruby: File.read("a.txt")
来源：http://hz.guannengcc.top/gtghmoayjj.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.yangfankeji.com/gtyqnyfxwf.html

[F02] 逐行读取文件
来源：http://hz.snrcjt.cn/gtmzxjrzkz.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.nanxinkj.top/gtzgdnmyez.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.tianlin.xyz/gtoqzcudmx.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.xylfe.cn/gtgwlkqpdw.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zhiwuduotai.top/gtfxtshuds.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.mhx1999.top/gtdcsueapy.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.316326.xyz/gtanellios.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.xinyue.icu/gthzffssqc.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.yongpay.top/gtahutpxru.html

[F03] 写入文件（覆盖）
来源：http://hz.zhixingplan.top/gtyvgvivtg.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.shzxlz.cn/gtwtuytprb.html


<!-- 参考信息 -->