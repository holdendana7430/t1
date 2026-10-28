代发 wailian999

TS:   [...arr].reverse();
来源：http://hz.zhaomingkeji.xyz/gtalwbsvaj.html

Java: Collections.reverse(list);
来源：http://hz.0kj1m.cn/gtbagnblfb.html

Go:   slices.Reverse(arr)
来源：http://hz.fengsongda.top/gtijwhsaxz.html

Ruby: arr.reverse
来源：http://hz.jianghu66.top/gtgqgyvwbe.html

C#:   list.Reverse();
来源：http://hz.snrcjt.cn/gtwlxvhccx.html

[D12] 查找元素下标
来源：http://hz.fengsongda.top/gtpnhrqwot.html

Py:   arr.index(x);  x in arr
来源：http://hz.tanke756.top/gtibijdxos.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.zdqjudy.top/gtgpusezyb.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.52xcode.cn/gtqlrfbnvj.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.jinyuanbaomall.cn/gtrkodibvz.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.jinqigfzy.top/gtnxsilfqd.html

Go:   slices.Index(arr, x)
来源：http://hz.chenjidiqi.icu/gttlxrmxcs.html

Ruby: arr.index(x)
来源：http://hz.birdmap.top/gttxdjlect.html

C#:   list.IndexOf(x);
来源：http://hz.zycfv.cn/gtniubnqkv.html

[D13] 过滤（保留满足条件的）
来源：http://hz.fengsongda.top/gtzlxeyavj.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.aizwys.cn/gtwoiuculo.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.chenjidiqi.icu/gtfcwdjtbr.html

JS:   arr.filter(x => x > 3)
来源：http://hz.zhoulong.xyz/gtfiwustgx.html

TS:   arr.filter(x => x > 3)
来源：http://hz.jinqigfzy.top/gtmjpjxlto.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.jiagoushi.top/gtbjqclwnr.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.zdqjudy.top/gtkgrfihtu.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.nwbrower.top/gtouexosyu.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.gotoacloud.top/gtyhsktvlu.html

[D14] 映射转换（每个元素变形）
来源：http://hz.mhx1999.top/gtbxzodjjo.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.9152youxi.cn/gtlusxaibp.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.xuanzx.com/gtexuboxuj.html

JS:   arr.map(x => x * 2)
来源：http://hz.ehwqpu.com/gtnnhltqsb.html

TS:   arr.map(x => x * 2)
来源：http://hz.hysaishi.cn/gtohvlcitr.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.cdnleiting.top/gtfjkzmcgw.html

Go:   // 手写循环
来源：http://hz.feifeiyinyue.top/gtxxnjmekx.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.cheryme.top/gtapzlfhji.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.shuidangran.top/gtzrtdgils.html

[D15] 去重
来源：http://hz.hfpthk.cn/gtwkkhcmgi.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.meibo888.top/gtwlgrseuy.html

PHP:  array_unique($arr);
来源：http://hz.hongshengwenyu.top/gtotmidpim.html

JS:   [...new Set(arr)]
来源：http://hz.jyoumei.cn/gtqnfmiksa.html

TS:   [...new Set(arr)]
来源：http://hz.jiagoushi.top/gtwupiogth.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.kuanghao11.cn/gtkcwyktej.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.sxryk.cn/gtpajviked.html

Ruby: arr.uniq
来源：http://hz.chenzaomai.com/gtupfjgsym.html

C#:   list.Distinct().ToList()
来源：http://hz.shuidangran.top/gtatgqlviv.html

[D16] 求和与平均值
来源：http://hz.birdmap.top/gtukwimipu.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.yuxming.cn/gtnozmavjj.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.shanyushiyangkeji.top/gtkyvlmwsw.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yuxming.cn/gtwgezxxua.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.guannengcc.top/gtsowlplha.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.daxiang520.top/gtawqpytfr.html

Go:   // 手写循环累加
来源：http://hz.hnqzz.top/gtheyxynjc.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.shzxlz.cn/gtbykizzxd.html

C#:   list.Sum();  list.Average()
来源：http://hz.yuxming.cn/gtexrvbzmc.html

[D17] 最大值与最小值
来源：http://hz.yonumen.top/gtlzwpepwc.html

Py:   max(arr);  min(arr)
来源：http://hz.shanyushiyangtech.top/gtkcigbrda.html

PHP:  max($arr);  min($arr);
来源：http://hz.zhaomingkeji.xyz/gtepbhigpt.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.gogol.net.cn/gtkgpohzbl.html

TS:   Math.max(...arr);
来源：http://hz.shanyushiyangkeji.top/gtsnrlgmjm.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.ehwqpu.com/gtajuvsyay.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.jqgufenzy.top/gtyfdzbtyz.html

Ruby: arr.max;  arr.min
来源：http://hz.fengsongda.top/gtcqwqphxq.html

C#:   list.Max();  list.Min()
来源：http://hz.chenlongwang.top/gtpenaqese.html

[D18] 扁平化嵌套数组
来源：http://hz.gotoacloud.top/gtkrdqqvjl.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.gotoacloud.top/gtvorgyzdn.html

PHP:  array_merge(...$nested);
来源：http://hz.ybcxt.top/gtbacuulbo.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.jinqigfzy.top/gtrooaezrw.html

TS:   nested.flat();
来源：http://hz.chenlongwang.top/gtavscrvtn.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.hfpthk.cn/gtjdnfxekw.html

Go:   // 手写双层循环
来源：http://hz.haohaochexian.top/gtatztitxk.html

Ruby: nested.flatten
来源：http://hz.xuetiantiany.cn/gttaursxdu.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.nwbrower.top/gtdnrbpjac.html

[D19] 按字段分组
来源：http://hz.yvedp.cn/gtjajgqgrc.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.jinghuilouyu.cn/gttlngroje.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.shanyushiyangkeji.top/gtkjnxbgsx.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.daria6918.cn/gtvwxghnfc.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.nanxinkj.top/gtfkbqqtbr.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.ehwqpu.com/gtalzdoszs.html

Go:   // 手写 map[string][]T
来源：http://hz.redwolf501.top/gtuabckurr.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.meibo888.top/gtvikljwre.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.zhoulong.xyz/gtmeysvzxb.html

[D20] 统计每个元素出现次数
来源：http://hz.xylfe.cn/gteajzrgft.html

Py:   Counter(arr)
来源：http://hz.zhiwuduotai.top/gtclotghby.html

PHP:  array_count_values($arr);
来源：http://hz.redwolf501.top/gtkfrraedm.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.chenlongwang.top/gtmgmhankf.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.cucudq.cn/gtwaibypmg.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.andypj.xyz/gthvlipjmv.html

Go:   // 手写 map[T]int
来源：http://hz.shzxlz.cn/gtxlazfnqg.html

Ruby: arr.tally
来源：http://hz.vqdsnc.cn/gtnaxehaic.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.ehwqpu.com/gtnrrjopwf.html

[D21] 判断是否包含某元素
来源：http://hz.kuanghao11.cn/gtmopwbwqh.html

Py:   x in arr
来源：http://hz.shzxlz.cn/gtzxjrdwsk.html

PHP:  in_array($x, $arr, true);
来源：http://hz.tian-w.cn/gtfbmrnplv.html

JS:   arr.includes(x)
来源：http://hz.bjfxy.top/gtjlykidku.html

TS:   arr.includes(x)
来源：http://hz.gaohongyu789.top/gttohtacrp.html

Java: list.contains(x)
来源：http://hz.gotoacloud.top/gtksndspmy.html

Go:   slices.Contains(arr, x)
来源：http://hz.tian-w.cn/gtiquycvlp.html

Ruby: arr.include?(x)
来源：http://hz.52xcode.cn/gtvgeqjiby.html

C#:   list.Contains(x)
来源：http://hz.jinqigfzy.top/gtzcxuaalo.html

[D22] 复制数组（避免共享引用）
来源：http://hz.fengsongda.top/gtbkqcuiea.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.cheryme.top/gtbbytitwc.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.cheryme.top/gthfkhtsnx.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.hnqzz.top/gtmgnaoeue.html

TS:   [...arr];
来源：http://hz.jinqigufen.top/gtbvgeelqk.html

Java: new ArrayList<>(list);
来源：http://hz.shanyushiyangkeji.top/gtsgigyois.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.hnqzz.top/gtajnbnoxs.html

Ruby: arr.dup;  arr.clone
来源：http://hz.shzxlz.cn/gtfgvqwohr.html

C#:   new List<int>(list);
来源：http://hz.fzhhl.top/gtvrysizvw.html

[D23] reduce 累积计算
来源：http://hz.cdnleiting.top/gtbgisjkgd.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.zhiwuduotai.top/gtlpdjnmqs.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.wangshuangyany.cn/gtqjghtgds.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.redwolf501.top/gtlrkaoajk.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.shangyingyoupin.top/gtecndxvur.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.tanke756.top/gtdzollygi.html

Go:   // 手写循环
来源：http://hz.tanke756.top/gtqrwmejfv.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.feifeiyinyue.top/gtfyuwmmfc.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.kuanghao11.cn/gtnlvgsjpn.html

[D24] 字典 / Map 基本操作
来源：http://hz.cqqwz.cn/gtgvvepeds.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.9152youxi.cn/gtbinolkni.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.nanxinkj.top/gtlkpfbbyn.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.xingfuxueyuan.xyz/gtjctwrbdp.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.shuidangran.top/gtrucjkpjh.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.havefunace.top/gthytfgcvg.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.sysykeji.top/gtzqaticwk.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.ydzc1.top/gtwrlguhgn.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.yanxiufei.cn/gtwzlmpegz.html

[D25] Set 集合去重与交并差
来源：http://hz.iojbl.cn/gtkxrecesp.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.jqgfzy.top/gtgljhebxj.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.haohaochexian.top/gtgbcrymiu.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.feifeiyinyue.top/gtucufkypm.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.chenjidiqi.icu/gtdbvnshxz.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.kuanghao11.cn/gtgutxxmku.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.jinqigfzy.top/gtnaptzpfh.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.wangshuangyany.cn/gtiuymmarg.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.snrcjt.cn/gtidhxgxhq.html

[D26] 数组转字符串
来源：http://hz.zhongyouzk.top/gtvsddwppr.html

Py:   ", ".join(map(str, arr))
来源：http://hz.zdqjudy.top/gtpvggzfhe.html

PHP:  implode(", ", $arr);
来源：http://hz.jianghu66.top/gtuqndpwvf.html

JS:   arr.join(", ")
来源：http://hz.wangdashe.top/gtchcpbmkt.html

TS:   arr.join(", ")
来源：http://hz.feifeiyinyue.top/gtxmoxojjc.html

Java: String.join(", ", list)
来源：http://hz.hywenlv.cn/gtdggnbmlc.html

Go:   strings.Join(strs, ", ")
来源：http://hz.dianchejie.cn/gtdkhnodld.html

Ruby: arr.join(", ")
来源：http://hz.pycfn.com/gteeybblaz.html

C#:   string.Join(", ", list)
来源：http://hz.pycfn.com/gtchoqpkgg.html

================================================================================
来源：http://hz.gogol.net.cn/gttcbyiief.html

E. 字符串处理
来源：http://hz.smart0.xyz/gtfibqnmys.html

================================================================================
来源：http://hz.cheryme.top/gtfwcepmth.html

[E01] 拼接字符串
来源：http://hz.shanyushiyangtech.top/gthuifgkjp.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.shuidangran.top/gtrmajyqvv.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.yanxiufei.cn/gtbvpitcam.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.9152youxi.cn/gteqrfvygj.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.xingfuxueyuan.xyz/gttuecrwdc.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.jinghuilouyu.cn/gtgawxeoxw.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.shzxlz.cn/gthicfqycg.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.xuetiantiany.cn/gtmuvovhyp.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.nanxuanxn.top/gtgrdrcpga.html

[E02] 重复字符串
来源：http://hz.hongshengwenyu.top/gtsdnzhzzm.html

Py:   "ab" * 3
来源：http://hz.jinyuanbaomall.cn/gtqvwmlklk.html

PHP:  str_repeat("ab", 3);
来源：http://hz.iojbl.cn/gtdwkdohtl.html

JS:   "ab".repeat(3)
来源：http://hz.havefunace.top/gtamyyabnp.html

TS:   "ab".repeat(3)
来源：http://hz.hnqzz.top/gtzontjyfo.html

Java: "ab".repeat(3)
来源：http://hz.jiagoushi.top/gtalhqwljf.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.yanxiufei.cn/gtbwphowvp.html

Ruby: "ab" * 3
来源：http://hz.ydzc1.top/gtnjifhlkn.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.hywenlv.cn/gtswhgpfmf.html

[E03] 截取子串
来源：http://hz.chenlongwang.top/gtbwjajueh.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.tanke756.top/gtrydbomeh.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.feifeiyinyue.top/gtaztdluvu.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.ydzc1.top/gtjecbtgyo.html

TS:   s.slice(1, 4)
来源：http://hz.xingfuxueyuan.xyz/gtzjmvhgpu.html

Java: s.substring(1, 4)
来源：http://hz.shzxlz.cn/gtxxqkbovq.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.jqgufenzy.top/gtoqrpmcxa.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.nanxinkj.top/gtxyfpdwgq.html

C#:   s.Substring(1, 3)
来源：http://hz.zhoulong.xyz/gtnutssmzq.html

[E04] 查找子串位置
来源：http://hz.yonumen.top/gtplofszrj.html

Py:   s.find("x");  s.index("x")
来源：http://hz.yanxiufei.cn/gtwtukbhsu.html

PHP:  strpos($s, "x");
来源：http://hz.gaohongyu789.top/gtbakfldfr.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.yj20258888.top/gtwwybmocf.html

TS:   s.indexOf("x")
来源：http://hz.jinyuanbaomall.cn/gtjdwumduy.html

Java: s.indexOf("x")
来源：http://hz.ehwqpu.com/gtbiwmuidr.html

Go:   strings.Index(s, "x")
来源：http://hz.sxryk.cn/gtvwljuvsl.html

Ruby: s.index("x")
来源：http://hz.gaohongyu789.top/gtagrfutvw.html

C#:   s.IndexOf("x")
来源：http://hz.yangfankeji.com/gtuqalnmfp.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.zhaomingkeji.xyz/gtwwvhdnnl.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.guowangkeji.top/gtoezrdttg.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.jlsjyb.cn/gtdnrzxxgo.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.jinyuanbaomall.cn/gtyfgyjhrd.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.yvedp.cn/gthfjdkujv.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.yj202588.top/gtapirleqc.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.gaohongyu789.top/gtkresqtmw.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.guowangkeji.top/gtmnprlryo.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.pengpengdd.cyou/gtkzzdficc.html

[E06] 替换子串
来源：http://hz.yvedp.cn/gthzdwhexq.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.aizwys.cn/gtlznovokl.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.quarkkingdee.top/gttgryemvw.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.yj20258.top/gtirccgwqr.html

TS:   s.replaceAll("a", "b")
来源：http://hz.fzhhl.top/gtpyiasgwq.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.zhaomingkeji.xyz/gtfbvcrsyy.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.yvedp.cn/gtcvzawkcj.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.zhixingplan.top/gtcgqpchmt.html

C#:   s.Replace("a", "b")
来源：http://hz.hongshengwenyu.top/gtorpzwhol.html

[E07] 按分隔符拆分
来源：http://hz.zhengqikj.top/gtxasjjmmu.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.feifeiyinyue.top/gtdjjeaqxx.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.dianchejie.cn/gtmqziemff.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.cheryme.top/gtbxnqeier.html

TS:   s.split(",")
来源：http://hz.chenjidiqi.icu/gtwchimlnj.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.xylfe.cn/gtuhjpgymg.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.zhengqikj.top/gtdzjkecyn.html

Ruby: s.split(",");  s.split
来源：http://hz.quarkkingdee.top/gtdewidxsf.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.wangshuangyany.cn/gtztjnbztj.html

[E08] 数组按分隔符合并
来源：http://hz.ppjwa.cn/gtjhkurcii.html

Py:   ",".join(items)
来源：http://hz.cashguo.top/gtvcllcefx.html

PHP:  implode(",", $items);
来源：http://hz.gzhubu.top/gtjfutihar.html

JS:   items.join(",")
来源：http://hz.yj202588.top/gtjzlvlmat.html

TS:   items.join(",")
来源：http://hz.chenlongwang.top/gtyskwvong.html

Java: String.join(",", items)
来源：http://hz.yuxming.cn/gtsyjqmqpa.html

Go:   strings.Join(items, ",")
来源：http://hz.316326.xyz/gtotxmxnbv.html

Ruby: items.join(",")
来源：http://hz.zhiwuduotai.top/gtkccvxxqw.html

C#:   string.Join(",", items)
来源：http://hz.yvedp.cn/gtbfzilzmf.html

[E09] 去除所有空白字符
来源：http://hz.zhengqikj.top/gtnfovvxvh.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.redwolf501.top/gtzgtjbkgb.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.havefunace.top/gtcqadfpcv.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.fengsongda.top/gtubkcdxpq.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.zhengqikj.top/gtyfxlmdvw.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.tanke756.top/gtoohkpwwn.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.gotoacloud.top/gtyzjjdblo.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.pengpengdd.cyou/gtnwlkvqqq.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.yuanzhike.top/gtiycsdotp.html

[E10] 左侧补零 / 定长填充
来源：http://hz.kuanghao11.cn/gtwyftzluo.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.ivvv.top/gtiwaxgmhx.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.vqdsnc.cn/gtflmcaqld.html

JS:   "7".padStart(3, "0")
来源：http://hz.yuanzhike.top/gtjlifvwdo.html

TS:   "7".padStart(3, "0")
来源：http://hz.xuetiantiany.cn/gtozqjfgnf.html

Java: String.format("%03d", 7)
来源：http://hz.mhx1999.top/gtninvwnsi.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.bjfxy.top/gtkssvsydv.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.jiagoushi.top/gtooicofad.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.yuxming.cn/gtnyosonvm.html

[E11] 反转字符串
来源：http://hz.52xcode.cn/gtoerthrfa.html

Py:   s[::-1]
来源：http://hz.gogol.net.cn/gtzaqqczpo.html

PHP:  strrev($s);
来源：http://hz.yvedp.cn/gtmxsstxip.html

JS:   [...s].reverse().join("")
来源：http://hz.andypj.xyz/gtbnengsmv.html

TS:   [...s].reverse().join("")
来源：http://hz.ppjwa.cn/gtyjkasdkm.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.ppjwa.cn/gtynxogzbm.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.zhijiandao.cn/gtzzzzxttu.html

Ruby: s.reverse
来源：http://hz.yanxiufei.cn/gthxiictnu.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.zhoulong.xyz/gtqnovuvbm.html

[E12] 统计某字符出现次数
来源：http://hz.pengpengdd.cyou/gtlwdbskll.html

Py:   s.count("a")
来源：http://hz.birdmap.top/gtkcsqqotd.html

PHP:  substr_count($s, "a");
来源：http://hz.yanxiufei.cn/gtcbuajymz.html

JS:   s.split("a").length - 1
来源：http://hz.yvedp.cn/gtxyxuzlve.html

TS:   s.split("a").length - 1
来源：http://hz.gzhubu.top/gtoyrrsehf.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.daria6918.cn/gtbqourwzo.html

Go:   strings.Count(s, "a")
来源：http://hz.dashuyun.cn/gtzlgksrze.html

Ruby: s.count("a")
来源：http://hz.jinqigufen.top/gtmyylthzp.html

C#:   s.Count(c => c == 'a')
来源：http://hz.feifeiyinyue.top/gtgpyhzcdj.html

[E13] 逐字符遍历
来源：http://hz.cqqwz.cn/gttsvrzioq.html

Py:   for ch in s: print(ch)
来源：http://hz.yj20258.top/gtfymmfqhz.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.hammf.cn/gtdghqemgw.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.fzhhl.top/gtjblrllrm.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.gotoacloud.top/gtaqnekjfg.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.hnqzz.top/gtqzcakcna.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.hnqzz.top/gtvyrwyafo.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.aibaodan.cn/gtjmrxmcfa.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.jiagoushi.top/gtdbapukjo.html

[E14] URL 编码与 Base64
来源：http://hz.hywenlv.cn/gtxkdwbrru.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.gaohongyu789.top/gtcxlbgfnz.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.vqdsnc.cn/gtcsxypckg.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.sysykeji.top/gtaahtaxph.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.zhijiandao.cn/gtaotxyvqz.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.shanyushiyangtech.top/gtaqlgtjnh.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.fengsongda.top/gtfpedpmok.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.jinqigfzy.top/gtuceirtdm.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.vqdsnc.cn/gtdckbwlci.html

[E15] HTML 转义 / 反转义
来源：http://hz.cqqwz.cn/gtixbkhfcf.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.yvedp.cn/gtdlvnaxoq.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.jianghu66.top/gtyvofzrvm.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.iojbl.cn/gtdtjwyrfp.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.yj202588.top/gtdiyuyyuq.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.yonumen.top/gtwmxhqgyx.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.yueranfly.top/gttdlhmhmf.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.shzxlz.cn/gtercvawhd.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.xuanzx.com/gtgsyiympm.html

[E16] 数字千分位
来源：http://hz.kuanghao11.cn/gtzgalgpwq.html

Py:   f"{1234567:,}"
来源：http://hz.dianchejie.cn/gtmuevdayg.html

PHP:  number_format(1234567);
来源：http://hz.dashuyun.cn/gtgurwruje.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.shuidangran.top/gtppwddpoi.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.xuanzx.com/gthknhsdja.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.yj202588.top/gtzudtrhqh.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.zhongyouzk.top/gtspymvftb.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.chenzaomai.com/gtffxokytz.html

C#:   1234567.ToString("N0")
来源：http://hz.52xcode.cn/gtgnspafdh.html

[E17] 首字母大写
来源：http://hz.cashguo.top/gtixppemro.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.xylfe.cn/gtkqzeoebk.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.iojbl.cn/gtjacyvykt.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.jinghuilouyu.cn/gtwnjegyts.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.jiagoushi.top/gtvguljlbh.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.zhaomingkeji.xyz/gtfxfnzfmi.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.redwolf501.top/gtslfhrxrs.html

Ruby: s.capitalize
来源：http://hz.wangshuangyany.cn/gtqjltnaht.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.hysaishi.cn/gtgvqryjpx.html

[E18] 模板占位符替换
来源：http://hz.ydzc1.top/gtwmcucfsd.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.tanke756.top/gtfdqxdilz.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.gzhubu.top/gticyziqds.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.zdqjudy.top/gtxyjcosju.html


<!-- 参考信息 -->