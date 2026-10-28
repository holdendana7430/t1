代发 wailian999

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.chenjidiqi.icu/gtujvxgjre.html

PHP:  array_merge(...$nested);
来源：http://hz.iojbl.cn/gtapdgobyt.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.jlsjyb.cn/gtaiywboqe.html

TS:   nested.flat();
来源：http://hz.sysykeji.top/gtlxmxgoon.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.sxryk.cn/gtphsqadsk.html

Go:   // 手写双层循环
来源：http://hz.hongshengwenyu.top/gtcwgslvrl.html

Ruby: nested.flatten
来源：http://hz.sweek.top/gtmfefxvst.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.cucudq.cn/gtmojpkeiq.html

[D19] 按字段分组
来源：http://hz.yj20258.top/gtdtmodpoy.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.chenlongwang.top/gtzugsinam.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.jinqigufen.top/gtldflqutu.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.gaohongyu789.top/gtmreicoes.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.jinqigufen.top/gtvwtecpdj.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.yangfankeji.com/gtomtkksmc.html

Go:   // 手写 map[string][]T
来源：http://hz.ehwqpu.com/gtynqahlty.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.guannengcc.top/gtsrjlosar.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.cdnleiting.top/gtdzprakrc.html

[D20] 统计每个元素出现次数
来源：http://hz.hnxiangtu.top/gtbjaaznzo.html

Py:   Counter(arr)
来源：http://hz.fzhhl.top/gtlxgpzbiz.html

PHP:  array_count_values($arr);
来源：http://hz.chenjidiqi.icu/gtgqbonfzd.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.sufxvd.cn/gtufuwcrgs.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.nanxuanxn.top/gtaimougjb.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.jlsjyb.cn/gtuuqrtxrm.html

Go:   // 手写 map[T]int
来源：http://hz.52xcode.cn/gtdipkdbhh.html

Ruby: arr.tally
来源：http://hz.jiagoushi.top/gtybflvlca.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.nwbrower.top/gtkisrqxmc.html

[D21] 判断是否包含某元素
来源：http://hz.sxryk.cn/gtyffhsrve.html

Py:   x in arr
来源：http://hz.xziqi.cn/gtlchikija.html

PHP:  in_array($x, $arr, true);
来源：http://hz.cqqwz.cn/gtgyrydrnr.html

JS:   arr.includes(x)
来源：http://hz.hnxiangtu.top/gtkzggzytm.html

TS:   arr.includes(x)
来源：http://hz.svipenyu.cn/gtdfvgqmha.html

Java: list.contains(x)
来源：http://hz.xingfuxueyuan.xyz/gtekzfljkm.html

Go:   slices.Contains(arr, x)
来源：http://hz.guowangkeji.top/gtgqbhgwkd.html

Ruby: arr.include?(x)
来源：http://hz.snrcjt.cn/gtjjhtnjct.html

C#:   list.Contains(x)
来源：http://hz.aizwys.cn/gtncqokhos.html

[D22] 复制数组（避免共享引用）
来源：http://hz.zhijiandao.cn/gtahcvolkn.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.hnqzz.top/gtjugzaxhf.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.sweek.top/gtbehzbbmv.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.gotoacloud.top/gtrhqkdxaa.html

TS:   [...arr];
来源：http://hz.aibaodan.cn/gtvfqihwyp.html

Java: new ArrayList<>(list);
来源：http://hz.guowangkeji.top/gtyarycyke.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.yj202588.top/gtzifztdpz.html

Ruby: arr.dup;  arr.clone
来源：http://hz.yj20258.top/gtzxjhuhsb.html

C#:   new List<int>(list);
来源：http://hz.sufxvd.cn/gtldishodk.html

[D23] reduce 累积计算
来源：http://hz.fengsongda.top/gtwkdygvve.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.xuetiantiany.cn/gtvqghqpce.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.shzxlz.cn/gttwdmsvwx.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.gogol.net.cn/gtcgorzclb.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yvedp.cn/gtzpuvqthc.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.shanyushiyangkeji.top/gtrcjtsghs.html

Go:   // 手写循环
来源：http://hz.sweek.top/gttjsrgwsv.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.hfpthk.cn/gtzbfxxqta.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.jqgufenzy.top/gtgbxbpsuf.html

[D24] 字典 / Map 基本操作
来源：http://hz.xylfe.cn/gtyiezjvxj.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.sweek.top/gtlfyfpgsu.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.hnqzz.top/gttaqazrpo.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.hammf.cn/gtyidvrwbb.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.nanxinkj.top/gtwevwevgb.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.snrcjt.cn/gtskruiqrx.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.kuanghao11.cn/gtdirdhzay.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.haohaochexian.top/gtcnfqvbwj.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.dianchejie.cn/gthknovurh.html

[D25] Set 集合去重与交并差
来源：http://hz.hywenlv.cn/gtkvprqhus.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.xuetiantiany.cn/gtntnvtyvz.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.tanke756.top/gtkrwimqzc.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.feifeiyinyue.top/gthrojbyxm.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.birdmap.top/gtuyjlzdib.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.guannengcc.top/gtnciufmid.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.mhx1999.top/gthdfceusm.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.tian-w.cn/gtloysbpbr.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.yangfankeji.com/gtrbznozys.html

[D26] 数组转字符串
来源：http://hz.jinyuanbaomall.cn/gtrvheypqq.html

Py:   ", ".join(map(str, arr))
来源：http://hz.yj20258.top/gtvjhtcbgc.html

PHP:  implode(", ", $arr);
来源：http://hz.gaohongyu789.top/gtwufmjxsu.html

JS:   arr.join(", ")
来源：http://hz.cdnleiting.top/gtlycthlns.html

TS:   arr.join(", ")
来源：http://hz.xingfuxueyuan.xyz/gtonukueol.html

Java: String.join(", ", list)
来源：http://hz.ivvv.top/gtgqdaogbm.html

Go:   strings.Join(strs, ", ")
来源：http://hz.feifeiyinyue.top/gtitzkfyqr.html

Ruby: arr.join(", ")
来源：http://hz.birdmap.top/gtldqduwus.html

C#:   string.Join(", ", list)
来源：http://hz.chenjidiqi.icu/gtgmnhuffc.html

================================================================================
来源：http://hz.hywenlv.cn/gtzpevfwac.html

E. 字符串处理
来源：http://hz.zhongyouzk.top/gtstpozbjm.html

================================================================================
来源：http://hz.cashguo.top/gtyaxkndjz.html

[E01] 拼接字符串
来源：http://hz.jianghu66.top/gtfqzgtqft.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.meibo888.top/gtzybivhhk.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.shuidangran.top/gtuukliamx.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.tanke756.top/gtzxevwcxl.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.cheryme.top/gtvqdemijv.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.meibo888.top/gtyhfxnjnh.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.xylfe.cn/gtxnpdcnre.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.yj20258.top/gtlabfkekf.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.gotoacloud.top/gtyuyddwzx.html

[E02] 重复字符串
来源：http://hz.birdmap.top/gtttsylmqd.html

Py:   "ab" * 3
来源：http://hz.yj20258888.top/gtfjdrrhmq.html

PHP:  str_repeat("ab", 3);
来源：http://hz.cashguo.top/gtnzcuhuzc.html

JS:   "ab".repeat(3)
来源：http://hz.zhengqikj.top/gtjootlgep.html

TS:   "ab".repeat(3)
来源：http://hz.meibo888.top/gtdsfyndcj.html

Java: "ab".repeat(3)
来源：http://hz.jlsjyb.cn/gttbtjgfkn.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.nwbrower.top/gtxhcyfory.html

Ruby: "ab" * 3
来源：http://hz.yvedp.cn/gtctsivgne.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.pengpengdd.cyou/gthtqmunii.html

[E03] 截取子串
来源：http://hz.yangfankeji.com/gttzmdadne.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.nanxuanxn.top/gtmndmljxj.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.xuetiantiany.cn/gtpoqkwopc.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.ywan-chungtsiang.top/gtvcaekubg.html

TS:   s.slice(1, 4)
来源：http://hz.52xcode.cn/gtyuhjlwzf.html

Java: s.substring(1, 4)
来源：http://hz.tanke756.top/gtniimrkji.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.cqqwz.cn/gtknghgibc.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.cheryme.top/gtduqsdnjv.html

C#:   s.Substring(1, 3)
来源：http://hz.ydzc1.top/gtkjaffsen.html

[E04] 查找子串位置
来源：http://hz.gogol.net.cn/gtailchfsh.html

Py:   s.find("x");  s.index("x")
来源：http://hz.hammf.cn/gthjtwexzw.html

PHP:  strpos($s, "x");
来源：http://hz.yangfankeji.com/gtkvwmkppv.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.jianghu66.top/gtzspjitft.html

TS:   s.indexOf("x")
来源：http://hz.fzhhl.top/gtpenrdvrc.html

Java: s.indexOf("x")
来源：http://hz.hnqzz.top/gtjjhixmum.html

Go:   strings.Index(s, "x")
来源：http://hz.fengsongda.top/gtzdziwfnx.html

Ruby: s.index("x")
来源：http://hz.zhongyouzk.top/gtumhiskzw.html

C#:   s.IndexOf("x")
来源：http://hz.ivvv.top/gtycyhrkoj.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.haohaochexian.top/gtiwegkpfv.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.sweek.top/gtqaphsdzg.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.jinyuanbaomall.cn/gtgensnfbl.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.jiagoushi.top/gtpwbtsrcl.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.pycfn.com/gtpwgxpzej.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.yj202588.top/gtpgeezkjt.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.jinyuanbaomall.cn/gtozhiubex.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.aizwys.cn/gtsyoqqtyq.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.jlsjyb.cn/gthhobtals.html

[E06] 替换子串
来源：http://hz.sxryk.cn/gtuivppawk.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.jinqigufen.top/gtwbyldnls.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.redwolf501.top/gtxgosrdjf.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.iojbl.cn/gtulvvciiq.html

TS:   s.replaceAll("a", "b")
来源：http://hz.xingfuxueyuan.xyz/gtxvirrlnw.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.bjfxy.top/gtgeugimgx.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.iojbl.cn/gtjadpmxwo.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.guowangkeji.top/gtinglpalh.html

C#:   s.Replace("a", "b")
来源：http://hz.dashuyun.cn/gthtengsuj.html

[E07] 按分隔符拆分
来源：http://hz.xylfe.cn/gtszrfeyrz.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.zhoulong.xyz/gtbdgkdiax.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.zhijiandao.cn/gtrptiksij.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.jianghu66.top/gtvufgxyty.html

TS:   s.split(",")
来源：http://hz.xziqi.cn/gtljgwrhrq.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.pengpengdd.cyou/gtatckgixk.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.xziqi.cn/gtvtpqgpvu.html

Ruby: s.split(",");  s.split
来源：http://hz.nanxuanxn.top/gtcsocficz.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.nwbrower.top/gtulbshzfq.html

[E08] 数组按分隔符合并
来源：http://hz.yangfankeji.com/gtzxkwsqdq.html

Py:   ",".join(items)
来源：http://hz.zhixingplan.top/gtaqxfgwsk.html

PHP:  implode(",", $items);
来源：http://hz.guannengcc.top/gtkhczrrly.html

JS:   items.join(",")
来源：http://hz.yonumen.top/gtjmfejnjj.html

TS:   items.join(",")
来源：http://hz.gzhubu.top/gtkzchljxk.html

Java: String.join(",", items)
来源：http://hz.shanyushiyangkeji.top/gtjoasqnzp.html

Go:   strings.Join(items, ",")
来源：http://hz.guannengcc.top/gtoxduynpz.html

Ruby: items.join(",")
来源：http://hz.316326.xyz/gtylgzrmgg.html

C#:   string.Join(",", items)
来源：http://hz.sweek.top/gtyelaxqwd.html

[E09] 去除所有空白字符
来源：http://hz.zhixingplan.top/gtsxflvkad.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.jyoumei.cn/gtzdyeytjr.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.jqgufenzy.top/gtxpvmjjli.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.jqgfzy.top/gtppjuvyyk.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.yanxiufei.cn/gtxjuqgghh.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.iojbl.cn/gtxmhtnmro.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.jqgfzy.top/gtxqsbokqw.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.cqqwz.cn/gtdutjdpjd.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.cheryme.top/gtinugjtzo.html

[E10] 左侧补零 / 定长填充
来源：http://hz.shangyingyoupin.top/gtsqswrwef.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.hywenlv.cn/gtdgtmvimq.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.quarkkingdee.top/gtykgzvart.html

JS:   "7".padStart(3, "0")
来源：http://hz.zhixingplan.top/gtuwwzlvoj.html

TS:   "7".padStart(3, "0")
来源：http://hz.c1oappe.top/gtbqgrkkgw.html

Java: String.format("%03d", 7)
来源：http://hz.hnqzz.top/gtangujowi.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.svipenyu.cn/gtkmejabez.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.gogol.net.cn/gtbdyfslfb.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.jqgufenzy.top/gtsunusrkf.html

[E11] 反转字符串
来源：http://hz.shanyushiyangtech.top/gtzgupewks.html

Py:   s[::-1]
来源：http://hz.hywenlv.cn/gtbrrghfnu.html

PHP:  strrev($s);
来源：http://hz.52xcode.cn/gtujmocvxh.html

JS:   [...s].reverse().join("")
来源：http://hz.sxryk.cn/gtwyfreqrw.html

TS:   [...s].reverse().join("")
来源：http://hz.svipenyu.cn/gtsccahydt.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.zhongyouzk.top/gtoohlbmvh.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.nanxuanxn.top/gtrxclpgon.html

Ruby: s.reverse
来源：http://hz.zhongyouzk.top/gtctndovuu.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.jinghuilouyu.cn/gtlbylezkv.html

[E12] 统计某字符出现次数
来源：http://hz.tanke756.top/gtockaokdg.html

Py:   s.count("a")
来源：http://hz.hnxiangtu.top/gttgirnxqv.html

PHP:  substr_count($s, "a");
来源：http://hz.jqgufenzy.top/gthiiebohe.html

JS:   s.split("a").length - 1
来源：http://hz.guannengcc.top/gtwmbrnpac.html

TS:   s.split("a").length - 1
来源：http://hz.birdmap.top/gtdrnvnzdo.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.yonumen.top/gtgldhyomv.html

Go:   strings.Count(s, "a")
来源：http://hz.feifeiyinyue.top/gthtbfhjiz.html

Ruby: s.count("a")
来源：http://hz.tianlin.xyz/gtumosheve.html

C#:   s.Count(c => c == 'a')
来源：http://hz.yuanzhike.top/gtjadobqyx.html

[E13] 逐字符遍历
来源：http://hz.yj20258888.top/gtikpumrnf.html

Py:   for ch in s: print(ch)
来源：http://hz.zhijiandao.cn/gtvwvyweqi.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.ywan-chungtsiang.top/gtoibwgqdy.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.cdnleiting.top/gtjhlrtcii.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.svipenyu.cn/gtkzfifjqp.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.kuanghao11.cn/gtdpcfwreo.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.hywenlv.cn/gtmqxuyfgx.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.havefunace.top/gtajjkjsfh.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.quarkkingdee.top/gttevfhuoj.html

[E14] URL 编码与 Base64
来源：http://hz.gotoacloud.top/gtrnteldek.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.xuanzx.com/gtaimpfycy.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.jinyuanbaomall.cn/gtkxumriar.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.chenlongwang.top/gtixlrtqln.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.birdmap.top/gtidjnpwaw.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.ywan-chungtsiang.top/gtibinginl.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.jinyuanbaomall.cn/gtlryfytqs.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.yj20258.top/gtgywovgju.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.yuanzhike.top/gtuvxjfjdx.html

[E15] HTML 转义 / 反转义
来源：http://hz.hysaishi.cn/gtbmsfggll.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.sxryk.cn/gtjzrtqogx.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.redwolf501.top/gtxaduvjft.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.zhixingplan.top/gtiserstbc.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.jqgufenzy.top/gtscbvvbei.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.hnqzz.top/gtcwkknrvu.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.iojbl.cn/gtqjcvnuxh.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.ydzc1.top/gtqaiilwow.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.nwbrower.top/gtoahkhpzc.html

[E16] 数字千分位
来源：http://hz.redwolf501.top/gthiekardy.html

Py:   f"{1234567:,}"
来源：http://hz.hongshengwenyu.top/gtscgyabgu.html

PHP:  number_format(1234567);
来源：http://hz.zhengqikj.top/gtusqixfvh.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.xuanzx.com/gtqnqcmptx.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.zhiwuduotai.top/gtbiqaycdb.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.tanke756.top/gtkbtirxcx.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.ivvv.top/gteadwohtb.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.tian-w.cn/gtozgckvku.html

C#:   1234567.ToString("N0")
来源：http://hz.jyoumei.cn/gtncldegbf.html

[E17] 首字母大写
来源：http://hz.jianghu66.top/gtknuclmgc.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.yuanzhike.top/gtcaoomsqe.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.yangfankeji.com/gtxqrwyceo.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.ywan-chungtsiang.top/gtznrnhqgf.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.birdmap.top/gtvpsanddh.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.cucudq.cn/gtutanvqhh.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.hywenlv.cn/gtkvfhvpzv.html

Ruby: s.capitalize
来源：http://hz.tanke756.top/gtwlcbfraa.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.jinyuanbaomall.cn/gtnbjryidd.html

[E18] 模板占位符替换
来源：http://hz.yonumen.top/gtyxojadig.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.hnqzz.top/gtnhoboyva.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.tian-w.cn/gtnwudrlsr.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.yonumen.top/gtrnwkrkrw.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.yuxming.cn/gtzhhhcapa.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.xylfe.cn/gtlrnvohkq.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.cdnleiting.top/gtyszmfgvd.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.xuetiantiany.cn/gtqyachkus.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.aibaodan.cn/gthpzbydix.html

[E19] 多行文本按行拆分
来源：http://hz.dashuyun.cn/gtonspnsgg.html

Py:   s.splitlines()
来源：http://hz.xziqi.cn/gtowcdfcbh.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.ydzc1.top/gttmrgxhdz.html

JS:   s.split(/\r?\n/)
来源：http://hz.xylfe.cn/gtrpvyqtmc.html

TS:   s.split(/\r?\n/)
来源：http://hz.chenjidiqi.icu/gtlgasnqkt.html

Java: s.lines().toList()
来源：http://hz.quarkkingdee.top/gtjsegywsv.html

Go:   strings.Split(s, "\n")
来源：http://hz.shanyushiyangtech.top/gtctzvrnsn.html

Ruby: s.lines
来源：http://hz.guowangkeji.top/gtaqakruyc.html

C#:   s.Split('\n')
来源：http://hz.yj20258.top/gttlzjnbaf.html

[E20] 判断字符串是否为空
来源：http://hz.xylfe.cn/gtucuqmndi.html

Py:   if not s:
来源：http://hz.c1oappe.top/gtfnnupniz.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.cqqwz.cn/gtivimfzsl.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.sweek.top/gtwazuhvjw.html

TS:   if (s === "") {}
来源：http://hz.zhoulong.xyz/gtmcnaswvt.html

Java: if (s.isEmpty()) {}
来源：http://hz.cucudq.cn/gtrtasotic.html

Go:   if s == "" {}
来源：http://hz.fengsongda.top/gtvvyvngbn.html

Ruby: if s.empty?
来源：http://hz.sweek.top/gthfxalwws.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.ehwqpu.com/gtonpgecgl.html

[E21] 超长截断加省略号
来源：http://hz.snrcjt.cn/gtcuxhcmkf.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.yj20258.top/gtheuprqva.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.ybcxt.top/gtvrbyiwqw.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.zhoulong.xyz/gtrmwwsbzb.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.sweek.top/gttfipooyh.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.jinyuanbaomall.cn/gtpfwyofsx.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.nwbrower.top/gtdgjofnnx.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.gzhubu.top/gtsvnhptdv.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.ppjwa.cn/gtidltvazc.html

[E22] 字节长度与字符长度
来源：http://hz.andypj.xyz/gtjxjxdkdb.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.shanyushiyangtech.top/gtmqaedczn.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.tian-w.cn/gtlxfomgak.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.wangshuangyany.cn/gtgrtvxhke.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.redwolf501.top/gtbwcvhjvp.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.tanke756.top/gtzevyahwl.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.quarkkingdee.top/gtazyvpplk.html

Ruby: s.bytesize;  s.length
来源：http://hz.shangyingyoupin.top/gtytzkjazv.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.iojbl.cn/gtrqmkkjkx.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtwaugprwy.html

F. 文件与目录
来源：http://hz.ybcxt.top/gtadtwrmxq.html

================================================================================
来源：http://hz.jqgfzy.top/gtjmwwxofj.html

[F01] 读取整个文件
来源：http://hz.cucudq.cn/gttmgydpfd.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.aizwys.cn/gtwabpmejj.html

PHP:  file_get_contents("a.txt");
来源：http://hz.zhoulong.xyz/gtfcrnlukj.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.wangdashe.top/gtduusgxjv.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.hnqzz.top/gtcsijzmak.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.hnxiangtu.top/gtzocowalw.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.quarkkingdee.top/gtysgkvskp.html

Ruby: File.read("a.txt")
来源：http://hz.yj20258.top/gtnazubfcr.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.hfpthk.cn/gtwlconbqi.html

[F02] 逐行读取文件
来源：http://hz.xziqi.cn/gtrlgyjxvk.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.vqdsnc.cn/gtjnheadje.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.ehwqpu.com/gtmhqnvtqc.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.xylfe.cn/gtmewbjioi.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.xylfe.cn/gtoacsypfb.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.guannengcc.top/gtuwpsmiym.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.kuanghao11.cn/gthjyerbge.html


<!-- 参考信息 -->