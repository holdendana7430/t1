代发 wailian999

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.ydzc1.top/gtmhwsqpjt.html

JS:   arr.filter(x => x > 3)
来源：http://hz.hammf.cn/gtiqnrzlpa.html

TS:   arr.filter(x => x > 3)
来源：http://hz.jqgfzy.top/gtgbmcyswx.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.zdqjudy.top/gtesiepxqg.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.nwbrower.top/gtekojoyda.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.ybcxt.top/gtnvcrcnwz.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.yonumen.top/gtpvteqyno.html

[D14] 映射转换（每个元素变形）
来源：http://hz.shzxlz.cn/gtfqthffrg.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.zhengqikj.top/gtvccpqrsm.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.chenzaomai.com/gturouvowu.html

JS:   arr.map(x => x * 2)
来源：http://hz.chenjidiqi.icu/gtederzdwl.html

TS:   arr.map(x => x * 2)
来源：http://hz.chenjidiqi.icu/gtwvtpatdk.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.bjfxy.top/gtfgghqjbx.html

Go:   // 手写循环
来源：http://hz.yuxming.cn/gtjexvultu.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.yueranfly.top/gtfbnlaoik.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.havefunace.top/gtoymsbnva.html

[D15] 去重
来源：http://hz.jiagoushi.top/gtnaswoksu.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.dianchejie.cn/gtlpnpiwza.html

PHP:  array_unique($arr);
来源：http://hz.c1oappe.top/gtsooozycy.html

JS:   [...new Set(arr)]
来源：http://hz.yj20258888.top/gtlwhbojwy.html

TS:   [...new Set(arr)]
来源：http://hz.dianchejie.cn/gtbdpigpbh.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.tanke756.top/gtakkqidnk.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.ppjwa.cn/gtlrvrjjyu.html

Ruby: arr.uniq
来源：http://hz.jyoumei.cn/gtouqwsnyy.html

C#:   list.Distinct().ToList()
来源：http://hz.sysykeji.top/gtpaaajlov.html

[D16] 求和与平均值
来源：http://hz.hnxiangtu.top/gtscxkaawt.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.yuxming.cn/gtpkqxswrp.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.dianchejie.cn/gtyfkjqhee.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.snrcjt.cn/gtyxcfrvml.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jinghuilouyu.cn/gtjmsbezem.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.yuanzhike.top/gtvpxoguri.html

Go:   // 手写循环累加
来源：http://hz.0kj1m.cn/gthfgotwoo.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.tanke756.top/gtpijexqei.html

C#:   list.Sum();  list.Average()
来源：http://hz.gaohongyu789.top/gtxczcablc.html

[D17] 最大值与最小值
来源：http://hz.cucudq.cn/gtkmjduyyv.html

Py:   max(arr);  min(arr)
来源：http://hz.dianchejie.cn/gtdusdmgdl.html

PHP:  max($arr);  min($arr);
来源：http://hz.jinghuilouyu.cn/gtudgxjyqm.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.sweek.top/gtapdcrzyg.html

TS:   Math.max(...arr);
来源：http://hz.c1oappe.top/gtbldkwsnu.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.guowangkeji.top/gtvfuhbzji.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.vqdsnc.cn/gtrufvlygw.html

Ruby: arr.max;  arr.min
来源：http://hz.vqdsnc.cn/gteraohybd.html

C#:   list.Max();  list.Min()
来源：http://hz.gzhubu.top/gttzaepcgz.html

[D18] 扁平化嵌套数组
来源：http://hz.gogol.net.cn/gtypsiazqs.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.zhoulong.xyz/gtphkpdkfu.html

PHP:  array_merge(...$nested);
来源：http://hz.ppjwa.cn/gtlzczakkv.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.gotoacloud.top/gtattyeshq.html

TS:   nested.flat();
来源：http://hz.xuanzx.com/gtnbvwsald.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.ydzc1.top/gtjnfvuqbl.html

Go:   // 手写双层循环
来源：http://hz.guowangkeji.top/gtmrbpdyka.html

Ruby: nested.flatten
来源：http://hz.316326.xyz/gtvsufvtfn.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.xuetiantiany.cn/gtrnihbcjw.html

[D19] 按字段分组
来源：http://hz.hfpthk.cn/gtkmwammtg.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.shuidangran.top/gtcycldpyw.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.guannengcc.top/gtbztuiprq.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.wangdashe.top/gtpvrzgddx.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.xziqi.cn/gtjgdrmcto.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.fzhhl.top/gttstocjlp.html

Go:   // 手写 map[string][]T
来源：http://hz.hysaishi.cn/gtnhnaoxcv.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.cheryme.top/gtsgkhvndi.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.jiagoushi.top/gtqwiwtepp.html

[D20] 统计每个元素出现次数
来源：http://hz.jqgfzy.top/gtbgiqyjpn.html

Py:   Counter(arr)
来源：http://hz.daxiang520.top/gtrgzkvztn.html

PHP:  array_count_values($arr);
来源：http://hz.hywenlv.cn/gtbwgzymcp.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.chenjidiqi.icu/gtztahfbas.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.daxiang520.top/gtaixvcsju.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.jlsjyb.cn/gtxrhtpotn.html

Go:   // 手写 map[T]int
来源：http://hz.shanyushiyangkeji.top/gtyoqmhxhh.html

Ruby: arr.tally
来源：http://hz.cdnleiting.top/gtquavtjuq.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.jqgufenzy.top/gtxmyrncfb.html

[D21] 判断是否包含某元素
来源：http://hz.yuanzhike.top/gtjmgbykjr.html

Py:   x in arr
来源：http://hz.shuidangran.top/gtorfhhstd.html

PHP:  in_array($x, $arr, true);
来源：http://hz.aibaodan.cn/gtfxuinfhp.html

JS:   arr.includes(x)
来源：http://hz.guannengcc.top/gtypurhaii.html

TS:   arr.includes(x)
来源：http://hz.meibo888.top/gtfhpsqchz.html

Java: list.contains(x)
来源：http://hz.yueranfly.top/gtysryhejh.html

Go:   slices.Contains(arr, x)
来源：http://hz.daxiang520.top/gtctfpjitv.html

Ruby: arr.include?(x)
来源：http://hz.jinqigfzy.top/gtsmunxruv.html

C#:   list.Contains(x)
来源：http://hz.yangfankeji.com/gtvxuzqpdk.html

[D22] 复制数组（避免共享引用）
来源：http://hz.nanxuanxn.top/gtxdvtdfhv.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.jqgufenzy.top/gthqhrxpls.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.jinyuanbaomall.cn/gtjznbaynb.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.jqgfzy.top/gtiacicjtk.html

TS:   [...arr];
来源：http://hz.svipenyu.cn/gtwiloszrp.html

Java: new ArrayList<>(list);
来源：http://hz.cashguo.top/gtjlgemqpv.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.chenjidiqi.icu/gtqnmmptdo.html

Ruby: arr.dup;  arr.clone
来源：http://hz.yj20258.top/gtxlsivqls.html

C#:   new List<int>(list);
来源：http://hz.zhijiandao.cn/gtjlalutds.html

[D23] reduce 累积计算
来源：http://hz.yj202588.top/gtglxonbgl.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.snrcjt.cn/gtpighhplg.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.tian-w.cn/gtephhoxgx.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.zhiwuduotai.top/gtiydnnfey.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.shanyushiyangkeji.top/gtomvblrmg.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.yuanzhike.top/gtfbewbjrl.html

Go:   // 手写循环
来源：http://hz.xziqi.cn/gtfctsolep.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.xuetiantiany.cn/gtjagmprfl.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.andypj.xyz/gtrplgshwz.html

[D24] 字典 / Map 基本操作
来源：http://hz.nanxuanxn.top/gtlxtgsbng.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.aizwys.cn/gtuqyrpkgy.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.cheryme.top/gtiacjhgpm.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.zycfv.cn/gtuzhuvmsq.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.tanke756.top/gtkunrzheq.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.dianchejie.cn/gthxswsoly.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.zhengqikj.top/gtydxqygcz.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.yonumen.top/gtfzmqpaip.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.jianghu66.top/gtjmnzqoec.html

[D25] Set 集合去重与交并差
来源：http://hz.shanyushiyangkeji.top/gtkchucgsx.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.wangdashe.top/gtpatrjhza.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.wangdashe.top/gtodrrzkqh.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.birdmap.top/gtiaypfwkc.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.yanxiufei.cn/gtmbymqipo.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.yueranfly.top/gtwfpnxrlg.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.hnqzz.top/gtoqwbadzk.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.cdnleiting.top/gtjnsmmxts.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.daria6918.cn/gtusgtdfhw.html

[D26] 数组转字符串
来源：http://hz.daxiang520.top/gtyhksrdwi.html

Py:   ", ".join(map(str, arr))
来源：http://hz.wangdashe.top/gtggjwatda.html

PHP:  implode(", ", $arr);
来源：http://hz.jyoumei.cn/gtubvibtsb.html

JS:   arr.join(", ")
来源：http://hz.ppjwa.cn/gthexhewlp.html

TS:   arr.join(", ")
来源：http://hz.guannengcc.top/gthppuhoyh.html

Java: String.join(", ", list)
来源：http://hz.haohaochexian.top/gtsdzmvlzd.html

Go:   strings.Join(strs, ", ")
来源：http://hz.zhongyouzk.top/gtabptxlkk.html

Ruby: arr.join(", ")
来源：http://hz.jqgfzy.top/gtscngaojd.html

C#:   string.Join(", ", list)
来源：http://hz.chenjidiqi.icu/gtkplefukd.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtuvyqceha.html

E. 字符串处理
来源：http://hz.tian-w.cn/gtvvrvdufo.html

================================================================================
来源：http://hz.chenzaomai.com/gttitvpqrr.html

[E01] 拼接字符串
来源：http://hz.guowangkeji.top/gtfkwiuadg.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.aizwys.cn/gtqdkktytx.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.hysaishi.cn/gtzuaawcyk.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yuanzhike.top/gtulucwjso.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.ydzc1.top/gtbprjhxec.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.zhixingplan.top/gtdmdmjayl.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.shanyushiyangkeji.top/gtawhgblzp.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.sweek.top/gtxeegtvkc.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.sweek.top/gtpqunxyup.html

[E02] 重复字符串
来源：http://hz.jianghu66.top/gtjdxwamkt.html

Py:   "ab" * 3
来源：http://hz.sufxvd.cn/gtbvnfgpwc.html

PHP:  str_repeat("ab", 3);
来源：http://hz.yueranfly.top/gtvnrcswwx.html

JS:   "ab".repeat(3)
来源：http://hz.jianghu66.top/gtxzrpunth.html

TS:   "ab".repeat(3)
来源：http://hz.chenlongwang.top/gtmvrslmli.html

Java: "ab".repeat(3)
来源：http://hz.redwolf501.top/gtcfyhopnq.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.52xcode.cn/gtoganchmp.html

Ruby: "ab" * 3
来源：http://hz.meibo888.top/gtthnnnfpf.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.havefunace.top/gtrlpihtjj.html

[E03] 截取子串
来源：http://hz.chenlongwang.top/gtbhyxdsyt.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.redwolf501.top/gtrleuvuhf.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.gogol.net.cn/gtvorbbrev.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.shangyingyoupin.top/gtohxhvgso.html

TS:   s.slice(1, 4)
来源：http://hz.jiagoushi.top/gtvwngsagz.html

Java: s.substring(1, 4)
来源：http://hz.wangdashe.top/gtautknlsn.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.snrcjt.cn/gtvlrzxulc.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.jqgufenzy.top/gtspjibbtf.html

C#:   s.Substring(1, 3)
来源：http://hz.havefunace.top/gtacbhvnii.html

[E04] 查找子串位置
来源：http://hz.xinyue.icu/gtjgpblhah.html

Py:   s.find("x");  s.index("x")
来源：http://hz.hongshengwenyu.top/gtntkzdblu.html

PHP:  strpos($s, "x");
来源：http://hz.9152youxi.cn/gtpbdcuzmt.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.haohaochexian.top/gtrkztwnqz.html

TS:   s.indexOf("x")
来源：http://hz.sysykeji.top/gthqziokof.html

Java: s.indexOf("x")
来源：http://hz.zycfv.cn/gttgceqrsj.html

Go:   strings.Index(s, "x")
来源：http://hz.ybcxt.top/gtdxvadbbg.html

Ruby: s.index("x")
来源：http://hz.jinghuilouyu.cn/gtqpguptwj.html

C#:   s.IndexOf("x")
来源：http://hz.svipenyu.cn/gtlkmwydrp.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.cucudq.cn/gtukawaaho.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.hammf.cn/gtlpxnttxl.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.feifeiyinyue.top/gttiizstwy.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.iojbl.cn/gtnxuqkigj.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.meibo888.top/gtkwzjnzyk.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.nanxinkj.top/gtjcjncuxn.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.ppjwa.cn/gtmntzxylw.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.zdqjudy.top/gtrfpbhknb.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.yanxiufei.cn/gtofqgfdlb.html

[E06] 替换子串
来源：http://hz.zhijiandao.cn/gteyjvfzby.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.hywenlv.cn/gtmrgyeuoz.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.haohaochexian.top/gtykdxnpqi.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.dianchejie.cn/gteywipbap.html

TS:   s.replaceAll("a", "b")
来源：http://hz.dashuyun.cn/gtxycplkym.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.jlsjyb.cn/gtjvjeasyw.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.yangfankeji.com/gtnamzaxmz.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.shzxlz.cn/gtttlcwmhi.html

C#:   s.Replace("a", "b")
来源：http://hz.quarkkingdee.top/gtkrgmnizo.html

[E07] 按分隔符拆分
来源：http://hz.cucudq.cn/gtfrykimjv.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.guannengcc.top/gthhochvdi.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.smart0.xyz/gtgbnqyjpu.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.wangdashe.top/gtnzziviuq.html

TS:   s.split(",")
来源：http://hz.shanyushiyangtech.top/gtrnafmmzw.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.sxryk.cn/gtccsjiszd.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.yj20258888.top/gtrrghgmxa.html

Ruby: s.split(",");  s.split
来源：http://hz.zdqjudy.top/gtupcbuoef.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.vqdsnc.cn/gtnglupjzg.html

[E08] 数组按分隔符合并
来源：http://hz.ybcxt.top/gthahmwzbi.html

Py:   ",".join(items)
来源：http://hz.jqgufenzy.top/gtupreqkui.html

PHP:  implode(",", $items);
来源：http://hz.cdnleiting.top/gtlnyoltdv.html

JS:   items.join(",")
来源：http://hz.hfpthk.cn/gtvctxcadu.html

TS:   items.join(",")
来源：http://hz.smart0.xyz/gtekswombx.html

Java: String.join(",", items)
来源：http://hz.zhengqikj.top/gtlqtsqycp.html

Go:   strings.Join(items, ",")
来源：http://hz.pycfn.com/gtqwpvxcou.html

Ruby: items.join(",")
来源：http://hz.ehwqpu.com/gtvkjamczv.html

C#:   string.Join(",", items)
来源：http://hz.0kj1m.cn/gtydtiftgt.html

[E09] 去除所有空白字符
来源：http://hz.ywan-chungtsiang.top/gtyfgbnszq.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.quarkkingdee.top/gtohdyvror.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.dashuyun.cn/gtcxowodda.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.fzhhl.top/gtnjjiqpsd.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.hysaishi.cn/gtsmpiitno.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.jinqigufen.top/gtkosscvja.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.svipenyu.cn/gthcilfejz.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.nwbrower.top/gtxcqrhxdi.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.sweek.top/gtarmmwkef.html

[E10] 左侧补零 / 定长填充
来源：http://hz.nanxinkj.top/gtqepyfmzi.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.daxiang520.top/gtxvxoqasv.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.zhoulong.xyz/gtflmanxhv.html

JS:   "7".padStart(3, "0")
来源：http://hz.yj20258.top/gtgiescrro.html

TS:   "7".padStart(3, "0")
来源：http://hz.hammf.cn/gtxriargzn.html

Java: String.format("%03d", 7)
来源：http://hz.ivvv.top/gtmzvrczfd.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.yvedp.cn/gtbpwwasuz.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.xziqi.cn/gtwgcrvuqx.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.zhongyouzk.top/gtqczxytji.html

[E11] 反转字符串
来源：http://hz.xinyue.icu/gtzcwmrckk.html

Py:   s[::-1]
来源：http://hz.zdqjudy.top/gtkjzsaofq.html

PHP:  strrev($s);
来源：http://hz.smart0.xyz/gthdftkmbo.html

JS:   [...s].reverse().join("")
来源：http://hz.chenzaomai.com/gtfdypgshm.html

TS:   [...s].reverse().join("")
来源：http://hz.wangshuangyany.cn/gtkomyqchf.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.zdqjudy.top/gtioaresfe.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.ydzc1.top/gtzspjetfm.html

Ruby: s.reverse
来源：http://hz.zhengqikj.top/gtjbmmlwth.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.yongpay.top/gtiqeidigx.html

[E12] 统计某字符出现次数
来源：http://hz.yuxming.cn/gtnhxblokx.html

Py:   s.count("a")
来源：http://hz.gaohongyu789.top/gtpjmxsoaj.html

PHP:  substr_count($s, "a");
来源：http://hz.xziqi.cn/gtqpqxfkkr.html

JS:   s.split("a").length - 1
来源：http://hz.wangshuangyany.cn/gtyfjdcmop.html

TS:   s.split("a").length - 1
来源：http://hz.jinyuanbaomall.cn/gtsmmauotw.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.xuetiantiany.cn/gtnkajaail.html

Go:   strings.Count(s, "a")
来源：http://hz.tian-w.cn/gtlfoiinxp.html

Ruby: s.count("a")
来源：http://hz.hammf.cn/gthjwyhgaz.html

C#:   s.Count(c => c == 'a')
来源：http://hz.hnxiangtu.top/gthzkwmrhd.html

[E13] 逐字符遍历
来源：http://hz.mhx1999.top/gtgfiluvfi.html

Py:   for ch in s: print(ch)
来源：http://hz.hnxiangtu.top/gtdfmkmnho.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.daria6918.cn/gtvpirwguj.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.dashuyun.cn/gtzkycyuna.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yanxiufei.cn/gtunmanaxl.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.redwolf501.top/gtwlierkfa.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.xingfuxueyuan.xyz/gtdcvykxky.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.ywan-chungtsiang.top/gtyipiawhv.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.zhoulong.xyz/gtmxeailts.html

[E14] URL 编码与 Base64
来源：http://hz.feifeiyinyue.top/gtdohqbbzn.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.0kj1m.cn/gtkipcrcxd.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.shuidangran.top/gtojobgvrd.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.snrcjt.cn/gtfpbpskuk.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.yueranfly.top/gtgqvclfvs.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.vqdsnc.cn/gtjtaoptim.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.chenlongwang.top/gtvdruopvv.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.yj20258888.top/gtsikrzngx.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.shzxlz.cn/gtkvhgjwkx.html

[E15] HTML 转义 / 反转义
来源：http://hz.sysykeji.top/gtdqlmafnb.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.hnxiangtu.top/gtxsidiovp.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.xziqi.cn/gtdqmxiyrq.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.havefunace.top/gtoimvrszk.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.jyoumei.cn/gtvlpkooun.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.yanxiufei.cn/gtkywxsgrk.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.xylfe.cn/gtsiaiaifr.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.hysaishi.cn/gtntksfjqw.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.jqgfzy.top/gtefgvexos.html

[E16] 数字千分位
来源：http://hz.gzhubu.top/gtzktgusan.html

Py:   f"{1234567:,}"
来源：http://hz.svipenyu.cn/gtewvbxenl.html

PHP:  number_format(1234567);
来源：http://hz.tanke756.top/gtsctsyqag.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.vqdsnc.cn/gtxfhmhidu.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.shuidangran.top/gtnvrnpzme.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.fzhhl.top/gtuvruprzv.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.jinghuilouyu.cn/gtzubhrjxh.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.316326.xyz/gtgjumuwdh.html

C#:   1234567.ToString("N0")
来源：http://hz.xylfe.cn/gtumpxwckd.html

[E17] 首字母大写
来源：http://hz.fzhhl.top/gtodoythje.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.hysaishi.cn/gtumfrjwnu.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.sufxvd.cn/gtrvkqeyaj.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.gogol.net.cn/gtixubjxpo.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.nwbrower.top/gtbpmowpzb.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.c1oappe.top/gtpqqvgnyx.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.yj20258888.top/gtmwehmjca.html

Ruby: s.capitalize
来源：http://hz.yangfankeji.com/gtxamnznpq.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.c1oappe.top/gtkjofonhm.html

[E18] 模板占位符替换
来源：http://hz.sufxvd.cn/gtsamggulf.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.cheryme.top/gtznvvmfwj.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.yvedp.cn/gtzjcvfbaa.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.zhoulong.xyz/gtsfltkfmu.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.yangfankeji.com/gtwoopjash.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.zdqjudy.top/gttnzvgasa.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.yongpay.top/gtfcbduzbt.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.zhixingplan.top/gtueidbwyz.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.shuidangran.top/gtymibxxlm.html

[E19] 多行文本按行拆分
来源：http://hz.yj20258888.top/gtcbmrxnvh.html

Py:   s.splitlines()
来源：http://hz.zhiwuduotai.top/gtjfssdjbo.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.hnxiangtu.top/gtqnbdofra.html

JS:   s.split(/\r?\n/)
来源：http://hz.jinghuilouyu.cn/gtmlcsfyrd.html

TS:   s.split(/\r?\n/)
来源：http://hz.mhx1999.top/gtjnebsbcn.html

Java: s.lines().toList()
来源：http://hz.daria6918.cn/gticgpkitx.html

Go:   strings.Split(s, "\n")
来源：http://hz.gogol.net.cn/gthxqfsfno.html

Ruby: s.lines
来源：http://hz.nwbrower.top/gtnrywcdkz.html

C#:   s.Split('\n')
来源：http://hz.chenzaomai.com/gtzzaqebnk.html

[E20] 判断字符串是否为空
来源：http://hz.gogol.net.cn/gtzfdlmrot.html

Py:   if not s:
来源：http://hz.cdnleiting.top/gtrgoabvnk.html


<!-- 参考信息 -->