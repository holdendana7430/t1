代发 wailian999

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.pycfn.com/gtedfghago.html

PHP:  array_merge(...$nested);
来源：http://hz.zhiwuduotai.top/gtexdaowmd.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.andypj.xyz/gttfusunoo.html

TS:   nested.flat();
来源：http://hz.pycfn.com/gtjsjvpuiy.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.vqdsnc.cn/gtdokpijgf.html

Go:   // 手写双层循环
来源：http://hz.gzhubu.top/gtwgmavemu.html

Ruby: nested.flatten
来源：http://hz.fzhhl.top/gtgmtqkiio.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.chenlongwang.top/gtyvhckxrx.html

[D19] 按字段分组
来源：http://hz.nanxinkj.top/gtaloqroij.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.shzxlz.cn/gtjjuunenz.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.haohaochexian.top/gtglschzle.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.jqgfzy.top/gtpyqxubfy.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.sweek.top/gtzyvwwcib.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.shuidangran.top/gtanksyrof.html

Go:   // 手写 map[string][]T
来源：http://hz.zhijiandao.cn/gtrzivtucl.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.hnxiangtu.top/gtusozvqzu.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.zycfv.cn/gtuuuxrggi.html

[D20] 统计每个元素出现次数
来源：http://hz.0kj1m.cn/gtpkxlzcjo.html

Py:   Counter(arr)
来源：http://hz.aizwys.cn/gtmltdltif.html

PHP:  array_count_values($arr);
来源：http://hz.jinqigufen.top/gtrtygqauw.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.xylfe.cn/gteuaukniw.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.sxryk.cn/gtuifnysfb.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.fzhhl.top/gtaudmolzw.html

Go:   // 手写 map[T]int
来源：http://hz.yj20258888.top/gteurenrvh.html

Ruby: arr.tally
来源：http://hz.yj20258888.top/gtktrozidd.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.haohaochexian.top/gtcfnzapbh.html

[D21] 判断是否包含某元素
来源：http://hz.hammf.cn/gtuwbromag.html

Py:   x in arr
来源：http://hz.yongpay.top/gtyazyygud.html

PHP:  in_array($x, $arr, true);
来源：http://hz.meibo888.top/gtgzzyvfsp.html

JS:   arr.includes(x)
来源：http://hz.sweek.top/gttmjgwxie.html

TS:   arr.includes(x)
来源：http://hz.fengsongda.top/gtuzispvay.html

Java: list.contains(x)
来源：http://hz.yuanzhike.top/gtzviovqke.html

Go:   slices.Contains(arr, x)
来源：http://hz.jqgfzy.top/gtglhzysxh.html

Ruby: arr.include?(x)
来源：http://hz.jinghuilouyu.cn/gtxmtckerw.html

C#:   list.Contains(x)
来源：http://hz.vqdsnc.cn/gtcqteqkji.html

[D22] 复制数组（避免共享引用）
来源：http://hz.meibo888.top/gtojnrakgj.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.yj202588.top/gttqolablx.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.sufxvd.cn/gthvuqqxzy.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.yvedp.cn/gttoebfpbp.html

TS:   [...arr];
来源：http://hz.c1oappe.top/gtrjlgpazy.html

Java: new ArrayList<>(list);
来源：http://hz.snrcjt.cn/gtwcqyochk.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.jinyuanbaomall.cn/gtvkxdbvgs.html

Ruby: arr.dup;  arr.clone
来源：http://hz.tianlin.xyz/gtvrnihpgi.html

C#:   new List<int>(list);
来源：http://hz.hnxiangtu.top/gtjkgaitbq.html

[D23] reduce 累积计算
来源：http://hz.dashuyun.cn/gtbpilnmeg.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.gaohongyu789.top/gtemgcbmbq.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.tianlin.xyz/gtmcnanaqy.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.guannengcc.top/gtigwtvjwm.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.vqdsnc.cn/gtpwibvgpy.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.xylfe.cn/gththacgqc.html

Go:   // 手写循环
来源：http://hz.zhaomingkeji.xyz/gtqkcqsjct.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.hysaishi.cn/gtdrpspznk.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.jiagoushi.top/gtoprkcymg.html

[D24] 字典 / Map 基本操作
来源：http://hz.fzhhl.top/gthdfyxxtv.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.xuanzx.com/gtxgqzmvyj.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.tanke756.top/gtdzzodliq.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.xuetiantiany.cn/gtktrlgzak.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.yonumen.top/gtsmpzgrrw.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.mhx1999.top/gtoabwmdvr.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.jlsjyb.cn/gtgmaeaxje.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.meibo888.top/gtsvmwepxm.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.iojbl.cn/gtdrpysbej.html

[D25] Set 集合去重与交并差
来源：http://hz.yj20258888.top/gtzdbmekwo.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.feifeiyinyue.top/gtluhfqgux.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.hfpthk.cn/gtcjptvmfm.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.zhixingplan.top/gtaqrpznkm.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.shanyushiyangkeji.top/gtzrygybxe.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.daria6918.cn/gtaomkxydg.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.gzhubu.top/gtfgxqkrrq.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.shuidangran.top/gthuleeysb.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.zhijiandao.cn/gthivvcldq.html

[D26] 数组转字符串
来源：http://hz.shanyushiyangtech.top/gtuhesnflv.html

Py:   ", ".join(map(str, arr))
来源：http://hz.aibaodan.cn/gtradsszfa.html

PHP:  implode(", ", $arr);
来源：http://hz.yj20258.top/gtsnuruuvq.html

JS:   arr.join(", ")
来源：http://hz.ivvv.top/gtaivykakf.html

TS:   arr.join(", ")
来源：http://hz.wangdashe.top/gtkbgdqtpg.html

Java: String.join(", ", list)
来源：http://hz.aibaodan.cn/gtgcnzppgp.html

Go:   strings.Join(strs, ", ")
来源：http://hz.ppjwa.cn/gthqlxkdrz.html

Ruby: arr.join(", ")
来源：http://hz.birdmap.top/gtarzeriui.html

C#:   string.Join(", ", list)
来源：http://hz.zhiwuduotai.top/gtqxkzculs.html

================================================================================
来源：http://hz.guowangkeji.top/gtnmqsqdjb.html

E. 字符串处理
来源：http://hz.andypj.xyz/gtijcormhg.html

================================================================================
来源：http://hz.jyoumei.cn/gtbyjqtycp.html

[E01] 拼接字符串
来源：http://hz.zhaomingkeji.xyz/gtahmsoaym.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.zdqjudy.top/gtiysckdjy.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.vqdsnc.cn/gtnspbovjf.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.gogol.net.cn/gtnmoaryyw.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.iojbl.cn/gthcbgvgbt.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.gotoacloud.top/gtzuqradmh.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.cashguo.top/gtkosanqff.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.ywan-chungtsiang.top/gtzvaxshul.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.xuetiantiany.cn/gthycopznw.html

[E02] 重复字符串
来源：http://hz.xingfuxueyuan.xyz/gtktkukckz.html

Py:   "ab" * 3
来源：http://hz.yuxming.cn/gtdqkuumkm.html

PHP:  str_repeat("ab", 3);
来源：http://hz.chenlongwang.top/gtzqpkpzwd.html

JS:   "ab".repeat(3)
来源：http://hz.jyoumei.cn/gtcacuwdwg.html

TS:   "ab".repeat(3)
来源：http://hz.jiagoushi.top/gtkidadgaa.html

Java: "ab".repeat(3)
来源：http://hz.hfpthk.cn/gtchinuxsu.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.nwbrower.top/gtdilcwxzw.html

Ruby: "ab" * 3
来源：http://hz.redwolf501.top/gtbhxoxbit.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.fzhhl.top/gtqnnqbbih.html

[E03] 截取子串
来源：http://hz.xinyue.icu/gtajlzrwro.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.yueranfly.top/gtoucaehmf.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.bjfxy.top/gtztgqolhm.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.yuanzhike.top/gtstbypnje.html

TS:   s.slice(1, 4)
来源：http://hz.316326.xyz/gthmddiqzt.html

Java: s.substring(1, 4)
来源：http://hz.haohaochexian.top/gtqwnvnmtn.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.nwbrower.top/gtqjkwtusj.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.zhijiandao.cn/gthhdffhlu.html

C#:   s.Substring(1, 3)
来源：http://hz.shanyushiyangtech.top/gthyfsnocj.html

[E04] 查找子串位置
来源：http://hz.jinqigfzy.top/gtqsahpcoh.html

Py:   s.find("x");  s.index("x")
来源：http://hz.jqgfzy.top/gtuaxwqpnd.html

PHP:  strpos($s, "x");
来源：http://hz.shuidangran.top/gtasmfhrza.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.quarkkingdee.top/gtiufsodjg.html

TS:   s.indexOf("x")
来源：http://hz.nanxuanxn.top/gttevygsfe.html

Java: s.indexOf("x")
来源：http://hz.zhaomingkeji.xyz/gtgmzuoxwq.html

Go:   strings.Index(s, "x")
来源：http://hz.dashuyun.cn/gtwpsmszsq.html

Ruby: s.index("x")
来源：http://hz.wangshuangyany.cn/gthrpyhxvq.html

C#:   s.IndexOf("x")
来源：http://hz.havefunace.top/gtdbeufcvn.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.dashuyun.cn/gtcaxhusbr.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.xingfuxueyuan.xyz/gtkjcacviy.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.nwbrower.top/gtvcrsszwf.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.snrcjt.cn/gtaorxbgbz.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.snrcjt.cn/gtdxjsgtqd.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.xinyue.icu/gtwtipojyh.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.hnxiangtu.top/gtxxqglokt.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.zhaomingkeji.xyz/gtjyqwqghc.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.zhoulong.xyz/gtxbghwuaa.html

[E06] 替换子串
来源：http://hz.cdnleiting.top/gtfnsorywk.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.fengsongda.top/gtbtsxomnf.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.c1oappe.top/gtnacocies.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.havefunace.top/gtkmvudvsg.html

TS:   s.replaceAll("a", "b")
来源：http://hz.pycfn.com/gtpeqggljh.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.0kj1m.cn/gtneozgjee.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.sufxvd.cn/gtmhhtuhlu.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.ivvv.top/gtjfjqebye.html

C#:   s.Replace("a", "b")
来源：http://hz.yangfankeji.com/gtrtxublhz.html

[E07] 按分隔符拆分
来源：http://hz.zycfv.cn/gtjynalgdd.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.sxryk.cn/gtfdlndljk.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.zhiwuduotai.top/gtdrdjsshk.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.zycfv.cn/gtvxnsfigv.html

TS:   s.split(",")
来源：http://hz.wangdashe.top/gtfglgrrch.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.iojbl.cn/gtxqvobsyl.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.dianchejie.cn/gtuznjpmjw.html

Ruby: s.split(",");  s.split
来源：http://hz.kuanghao11.cn/gtxlcbjhsk.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.tian-w.cn/gtjqfsntpk.html

[E08] 数组按分隔符合并
来源：http://hz.nwbrower.top/gtihidivyq.html

Py:   ",".join(items)
来源：http://hz.hfpthk.cn/gtxxpbkrpl.html

PHP:  implode(",", $items);
来源：http://hz.0kj1m.cn/gtxwynqsgk.html

JS:   items.join(",")
来源：http://hz.jinqigufen.top/gtdwgannem.html

TS:   items.join(",")
来源：http://hz.birdmap.top/gtvdtwerbs.html

Java: String.join(",", items)
来源：http://hz.haohaochexian.top/gtpjhofnff.html

Go:   strings.Join(items, ",")
来源：http://hz.jiagoushi.top/gtjzdhmhkz.html

Ruby: items.join(",")
来源：http://hz.jyoumei.cn/gtqzllcarb.html

C#:   string.Join(",", items)
来源：http://hz.cucudq.cn/gtkkaovwsl.html

[E09] 去除所有空白字符
来源：http://hz.jinqigufen.top/gtxhlzvfbq.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.shanyushiyangkeji.top/gtuiygagfx.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.chenjidiqi.icu/gtocentjnt.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.ybcxt.top/gtexnltuqe.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.iojbl.cn/gtulxavepd.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.hywenlv.cn/gtrkcpjmfz.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.0kj1m.cn/gtakhwckmg.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.hywenlv.cn/gttopdgctm.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.yanxiufei.cn/gtpsllrkky.html

[E10] 左侧补零 / 定长填充
来源：http://hz.zhixingplan.top/gtukffmgtl.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.fzhhl.top/gtxhnvwbee.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.zycfv.cn/gtiwyuhdjh.html

JS:   "7".padStart(3, "0")
来源：http://hz.yj20258888.top/gtllmpkpus.html

TS:   "7".padStart(3, "0")
来源：http://hz.zhongyouzk.top/gtulndepdy.html

Java: String.format("%03d", 7)
来源：http://hz.wangdashe.top/gthqovupee.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.jinyuanbaomall.cn/gtetdlfxav.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.gotoacloud.top/gttkcjfdbc.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.daxiang520.top/gtucgafroo.html

[E11] 反转字符串
来源：http://hz.yangfankeji.com/gtyrawcmut.html

Py:   s[::-1]
来源：http://hz.chenzaomai.com/gtzuxzfzdd.html

PHP:  strrev($s);
来源：http://hz.xylfe.cn/gtpaoloytj.html

JS:   [...s].reverse().join("")
来源：http://hz.nanxinkj.top/gtlcnlmurx.html

TS:   [...s].reverse().join("")
来源：http://hz.ivvv.top/gtnfcvarjt.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.guannengcc.top/gtljfuqxyo.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.yueranfly.top/gtzujihkjs.html

Ruby: s.reverse
来源：http://hz.yongpay.top/gtmdreeqdo.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.fzhhl.top/gtfjbljwoz.html

[E12] 统计某字符出现次数
来源：http://hz.dashuyun.cn/gtgfrexnuf.html

Py:   s.count("a")
来源：http://hz.yj202588.top/gtwctgpclr.html

PHP:  substr_count($s, "a");
来源：http://hz.havefunace.top/gthxgohnsg.html

JS:   s.split("a").length - 1
来源：http://hz.gotoacloud.top/gtoeyinlnj.html

TS:   s.split("a").length - 1
来源：http://hz.jiagoushi.top/gtiuhynlth.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.daria6918.cn/gtrfsodhzs.html

Go:   strings.Count(s, "a")
来源：http://hz.andypj.xyz/gtkxbbyisg.html

Ruby: s.count("a")
来源：http://hz.feifeiyinyue.top/gtgdyccaqz.html

C#:   s.Count(c => c == 'a')
来源：http://hz.gaohongyu789.top/gtlmvunszi.html

[E13] 逐字符遍历
来源：http://hz.yuxming.cn/gtqnioudzd.html

Py:   for ch in s: print(ch)
来源：http://hz.ivvv.top/gtzfzosoqu.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.ppjwa.cn/gtzfaeoxgi.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yanxiufei.cn/gtokaubuxs.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yuxming.cn/gtzsbzdpav.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.jinqigfzy.top/gtxziohhoj.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.shanyushiyangtech.top/gtyfahhrbg.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.cucudq.cn/gtxqlaxmyc.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.wangshuangyany.cn/gtbleqycsn.html

[E14] URL 编码与 Base64
来源：http://hz.c1oappe.top/gtlvgzuuqf.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.nanxinkj.top/gtuyzqcpxw.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.vqdsnc.cn/gtbbgzxcnd.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.xinyue.icu/gtvyoyxknj.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.shzxlz.cn/gtwxhkhhjb.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.jinqigfzy.top/gtrrxzyegt.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.hfpthk.cn/gttburncoz.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.ywan-chungtsiang.top/gtjilojwws.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.yangfankeji.com/gtqklgpzia.html

[E15] HTML 转义 / 反转义
来源：http://hz.jinghuilouyu.cn/gtikwifhfj.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.nwbrower.top/gthhouncqv.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.mhx1999.top/gtwlikmwvu.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.ybcxt.top/gtwfsfplfl.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.yueranfly.top/gtovgqhxfd.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.zycfv.cn/gtutsibgby.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.sxryk.cn/gthgtuinrj.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.ehwqpu.com/gtyktgtbjs.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.smart0.xyz/gtpmkjqeff.html

[E16] 数字千分位
来源：http://hz.zhengqikj.top/gtucnzfcnr.html

Py:   f"{1234567:,}"
来源：http://hz.xuanzx.com/gtjogjbsiw.html

PHP:  number_format(1234567);
来源：http://hz.hnqzz.top/gtfsrjovgs.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.aizwys.cn/gtilgvcikh.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.zhengqikj.top/gtilkillds.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.smart0.xyz/gtvxjygbbs.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.pycfn.com/gtieshneit.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.yonumen.top/gtqtbvkske.html

C#:   1234567.ToString("N0")
来源：http://hz.dashuyun.cn/gtdtpohmvp.html

[E17] 首字母大写
来源：http://hz.yongpay.top/gticgezhpz.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.zhengqikj.top/gtpkzyrcdz.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.jinyuanbaomall.cn/gtpcbuxdju.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.chenzaomai.com/gtlblawmxh.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.snrcjt.cn/gtmfizvmwc.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.yvedp.cn/gtuaujpeyt.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.svipenyu.cn/gtofvhngix.html

Ruby: s.capitalize
来源：http://hz.feifeiyinyue.top/gtlyxwnsea.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.gotoacloud.top/gtyysnmimx.html

[E18] 模板占位符替换
来源：http://hz.cashguo.top/gtujgabxgw.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.cashguo.top/gtzdcskpuv.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.havefunace.top/gtgvqhcmid.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.hnxiangtu.top/gthcyfiicg.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.xinyue.icu/gtvtumkqfd.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.ppjwa.cn/gtkfodbqld.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.zycfv.cn/gtzmornhuk.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.nanxuanxn.top/gtonbokgpy.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.aizwys.cn/gtipjqpxmg.html

[E19] 多行文本按行拆分
来源：http://hz.zhaomingkeji.xyz/gtucitmqpf.html

Py:   s.splitlines()
来源：http://hz.yvedp.cn/gtfpdgqdlr.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.cqqwz.cn/gtzzdpwvnm.html

JS:   s.split(/\r?\n/)
来源：http://hz.xuanzx.com/gtbxkvmvcu.html

TS:   s.split(/\r?\n/)
来源：http://hz.mhx1999.top/gthtwkndpu.html

Java: s.lines().toList()
来源：http://hz.hywenlv.cn/gtiomvevux.html

Go:   strings.Split(s, "\n")
来源：http://hz.chenzaomai.com/gtxotiaaoa.html

Ruby: s.lines
来源：http://hz.jianghu66.top/gtniypipga.html

C#:   s.Split('\n')
来源：http://hz.hfpthk.cn/gtxhlbprqf.html

[E20] 判断字符串是否为空
来源：http://hz.sweek.top/gtbhgrswgx.html

Py:   if not s:
来源：http://hz.jinyuanbaomall.cn/gtgnvcbcsx.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.snrcjt.cn/gtgjfwqmuv.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.nanxinkj.top/gtzkcjitks.html

TS:   if (s === "") {}
来源：http://hz.meibo888.top/gtqvrmxxid.html

Java: if (s.isEmpty()) {}
来源：http://hz.cucudq.cn/gtkjjhdbnr.html

Go:   if s == "" {}
来源：http://hz.xylfe.cn/gttqnipikw.html

Ruby: if s.empty?
来源：http://hz.ppjwa.cn/gtbgpqozkj.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.sweek.top/gtxgtduqvg.html

[E21] 超长截断加省略号
来源：http://hz.pengpengdd.cyou/gtqjrkkbwo.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.chenlongwang.top/gtfqkwxhbe.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.9152youxi.cn/gtpqlhelgr.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.shuidangran.top/gthkagujax.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.cdnleiting.top/gttgchzfmv.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.yangfankeji.com/gtullavyep.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.zhijiandao.cn/gtzvkbvzrv.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.xinyue.icu/gtvfdxejij.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.vqdsnc.cn/gttgmerqvf.html

[E22] 字节长度与字符长度
来源：http://hz.bjfxy.top/gtnrgkvfir.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.shuidangran.top/gtbbswdake.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.kuanghao11.cn/gtmxnvwltd.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yangfankeji.com/gthkcedjla.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jinqigfzy.top/gtdjgvwjbw.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.fzhhl.top/gteokxzqur.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.andypj.xyz/gtfewaxstu.html

Ruby: s.bytesize;  s.length
来源：http://hz.meibo888.top/gtpovtokqb.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.jyoumei.cn/gtcjiyklsa.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtydjjiemx.html

F. 文件与目录
来源：http://hz.birdmap.top/gtfuiohxfm.html

================================================================================
来源：http://hz.c1oappe.top/gttezbckak.html

[F01] 读取整个文件
来源：http://hz.zycfv.cn/gtaxmzeuuu.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.dashuyun.cn/gtcdrvmcvi.html

PHP:  file_get_contents("a.txt");
来源：http://hz.mhx1999.top/gthnrynklm.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.yangfankeji.com/gtfowfpoox.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.svipenyu.cn/gtfxefdohj.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.chenlongwang.top/gtqftsefoj.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.gogol.net.cn/gtcdzxvxsk.html

Ruby: File.read("a.txt")
来源：http://hz.haohaochexian.top/gtldwuoxjk.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.yvedp.cn/gtmakeymzd.html

[F02] 逐行读取文件
来源：http://hz.snrcjt.cn/gtuondvkji.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.iojbl.cn/gtkfrxhvxy.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.svipenyu.cn/gtsfunpnlp.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.havefunace.top/gtuxlvxfbq.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.jinqigfzy.top/gtfenqygie.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.ywan-chungtsiang.top/gtawtfkkeb.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.guowangkeji.top/gtnqwcghkk.html


<!-- 参考信息 -->