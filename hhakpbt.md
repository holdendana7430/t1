代发 wailian999

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.zdbjq.cn/Article/details/gghfgkwgm.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.hesvh.cn/Article/details/gtnrsnltt.sHtML

Java: // 无解构
来源：http://wap.hesvh.cn/Article/details/gbgmufgyu.sHtML

Go:   // 无解构
来源：http://blog.hesvh.cn/Article/details/guztqwfvb.sHtML

Ruby: a, b = pair
来源：http://www.share.zdbjq.cn/Article/details/gkdvqsboe.sHtML

C#:   var (a, b) = pair;
来源：http://blog.hesvh.cn/Article/details/gujuzjcat.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.hesvh.cn/Article/details/gptunbqap.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.hesvh.cn/Article/details/gzljlaizt.sHtML

PHP:  // 无重载
来源：http://baike.zdbjq.cn/Article/details/gyodkgtlg.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.hesvh.cn/Article/details/gcnsnnhqj.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.hesvh.cn/Article/details/grcinkqoo.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.fehbvm.com/Article/details/gicpfjqhi.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.fehbvm.com/Article/details/gvpkehvxk.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.hesvh.cn/Article/details/guxadcbdb.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.hesvh.cn/Article/details/gimkisgem.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/geftupdxd.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.hesvh.cn/Article/details/grtuozvjh.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gfbpsxacg.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.fehbvm.com/Article/details/grfcsbfwp.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.hesvh.cn/Article/details/gsiywcezv.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.hesvh.cn/Article/details/gbziroakz.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.hesvh.cn/Article/details/gdvmaxnrw.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.hesvh.cn/Article/details/gyliyddzp.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.zdbjq.cn/Article/details/gbqrvnumz.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.hesvh.cn/Article/details/gacigsxdf.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.hesvh.cn/Article/details/gdfrebyqn.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.hesvh.cn/Article/details/gpwgicijf.sHtML

[D02] 追加元素到末尾
来源：http://baike.zdbjq.cn/Article/details/gkuybqxcd.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.zdbjq.cn/Article/details/ghesteeir.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.hesvh.cn/Article/details/gxlorbmkm.sHtML

JS:   arr.push(4);
来源：http://baike.zdbjq.cn/Article/details/ghbzsfkgq.sHtML

TS:   arr.push(4);
来源：http://blog.zdbjq.cn/Article/details/glvccuobk.sHtML

Java: list.add(4);
来源：http://www.share.zdbjq.cn/Article/details/ghiiyjhof.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.zdbjq.cn/Article/details/gjokbbhnr.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.zdbjq.cn/Article/details/glzhfjwey.sHtML

C#:   list.Add(4);
来源：http://www.blog.hesvh.cn/Article/details/gedkborsa.sHtML

[D03] 在指定位置插入元素
来源：http://3g.hesvh.cn/Article/details/gwjivjypl.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.fehbvm.com/Article/details/gsfciynbc.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.fehbvm.com/Article/details/gdepsqhdg.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.hesvh.cn/Article/details/gmcnpyqwj.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gtjshnimg.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gmkzqtjls.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.fehbvm.com/Article/details/gusnmmela.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.hesvh.cn/Article/details/gapkpjdvc.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gquarogmd.sHtML

[D04] 删除元素
来源：http://3g.fehbvm.com/Article/details/gzblzzwxl.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.hesvh.cn/Article/details/gvdvhksyu.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.fehbvm.com/Article/details/gpdhahesl.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.zdbjq.cn/Article/details/gvjywnmok.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.zdbjq.cn/Article/details/gggpgijil.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.zdbjq.cn/Article/details/govphdoya.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.zdbjq.cn/Article/details/gyxnndlsm.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.fehbvm.com/Article/details/gwtjjhhrs.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.hesvh.cn/Article/details/gzzddnkvh.sHtML

[D05] 访问与修改元素
来源：http://www.blog.hesvh.cn/Article/details/gxnwozvpo.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/gqsivsiwd.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/gkxoeofjo.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.fehbvm.com/Article/details/gfxkjvlbk.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.hesvh.cn/Article/details/gjewmhmsz.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.hesvh.cn/Article/details/gzpegijbo.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/gihsfruzt.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/growybpzt.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/gbaqbxvzv.sHtML

[D06] 数组长度
来源：http://www.m.share.fehbvm.com/Article/details/gmbtkneor.sHtML

Py:   len(arr)
来源：http://read.share.zdbjq.cn/Article/details/gzmyyqlyk.sHtML

PHP:  count($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/geisrerev.sHtML

JS:   arr.length
来源：http://blog.fehbvm.com/Article/details/gserpnztq.sHtML

TS:   arr.length
来源：http://baike.hesvh.cn/Article/details/graeijwdx.sHtML

Java: list.size();
来源：http://www.share.hesvh.cn/Article/details/gwydcgxpo.sHtML

Go:   len(arr)
来源：http://3g.zdbjq.cn/Article/details/gqadpdbzs.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.zdbjq.cn/Article/details/guisleqjs.sHtML

C#:   list.Count;
来源：http://www.share.hesvh.cn/Article/details/gnfhofrir.sHtML

[D07] 切片 / 取子数组
来源：http://blog.hesvh.cn/Article/details/gtewahaxk.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.zdbjq.cn/Article/details/goovdkrdr.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.fehbvm.com/Article/details/gasdkyjuh.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.hesvh.cn/Article/details/gapzgvrpi.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.hesvh.cn/Article/details/gbbkltymh.sHtML

Java: list.subList(1, 4);
来源：http://baike.hesvh.cn/Article/details/gkwybmssg.sHtML

Go:   arr[1:4]
来源：http://blog.fehbvm.com/Article/details/gwgbsnziw.sHtML

Ruby: arr[1, 3]
来源：http://m.share.fehbvm.com/Article/details/ghstlhpue.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gmelfyzdm.sHtML

[D08] 合并两个数组
来源：http://baike.hesvh.cn/Article/details/gztjxmxzz.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.fehbvm.com/Article/details/gyxifmqlu.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.zdbjq.cn/Article/details/gqtfgttxr.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.hesvh.cn/Article/details/gdoimwgwi.sHtML

TS:   [...a, ...b];
来源：http://baike.hesvh.cn/Article/details/gshmxgoxc.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.hesvh.cn/Article/details/gvnlzfjlv.sHtML

Go:   append(a, b...)
来源：http://www.blog.fehbvm.com/Article/details/gfaulytyd.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.fehbvm.com/Article/details/gqhurfhpg.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.hesvh.cn/Article/details/gsqllvltn.sHtML

[D09] 排序（升序）
来源：http://www.share.zdbjq.cn/Article/details/gitnefdgf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fehbvm.com/Article/details/gauosgsol.sHtML

PHP:  sort($arr);
来源：http://wap.zdbjq.cn/Article/details/gubwatrte.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.hesvh.cn/Article/details/ghkkburgo.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.zdbjq.cn/Article/details/gkspvwssi.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.fehbvm.com/Article/details/garbfzzjb.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.hesvh.cn/Article/details/gdsyxgwvn.sHtML

Ruby: arr.sort
来源：http://www.m.share.hesvh.cn/Article/details/ghymmcqri.sHtML

C#:   list.Sort();
来源：http://m.share.hesvh.cn/Article/details/gxdoeavwk.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.zdbjq.cn/Article/details/gwsjpogyf.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.hesvh.cn/Article/details/ghtdfwlae.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fehbvm.com/Article/details/gpyoboonf.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.zdbjq.cn/Article/details/gohywmtfp.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.zdbjq.cn/Article/details/gcqnrjyup.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.fehbvm.com/Article/details/gwapyoifz.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.zdbjq.cn/Article/details/gyxlxpnob.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.zdbjq.cn/Article/details/gaqsheikg.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.hesvh.cn/Article/details/grufajrja.sHtML

[D11] 反转数组
来源：http://www.m.share.fehbvm.com/Article/details/gjxrolttf.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.fehbvm.com/Article/details/giglnqsfm.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gsqvsqkcl.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.fehbvm.com/Article/details/gcifjfxui.sHtML

TS:   [...arr].reverse();
来源：http://3g.hesvh.cn/Article/details/gscnllhrj.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.hesvh.cn/Article/details/gynyzzams.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.fehbvm.com/Article/details/gytlqiohe.sHtML

Ruby: arr.reverse
来源：http://blog.zdbjq.cn/Article/details/gpitghugg.sHtML

C#:   list.Reverse();
来源：http://read.share.hesvh.cn/Article/details/gbdrfsbhn.sHtML

[D12] 查找元素下标
来源：http://read.share.hesvh.cn/Article/details/gpefqfnmt.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.fehbvm.com/Article/details/gojfurcnd.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.zdbjq.cn/Article/details/gmeyhtbyf.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.zdbjq.cn/Article/details/glmlptmdc.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.hesvh.cn/Article/details/gqhzpjzke.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.hesvh.cn/Article/details/gjczxwchk.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.hesvh.cn/Article/details/glhszodml.sHtML

Ruby: arr.index(x)
来源：http://www.blog.zdbjq.cn/Article/details/gzfgsszue.sHtML

C#:   list.IndexOf(x);
来源：http://wap.zdbjq.cn/Article/details/gchpnmclq.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.fehbvm.com/Article/details/guikzpxoj.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.fehbvm.com/Article/details/gglmhvhdm.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.hesvh.cn/Article/details/gxkmwdagc.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.hesvh.cn/Article/details/gebjngnem.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.hesvh.cn/Article/details/gtdtlxabx.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.zdbjq.cn/Article/details/ggpswmzau.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.hesvh.cn/Article/details/gucyaihlx.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.zdbjq.cn/Article/details/gcailorsq.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.fehbvm.com/Article/details/gobpzxqsv.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.zdbjq.cn/Article/details/gatogrbtk.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.hesvh.cn/Article/details/gfnjvuldc.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.hesvh.cn/Article/details/grnjddpqa.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.zdbjq.cn/Article/details/gmitfgqec.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.fehbvm.com/Article/details/gsboduuqj.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.fehbvm.com/Article/details/grlcpsvwg.sHtML

Go:   // 手写循环
来源：http://www.m.share.zdbjq.cn/Article/details/gxaqupiir.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gvxkheusk.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.fehbvm.com/Article/details/gkmyxmjto.sHtML

[D15] 去重
来源：http://read.share.fehbvm.com/Article/details/gkhzmdnzj.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.zdbjq.cn/Article/details/gmyshcxus.sHtML

PHP:  array_unique($arr);
来源：http://baike.zdbjq.cn/Article/details/grascixvs.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/gejuagmrj.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/gntptzsua.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.fehbvm.com/Article/details/goycccsuu.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.hesvh.cn/Article/details/gmygbrisi.sHtML

Ruby: arr.uniq
来源：http://wap.hesvh.cn/Article/details/gptqrvgiq.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.fehbvm.com/Article/details/ghccubzwl.sHtML

[D16] 求和与平均值
来源：http://wap.fehbvm.com/Article/details/gqvdaxowh.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.fehbvm.com/Article/details/gvbquvlhz.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.fehbvm.com/Article/details/ghyytfbca.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fehbvm.com/Article/details/gmretzwlb.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.hesvh.cn/Article/details/gdvjkzmws.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.zdbjq.cn/Article/details/gyfzxywkz.sHtML

Go:   // 手写循环累加
来源：http://wap.fehbvm.com/Article/details/gewchvoal.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.zdbjq.cn/Article/details/guqhnmfvc.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.hesvh.cn/Article/details/gadubrrlp.sHtML

[D17] 最大值与最小值
来源：http://wap.zdbjq.cn/Article/details/gezbhtdpe.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.zdbjq.cn/Article/details/gaxkblwoz.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.fehbvm.com/Article/details/gsshwiivu.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.hesvh.cn/Article/details/gnpfmhkau.sHtML

TS:   Math.max(...arr);
来源：http://mobile.hesvh.cn/Article/details/gfudhvqdj.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.zdbjq.cn/Article/details/guxviwxta.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.zdbjq.cn/Article/details/gksjdvnqs.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.fehbvm.com/Article/details/geqogfagc.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.fehbvm.com/Article/details/gtajkzoog.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.fehbvm.com/Article/details/grqdfulsy.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.fehbvm.com/Article/details/gfdjynxbd.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.fehbvm.com/Article/details/ggqkzvwjp.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.hesvh.cn/Article/details/guuplvhvk.sHtML

TS:   nested.flat();
来源：http://www.blog.fehbvm.com/Article/details/gjjvjdheo.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.zdbjq.cn/Article/details/gkizovdes.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.fehbvm.com/Article/details/gbgvtnvhq.sHtML

Ruby: nested.flatten
来源：http://www.m.share.zdbjq.cn/Article/details/gobsqqhkl.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gtcbarfbw.sHtML

[D19] 按字段分组
来源：http://www.blog.hesvh.cn/Article/details/gpjqhzzep.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.fehbvm.com/Article/details/gaitlzawg.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.zdbjq.cn/Article/details/gjlfgeiyd.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.hesvh.cn/Article/details/gybdadzlu.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.hesvh.cn/Article/details/glyffjmml.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.fehbvm.com/Article/details/gmahmaftl.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.zdbjq.cn/Article/details/gsztwqyza.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.zdbjq.cn/Article/details/gejwmzuiu.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.hesvh.cn/Article/details/gsjuikkbv.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.fehbvm.com/Article/details/ghgneycxf.sHtML

Py:   Counter(arr)
来源：http://baike.fehbvm.com/Article/details/gboqyfybi.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.fehbvm.com/Article/details/gwwsjgium.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.hesvh.cn/Article/details/gtqvjhdmu.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.hesvh.cn/Article/details/gzdshpdzk.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.fehbvm.com/Article/details/gntpywumm.sHtML

Go:   // 手写 map[T]int
来源：http://blog.hesvh.cn/Article/details/gsiddnmfc.sHtML

Ruby: arr.tally
来源：http://www.blog.zdbjq.cn/Article/details/gqsgbmrls.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.zdbjq.cn/Article/details/ggvcgoxvq.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.hesvh.cn/Article/details/gbqqfdwbr.sHtML

Py:   x in arr
来源：http://mobile.zdbjq.cn/Article/details/gllaqsqss.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.fehbvm.com/Article/details/gntwnhfcn.sHtML

JS:   arr.includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gocuuitro.sHtML

TS:   arr.includes(x)
来源：http://3g.zdbjq.cn/Article/details/gknrjncpw.sHtML

Java: list.contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gqqswunyv.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.fehbvm.com/Article/details/gcmjgplvn.sHtML

Ruby: arr.include?(x)
来源：http://3g.fehbvm.com/Article/details/gegtfoqfr.sHtML

C#:   list.Contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gpisahxnw.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.hesvh.cn/Article/details/gkyzovonk.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.fehbvm.com/Article/details/gjbwzubge.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.zdbjq.cn/Article/details/gozuhknqd.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.hesvh.cn/Article/details/ggfccrzow.sHtML

TS:   [...arr];
来源：http://www.share.hesvh.cn/Article/details/gdjnmntgi.sHtML

Java: new ArrayList<>(list);
来源：http://3g.fehbvm.com/Article/details/gkcllnwmw.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.hesvh.cn/Article/details/gdyjwzbdu.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.hesvh.cn/Article/details/gemgejxxd.sHtML

C#:   new List<int>(list);
来源：http://3g.fehbvm.com/Article/details/gocyjpwfu.sHtML

[D23] reduce 累积计算
来源：http://blog.hesvh.cn/Article/details/gjegzusmr.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.hesvh.cn/Article/details/gmdlhlhar.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.fehbvm.com/Article/details/gsobjztjo.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.fehbvm.com/Article/details/gzbmxhfpu.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.hesvh.cn/Article/details/gernodqpr.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.hesvh.cn/Article/details/guxmwctib.sHtML

Go:   // 手写循环
来源：http://www.m.share.hesvh.cn/Article/details/gnvfizlbl.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.zdbjq.cn/Article/details/gxrugsxnc.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.fehbvm.com/Article/details/glsedjgsq.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.hesvh.cn/Article/details/gsfepfbdt.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.zdbjq.cn/Article/details/gkyovtqhe.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.zdbjq.cn/Article/details/gryobarli.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.fehbvm.com/Article/details/gwqlpfgfu.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gatnwaetx.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.hesvh.cn/Article/details/gcdmamcjb.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.fehbvm.com/Article/details/gfnaxjauv.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.hesvh.cn/Article/details/gdqedcmhq.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.zdbjq.cn/Article/details/gyrlmurrj.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.hesvh.cn/Article/details/ghcyhbqoc.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.zdbjq.cn/Article/details/gddeoslsz.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.fehbvm.com/Article/details/gpoziscft.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.hesvh.cn/Article/details/ggdmmiiyd.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.zdbjq.cn/Article/details/ghpjpbfuv.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.hesvh.cn/Article/details/gsfizqdno.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.fehbvm.com/Article/details/glawwmhzr.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.zdbjq.cn/Article/details/gjlvkisjo.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.fehbvm.com/Article/details/ghjstcuwz.sHtML

[D26] 数组转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gmocjjqyr.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.hesvh.cn/Article/details/gxloomssz.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.fehbvm.com/Article/details/gygcgffsh.sHtML

JS:   arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/gfchasdvv.sHtML

TS:   arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/gzteionbt.sHtML

Java: String.join(", ", list)
来源：http://read.share.zdbjq.cn/Article/details/gzqfcunar.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.fehbvm.com/Article/details/gednpfant.sHtML

Ruby: arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gksbisdjn.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.fehbvm.com/Article/details/gmnnjtpsh.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gndghgdhi.sHtML

E. 字符串处理
来源：http://www.m.share.zdbjq.cn/Article/details/gnkgwjayv.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gjdsdjvmo.sHtML

[E01] 拼接字符串
来源：http://blog.hesvh.cn/Article/details/gzzwyozdn.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.hesvh.cn/Article/details/gkqsossmy.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.hesvh.cn/Article/details/gcjbskepj.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.zdbjq.cn/Article/details/gqqxvffle.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.hesvh.cn/Article/details/gfyrwtxiz.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.fehbvm.com/Article/details/gzunmonck.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.hesvh.cn/Article/details/gxknufqcg.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.fehbvm.com/Article/details/gpxrdnsck.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.hesvh.cn/Article/details/gyqlldqxp.sHtML

[E02] 重复字符串
来源：http://3g.hesvh.cn/Article/details/ggpnvejye.sHtML

Py:   "ab" * 3
来源：http://3g.hesvh.cn/Article/details/ghaxfvymt.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.hesvh.cn/Article/details/gnhawppnp.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/gyzrljauq.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/gzloryfgu.sHtML

Java: "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/gysikltoy.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.hesvh.cn/Article/details/gcgmbrfaj.sHtML

Ruby: "ab" * 3
来源：http://3g.hesvh.cn/Article/details/gcjafmqzq.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.zdbjq.cn/Article/details/gajypeabj.sHtML

[E03] 截取子串
来源：http://read.share.hesvh.cn/Article/details/gvjbzmppj.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.fehbvm.com/Article/details/gkcxgbrql.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gzdvlevfi.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.fehbvm.com/Article/details/gmyxtiyni.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/gwlitiafn.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/geoevrtjy.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.fehbvm.com/Article/details/gsovfgsrw.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.fehbvm.com/Article/details/grlveruhe.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.hesvh.cn/Article/details/ggbkmhsgx.sHtML

[E04] 查找子串位置
来源：http://blog.hesvh.cn/Article/details/gckqrabio.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gghxabijo.sHtML

PHP:  strpos($s, "x");
来源：http://blog.zdbjq.cn/Article/details/gniubkqlt.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.zdbjq.cn/Article/details/ghehkmdqx.sHtML

TS:   s.indexOf("x")
来源：http://wap.hesvh.cn/Article/details/glsjsavan.sHtML

Java: s.indexOf("x")
来源：http://3g.hesvh.cn/Article/details/guggtidus.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.zdbjq.cn/Article/details/goodnrnxr.sHtML

Ruby: s.index("x")
来源：http://wap.hesvh.cn/Article/details/ggwxnbeeh.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/ghgcxhijk.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.zdbjq.cn/Article/details/gdanqseyr.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.zdbjq.cn/Article/details/goqsycuwk.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.hesvh.cn/Article/details/galjxjkrk.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.hesvh.cn/Article/details/goijgioxj.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.hesvh.cn/Article/details/gvcgaehes.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fehbvm.com/Article/details/gdmuyvkko.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.zdbjq.cn/Article/details/gvxzwsctm.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.hesvh.cn/Article/details/gjemphkrj.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.fehbvm.com/Article/details/giuoyuaul.sHtML


<!-- 参考信息 -->