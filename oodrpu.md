代发 wailian999

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.wangdashe.top/gtvujcbqow.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.pengpengdd.cyou/gtoweaezxt.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.zdqjudy.top/gtetlkufzb.html

[D14] 映射转换（每个元素变形）
来源：http://hz.andypj.xyz/gtqkzmxrry.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.quarkkingdee.top/gthubfllef.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.hfpthk.cn/gttkehqodr.html

JS:   arr.map(x => x * 2)
来源：http://hz.mhx1999.top/gtqwcmchxa.html

TS:   arr.map(x => x * 2)
来源：http://hz.zhiwuduotai.top/gtpcimbmqp.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.pengpengdd.cyou/gttzyoitvo.html

Go:   // 手写循环
来源：http://hz.cqqwz.cn/gtkdfvitci.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.hongshengwenyu.top/gtekurnnte.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.wangshuangyany.cn/gtjjixciil.html

[D15] 去重
来源：http://hz.xinyue.icu/gtqcdpjnrm.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.gotoacloud.top/gtdsjjxxqs.html

PHP:  array_unique($arr);
来源：http://hz.yanxiufei.cn/gthnlmteac.html

JS:   [...new Set(arr)]
来源：http://hz.yueranfly.top/gtdppzdoao.html

TS:   [...new Set(arr)]
来源：http://hz.fzhhl.top/gtlvvthime.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.gotoacloud.top/gtrolxhswo.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.nanxinkj.top/gtvtzzclmw.html

Ruby: arr.uniq
来源：http://hz.yuanzhike.top/gtmcqqzkye.html

C#:   list.Distinct().ToList()
来源：http://hz.ywan-chungtsiang.top/gtjulqwuar.html

[D16] 求和与平均值
来源：http://hz.guannengcc.top/gtdmkdjbgi.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.pycfn.com/gtndolmrrq.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.mhx1999.top/gtabvwwnop.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.0kj1m.cn/gtfluqpmtc.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.cucudq.cn/gtabvedgrj.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.yuxming.cn/gtgljttqkh.html

Go:   // 手写循环累加
来源：http://hz.tian-w.cn/gtnraaxynz.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.hnxiangtu.top/gtkazdepac.html

C#:   list.Sum();  list.Average()
来源：http://hz.aizwys.cn/gtllshkgks.html

[D17] 最大值与最小值
来源：http://hz.aibaodan.cn/gtozcktmnx.html

Py:   max(arr);  min(arr)
来源：http://hz.nanxuanxn.top/gtknlschmm.html

PHP:  max($arr);  min($arr);
来源：http://hz.daria6918.cn/gtgzvhroqf.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.sweek.top/gtjgqlafcz.html

TS:   Math.max(...arr);
来源：http://hz.ivvv.top/gtokarovhr.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.yuxming.cn/gtzmevfoia.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.bjfxy.top/gtemuieege.html

Ruby: arr.max;  arr.min
来源：http://hz.xylfe.cn/gtekuunwaa.html

C#:   list.Max();  list.Min()
来源：http://hz.smart0.xyz/gtpipbngog.html

[D18] 扁平化嵌套数组
来源：http://hz.aibaodan.cn/gtrfvzjhaj.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.xinyue.icu/gtozbakeiv.html

PHP:  array_merge(...$nested);
来源：http://hz.haohaochexian.top/gtxlurysgp.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.xinyue.icu/gtoxyyvzia.html

TS:   nested.flat();
来源：http://hz.yueranfly.top/gtyeajerfr.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.redwolf501.top/gtkweguqmn.html

Go:   // 手写双层循环
来源：http://hz.ydzc1.top/gttgxknypv.html

Ruby: nested.flatten
来源：http://hz.guowangkeji.top/gtkascgcan.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.xuetiantiany.cn/gtnmuuhpzu.html

[D19] 按字段分组
来源：http://hz.birdmap.top/gtqqjruwjx.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.shzxlz.cn/gtmxshzdpt.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.yvedp.cn/gtbegxrftj.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.52xcode.cn/gtyttapohm.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.haohaochexian.top/gtgpbjbjan.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.ehwqpu.com/gtqtsetrbn.html

Go:   // 手写 map[string][]T
来源：http://hz.ehwqpu.com/gtnvogetax.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.ybcxt.top/gtaqbcuhsk.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.yj202588.top/gttapmhdta.html

[D20] 统计每个元素出现次数
来源：http://hz.sxryk.cn/gttudeztkr.html

Py:   Counter(arr)
来源：http://hz.gogol.net.cn/gtwcpqphrl.html

PHP:  array_count_values($arr);
来源：http://hz.yvedp.cn/gtvyrtrzol.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.gzhubu.top/gtbuwghqkj.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.gotoacloud.top/gtwwqlbgtt.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.xylfe.cn/gtwgvvqnoh.html

Go:   // 手写 map[T]int
来源：http://hz.gotoacloud.top/gtlrmyaccu.html

Ruby: arr.tally
来源：http://hz.hnqzz.top/gteyrqythq.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.sweek.top/gtejfbzymt.html

[D21] 判断是否包含某元素
来源：http://hz.xingfuxueyuan.xyz/gtgosbjowu.html

Py:   x in arr
来源：http://hz.daxiang520.top/gtusablrfo.html

PHP:  in_array($x, $arr, true);
来源：http://hz.tian-w.cn/gtfkhjsjns.html

JS:   arr.includes(x)
来源：http://hz.cucudq.cn/gtavdzikpm.html

TS:   arr.includes(x)
来源：http://hz.0kj1m.cn/gterwpqmcs.html

Java: list.contains(x)
来源：http://hz.hnqzz.top/gtiauzppmd.html

Go:   slices.Contains(arr, x)
来源：http://hz.hnqzz.top/gtvtzpsman.html

Ruby: arr.include?(x)
来源：http://hz.feifeiyinyue.top/gtmwpcekbq.html

C#:   list.Contains(x)
来源：http://hz.yj20258888.top/gtetfatfqy.html

[D22] 复制数组（避免共享引用）
来源：http://hz.ppjwa.cn/gtdtnedrzm.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.birdmap.top/gtlvzpzqjo.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.316326.xyz/gtkogvciiw.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.birdmap.top/gtdjrjavbp.html

TS:   [...arr];
来源：http://hz.sxryk.cn/gtmsfwcmzk.html

Java: new ArrayList<>(list);
来源：http://hz.nwbrower.top/gtaceoxfpr.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.dianchejie.cn/gtsaauvjfx.html

Ruby: arr.dup;  arr.clone
来源：http://hz.xuetiantiany.cn/gthrpxbiff.html

C#:   new List<int>(list);
来源：http://hz.yueranfly.top/gtdctwtqna.html

[D23] reduce 累积计算
来源：http://hz.quarkkingdee.top/gteehwbtdo.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.jiagoushi.top/gtastebbit.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.quarkkingdee.top/gtzvvlexuf.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.xziqi.cn/gtrwhtmakc.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jqgfzy.top/gtpinyqacj.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.yueranfly.top/gtegeniaor.html

Go:   // 手写循环
来源：http://hz.yj202588.top/gtfzimttav.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.yvedp.cn/gtfoewwszk.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.cqqwz.cn/gtutllzzva.html

[D24] 字典 / Map 基本操作
来源：http://hz.52xcode.cn/gtwnvbnurv.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.316326.xyz/gtlnuaxfjc.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.ywan-chungtsiang.top/gtrirxvxet.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.yanxiufei.cn/gtvrfkjeqc.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.zhijiandao.cn/gtnxxmxvkn.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.tian-w.cn/gthgxpggzk.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.ivvv.top/gtbfidqdcx.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.zycfv.cn/gtodkiajyr.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.sxryk.cn/gtappbmhnw.html

[D25] Set 集合去重与交并差
来源：http://hz.pycfn.com/gtxffgplle.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.kuanghao11.cn/gtypgemyqs.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.gogol.net.cn/gtypbrshun.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.sysykeji.top/gtmjxmdlgr.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.xziqi.cn/gtfqeylihz.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.tian-w.cn/gtyperzewa.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.yangfankeji.com/gtxorgkuuz.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.yonumen.top/gtcjpflvaj.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.fzhhl.top/gtdqazaopu.html

[D26] 数组转字符串
来源：http://hz.tianlin.xyz/gtrgzapmpx.html

Py:   ", ".join(map(str, arr))
来源：http://hz.cucudq.cn/gtfnmkbywn.html

PHP:  implode(", ", $arr);
来源：http://hz.jinqigufen.top/gtoyoyadxe.html

JS:   arr.join(", ")
来源：http://hz.aibaodan.cn/gtdxdnerok.html

TS:   arr.join(", ")
来源：http://hz.hysaishi.cn/gtambidppq.html

Java: String.join(", ", list)
来源：http://hz.yuanzhike.top/gtjvpkxgcq.html

Go:   strings.Join(strs, ", ")
来源：http://hz.chenjidiqi.icu/gtnoqnkjtl.html

Ruby: arr.join(", ")
来源：http://hz.dianchejie.cn/gtrelsfoms.html

C#:   string.Join(", ", list)
来源：http://hz.haohaochexian.top/gtglcfwasp.html

================================================================================
来源：http://hz.ydzc1.top/gtcuszhpia.html

E. 字符串处理
来源：http://hz.cdnleiting.top/gtrcylfgte.html

================================================================================
来源：http://hz.bjfxy.top/gtqaixdyev.html

[E01] 拼接字符串
来源：http://hz.jqgfzy.top/gtrigupmsr.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.ywan-chungtsiang.top/gtxoulresl.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.yuxming.cn/gtsrcrsiii.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jiagoushi.top/gtdatqbvsv.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.andypj.xyz/gtflaaaesm.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.jinyuanbaomall.cn/gtnqzrvrcg.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.zdqjudy.top/gtntvswpjj.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.jyoumei.cn/gtktokzgad.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.hammf.cn/gteeddpwcw.html

[E02] 重复字符串
来源：http://hz.zhixingplan.top/gtfutltgxr.html

Py:   "ab" * 3
来源：http://hz.jlsjyb.cn/gtqpnkapmh.html

PHP:  str_repeat("ab", 3);
来源：http://hz.wangdashe.top/gthkeqmblh.html

JS:   "ab".repeat(3)
来源：http://hz.pengpengdd.cyou/gtnllkienx.html

TS:   "ab".repeat(3)
来源：http://hz.xingfuxueyuan.xyz/gtjzkhpyzm.html

Java: "ab".repeat(3)
来源：http://hz.nanxinkj.top/gtddqpgvpa.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.ehwqpu.com/gthtmflmkl.html

Ruby: "ab" * 3
来源：http://hz.zhaomingkeji.xyz/gtlkyprwun.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.hnqzz.top/gtujscitsm.html

[E03] 截取子串
来源：http://hz.fzhhl.top/gtimyzugbv.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.chenjidiqi.icu/gtrqyhpemk.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.52xcode.cn/gtdxxmfzib.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.zhongyouzk.top/gtlrwxcfbq.html

TS:   s.slice(1, 4)
来源：http://hz.chenjidiqi.icu/gtkrgcwwlb.html

Java: s.substring(1, 4)
来源：http://hz.hnxiangtu.top/gtopyswkit.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.wangdashe.top/gtzykgeegr.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.zhijiandao.cn/gthwfayjtx.html

C#:   s.Substring(1, 3)
来源：http://hz.ivvv.top/gtutooebdr.html

[E04] 查找子串位置
来源：http://hz.c1oappe.top/gtvsigjvxv.html

Py:   s.find("x");  s.index("x")
来源：http://hz.hfpthk.cn/gtryikubfn.html

PHP:  strpos($s, "x");
来源：http://hz.smart0.xyz/gtynqxzrts.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.yueranfly.top/gthkrsaoim.html

TS:   s.indexOf("x")
来源：http://hz.nanxinkj.top/gtitwpntrt.html

Java: s.indexOf("x")
来源：http://hz.yueranfly.top/gtprpynbhp.html

Go:   strings.Index(s, "x")
来源：http://hz.chenzaomai.com/gtqarbqbfx.html

Ruby: s.index("x")
来源：http://hz.iojbl.cn/gtczqqtdyt.html

C#:   s.IndexOf("x")
来源：http://hz.jinqigufen.top/gtsfptbzfn.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.hammf.cn/gtvuyzpzsp.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.tianlin.xyz/gtissqkvgh.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.birdmap.top/gtqousyeal.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.ehwqpu.com/gtphqiqiph.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.quarkkingdee.top/gtgmyiucqn.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.redwolf501.top/gtzswzgrkl.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.hnxiangtu.top/gtxygyhekv.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.hongshengwenyu.top/gtdzdvcuau.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.xingfuxueyuan.xyz/gtcvtgbppv.html

[E06] 替换子串
来源：http://hz.nanxinkj.top/gtfxypchpj.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.yueranfly.top/gtafhnazmx.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.jlsjyb.cn/gtvdgtxbaj.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.dianchejie.cn/gtnqhjsruo.html

TS:   s.replaceAll("a", "b")
来源：http://hz.quarkkingdee.top/gthmqoyvhq.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.jianghu66.top/gtndizqvuz.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.tanke756.top/gthgflxdid.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.sysykeji.top/gthlbmesti.html

C#:   s.Replace("a", "b")
来源：http://hz.cdnleiting.top/gtqdpdhsep.html

[E07] 按分隔符拆分
来源：http://hz.9152youxi.cn/gtqjtqfann.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.chenjidiqi.icu/gtnmyskuof.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.xziqi.cn/gtzhmjgwsk.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.iojbl.cn/gtycrsokmo.html

TS:   s.split(",")
来源：http://hz.daxiang520.top/gtamjtvkcv.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.gaohongyu789.top/gtazjgxqak.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.zycfv.cn/gtxysyasyi.html

Ruby: s.split(",");  s.split
来源：http://hz.jinyuanbaomall.cn/gtydoczoze.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.c1oappe.top/gtwftebgpi.html

[E08] 数组按分隔符合并
来源：http://hz.nwbrower.top/gtmlkazacy.html

Py:   ",".join(items)
来源：http://hz.zhaomingkeji.xyz/gtjoqdzzcu.html

PHP:  implode(",", $items);
来源：http://hz.ywan-chungtsiang.top/gtrmyhevud.html

JS:   items.join(",")
来源：http://hz.cdnleiting.top/gtmwimplmu.html

TS:   items.join(",")
来源：http://hz.haohaochexian.top/gtgxbmdmyy.html

Java: String.join(",", items)
来源：http://hz.dianchejie.cn/gtwdasdhnh.html

Go:   strings.Join(items, ",")
来源：http://hz.jqgufenzy.top/gtzrimumwy.html

Ruby: items.join(",")
来源：http://hz.feifeiyinyue.top/gtrfwrsawv.html

C#:   string.Join(",", items)
来源：http://hz.havefunace.top/gtrlbxznws.html

[E09] 去除所有空白字符
来源：http://hz.yangfankeji.com/gtzdmslvuf.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.shangyingyoupin.top/gtslvmwfzn.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.xziqi.cn/gtvkidecza.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.tian-w.cn/gtozivepne.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.0kj1m.cn/gtxewuwszc.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.pengpengdd.cyou/gtmpnqaqln.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.0kj1m.cn/gtpcbtrvpi.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.0kj1m.cn/gtqbdvwgly.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.haohaochexian.top/gtheupvecy.html

[E10] 左侧补零 / 定长填充
来源：http://hz.guowangkeji.top/gtvxtjguxy.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.svipenyu.cn/gtzbtltewv.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.guowangkeji.top/gtngwkhxyy.html

JS:   "7".padStart(3, "0")
来源：http://hz.yuxming.cn/gtionoecwg.html

TS:   "7".padStart(3, "0")
来源：http://hz.jiagoushi.top/gtpsskxnmc.html

Java: String.format("%03d", 7)
来源：http://hz.nanxinkj.top/gtdunwpnzg.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.gotoacloud.top/gtgiuyhfyj.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.pycfn.com/gtvfdnmtyt.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.feifeiyinyue.top/gtfvnwsrhk.html

[E11] 反转字符串
来源：http://hz.hywenlv.cn/gtrvglmels.html

Py:   s[::-1]
来源：http://hz.sysykeji.top/gtnthnxzqo.html

PHP:  strrev($s);
来源：http://hz.shangyingyoupin.top/gtayedzdfk.html

JS:   [...s].reverse().join("")
来源：http://hz.kuanghao11.cn/gtxgsttine.html

TS:   [...s].reverse().join("")
来源：http://hz.wangdashe.top/gtxmkebdvo.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.cheryme.top/gtwznihzhn.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.zhixingplan.top/gthjkbdvwp.html

Ruby: s.reverse
来源：http://hz.cqqwz.cn/gtzdrljilu.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.9152youxi.cn/gtxkrcdvju.html

[E12] 统计某字符出现次数
来源：http://hz.hfpthk.cn/gtwdnqpiqf.html

Py:   s.count("a")
来源：http://hz.ydjk.org.cn/gtobfocpvx.html

PHP:  substr_count($s, "a");
来源：http://hz.gaohongyu789.top/gtbhiiidzc.html

JS:   s.split("a").length - 1
来源：http://hz.jiagoushi.top/gtgydwtfbo.html

TS:   s.split("a").length - 1
来源：http://hz.wangshuangyany.cn/gtsczixzrg.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.dianchejie.cn/gtczjhftjj.html

Go:   strings.Count(s, "a")
来源：http://hz.zhengqikj.top/gtclfuwayt.html

Ruby: s.count("a")
来源：http://hz.zhixingplan.top/gtpfgqqapt.html

C#:   s.Count(c => c == 'a')
来源：http://hz.cdnleiting.top/gtcvezbdax.html

[E13] 逐字符遍历
来源：http://hz.kuanghao11.cn/gthtabxumc.html

Py:   for ch in s: print(ch)
来源：http://hz.hfpthk.cn/gtqzfnxayz.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.yonumen.top/gtmfykrcsk.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.aibaodan.cn/gttyclgshg.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.xingfuxueyuan.xyz/gtipgsuxnm.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.svipenyu.cn/gtkpbfekpt.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.gogol.net.cn/gtjlefyoig.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.yanxiufei.cn/gtwikaoixh.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.ywan-chungtsiang.top/gtsogldxal.html

[E14] URL 编码与 Base64
来源：http://hz.316326.xyz/gtivfzhwmu.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.hnqzz.top/gtlpazfswq.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.nanxuanxn.top/gtbexiswwg.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.tianlin.xyz/gtiqjqscbe.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.xziqi.cn/gtmcavahsw.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.feifeiyinyue.top/gtranyxlao.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.cheryme.top/gtvqfudzky.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.aibaodan.cn/gtwsmctmty.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.shuidangran.top/gtxycdxpbk.html

[E15] HTML 转义 / 反转义
来源：http://hz.meibo888.top/gtkbpiowzt.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.quarkkingdee.top/gtiwvbcfqz.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.gogol.net.cn/gtfssnymra.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.gzhubu.top/gtkvtshrvk.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.hysaishi.cn/gtsabeumwc.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.jinyuanbaomall.cn/gtimzpabsx.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.hammf.cn/gtkmyrwseh.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.wangdashe.top/gtwvvfddmp.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.sysykeji.top/gtufyhrrul.html

[E16] 数字千分位
来源：http://hz.hfpthk.cn/gtjvalkigh.html

Py:   f"{1234567:,}"
来源：http://hz.aibaodan.cn/gtisdhvxzh.html

PHP:  number_format(1234567);
来源：http://hz.dianchejie.cn/gtryyyukpp.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.jinyuanbaomall.cn/gtealixggj.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.jqgfzy.top/gtwpwzucnn.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.jqgufenzy.top/gtcrejjorj.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.hammf.cn/gtsorxtoba.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.aizwys.cn/gtwalqvpou.html

C#:   1234567.ToString("N0")
来源：http://hz.cdnleiting.top/gtbcovycwp.html

[E17] 首字母大写
来源：http://hz.shanyushiyangtech.top/gtfazukjnh.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.zhijiandao.cn/gtkmvtuqjb.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.0kj1m.cn/gtdkqwxjgz.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.ybcxt.top/gttarbhtdf.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.yueranfly.top/gtbmyvoonh.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.zhiwuduotai.top/gtmydxdgkv.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.zhongyouzk.top/gtowbnabpr.html

Ruby: s.capitalize
来源：http://hz.wangshuangyany.cn/gtexhonrlh.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.c1oappe.top/gtzeregavc.html

[E18] 模板占位符替换
来源：http://hz.cdnleiting.top/gturawczcf.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.zhaomingkeji.xyz/gtfkldeecq.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.vqdsnc.cn/gtxsptrkde.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.gzhubu.top/gtjoumqnkh.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.chenjidiqi.icu/gthbmifyey.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.shanyushiyangkeji.top/gtkjuddmol.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.yanxiufei.cn/gtqlyfylhs.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.aibaodan.cn/gtycawvdki.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.zdqjudy.top/gttdwzjgsh.html

[E19] 多行文本按行拆分
来源：http://hz.nanxinkj.top/gtohpewehb.html

Py:   s.splitlines()
来源：http://hz.dashuyun.cn/gtrxymwuux.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.cqqwz.cn/gtxkhihjfe.html

JS:   s.split(/\r?\n/)
来源：http://hz.zdqjudy.top/gtpswbujhf.html

TS:   s.split(/\r?\n/)
来源：http://hz.gotoacloud.top/gtzhpzntyj.html

Java: s.lines().toList()
来源：http://hz.jqgufenzy.top/gtfzxveyqh.html

Go:   strings.Split(s, "\n")
来源：http://hz.bjfxy.top/gtzgotszos.html

Ruby: s.lines
来源：http://hz.jinqigfzy.top/gtpkhhlwnm.html

C#:   s.Split('\n')
来源：http://hz.hfpthk.cn/gtiodetnfn.html

[E20] 判断字符串是否为空
来源：http://hz.ppjwa.cn/gtuudslezf.html

Py:   if not s:
来源：http://hz.52xcode.cn/gtuvfzzhpb.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.jinyuanbaomall.cn/gtpzpegqpk.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.pycfn.com/gtiaeoviob.html

TS:   if (s === "") {}
来源：http://hz.meibo888.top/gthbdbleoc.html

Java: if (s.isEmpty()) {}
来源：http://hz.guowangkeji.top/gttcchovtu.html


<!-- 参考信息 -->