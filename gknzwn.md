代发 wailian999

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.zhiwuduotai.top/gtcdatyzck.html

Go:   // 手写双层循环
来源：http://hz.aibaodan.cn/gtztzhxilu.html

Ruby: nested.flatten
来源：http://hz.ehwqpu.com/gtbokznemd.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.iojbl.cn/gtflbfzgdq.html

[D19] 按字段分组
来源：http://hz.sysykeji.top/gtumclswcr.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.hywenlv.cn/gtxcifocfp.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.hnxiangtu.top/gtukliuuyb.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.fzhhl.top/gtpukbffeb.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.chenjidiqi.icu/gtlhdmppjx.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.redwolf501.top/gtlscvkpjw.html

Go:   // 手写 map[string][]T
来源：http://hz.shangyingyoupin.top/gtczdjizre.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.shuidangran.top/gtamhuupyq.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.yj20258.top/gttdecofha.html

[D20] 统计每个元素出现次数
来源：http://hz.jinqigfzy.top/gtaileftfa.html

Py:   Counter(arr)
来源：http://hz.zhoulong.xyz/gtgaqkorzg.html

PHP:  array_count_values($arr);
来源：http://hz.snrcjt.cn/gtnupynire.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.yanxiufei.cn/gtgiztobxn.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.ydjk.org.cn/gtwcbdjhfc.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.yangfankeji.com/gtcxvitmof.html

Go:   // 手写 map[T]int
来源：http://hz.ehwqpu.com/gtajnynukb.html

Ruby: arr.tally
来源：http://hz.shangyingyoupin.top/gtczsdmxbs.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.0kj1m.cn/gtyzbhtcba.html

[D21] 判断是否包含某元素
来源：http://hz.yj20258.top/gtbwoybery.html

Py:   x in arr
来源：http://hz.xziqi.cn/gtepfkgsia.html

PHP:  in_array($x, $arr, true);
来源：http://hz.tianlin.xyz/gtqedpiwkt.html

JS:   arr.includes(x)
来源：http://hz.yanxiufei.cn/gtfenoyjyv.html

TS:   arr.includes(x)
来源：http://hz.sufxvd.cn/gtxkddydtw.html

Java: list.contains(x)
来源：http://hz.nanxuanxn.top/gtwpjzebjv.html

Go:   slices.Contains(arr, x)
来源：http://hz.0kj1m.cn/gteoqpmrzh.html

Ruby: arr.include?(x)
来源：http://hz.kuanghao11.cn/gtxkvxyzat.html

C#:   list.Contains(x)
来源：http://hz.haohaochexian.top/gtwnfgovwh.html

[D22] 复制数组（避免共享引用）
来源：http://hz.yueranfly.top/gtdrurahgo.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.dianchejie.cn/gtxdmvhyqh.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.zhiwuduotai.top/gtaojztods.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.sweek.top/gtoxgpizsf.html

TS:   [...arr];
来源：http://hz.daria6918.cn/gtzrsetmdh.html

Java: new ArrayList<>(list);
来源：http://hz.tianlin.xyz/gtqgzclhyf.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.kuanghao11.cn/gtgvvkcycl.html

Ruby: arr.dup;  arr.clone
来源：http://hz.aibaodan.cn/gtqpjrtqac.html

C#:   new List<int>(list);
来源：http://hz.gzhubu.top/gtpbuegbor.html

[D23] reduce 累积计算
来源：http://hz.xuanzx.com/gtfdsajjbz.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.yuanzhike.top/gtpvzzhrhp.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.cucudq.cn/gtjgsoxuvy.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.svipenyu.cn/gtttjlhodn.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.hnxiangtu.top/gtbkitlyko.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.sweek.top/gtiodhtmcv.html

Go:   // 手写循环
来源：http://hz.yueranfly.top/gtgrlpyora.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.gzhubu.top/gtdumovajh.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.hnxiangtu.top/gtgemjhwpk.html

[D24] 字典 / Map 基本操作
来源：http://hz.jyoumei.cn/gtyanulevg.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.vqdsnc.cn/gtwwqsbowv.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.sxryk.cn/gtzssakmws.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.xinyue.icu/gtuflbvnwh.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.yj20258888.top/gtdgobzvon.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.xuanzx.com/gtejgvponk.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.cashguo.top/gtkszdknjf.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.xziqi.cn/gthhlznevk.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.xingfuxueyuan.xyz/gtxwegrbvg.html

[D25] Set 集合去重与交并差
来源：http://hz.hysaishi.cn/gtlqrrqukz.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.ppjwa.cn/gtjdryzgoc.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.jqgufenzy.top/gtkshlpycj.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.quarkkingdee.top/gtpylhlkvv.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.shangyingyoupin.top/gtctrsemwo.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.zhoulong.xyz/gtvudixfyj.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.cqqwz.cn/gtyxvbztwn.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.9152youxi.cn/gtskazwckx.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.shangyingyoupin.top/gtioxbhkxa.html

[D26] 数组转字符串
来源：http://hz.hysaishi.cn/gtumvgjxlb.html

Py:   ", ".join(map(str, arr))
来源：http://hz.jqgufenzy.top/gtqgcmmbla.html

PHP:  implode(", ", $arr);
来源：http://hz.zdqjudy.top/gtclfjvmxz.html

JS:   arr.join(", ")
来源：http://hz.birdmap.top/gtledkvnzi.html

TS:   arr.join(", ")
来源：http://hz.chenjidiqi.icu/gtrdbyvejk.html

Java: String.join(", ", list)
来源：http://hz.yanxiufei.cn/gtqvltkbll.html

Go:   strings.Join(strs, ", ")
来源：http://hz.316326.xyz/gttjjrvsgs.html

Ruby: arr.join(", ")
来源：http://hz.hysaishi.cn/gtxcwiosnd.html

C#:   string.Join(", ", list)
来源：http://hz.ywan-chungtsiang.top/gtavkbjepw.html

================================================================================
来源：http://hz.wangdashe.top/gtcnlgyeva.html

E. 字符串处理
来源：http://hz.snrcjt.cn/gtryezfoex.html

================================================================================
来源：http://hz.xinyue.icu/gtwrkeigtx.html

[E01] 拼接字符串
来源：http://hz.dianchejie.cn/gtwimrrqxq.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.fzhhl.top/gtsxkajnom.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.yonumen.top/gtqymeedsw.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.ybcxt.top/gtfkathqfe.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.nanxinkj.top/gtnuobepvs.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.cdnleiting.top/gtukzfzazc.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.daxiang520.top/gtlexujlvh.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.yongpay.top/gtospbaoms.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.zdqjudy.top/gtnrzodaoi.html

[E02] 重复字符串
来源：http://hz.jinyuanbaomall.cn/gtfbocyjll.html

Py:   "ab" * 3
来源：http://hz.shzxlz.cn/gtgjoenqsn.html

PHP:  str_repeat("ab", 3);
来源：http://hz.c1oappe.top/gtlapaurug.html

JS:   "ab".repeat(3)
来源：http://hz.sufxvd.cn/gtjwjxoonq.html

TS:   "ab".repeat(3)
来源：http://hz.jinqigfzy.top/gtuweplsbn.html

Java: "ab".repeat(3)
来源：http://hz.hfpthk.cn/gtnmhmfhbz.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.jlsjyb.cn/gtnjyzuykg.html

Ruby: "ab" * 3
来源：http://hz.jiagoushi.top/gtsyjjyfpm.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.hongshengwenyu.top/gtyfmpwyiz.html

[E03] 截取子串
来源：http://hz.smart0.xyz/gthfyucayp.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.yangfankeji.com/gtuwvzockl.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.cheryme.top/gtlfujcine.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.chenzaomai.com/gteazrpmnk.html

TS:   s.slice(1, 4)
来源：http://hz.haohaochexian.top/gtlsvblcaj.html

Java: s.substring(1, 4)
来源：http://hz.zhixingplan.top/gtmelniwxd.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.sxryk.cn/gtxfvdnyrv.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.hywenlv.cn/gtaotonymi.html

C#:   s.Substring(1, 3)
来源：http://hz.jyoumei.cn/gtplbvjdvo.html

[E04] 查找子串位置
来源：http://hz.hnxiangtu.top/gtallvbgpw.html

Py:   s.find("x");  s.index("x")
来源：http://hz.nanxinkj.top/gtuwkxkjnf.html

PHP:  strpos($s, "x");
来源：http://hz.pycfn.com/gtnykadylw.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.shanyushiyangkeji.top/gthwvflclf.html

TS:   s.indexOf("x")
来源：http://hz.andypj.xyz/gtdwstitdp.html

Java: s.indexOf("x")
来源：http://hz.gzhubu.top/gtxlelsdfj.html

Go:   strings.Index(s, "x")
来源：http://hz.wangdashe.top/gtdapfltsx.html

Ruby: s.index("x")
来源：http://hz.0kj1m.cn/gtykwuoxcw.html

C#:   s.IndexOf("x")
来源：http://hz.dashuyun.cn/gtlkhmtabz.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.9152youxi.cn/gtviwedwyp.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.smart0.xyz/gtmxtkkvdj.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.vqdsnc.cn/gtqvzdgjqi.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.jinghuilouyu.cn/gtditycnjj.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.chenjidiqi.icu/gtgbitvrux.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.jinqigfzy.top/gtzfbbtmnr.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.zhongyouzk.top/gtnrsnqlfo.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.smart0.xyz/gtqdsxtzpj.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.feifeiyinyue.top/gtvfnkqbqx.html

[E06] 替换子串
来源：http://hz.yuxming.cn/gtmphcprpb.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.yj202588.top/gtexywmikn.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.iojbl.cn/gtrqcryrup.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.yj202588.top/gtqcljmtrj.html

TS:   s.replaceAll("a", "b")
来源：http://hz.jinqigufen.top/gtkcpezcvq.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.haohaochexian.top/gtiwyzoxyz.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.sysykeji.top/gtmtcxebyu.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.xuanzx.com/gtutgdrqxf.html

C#:   s.Replace("a", "b")
来源：http://hz.birdmap.top/gtemodbrra.html

[E07] 按分隔符拆分
来源：http://hz.yonumen.top/gtriqqryif.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.9152youxi.cn/gtjpbgoevs.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.fzhhl.top/gtorvepkwq.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.gotoacloud.top/gtqiicsnsa.html

TS:   s.split(",")
来源：http://hz.zhaomingkeji.xyz/gtmnjhtqzo.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.yonumen.top/gtkzppyeas.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.zhengqikj.top/gtmakffmzx.html

Ruby: s.split(",");  s.split
来源：http://hz.shangyingyoupin.top/gtbobhklso.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.zhoulong.xyz/gtmddqgols.html

[E08] 数组按分隔符合并
来源：http://hz.jqgufenzy.top/gttxomjghr.html

Py:   ",".join(items)
来源：http://hz.tian-w.cn/gtzzkkpcgc.html

PHP:  implode(",", $items);
来源：http://hz.shanyushiyangtech.top/gtvkwljxhd.html

JS:   items.join(",")
来源：http://hz.zhijiandao.cn/gtbzytqgpl.html

TS:   items.join(",")
来源：http://hz.cucudq.cn/gtujgymcbe.html

Java: String.join(",", items)
来源：http://hz.jiagoushi.top/gtmaamoxfi.html

Go:   strings.Join(items, ",")
来源：http://hz.jyoumei.cn/gtjuflynyx.html

Ruby: items.join(",")
来源：http://hz.dashuyun.cn/gtyumksjzb.html

C#:   string.Join(",", items)
来源：http://hz.yj20258.top/gtwitbrkyp.html

[E09] 去除所有空白字符
来源：http://hz.shanyushiyangtech.top/gtnjxulhra.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.shanyushiyangkeji.top/gtodftbahi.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.pengpengdd.cyou/gtncbrfrvr.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.smart0.xyz/gtkcjzgkco.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.jinyuanbaomall.cn/gtunijgsjo.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.zhijiandao.cn/gtvayidihw.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.shzxlz.cn/gtruaujatb.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.wangdashe.top/gtbpzyywdk.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.tanke756.top/gtqwjzsxzx.html

[E10] 左侧补零 / 定长填充
来源：http://hz.guowangkeji.top/gtmutkjssk.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.tanke756.top/gtwgjuuvkg.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.jlsjyb.cn/gtahoqqwta.html

JS:   "7".padStart(3, "0")
来源：http://hz.nanxuanxn.top/gthktmyjjz.html

TS:   "7".padStart(3, "0")
来源：http://hz.yuanzhike.top/gtddfmsote.html

Java: String.format("%03d", 7)
来源：http://hz.shuidangran.top/gtgwakazyo.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.guowangkeji.top/gtdeslhscx.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.iojbl.cn/gthjpqbkrr.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.zhengqikj.top/gtmnvzzkuw.html

[E11] 反转字符串
来源：http://hz.quarkkingdee.top/gteactrfmi.html

Py:   s[::-1]
来源：http://hz.cucudq.cn/gtekyoixvl.html

PHP:  strrev($s);
来源：http://hz.ppjwa.cn/gtmxpkvurj.html

JS:   [...s].reverse().join("")
来源：http://hz.jinqigufen.top/gtpwnvloyg.html

TS:   [...s].reverse().join("")
来源：http://hz.redwolf501.top/gtbazijkcf.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.jqgufenzy.top/gteqlblsxg.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.meibo888.top/gtnbxrjxla.html

Ruby: s.reverse
来源：http://hz.zhijiandao.cn/gthcccfnua.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.xuanzx.com/gtbhegumqp.html

[E12] 统计某字符出现次数
来源：http://hz.yvedp.cn/gtirsmsezq.html

Py:   s.count("a")
来源：http://hz.ywan-chungtsiang.top/gtvdfpnbvg.html

PHP:  substr_count($s, "a");
来源：http://hz.zhiwuduotai.top/gthfitvrmu.html

JS:   s.split("a").length - 1
来源：http://hz.mhx1999.top/gtkwleamte.html

TS:   s.split("a").length - 1
来源：http://hz.shuidangran.top/gtebizffgg.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.xinyue.icu/gtjeduizvg.html

Go:   strings.Count(s, "a")
来源：http://hz.cashguo.top/gtjchxiowx.html

Ruby: s.count("a")
来源：http://hz.xuetiantiany.cn/gtaclgycsu.html

C#:   s.Count(c => c == 'a')
来源：http://hz.gaohongyu789.top/gtssqbpcxv.html

[E13] 逐字符遍历
来源：http://hz.pycfn.com/gtrxbraten.html

Py:   for ch in s: print(ch)
来源：http://hz.redwolf501.top/gtjdsrnbgv.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.hammf.cn/gtruvqccec.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.hammf.cn/gtcdqalqpp.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yanxiufei.cn/gthnihccja.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.hnqzz.top/gtwxgqmeeo.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.shangyingyoupin.top/gtpycmdmzs.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.jinyuanbaomall.cn/gtaofhdomn.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.jqgufenzy.top/gtklftvqhj.html

[E14] URL 编码与 Base64
来源：http://hz.cheryme.top/gtuktjapyc.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.jinghuilouyu.cn/gtisgywozw.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.sweek.top/gtykaynzhn.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.yanxiufei.cn/gtmjkwdipe.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.daxiang520.top/gtbneaunoh.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.jqgfzy.top/gthavojiee.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.pycfn.com/gtqcnsysae.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.nanxinkj.top/gtyqfgihfn.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.yangfankeji.com/gtncnnutrf.html

[E15] HTML 转义 / 反转义
来源：http://hz.ydjk.org.cn/gtvvjpmdlz.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.jqgfzy.top/gtvszdlalb.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.redwolf501.top/gtdqfbtnbs.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.shanyushiyangtech.top/gtutbmxlth.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.xylfe.cn/gtnymlczfq.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.daria6918.cn/gtliljltry.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.yuxming.cn/gtkyphjslv.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.hammf.cn/gtxuumqtvv.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.feifeiyinyue.top/gtjsfnkzku.html

[E16] 数字千分位
来源：http://hz.shangyingyoupin.top/gtwjyzulhu.html

Py:   f"{1234567:,}"
来源：http://hz.gotoacloud.top/gtpkqeifpk.html

PHP:  number_format(1234567);
来源：http://hz.pengpengdd.cyou/gtofgrocbn.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.havefunace.top/gtvktkygtg.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.svipenyu.cn/gtueqvxlnj.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.ydjk.org.cn/gtquiqddar.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.nanxuanxn.top/gtsvaycqqk.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.zycfv.cn/gtwdgmhjzq.html

C#:   1234567.ToString("N0")
来源：http://hz.shangyingyoupin.top/gtuogkpvgk.html

[E17] 首字母大写
来源：http://hz.zhengqikj.top/gtycilzahr.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.dashuyun.cn/gtbfshfirh.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.guowangkeji.top/gtsoslguxz.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.feifeiyinyue.top/gtwakakzul.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.hongshengwenyu.top/gteeghiqfn.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.shanyushiyangkeji.top/gtlfunnxfp.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.iojbl.cn/gtekqdjksw.html

Ruby: s.capitalize
来源：http://hz.dianchejie.cn/gtiynprqqp.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.hongshengwenyu.top/gtlzedkems.html

[E18] 模板占位符替换
来源：http://hz.gotoacloud.top/gtiqdlxxbb.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.cucudq.cn/gtsdlkfcuj.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.gaohongyu789.top/gtxmfofuji.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.shangyingyoupin.top/gtyhrrxjkw.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.yueranfly.top/gtdxaxpmnr.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.nanxinkj.top/gtnmttpnsd.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.jinqigfzy.top/gtsanldngb.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.316326.xyz/gtjyzchdas.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.ydjk.org.cn/gtklppbvou.html

[E19] 多行文本按行拆分
来源：http://hz.gogol.net.cn/gtsfdoeome.html

Py:   s.splitlines()
来源：http://hz.snrcjt.cn/gtfaygffyg.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.xuanzx.com/gtefpojbkj.html

JS:   s.split(/\r?\n/)
来源：http://hz.hnxiangtu.top/gtbgimrsnw.html

TS:   s.split(/\r?\n/)
来源：http://hz.meibo888.top/gtqdlxcwxm.html

Java: s.lines().toList()
来源：http://hz.xingfuxueyuan.xyz/gtnihhvlal.html

Go:   strings.Split(s, "\n")
来源：http://hz.svipenyu.cn/gthxcktssn.html

Ruby: s.lines
来源：http://hz.bjfxy.top/gtqeiiyqoy.html

C#:   s.Split('\n')
来源：http://hz.ppjwa.cn/gtoiemrxtn.html

[E20] 判断字符串是否为空
来源：http://hz.xinyue.icu/gtowbcjivg.html

Py:   if not s:
来源：http://hz.redwolf501.top/gtjpsjoiuh.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.xuanzx.com/gtmznohbap.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.svipenyu.cn/gtfbkavves.html

TS:   if (s === "") {}
来源：http://hz.snrcjt.cn/gtnajoyarb.html

Java: if (s.isEmpty()) {}
来源：http://hz.sysykeji.top/gtzoxjhrom.html

Go:   if s == "" {}
来源：http://hz.9152youxi.cn/gthvvskcyy.html

Ruby: if s.empty?
来源：http://hz.tian-w.cn/gtoqddhkow.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.gotoacloud.top/gtsjyvryjd.html

[E21] 超长截断加省略号
来源：http://hz.316326.xyz/gtzrijaixd.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.wangdashe.top/gtjdhsvlab.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.havefunace.top/gtoyibruxs.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.gogol.net.cn/gtfifstend.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.ydzc1.top/gtcrtokfwk.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.zycfv.cn/gtawvvngmw.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.dianchejie.cn/gtugsdsijf.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.fengsongda.top/gtnrczcqkb.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.jiagoushi.top/gtfuzuxgmg.html

[E22] 字节长度与字符长度
来源：http://hz.shuidangran.top/gtknxdziqe.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.yj20258.top/gtpkladsql.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.dashuyun.cn/gtvmtwnghc.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.chenzaomai.com/gtvjojfvuu.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.daxiang520.top/gtcitewwpo.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.fengsongda.top/gtbgrzsdul.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.redwolf501.top/gtwpoiuwak.html

Ruby: s.bytesize;  s.length
来源：http://hz.aizwys.cn/gtmbyhvumk.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.redwolf501.top/gtemaczrak.html

================================================================================
来源：http://hz.hnxiangtu.top/gtiqwdqvwo.html

F. 文件与目录
来源：http://hz.yuxming.cn/gtiobgggnf.html

================================================================================
来源：http://hz.smart0.xyz/gttvnesini.html

[F01] 读取整个文件
来源：http://hz.shzxlz.cn/gtfeshuhxd.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.yongpay.top/gtablrxuer.html

PHP:  file_get_contents("a.txt");
来源：http://hz.chenzaomai.com/gtaemethnl.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.zhixingplan.top/gtoxjunofh.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.zhijiandao.cn/gtenjivgsu.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.nanxinkj.top/gtjqjxkmyj.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.zycfv.cn/gtpxyfbgax.html

Ruby: File.read("a.txt")
来源：http://hz.yj20258.top/gtlomatvrn.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.kuanghao11.cn/gtrewtswjm.html

[F02] 逐行读取文件
来源：http://hz.smart0.xyz/gtwwqgmrbp.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.sweek.top/gtfxbnhtlx.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.yanxiufei.cn/gthmcgfibl.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yj20258.top/gtygzjuwmv.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yuxming.cn/gttrfcejsq.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.cdnleiting.top/gtcwwuknqw.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.zhongyouzk.top/gtslipalph.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.hfpthk.cn/gtrdwgbdwn.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.zdqjudy.top/gtkmewnnga.html

[F03] 写入文件（覆盖）
来源：http://hz.yonumen.top/gtnfbfzcyd.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.nanxuanxn.top/gtziqrizuj.html


<!-- 参考信息 -->