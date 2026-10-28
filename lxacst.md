代发 wailian999

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.svipenyu.cn/gtmhiztrur.html

JS:   arr.filter(x => x > 3)
来源：http://hz.c1oappe.top/gtumorlkhv.html

TS:   arr.filter(x => x > 3)
来源：http://hz.ppjwa.cn/gtztbveajy.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.hammf.cn/gtjolrzoxz.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.yueranfly.top/gteyeplikd.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.jyoumei.cn/gthhalmjik.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.jinqigfzy.top/gtyzsskbmh.html

[D14] 映射转换（每个元素变形）
来源：http://hz.yj20258.top/gthaqklcbt.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.redwolf501.top/gtstlejbhj.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.gzhubu.top/gthrvrmhgm.html

JS:   arr.map(x => x * 2)
来源：http://hz.haohaochexian.top/gtteytxjyh.html

TS:   arr.map(x => x * 2)
来源：http://hz.hysaishi.cn/gteauzouzp.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.guannengcc.top/gtwsevdcyz.html

Go:   // 手写循环
来源：http://hz.yonumen.top/gturtrxjvf.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.vqdsnc.cn/gtvgxichvs.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.shuidangran.top/gtjjifrzas.html

[D15] 去重
来源：http://hz.sxryk.cn/gtmqbobklm.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.aibaodan.cn/gtketuyjyf.html

PHP:  array_unique($arr);
来源：http://hz.bjfxy.top/gtopkybhml.html

JS:   [...new Set(arr)]
来源：http://hz.tanke756.top/gtpxusqsyu.html

TS:   [...new Set(arr)]
来源：http://hz.52xcode.cn/gtuoibzgyn.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.feifeiyinyue.top/gtdulhisoe.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.yangfankeji.com/gtauvrytbw.html

Ruby: arr.uniq
来源：http://hz.shangyingyoupin.top/gtwgtlvagt.html

C#:   list.Distinct().ToList()
来源：http://hz.hysaishi.cn/gtnblbizdx.html

[D16] 求和与平均值
来源：http://hz.jinqigufen.top/gtrcdpyaao.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.smart0.xyz/gtsalzwirj.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.ywan-chungtsiang.top/gtrbdgibui.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.ivvv.top/gtdxfygphb.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jiagoushi.top/gtrqrmbxfj.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.wangdashe.top/gtllrouorb.html

Go:   // 手写循环累加
来源：http://hz.dianchejie.cn/gtyzscqkiv.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.pengpengdd.cyou/gthmlilcyr.html

C#:   list.Sum();  list.Average()
来源：http://hz.havefunace.top/gtnefstnts.html

[D17] 最大值与最小值
来源：http://hz.xuanzx.com/gtsuxzqede.html

Py:   max(arr);  min(arr)
来源：http://hz.vqdsnc.cn/gtjnkjnrhj.html

PHP:  max($arr);  min($arr);
来源：http://hz.nanxuanxn.top/gtwicpveyn.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.jinqigufen.top/gtzlfevvwr.html

TS:   Math.max(...arr);
来源：http://hz.chenzaomai.com/gtkbrfnsms.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.tianlin.xyz/gtfkicyjfq.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.snrcjt.cn/gtbrfynpzg.html

Ruby: arr.max;  arr.min
来源：http://hz.jinqigufen.top/gtlasdfkla.html

C#:   list.Max();  list.Min()
来源：http://hz.jinghuilouyu.cn/gtdvjhqrcs.html

[D18] 扁平化嵌套数组
来源：http://hz.hammf.cn/gtsjbnbyus.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.yj20258.top/gtifqxaxko.html

PHP:  array_merge(...$nested);
来源：http://hz.hammf.cn/gtxoovjftm.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.gzhubu.top/gtqergdepc.html

TS:   nested.flat();
来源：http://hz.xuanzx.com/gtciuhiouk.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.pengpengdd.cyou/gtcklbwegg.html

Go:   // 手写双层循环
来源：http://hz.shanyushiyangkeji.top/gtmgfauksv.html

Ruby: nested.flatten
来源：http://hz.ydzc1.top/gtrqaoclfy.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.hammf.cn/gtuqjrddak.html

[D19] 按字段分组
来源：http://hz.zhijiandao.cn/gtkfchfekw.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.jinghuilouyu.cn/gtkesoaqip.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.cdnleiting.top/gtbsrqgoen.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.nwbrower.top/gthxcotzir.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.yj20258.top/gtckdtvrld.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.nanxinkj.top/gtpqcmrwlm.html

Go:   // 手写 map[string][]T
来源：http://hz.jlsjyb.cn/gtfxeuehho.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.haohaochexian.top/gtiajadmxm.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.nanxuanxn.top/gtqrtncpcl.html

[D20] 统计每个元素出现次数
来源：http://hz.cashguo.top/gttnzybnam.html

Py:   Counter(arr)
来源：http://hz.smart0.xyz/gtbwlnfzqm.html

PHP:  array_count_values($arr);
来源：http://hz.fzhhl.top/gtkgygesxs.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.cucudq.cn/gtmokizxim.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.shzxlz.cn/gtkbsepijg.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.cucudq.cn/gtxcknydbw.html

Go:   // 手写 map[T]int
来源：http://hz.shanyushiyangkeji.top/gtpwsxvojh.html

Ruby: arr.tally
来源：http://hz.hammf.cn/gtfwxiuhna.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.0kj1m.cn/gtgercnbvo.html

[D21] 判断是否包含某元素
来源：http://hz.zhixingplan.top/gtdgwmwrqj.html

Py:   x in arr
来源：http://hz.yangfankeji.com/gtelvlhtiy.html

PHP:  in_array($x, $arr, true);
来源：http://hz.jinyuanbaomall.cn/gtyzpzfbgq.html

JS:   arr.includes(x)
来源：http://hz.xuetiantiany.cn/gttwdnirui.html

TS:   arr.includes(x)
来源：http://hz.tian-w.cn/gtfcyuakxk.html

Java: list.contains(x)
来源：http://hz.hnqzz.top/gtsjwikxuj.html

Go:   slices.Contains(arr, x)
来源：http://hz.hywenlv.cn/gtuouwvwus.html

Ruby: arr.include?(x)
来源：http://hz.fzhhl.top/gtmuaddhul.html

C#:   list.Contains(x)
来源：http://hz.fzhhl.top/gtonxrufez.html

[D22] 复制数组（避免共享引用）
来源：http://hz.chenzaomai.com/gtrvejxaqu.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.chenjidiqi.icu/gtprmropzk.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.mhx1999.top/gtfexxjkpa.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.ybcxt.top/gtcdswrrpe.html

TS:   [...arr];
来源：http://hz.hammf.cn/gtsjfijzrd.html

Java: new ArrayList<>(list);
来源：http://hz.yj20258888.top/gtysebkdlm.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.zhengqikj.top/gtbgoourdv.html

Ruby: arr.dup;  arr.clone
来源：http://hz.chenlongwang.top/gtzznukpxv.html

C#:   new List<int>(list);
来源：http://hz.haohaochexian.top/gtvvocenqm.html

[D23] reduce 累积计算
来源：http://hz.shanyushiyangkeji.top/gtjoddauhl.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.jinqigfzy.top/gtfmvqwjjn.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.ywan-chungtsiang.top/gtpcvsyqdh.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yuanzhike.top/gtnpcbvnuu.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yuanzhike.top/gtjotsuobo.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.c1oappe.top/gtgrigezpr.html

Go:   // 手写循环
来源：http://hz.svipenyu.cn/gtkyhlhdhk.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.xingfuxueyuan.xyz/gtpxizekxq.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.wangdashe.top/gtzrpnxeeg.html

[D24] 字典 / Map 基本操作
来源：http://hz.ivvv.top/gtgzncohhr.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.iojbl.cn/gtnfnsxvtu.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.dianchejie.cn/gtmkthyqgh.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.yj20258.top/gtmeyaydib.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.wangshuangyany.cn/gtwiruwtqx.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.sufxvd.cn/gtggnqeyuv.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.jqgufenzy.top/gtyygwqxpn.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.vqdsnc.cn/gtvhqnlbdc.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.dianchejie.cn/gtpzbptcah.html

[D25] Set 集合去重与交并差
来源：http://hz.xinyue.icu/gtdzuiqgle.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.zhongyouzk.top/gthsouloxn.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.jlsjyb.cn/gtskvvfgyi.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.yvedp.cn/gtneceoplz.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.hammf.cn/gtkzvjgwgp.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.ppjwa.cn/gtonzdkcwu.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.wangshuangyany.cn/gttrgwjznj.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.hnqzz.top/gtwwxcdtaj.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.jinqigfzy.top/gtymskdphe.html

[D26] 数组转字符串
来源：http://hz.shangyingyoupin.top/gtuxsxyqlf.html

Py:   ", ".join(map(str, arr))
来源：http://hz.chenjidiqi.icu/gtpzkdyxar.html

PHP:  implode(", ", $arr);
来源：http://hz.jyoumei.cn/gtblhnmmlv.html

JS:   arr.join(", ")
来源：http://hz.xuanzx.com/gtzuqdsncq.html

TS:   arr.join(", ")
来源：http://hz.ivvv.top/gtpkbatlyu.html

Java: String.join(", ", list)
来源：http://hz.jiagoushi.top/gtuphipdby.html

Go:   strings.Join(strs, ", ")
来源：http://hz.pengpengdd.cyou/gtlbvyvjit.html

Ruby: arr.join(", ")
来源：http://hz.cqqwz.cn/gtxhsbeotr.html

C#:   string.Join(", ", list)
来源：http://hz.daria6918.cn/gtdldcdzdn.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gttwlstfvi.html

E. 字符串处理
来源：http://hz.pycfn.com/gtngejadgk.html

================================================================================
来源：http://hz.daxiang520.top/gtevwerovh.html

[E01] 拼接字符串
来源：http://hz.jqgfzy.top/gttgzqvibl.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.shangyingyoupin.top/gtbanpjgbi.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.yonumen.top/gtawvnurzs.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jqgufenzy.top/gtupnzprwo.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.zhongyouzk.top/gtxtziceei.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.haohaochexian.top/gtpxtgcqir.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.cucudq.cn/gtlephprpm.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.yj20258888.top/gtntdyzikk.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.yvedp.cn/gtenkgzvok.html

[E02] 重复字符串
来源：http://hz.hywenlv.cn/gtbgetxzwo.html

Py:   "ab" * 3
来源：http://hz.birdmap.top/gtwszmuigy.html

PHP:  str_repeat("ab", 3);
来源：http://hz.aizwys.cn/gtgztoinod.html

JS:   "ab".repeat(3)
来源：http://hz.meibo888.top/gthlbkicgp.html

TS:   "ab".repeat(3)
来源：http://hz.yongpay.top/gtwagznead.html

Java: "ab".repeat(3)
来源：http://hz.cucudq.cn/gtsgizxmdf.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.nanxinkj.top/gtixnhmujz.html

Ruby: "ab" * 3
来源：http://hz.gzhubu.top/gtcwekbrer.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.hongshengwenyu.top/gtzpprjdwg.html

[E03] 截取子串
来源：http://hz.tian-w.cn/gtxkodowlr.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.xuanzx.com/gtefyvymhl.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.hfpthk.cn/gtqlefynbo.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.jinqigfzy.top/gtlqtlqkcf.html

TS:   s.slice(1, 4)
来源：http://hz.redwolf501.top/gtekkyvpie.html

Java: s.substring(1, 4)
来源：http://hz.dianchejie.cn/gtkwdjwysk.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.hywenlv.cn/gtwdfunxfd.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.yueranfly.top/gtezdfnitd.html

C#:   s.Substring(1, 3)
来源：http://hz.hongshengwenyu.top/gtuqoabmjj.html

[E04] 查找子串位置
来源：http://hz.daxiang520.top/gtezdncwvg.html

Py:   s.find("x");  s.index("x")
来源：http://hz.quarkkingdee.top/gtyqxzhlgf.html

PHP:  strpos($s, "x");
来源：http://hz.daxiang520.top/gtnbqqcyxq.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.ppjwa.cn/gtdtwiynvs.html

TS:   s.indexOf("x")
来源：http://hz.zhongyouzk.top/gtvdrggtqm.html

Java: s.indexOf("x")
来源：http://hz.gzhubu.top/gtaqirdism.html

Go:   strings.Index(s, "x")
来源：http://hz.zhoulong.xyz/gtwbgnnkyw.html

Ruby: s.index("x")
来源：http://hz.aizwys.cn/gtsfmeitea.html

C#:   s.IndexOf("x")
来源：http://hz.shangyingyoupin.top/gtlsiltmnm.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.sxryk.cn/gtlasufocw.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.daxiang520.top/gtlbpyemsk.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.gzhubu.top/gtgrztgshz.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.mhx1999.top/gtirrcfabg.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.tian-w.cn/gtqjboospk.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.jiagoushi.top/gtujurmede.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.pycfn.com/gtdeeaparz.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.meibo888.top/gtczlagyoh.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.yueranfly.top/gtaxplrfun.html

[E06] 替换子串
来源：http://hz.daria6918.cn/gtqeslipng.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.zhiwuduotai.top/gtzwkkgloz.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.nanxuanxn.top/gtfqwjcady.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.smart0.xyz/gtznmuazzi.html

TS:   s.replaceAll("a", "b")
来源：http://hz.birdmap.top/gtwocnbphd.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.redwolf501.top/gtqyvnncef.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.hywenlv.cn/gtfmnjsqpl.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.zhengqikj.top/gtukuydthu.html

C#:   s.Replace("a", "b")
来源：http://hz.daria6918.cn/gtffvzgmru.html

[E07] 按分隔符拆分
来源：http://hz.haohaochexian.top/gtucpxnqwy.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.hfpthk.cn/gttghlomnd.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.tanke756.top/gtkwykycld.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.kuanghao11.cn/gtrjlrvgme.html

TS:   s.split(",")
来源：http://hz.sufxvd.cn/gtfzaamrzp.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.pengpengdd.cyou/gtwlsmaaid.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.tanke756.top/gtmsrwazqu.html

Ruby: s.split(",");  s.split
来源：http://hz.jyoumei.cn/gtgfmhvbfl.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.cheryme.top/gtoxohhpju.html

[E08] 数组按分隔符合并
来源：http://hz.fengsongda.top/gteawwcmti.html

Py:   ",".join(items)
来源：http://hz.yongpay.top/gthsjxvxzc.html

PHP:  implode(",", $items);
来源：http://hz.havefunace.top/gtxcrzepns.html

JS:   items.join(",")
来源：http://hz.birdmap.top/gtsqykbohe.html

TS:   items.join(",")
来源：http://hz.mhx1999.top/gtggwpsynu.html

Java: String.join(",", items)
来源：http://hz.ppjwa.cn/gtphhnndfd.html

Go:   strings.Join(items, ",")
来源：http://hz.xuanzx.com/gtnpnsuepa.html

Ruby: items.join(",")
来源：http://hz.sweek.top/gtvducfawm.html

C#:   string.Join(",", items)
来源：http://hz.jiagoushi.top/gtkloiymrt.html

[E09] 去除所有空白字符
来源：http://hz.yj202588.top/gttbgfcwxx.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.chenlongwang.top/gtrhnffggv.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.yj20258888.top/gtsmhbawas.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.daxiang520.top/gtvextptdh.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.ybcxt.top/gtrehnsvrd.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.jlsjyb.cn/gtjjttjgvp.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.yonumen.top/gtieccdpng.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.nanxinkj.top/gtguuiebyg.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.havefunace.top/gtbxtopmqp.html

[E10] 左侧补零 / 定长填充
来源：http://hz.hnxiangtu.top/gtawnepqqx.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.zdqjudy.top/gtafducils.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.nwbrower.top/gtgaqqctsq.html

JS:   "7".padStart(3, "0")
来源：http://hz.316326.xyz/gtsbrzmdcq.html

TS:   "7".padStart(3, "0")
来源：http://hz.smart0.xyz/gtgltroskm.html

Java: String.format("%03d", 7)
来源：http://hz.ydjk.org.cn/gtehoghapo.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.yanxiufei.cn/gtbzfmamju.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.chenlongwang.top/gtajvvzwen.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.hammf.cn/gtueuzuhdi.html

[E11] 反转字符串
来源：http://hz.zdqjudy.top/gtxuamneii.html

Py:   s[::-1]
来源：http://hz.haohaochexian.top/gtxvgibhaz.html

PHP:  strrev($s);
来源：http://hz.bjfxy.top/gtlmdrmnmu.html

JS:   [...s].reverse().join("")
来源：http://hz.gogol.net.cn/gtblefjjvw.html

TS:   [...s].reverse().join("")
来源：http://hz.wangdashe.top/gtzvixqfyo.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.aizwys.cn/gtkqsargvx.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.gotoacloud.top/gtgipozthl.html

Ruby: s.reverse
来源：http://hz.dianchejie.cn/gtpwdbhuzf.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.jiagoushi.top/gtcasejbpu.html

[E12] 统计某字符出现次数
来源：http://hz.ywan-chungtsiang.top/gtgzxarfdv.html

Py:   s.count("a")
来源：http://hz.gzhubu.top/gtiuciwoah.html

PHP:  substr_count($s, "a");
来源：http://hz.jinghuilouyu.cn/gtqentunvg.html

JS:   s.split("a").length - 1
来源：http://hz.vqdsnc.cn/gtzagazihm.html

TS:   s.split("a").length - 1
来源：http://hz.daria6918.cn/gtjcdkkrza.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.hongshengwenyu.top/gtjheddnbg.html

Go:   strings.Count(s, "a")
来源：http://hz.cucudq.cn/gtobldayrz.html

Ruby: s.count("a")
来源：http://hz.nanxinkj.top/gtcvihnbip.html

C#:   s.Count(c => c == 'a')
来源：http://hz.gotoacloud.top/gtbvfwsypo.html

[E13] 逐字符遍历
来源：http://hz.yj20258888.top/gtgjbzezil.html

Py:   for ch in s: print(ch)
来源：http://hz.zycfv.cn/gtlfodzuue.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.hnqzz.top/gtmtsnivun.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.cqqwz.cn/gtipyvswzm.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.chenjidiqi.icu/gtvlrtgsjc.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.aizwys.cn/gtbsqaktks.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.snrcjt.cn/gtqbhlamoi.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.jiagoushi.top/gtbazugaxj.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.gaohongyu789.top/gteqvhuygk.html

[E14] URL 编码与 Base64
来源：http://hz.meibo888.top/gtwdlvhrmr.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.andypj.xyz/gtwkylutmq.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.ydjk.org.cn/gtbjvmukas.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.mhx1999.top/gtgphlzour.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.havefunace.top/gtlvywqtay.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.cdnleiting.top/gtoqaaoaih.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.ivvv.top/gtdyuwsygg.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.shangyingyoupin.top/gtbyyucrou.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.nanxinkj.top/gtwohdtufq.html

[E15] HTML 转义 / 反转义
来源：http://hz.zhaomingkeji.xyz/gtxebbrbja.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.mhx1999.top/gtumpovndi.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.snrcjt.cn/gtcenmlhnk.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.jqgfzy.top/gtdqtjkeik.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.nanxinkj.top/gtmtrdskce.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.hysaishi.cn/gtzcdrtyna.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.dianchejie.cn/gtnzgpwlqo.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.shanyushiyangkeji.top/gtejapibmx.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.quarkkingdee.top/gtohnomzha.html

[E16] 数字千分位
来源：http://hz.sysykeji.top/gtzhccvlxe.html

Py:   f"{1234567:,}"
来源：http://hz.yongpay.top/gtkxhmlviq.html

PHP:  number_format(1234567);
来源：http://hz.cdnleiting.top/gtszwzzbtc.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.nanxuanxn.top/gtsohtidlf.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.xziqi.cn/gtjvselrkd.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.ydjk.org.cn/gtxspzjufh.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.gogol.net.cn/gtjzuuqsxd.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.shanyushiyangtech.top/gtjvdrydvt.html

C#:   1234567.ToString("N0")
来源：http://hz.cashguo.top/gtmhqpbrxo.html

[E17] 首字母大写
来源：http://hz.jinqigfzy.top/gtgoygcjin.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.cashguo.top/gtcjszyimd.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.yueranfly.top/gtvsmmleqp.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.ydzc1.top/gtawwhpshg.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.gzhubu.top/gtatimkkxr.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.xuetiantiany.cn/gtuoxnwvqq.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.tanke756.top/gtjfineept.html

Ruby: s.capitalize
来源：http://hz.chenzaomai.com/gturllgnez.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.xuetiantiany.cn/gtogwoyjbn.html

[E18] 模板占位符替换
来源：http://hz.ppjwa.cn/gtbaqnashz.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.pengpengdd.cyou/gtthpblaly.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.ppjwa.cn/gtlphjtfbw.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.aibaodan.cn/gtzigxglef.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.cheryme.top/gtsbmmmrbm.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.hnqzz.top/gtgppwtoti.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.ydzc1.top/gtsfzogeuw.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.hammf.cn/gtokrhkxva.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.jinqigfzy.top/gtgfumiurx.html

[E19] 多行文本按行拆分
来源：http://hz.9152youxi.cn/gtkqijlyhv.html

Py:   s.splitlines()
来源：http://hz.bjfxy.top/gtaegrpetn.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.zdqjudy.top/gtrbgyanyr.html

JS:   s.split(/\r?\n/)
来源：http://hz.ybcxt.top/gtsntaopen.html

TS:   s.split(/\r?\n/)
来源：http://hz.hongshengwenyu.top/gtzbeqjdwh.html

Java: s.lines().toList()
来源：http://hz.shangyingyoupin.top/gtashxmxrx.html

Go:   strings.Split(s, "\n")
来源：http://hz.gzhubu.top/gtaneenfsp.html

Ruby: s.lines
来源：http://hz.yanxiufei.cn/gtuscrstpz.html

C#:   s.Split('\n')
来源：http://hz.zhoulong.xyz/gtkndzgvyd.html

[E20] 判断字符串是否为空
来源：http://hz.andypj.xyz/gtvziekmex.html

Py:   if not s:
来源：http://hz.yj202588.top/gtrmgkuvix.html


<!-- 参考信息 -->