代发 wailian999

PHP:  max($arr);  min($arr);
来源：http://hz.hnqzz.top/gtxogbyict.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.jinyuanbaomall.cn/gtlplbcleh.html

TS:   Math.max(...arr);
来源：http://hz.cqqwz.cn/gthpkgvtzz.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.cheryme.top/gtodhijhzi.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.dianchejie.cn/gtgfokvfef.html

Ruby: arr.max;  arr.min
来源：http://hz.sysykeji.top/gtmztaddbe.html

C#:   list.Max();  list.Min()
来源：http://hz.cucudq.cn/gtsgzrntka.html

[D18] 扁平化嵌套数组
来源：http://hz.ivvv.top/gtjgkaeotr.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.xinyue.icu/gtgjsivwvf.html

PHP:  array_merge(...$nested);
来源：http://hz.nanxinkj.top/gtfezljxve.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.xinyue.icu/gtnxixsorx.html

TS:   nested.flat();
来源：http://hz.chenjidiqi.icu/gtxvuvddkj.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.shanyushiyangtech.top/gtoisqgwmk.html

Go:   // 手写双层循环
来源：http://hz.birdmap.top/gtquikoypn.html

Ruby: nested.flatten
来源：http://hz.zhixingplan.top/gtmrfdbeto.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.daxiang520.top/gtjjzpzjcq.html

[D19] 按字段分组
来源：http://hz.ywan-chungtsiang.top/gtxddinwbc.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.bjfxy.top/gtqtxednkp.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.cqqwz.cn/gtpyfgvxxi.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.jqgfzy.top/gtpyfqqsbh.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.xuetiantiany.cn/gtgztmnojk.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.gzhubu.top/gtefqxzzhn.html

Go:   // 手写 map[string][]T
来源：http://hz.guannengcc.top/gtdymuwufw.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.hammf.cn/gthefwgbyx.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.yonumen.top/gtfckvlqzw.html

[D20] 统计每个元素出现次数
来源：http://hz.shanyushiyangkeji.top/gtaykdorpc.html

Py:   Counter(arr)
来源：http://hz.pycfn.com/gtkzgudvup.html

PHP:  array_count_values($arr);
来源：http://hz.ivvv.top/gtyzdghgyy.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.shanyushiyangkeji.top/gtixeqwslx.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.pengpengdd.cyou/gtxilbdhzr.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.xuetiantiany.cn/gtxyqvmdvp.html

Go:   // 手写 map[T]int
来源：http://hz.jqgufenzy.top/gteupvstfz.html

Ruby: arr.tally
来源：http://hz.mhx1999.top/gtzjppzlcg.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.cheryme.top/gtrchvjxrw.html

[D21] 判断是否包含某元素
来源：http://hz.ppjwa.cn/gtnvqinmhj.html

Py:   x in arr
来源：http://hz.birdmap.top/gtmkkqsmwt.html

PHP:  in_array($x, $arr, true);
来源：http://hz.ehwqpu.com/gtseajuaqd.html

JS:   arr.includes(x)
来源：http://hz.cqqwz.cn/gtcbnpzekw.html

TS:   arr.includes(x)
来源：http://hz.nanxuanxn.top/gtswxfgdom.html

Java: list.contains(x)
来源：http://hz.nanxinkj.top/gtfmjuxaqt.html

Go:   slices.Contains(arr, x)
来源：http://hz.fzhhl.top/gtcuwpdyvd.html

Ruby: arr.include?(x)
来源：http://hz.hammf.cn/gtwsibrpjj.html

C#:   list.Contains(x)
来源：http://hz.zdqjudy.top/gtuwnaabyd.html

[D22] 复制数组（避免共享引用）
来源：http://hz.chenjidiqi.icu/gtzazziefk.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.zhaomingkeji.xyz/gtujeptvrk.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.yvedp.cn/gtejerwzej.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.pengpengdd.cyou/gtztyujryj.html

TS:   [...arr];
来源：http://hz.pengpengdd.cyou/gtbattzynj.html

Java: new ArrayList<>(list);
来源：http://hz.zhaomingkeji.xyz/gtnqvrvihn.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.jyoumei.cn/gtnmdmjutn.html

Ruby: arr.dup;  arr.clone
来源：http://hz.dashuyun.cn/gtsblwqjbf.html

C#:   new List<int>(list);
来源：http://hz.shanyushiyangtech.top/gtdymttxod.html

[D23] reduce 累积计算
来源：http://hz.jqgufenzy.top/gtxbttrrtw.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.zhixingplan.top/gtfdjmgctx.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.jiagoushi.top/gtejgueujh.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.gotoacloud.top/gtyadradti.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jlsjyb.cn/gtwdxnvlqu.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.hysaishi.cn/gtdxfdubdc.html

Go:   // 手写循环
来源：http://hz.yangfankeji.com/gtpkmrkepe.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.jinyuanbaomall.cn/gtbnqpkwie.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.yanxiufei.cn/gtcmnzelgv.html

[D24] 字典 / Map 基本操作
来源：http://hz.yonumen.top/gtouyclilu.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.jqgfzy.top/gtkvplzsjr.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.sweek.top/gtemebgqra.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.yj202588.top/gtlpyjqvvo.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.xingfuxueyuan.xyz/gtcftercpp.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.dashuyun.cn/gtsxsnwlmz.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.xuanzx.com/gtqzjmgutu.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.pycfn.com/gtxfxqiopi.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.aibaodan.cn/gtncnrgufl.html

[D25] Set 集合去重与交并差
来源：http://hz.yuanzhike.top/gtlbbkdfyf.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.daxiang520.top/gtthyxialz.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.sxryk.cn/gtaurbexcg.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.nwbrower.top/gtvehgnxke.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.gzhubu.top/gtohisvixg.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.yanxiufei.cn/gtuftkxvth.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.52xcode.cn/gtsxcxffts.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.nwbrower.top/gtjqbvhepr.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.chenlongwang.top/gtwrystziq.html

[D26] 数组转字符串
来源：http://hz.tianlin.xyz/gtjxaggfpp.html

Py:   ", ".join(map(str, arr))
来源：http://hz.birdmap.top/gtfvcbuazy.html

PHP:  implode(", ", $arr);
来源：http://hz.gaohongyu789.top/gtunbouhqy.html

JS:   arr.join(", ")
来源：http://hz.jinqigfzy.top/gtcqrsndzf.html

TS:   arr.join(", ")
来源：http://hz.yj20258.top/gtkzimhucw.html

Java: String.join(", ", list)
来源：http://hz.chenlongwang.top/gtstrnikpw.html

Go:   strings.Join(strs, ", ")
来源：http://hz.shanyushiyangtech.top/gtxfsiszcj.html

Ruby: arr.join(", ")
来源：http://hz.tanke756.top/gtgzrzdgtt.html

C#:   string.Join(", ", list)
来源：http://hz.ehwqpu.com/gtwcsycxxb.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtcfgvozef.html

E. 字符串处理
来源：http://hz.havefunace.top/gtssqhdvgl.html

================================================================================
来源：http://hz.fzhhl.top/gtwaekwzwr.html

[E01] 拼接字符串
来源：http://hz.jqgufenzy.top/gtmvliqwkf.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.zhoulong.xyz/gtvrqmfcut.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.jinghuilouyu.cn/gtjxggkauv.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.cucudq.cn/gtdcqynspw.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.vqdsnc.cn/gtqhuahanq.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.yj202588.top/gtiasuvrry.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.bjfxy.top/gtfkdmntxd.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.dashuyun.cn/gtmwessiec.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.nwbrower.top/gthpqupest.html

[E02] 重复字符串
来源：http://hz.hnxiangtu.top/gthdyuobrm.html

Py:   "ab" * 3
来源：http://hz.jlsjyb.cn/gtqbydmmof.html

PHP:  str_repeat("ab", 3);
来源：http://hz.wangshuangyany.cn/gtyvhsdble.html

JS:   "ab".repeat(3)
来源：http://hz.jqgufenzy.top/gtgbgduffn.html

TS:   "ab".repeat(3)
来源：http://hz.nanxuanxn.top/gteqhefhgt.html

Java: "ab".repeat(3)
来源：http://hz.tian-w.cn/gtnuooault.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.ywan-chungtsiang.top/gtvtbjifzk.html

Ruby: "ab" * 3
来源：http://hz.ehwqpu.com/gtugzfbqxr.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.bjfxy.top/gtfnflhlfn.html

[E03] 截取子串
来源：http://hz.52xcode.cn/gthlfogtdx.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.jinyuanbaomall.cn/gtcuvqkhoh.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.zycfv.cn/gttketeoro.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.cheryme.top/gtfheaytpb.html

TS:   s.slice(1, 4)
来源：http://hz.fzhhl.top/gtvjpkuzaa.html

Java: s.substring(1, 4)
来源：http://hz.svipenyu.cn/gtizepeyyp.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.jinyuanbaomall.cn/gtzbcjbscv.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.fzhhl.top/gtehugtwly.html

C#:   s.Substring(1, 3)
来源：http://hz.zycfv.cn/gtosfxyizk.html

[E04] 查找子串位置
来源：http://hz.feifeiyinyue.top/gtlkcvclcb.html

Py:   s.find("x");  s.index("x")
来源：http://hz.guowangkeji.top/gtgadtgiwx.html

PHP:  strpos($s, "x");
来源：http://hz.chenjidiqi.icu/gtopgnuxtq.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.zhiwuduotai.top/gtpgngcgjn.html

TS:   s.indexOf("x")
来源：http://hz.yueranfly.top/gtyggpdusg.html

Java: s.indexOf("x")
来源：http://hz.jinqigfzy.top/gtzbcmdvlf.html

Go:   strings.Index(s, "x")
来源：http://hz.zdqjudy.top/gtlllffzjz.html

Ruby: s.index("x")
来源：http://hz.zhengqikj.top/gtrqpsmqop.html

C#:   s.IndexOf("x")
来源：http://hz.yueranfly.top/gtsjsseoof.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.cqqwz.cn/gtmvyxmprj.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.yj202588.top/gtberjwzql.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.ydjk.org.cn/gtbovjoxdv.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.nanxinkj.top/gtvbjzycpe.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.nanxuanxn.top/gtipbbnune.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.hnqzz.top/gtlblkjxnp.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.zdqjudy.top/gtpuqhqxra.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.sxryk.cn/gtniiscqrq.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.gotoacloud.top/gtxbkswsmb.html

[E06] 替换子串
来源：http://hz.sufxvd.cn/gtqcizmshl.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.chenzaomai.com/gtvhjlnjmq.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.xinyue.icu/gtrhxxpcgf.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.zhoulong.xyz/gtmabmpwsp.html

TS:   s.replaceAll("a", "b")
来源：http://hz.gogol.net.cn/gtrogbjhjv.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.xuetiantiany.cn/gtkrgjwqpu.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.zhengqikj.top/gtvncssyhi.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.ywan-chungtsiang.top/gtoztxazqq.html

C#:   s.Replace("a", "b")
来源：http://hz.yvedp.cn/gtzpbsbqnr.html

[E07] 按分隔符拆分
来源：http://hz.ppjwa.cn/gthikmmulx.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.yvedp.cn/gtegvigjtv.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.havefunace.top/gtxonbfcuf.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.nanxinkj.top/gtzcxvbswc.html

TS:   s.split(",")
来源：http://hz.c1oappe.top/gtokhddmpv.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.smart0.xyz/gtxphgtqnk.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.pengpengdd.cyou/gtjvicpqiy.html

Ruby: s.split(",");  s.split
来源：http://hz.wangdashe.top/gttcimlrxj.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.cqqwz.cn/gtzaarswqw.html

[E08] 数组按分隔符合并
来源：http://hz.yuanzhike.top/gtganyqbvw.html

Py:   ",".join(items)
来源：http://hz.jyoumei.cn/gttiilqchw.html

PHP:  implode(",", $items);
来源：http://hz.sysykeji.top/gtvjlwimnj.html

JS:   items.join(",")
来源：http://hz.aizwys.cn/gtzofxzjan.html

TS:   items.join(",")
来源：http://hz.zhixingplan.top/gtanjjtufo.html

Java: String.join(",", items)
来源：http://hz.daria6918.cn/gtkftwqdkc.html

Go:   strings.Join(items, ",")
来源：http://hz.sufxvd.cn/gtfjcbawee.html

Ruby: items.join(",")
来源：http://hz.nwbrower.top/gtoyoqzvzr.html

C#:   string.Join(",", items)
来源：http://hz.0kj1m.cn/gtgyjwoqji.html

[E09] 去除所有空白字符
来源：http://hz.nwbrower.top/gttztfkyoi.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.redwolf501.top/gtsppaywae.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.shanyushiyangtech.top/gttcmierha.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.gzhubu.top/gtwccwpgnr.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.svipenyu.cn/gtfiuifwab.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.yj20258888.top/gtimliddis.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.zycfv.cn/gtwxsiquii.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.yj202588.top/gthtjbxpzn.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.9152youxi.cn/gtwmkqcmbq.html

[E10] 左侧补零 / 定长填充
来源：http://hz.snrcjt.cn/gtingjpxpr.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.aibaodan.cn/gtdqixicwx.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.smart0.xyz/gtlufuamlb.html

JS:   "7".padStart(3, "0")
来源：http://hz.guannengcc.top/gtrjgmfyyg.html

TS:   "7".padStart(3, "0")
来源：http://hz.yuxming.cn/gtazmopekm.html

Java: String.format("%03d", 7)
来源：http://hz.hywenlv.cn/gtwbxclspj.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.ppjwa.cn/gtvqhrteae.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.jiagoushi.top/gtcisgekbd.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.yj20258888.top/gtnxzbpqbd.html

[E11] 反转字符串
来源：http://hz.tanke756.top/gtfwopcuvq.html

Py:   s[::-1]
来源：http://hz.xingfuxueyuan.xyz/gttxxtrelz.html

PHP:  strrev($s);
来源：http://hz.havefunace.top/gtgrarzaee.html

JS:   [...s].reverse().join("")
来源：http://hz.zhiwuduotai.top/gttwnxuawr.html

TS:   [...s].reverse().join("")
来源：http://hz.cashguo.top/gtbywccpsb.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.havefunace.top/gtodebhouu.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.yanxiufei.cn/gtikxpmtsc.html

Ruby: s.reverse
来源：http://hz.jinghuilouyu.cn/gttjylidkm.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.redwolf501.top/gtrsxpsicb.html

[E12] 统计某字符出现次数
来源：http://hz.yvedp.cn/gtosmyjlip.html

Py:   s.count("a")
来源：http://hz.gaohongyu789.top/gtvuwknlip.html

PHP:  substr_count($s, "a");
来源：http://hz.chenlongwang.top/gtndlbzxug.html

JS:   s.split("a").length - 1
来源：http://hz.wangshuangyany.cn/gttneftdkg.html

TS:   s.split("a").length - 1
来源：http://hz.quarkkingdee.top/gtnfdelqpp.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.cdnleiting.top/gtitfqvfap.html

Go:   strings.Count(s, "a")
来源：http://hz.xylfe.cn/gtxamymthi.html

Ruby: s.count("a")
来源：http://hz.fzhhl.top/gtjjzuqfcf.html

C#:   s.Count(c => c == 'a')
来源：http://hz.zhongyouzk.top/gtjtwnymrf.html

[E13] 逐字符遍历
来源：http://hz.cheryme.top/gtqsgwkypw.html

Py:   for ch in s: print(ch)
来源：http://hz.iojbl.cn/gtrosevwln.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.zhiwuduotai.top/gtewnyshlk.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.dashuyun.cn/gtmabogfoi.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.ydjk.org.cn/gtaumyblpw.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.zhaomingkeji.xyz/gtsfyqwleg.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.chenlongwang.top/gtwdoylpgw.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.svipenyu.cn/gtwqqqforg.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.dashuyun.cn/gtwctkvocs.html

[E14] URL 编码与 Base64
来源：http://hz.jqgufenzy.top/gtewaghxtu.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.yangfankeji.com/gtmlkkpiys.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.dashuyun.cn/gtxzavswgv.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.xingfuxueyuan.xyz/gtreegyqwu.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.cucudq.cn/gtjynamvwg.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.zhengqikj.top/gtdmfdxpfx.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.smart0.xyz/gtqvraesmj.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.ppjwa.cn/gtiflvjzqn.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.ehwqpu.com/gtwymaejbs.html

[E15] HTML 转义 / 反转义
来源：http://hz.shuidangran.top/gtuvheykbf.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.jinqigufen.top/gtvoyspwyt.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.yueranfly.top/gtkulilvpc.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.52xcode.cn/gtxmekvxwv.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.zhijiandao.cn/gtiduxpiba.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.jinqigfzy.top/gtkregfsug.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.vqdsnc.cn/gtuxrsmoqf.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.hammf.cn/gttbdtlkrq.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.jinqigfzy.top/gtrtripiim.html

[E16] 数字千分位
来源：http://hz.shzxlz.cn/gtnijqkulp.html

Py:   f"{1234567:,}"
来源：http://hz.zhijiandao.cn/gtlaalmhii.html

PHP:  number_format(1234567);
来源：http://hz.jyoumei.cn/gtrqvplcsq.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.tanke756.top/gtbpnetsky.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.yj20258888.top/gtcwustvjw.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.smart0.xyz/gthmbkefdo.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.daxiang520.top/gtltpzsywo.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.aibaodan.cn/gtyhsqhmdz.html

C#:   1234567.ToString("N0")
来源：http://hz.cdnleiting.top/gtyonqjabz.html

[E17] 首字母大写
来源：http://hz.yuanzhike.top/gtklzxvlsp.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.havefunace.top/gtztduhija.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.wangshuangyany.cn/gtvzzzovjp.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.havefunace.top/gtdawfmitq.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.52xcode.cn/gtbceihrsy.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.gzhubu.top/gtcoxxrkjo.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.yj20258.top/gtywniqlcb.html

Ruby: s.capitalize
来源：http://hz.aizwys.cn/gtvprxzzct.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.xingfuxueyuan.xyz/gtvpmklcbd.html

[E18] 模板占位符替换
来源：http://hz.jinqigufen.top/gtqgscrlrh.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.xuanzx.com/gtklhjuqiw.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.jinghuilouyu.cn/gtqiroukzr.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.quarkkingdee.top/gtsuubmqlq.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.gogol.net.cn/gtbjnlkuwr.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.shanyushiyangkeji.top/gtjqnxjtya.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.shanyushiyangtech.top/gteghaonda.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.cucudq.cn/gticgyvlee.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.wangshuangyany.cn/gtmjanfgdq.html

[E19] 多行文本按行拆分
来源：http://hz.cheryme.top/gtryeyfhrb.html

Py:   s.splitlines()
来源：http://hz.yj20258.top/gtorrpvxbe.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.yj20258.top/gtjubqwvmt.html

JS:   s.split(/\r?\n/)
来源：http://hz.nwbrower.top/gtvwqensxz.html

TS:   s.split(/\r?\n/)
来源：http://hz.hammf.cn/gttgpyhnep.html

Java: s.lines().toList()
来源：http://hz.fzhhl.top/gtjzmqcnkz.html

Go:   strings.Split(s, "\n")
来源：http://hz.xuanzx.com/gtejganyln.html

Ruby: s.lines
来源：http://hz.iojbl.cn/gtqxzqefmw.html

C#:   s.Split('\n')
来源：http://hz.xuanzx.com/gtpigfpmzq.html

[E20] 判断字符串是否为空
来源：http://hz.jinqigufen.top/gtgufusloi.html

Py:   if not s:
来源：http://hz.sweek.top/gtwbrxogjd.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.nwbrower.top/gtxapxlmua.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.yvedp.cn/gtsangozti.html

TS:   if (s === "") {}
来源：http://hz.cheryme.top/gtpyziwxbx.html

Java: if (s.isEmpty()) {}
来源：http://hz.jianghu66.top/gtwqtywyml.html

Go:   if s == "" {}
来源：http://hz.haohaochexian.top/gthndianrf.html

Ruby: if s.empty?
来源：http://hz.52xcode.cn/gtazfiyyiw.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.aizwys.cn/gtaqbwnxoh.html

[E21] 超长截断加省略号
来源：http://hz.aizwys.cn/gteclwfrcz.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.snrcjt.cn/gtjhjzwqkp.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.chenzaomai.com/gthwtgdxkd.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.ppjwa.cn/gtofnxbyqi.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.daxiang520.top/gtwevjkghm.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.zhoulong.xyz/gtsjcestss.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.hfpthk.cn/gtuumfwcab.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.hysaishi.cn/gtbhayjixi.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.vqdsnc.cn/gttjrqdakf.html

[E22] 字节长度与字符长度
来源：http://hz.cqqwz.cn/gtalovamfu.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.iojbl.cn/gtobqfvjfp.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.xylfe.cn/gtllrebhbs.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.xziqi.cn/gtqvanyuvi.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.chenlongwang.top/gtuwckadan.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.xingfuxueyuan.xyz/gtrkoqosym.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.gotoacloud.top/gtwehnnlcq.html

Ruby: s.bytesize;  s.length
来源：http://hz.zycfv.cn/gtgedeexsb.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.hfpthk.cn/gtblzgzpqn.html

================================================================================
来源：http://hz.yj20258888.top/gttejrozgt.html

F. 文件与目录
来源：http://hz.316326.xyz/gtaxzweohb.html

================================================================================
来源：http://hz.xuanzx.com/gtacwnjsxa.html

[F01] 读取整个文件
来源：http://hz.havefunace.top/gttzlapnwe.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.andypj.xyz/gtcxgjxauv.html

PHP:  file_get_contents("a.txt");
来源：http://hz.yongpay.top/gtvapzvieg.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.zhengqikj.top/gtbsnufhkv.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.fzhhl.top/gtcpekdvmk.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.sufxvd.cn/gtkthaggmw.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.gaohongyu789.top/gtyfcuodwp.html

Ruby: File.read("a.txt")
来源：http://hz.chenjidiqi.icu/gtgvhuumwg.html


<!-- 参考信息 -->