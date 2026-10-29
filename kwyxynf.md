代发 wailian999

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.hesvh.cn/Article/details/ggatjelgn.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.zdbjq.cn/Article/details/glvlmvepy.sHtML

Java: // 无解构
来源：http://www.m.share.zdbjq.cn/Article/details/gmoawebvv.sHtML

Go:   // 无解构
来源：http://blog.zdbjq.cn/Article/details/grsnborbe.sHtML

Ruby: a, b = pair
来源：http://wap.hesvh.cn/Article/details/grjtuhfpw.sHtML

C#:   var (a, b) = pair;
来源：http://wap.hesvh.cn/Article/details/gcorhsmjq.sHtML

[C16] 函数 / 方法重载
来源：http://blog.fehbvm.com/Article/details/groenwicq.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.zdbjq.cn/Article/details/gzzftdchb.sHtML

PHP:  // 无重载
来源：http://blog.zdbjq.cn/Article/details/gopgokiva.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.hesvh.cn/Article/details/gcveysgsw.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.fehbvm.com/Article/details/giqckrfeq.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.fehbvm.com/Article/details/ggxwqislx.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.fehbvm.com/Article/details/gidlgeede.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.zdbjq.cn/Article/details/gpunrqdwm.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.zdbjq.cn/Article/details/gwuhallcq.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gqpjbkqfu.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.fehbvm.com/Article/details/gcltxmnmi.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gkswmtuui.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.hesvh.cn/Article/details/gwwexlqiu.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.zdbjq.cn/Article/details/gybdkuvtz.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.zdbjq.cn/Article/details/gikdptejg.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.fehbvm.com/Article/details/gmznlmzil.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.hesvh.cn/Article/details/gxzjrbfds.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.fehbvm.com/Article/details/goynywfoz.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.fehbvm.com/Article/details/gkfhjsnuv.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.hesvh.cn/Article/details/gqjrmvxbs.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.hesvh.cn/Article/details/gldtumbxy.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.zdbjq.cn/Article/details/gugkjyqxw.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.fehbvm.com/Article/details/gqhxlmcif.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.hesvh.cn/Article/details/gmzwdeszv.sHtML

JS:   arr.push(4);
来源：http://mobile.zdbjq.cn/Article/details/ghvptxvzv.sHtML

TS:   arr.push(4);
来源：http://www.blog.hesvh.cn/Article/details/giavbbpho.sHtML

Java: list.add(4);
来源：http://www.m.share.hesvh.cn/Article/details/gzzdnhrnr.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.zdbjq.cn/Article/details/gvzpwocpy.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.zdbjq.cn/Article/details/gjvfrbywi.sHtML

C#:   list.Add(4);
来源：http://blog.hesvh.cn/Article/details/gmxuehxhs.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.hesvh.cn/Article/details/gawrxdyti.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.fehbvm.com/Article/details/gwgzbygrk.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.zdbjq.cn/Article/details/gxhjibwfk.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.fehbvm.com/Article/details/ggdfamtwj.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.fehbvm.com/Article/details/glrcrtlti.sHtML

Java: list.add(0, 0);
来源：http://3g.hesvh.cn/Article/details/glnobojzu.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.hesvh.cn/Article/details/gggpgkjnz.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.hesvh.cn/Article/details/grrqmxdyt.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.zdbjq.cn/Article/details/gereyuvei.sHtML

[D04] 删除元素
来源：http://read.share.zdbjq.cn/Article/details/gbghskbxj.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.zdbjq.cn/Article/details/gzeeqwgon.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.hesvh.cn/Article/details/gqcfnsfoc.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.hesvh.cn/Article/details/gfkiaoosh.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.zdbjq.cn/Article/details/grrbewviq.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.fehbvm.com/Article/details/gpqewqvvs.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.zdbjq.cn/Article/details/gfrtculrw.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.zdbjq.cn/Article/details/gmnnnmayf.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.hesvh.cn/Article/details/gzkfvmzdd.sHtML

[D05] 访问与修改元素
来源：http://wap.fehbvm.com/Article/details/gexiklhjo.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/guccnqqhk.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/gyehcsxhi.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/gadwhhide.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.zdbjq.cn/Article/details/gikengoah.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.zdbjq.cn/Article/details/gvlrhbepx.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/glzeeajgn.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/gmpenvmxm.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/ghrnjhsnk.sHtML

[D06] 数组长度
来源：http://read.share.hesvh.cn/Article/details/gltmzbdml.sHtML

Py:   len(arr)
来源：http://3g.zdbjq.cn/Article/details/gdpycoise.sHtML

PHP:  count($arr);
来源：http://read.share.zdbjq.cn/Article/details/gzshbedtd.sHtML

JS:   arr.length
来源：http://blog.zdbjq.cn/Article/details/gvhonuwlf.sHtML

TS:   arr.length
来源：http://www.m.share.zdbjq.cn/Article/details/guxuevcsi.sHtML

Java: list.size();
来源：http://3g.hesvh.cn/Article/details/gqrnrzfmb.sHtML

Go:   len(arr)
来源：http://3g.hesvh.cn/Article/details/gejrwrpbq.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.hesvh.cn/Article/details/gejqhebhm.sHtML

C#:   list.Count;
来源：http://wap.fehbvm.com/Article/details/grrkpqceg.sHtML

[D07] 切片 / 取子数组
来源：http://baike.zdbjq.cn/Article/details/gugscumcz.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.zdbjq.cn/Article/details/gbxnkkmdl.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.hesvh.cn/Article/details/gwcuhcmeo.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/gmlmnyoyk.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gkuouqlst.sHtML

Java: list.subList(1, 4);
来源：http://www.share.fehbvm.com/Article/details/grknqbbjl.sHtML

Go:   arr[1:4]
来源：http://www.share.fehbvm.com/Article/details/gqrpuulao.sHtML

Ruby: arr[1, 3]
来源：http://baike.zdbjq.cn/Article/details/gftwkrfec.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.fehbvm.com/Article/details/gfabkreob.sHtML

[D08] 合并两个数组
来源：http://www.blog.zdbjq.cn/Article/details/gwihkfwte.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gdvviukvo.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.fehbvm.com/Article/details/grjklepev.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.fehbvm.com/Article/details/gcnfcyokp.sHtML

TS:   [...a, ...b];
来源：http://baike.zdbjq.cn/Article/details/guvbpqyov.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.hesvh.cn/Article/details/gfgpccilt.sHtML

Go:   append(a, b...)
来源：http://3g.zdbjq.cn/Article/details/gtrutaczb.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.fehbvm.com/Article/details/gbnvatirz.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.hesvh.cn/Article/details/glcimrqdt.sHtML

[D09] 排序（升序）
来源：http://mobile.fehbvm.com/Article/details/gflzgmptb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.zdbjq.cn/Article/details/gsczwvaus.sHtML

PHP:  sort($arr);
来源：http://www.share.zdbjq.cn/Article/details/gthzpkhup.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.zdbjq.cn/Article/details/gspdiqneq.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.zdbjq.cn/Article/details/gqwkpiang.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.fehbvm.com/Article/details/gtjrbrdtm.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gzhpiabxg.sHtML

Ruby: arr.sort
来源：http://baike.zdbjq.cn/Article/details/gbpkknnop.sHtML

C#:   list.Sort();
来源：http://baike.hesvh.cn/Article/details/grovrpbvq.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.hesvh.cn/Article/details/gugdrdtmr.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.fehbvm.com/Article/details/gxehtucai.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.zdbjq.cn/Article/details/gkjkcycbf.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.fehbvm.com/Article/details/guxqvqrar.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.zdbjq.cn/Article/details/gtxpapxsn.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.hesvh.cn/Article/details/gmkyebdhb.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.fehbvm.com/Article/details/gckwiajgt.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.fehbvm.com/Article/details/gbrltzdmt.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.fehbvm.com/Article/details/gsziweham.sHtML

[D11] 反转数组
来源：http://3g.zdbjq.cn/Article/details/gyjrgkuct.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.hesvh.cn/Article/details/gomyugcog.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.hesvh.cn/Article/details/gyqnmbdkk.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.zdbjq.cn/Article/details/ggopmslrn.sHtML

TS:   [...arr].reverse();
来源：http://read.share.fehbvm.com/Article/details/gzdzimraz.sHtML

Java: Collections.reverse(list);
来源：http://read.share.zdbjq.cn/Article/details/glvfwtsjw.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.hesvh.cn/Article/details/gfdnhbkmv.sHtML

Ruby: arr.reverse
来源：http://wap.zdbjq.cn/Article/details/goimowidh.sHtML

C#:   list.Reverse();
来源：http://baike.fehbvm.com/Article/details/giesgiavv.sHtML

[D12] 查找元素下标
来源：http://www.m.share.zdbjq.cn/Article/details/ginqxknlx.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.hesvh.cn/Article/details/gkjlmauck.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.fehbvm.com/Article/details/gxeqmnrfw.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.hesvh.cn/Article/details/gffcgczrg.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.fehbvm.com/Article/details/gafybnedu.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.fehbvm.com/Article/details/gutdeuzty.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.hesvh.cn/Article/details/gglphldhm.sHtML

Ruby: arr.index(x)
来源：http://www.blog.fehbvm.com/Article/details/glkmfbgoj.sHtML

C#:   list.IndexOf(x);
来源：http://baike.fehbvm.com/Article/details/gfrjpqjii.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.fehbvm.com/Article/details/gjajwptbv.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.zdbjq.cn/Article/details/ghyvzobdf.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.zdbjq.cn/Article/details/gadyzovzp.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.hesvh.cn/Article/details/gfljjmiur.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.hesvh.cn/Article/details/gvgfrhfhx.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.hesvh.cn/Article/details/gmbvteeyo.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.hesvh.cn/Article/details/ggshpatpd.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.zdbjq.cn/Article/details/grmsrsstq.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.hesvh.cn/Article/details/glmxdtezv.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.zdbjq.cn/Article/details/gxbkkkssw.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.hesvh.cn/Article/details/gngggyvfq.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.fehbvm.com/Article/details/gpalenorp.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.hesvh.cn/Article/details/gwjlmdtms.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.hesvh.cn/Article/details/gfciyoyrb.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.hesvh.cn/Article/details/gzmaatfzg.sHtML

Go:   // 手写循环
来源：http://www.share.zdbjq.cn/Article/details/gcxkwrgcd.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.fehbvm.com/Article/details/gbpjdnthp.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.zdbjq.cn/Article/details/gqqgkxrhk.sHtML

[D15] 去重
来源：http://read.share.zdbjq.cn/Article/details/gvsoiscom.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.fehbvm.com/Article/details/gkgdfvqbs.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gpewacvsu.sHtML

JS:   [...new Set(arr)]
来源：http://baike.hesvh.cn/Article/details/ghkbynrft.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/gepgavgbm.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.zdbjq.cn/Article/details/gizavtfts.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.hesvh.cn/Article/details/goqwmsyxa.sHtML

Ruby: arr.uniq
来源：http://www.m.share.hesvh.cn/Article/details/gxhhxzlly.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.hesvh.cn/Article/details/gkrmcnlul.sHtML

[D16] 求和与平均值
来源：http://www.blog.fehbvm.com/Article/details/gtntfaoam.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.zdbjq.cn/Article/details/ggwkykcog.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gcxehtdbv.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.zdbjq.cn/Article/details/gejfqejul.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.zdbjq.cn/Article/details/gyglxeyoo.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.hesvh.cn/Article/details/gkiyweigm.sHtML

Go:   // 手写循环累加
来源：http://3g.zdbjq.cn/Article/details/grciodtvp.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.zdbjq.cn/Article/details/gdeqjcnsn.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.zdbjq.cn/Article/details/gpvakbctq.sHtML

[D17] 最大值与最小值
来源：http://3g.hesvh.cn/Article/details/gyvmhseoj.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gauraljrw.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gjnihcrjg.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gqcfifhyb.sHtML

TS:   Math.max(...arr);
来源：http://mobile.fehbvm.com/Article/details/ggwgqjkpj.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.zdbjq.cn/Article/details/gbqiibrvk.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.hesvh.cn/Article/details/gcoigstfk.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.fehbvm.com/Article/details/gndcwjjnx.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.zdbjq.cn/Article/details/gulbmleso.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.fehbvm.com/Article/details/gudsqwbmq.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.zdbjq.cn/Article/details/glulgjfwh.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.fehbvm.com/Article/details/gkfbbshzc.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.zdbjq.cn/Article/details/gyivtohns.sHtML

TS:   nested.flat();
来源：http://blog.fehbvm.com/Article/details/gpmdwkted.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gbqyinvbo.sHtML

Go:   // 手写双层循环
来源：http://3g.hesvh.cn/Article/details/gokrywwcz.sHtML

Ruby: nested.flatten
来源：http://3g.hesvh.cn/Article/details/grhbbynhj.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.fehbvm.com/Article/details/gtehsoaal.sHtML

[D19] 按字段分组
来源：http://baike.fehbvm.com/Article/details/gkzuuwkhu.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.fehbvm.com/Article/details/glrzmnbxz.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.hesvh.cn/Article/details/gwwxadboz.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.zdbjq.cn/Article/details/gyyudamlo.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.zdbjq.cn/Article/details/gllqhlbxc.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.hesvh.cn/Article/details/gbgbqeprk.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.hesvh.cn/Article/details/gjjvwxggf.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.zdbjq.cn/Article/details/gjfbugpne.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.zdbjq.cn/Article/details/gveyubvhr.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.fehbvm.com/Article/details/gkaiuafsr.sHtML

Py:   Counter(arr)
来源：http://mobile.zdbjq.cn/Article/details/gojtbqrjt.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.hesvh.cn/Article/details/gouvhqrgm.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.fehbvm.com/Article/details/grsnibaxk.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.hesvh.cn/Article/details/gbkbznezs.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.hesvh.cn/Article/details/guqwfmpep.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.hesvh.cn/Article/details/gqzqyzruj.sHtML

Ruby: arr.tally
来源：http://read.share.fehbvm.com/Article/details/ggwncukrh.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.fehbvm.com/Article/details/gaanvmtwt.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.fehbvm.com/Article/details/gzrnvvodx.sHtML

Py:   x in arr
来源：http://www.m.share.zdbjq.cn/Article/details/gonvqccat.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.hesvh.cn/Article/details/gvrcytiww.sHtML

JS:   arr.includes(x)
来源：http://www.share.fehbvm.com/Article/details/gligtslkw.sHtML

TS:   arr.includes(x)
来源：http://www.blog.fehbvm.com/Article/details/gwepzekho.sHtML

Java: list.contains(x)
来源：http://wap.zdbjq.cn/Article/details/ghunpmavk.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gqcirlgip.sHtML

Ruby: arr.include?(x)
来源：http://read.share.hesvh.cn/Article/details/gybwyhsth.sHtML

C#:   list.Contains(x)
来源：http://m.share.hesvh.cn/Article/details/gpyionuje.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.zdbjq.cn/Article/details/guilrgpnh.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.hesvh.cn/Article/details/gtumpfujw.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.zdbjq.cn/Article/details/gueeuasqu.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.zdbjq.cn/Article/details/gwvitijfl.sHtML

TS:   [...arr];
来源：http://mobile.fehbvm.com/Article/details/gmqxchcll.sHtML

Java: new ArrayList<>(list);
来源：http://wap.hesvh.cn/Article/details/gfcelzhui.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.zdbjq.cn/Article/details/gmapwaopp.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.fehbvm.com/Article/details/gjgybnvwf.sHtML

C#:   new List<int>(list);
来源：http://3g.fehbvm.com/Article/details/gvoabqxma.sHtML

[D23] reduce 累积计算
来源：http://wap.zdbjq.cn/Article/details/gmwxqflfk.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.fehbvm.com/Article/details/gwdsxogkj.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.hesvh.cn/Article/details/gmnpffbpc.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.hesvh.cn/Article/details/gvcnjqqdv.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.zdbjq.cn/Article/details/golllgynw.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.hesvh.cn/Article/details/golwvawit.sHtML

Go:   // 手写循环
来源：http://3g.hesvh.cn/Article/details/gkupukmip.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.hesvh.cn/Article/details/gdenekwqg.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.hesvh.cn/Article/details/gouluoron.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.hesvh.cn/Article/details/gobyzdknl.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.fehbvm.com/Article/details/gsgaspmpx.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.hesvh.cn/Article/details/gijsxmdjg.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.hesvh.cn/Article/details/gnnoyfazz.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.fehbvm.com/Article/details/gkrzhmdzu.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.zdbjq.cn/Article/details/gksanlyop.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.hesvh.cn/Article/details/goyvgebdd.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.fehbvm.com/Article/details/gmnaovoqu.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.hesvh.cn/Article/details/gwfihjano.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.zdbjq.cn/Article/details/gcggtgxer.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.hesvh.cn/Article/details/gsulvqfxs.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.zdbjq.cn/Article/details/gkysgdrci.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.fehbvm.com/Article/details/gcmrjdyjc.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.zdbjq.cn/Article/details/gnqgrpvcw.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.hesvh.cn/Article/details/ggvocrddj.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.fehbvm.com/Article/details/ggzzruyaz.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.fehbvm.com/Article/details/gctwisukk.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.fehbvm.com/Article/details/gwobjgjno.sHtML

[D26] 数组转字符串
来源：http://mobile.zdbjq.cn/Article/details/grwpouqoj.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.fehbvm.com/Article/details/guzwuygpi.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gjxbgktvq.sHtML

JS:   arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gtgwisbqs.sHtML

TS:   arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/gezwoirzf.sHtML

Java: String.join(", ", list)
来源：http://www.share.fehbvm.com/Article/details/gpsldcrca.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.hesvh.cn/Article/details/glgjsohed.sHtML

Ruby: arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gtfjrtvff.sHtML

C#:   string.Join(", ", list)
来源：http://baike.hesvh.cn/Article/details/gebvwvthb.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gznsgapsn.sHtML

E. 字符串处理
来源：http://wap.zdbjq.cn/Article/details/gvhcfvxoq.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gnbrafuex.sHtML

[E01] 拼接字符串
来源：http://blog.fehbvm.com/Article/details/ghazkqsms.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.zdbjq.cn/Article/details/gzdwaskyy.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.zdbjq.cn/Article/details/gumranuno.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.hesvh.cn/Article/details/gjzavnqbg.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.hesvh.cn/Article/details/glszdffbu.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.zdbjq.cn/Article/details/glyalmipi.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.zdbjq.cn/Article/details/gapienjdl.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.zdbjq.cn/Article/details/gmruifjaw.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.hesvh.cn/Article/details/givvyrjrn.sHtML

[E02] 重复字符串
来源：http://read.share.zdbjq.cn/Article/details/ggvjudyws.sHtML

Py:   "ab" * 3
来源：http://wap.zdbjq.cn/Article/details/gtcffabka.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.zdbjq.cn/Article/details/gzwnonuxo.sHtML

JS:   "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/gxezqlpkr.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/ggokvmsat.sHtML

Java: "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/geaysxozc.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.hesvh.cn/Article/details/gffqnataa.sHtML

Ruby: "ab" * 3
来源：http://read.share.hesvh.cn/Article/details/gispenule.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.zdbjq.cn/Article/details/gkzffiyhd.sHtML

[E03] 截取子串
来源：http://m.share.fehbvm.com/Article/details/gavspxbox.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.hesvh.cn/Article/details/gejmijodn.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gmmyrdgyf.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.fehbvm.com/Article/details/gchsxpntj.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.fehbvm.com/Article/details/gvtyrkzmh.sHtML

Java: s.substring(1, 4)
来源：http://m.share.hesvh.cn/Article/details/gsdbvrooo.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.fehbvm.com/Article/details/gijngsbea.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.hesvh.cn/Article/details/gcgswokkc.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gfrlzdmwp.sHtML

[E04] 查找子串位置
来源：http://baike.fehbvm.com/Article/details/ggbjklpbt.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.fehbvm.com/Article/details/gsnndhlld.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.zdbjq.cn/Article/details/ghvttmcqz.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.hesvh.cn/Article/details/gijsuswko.sHtML

TS:   s.indexOf("x")
来源：http://mobile.fehbvm.com/Article/details/gccmomtoj.sHtML

Java: s.indexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/giouwhygt.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.zdbjq.cn/Article/details/gggqjnhld.sHtML

Ruby: s.index("x")
来源：http://mobile.hesvh.cn/Article/details/ggtelzgja.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/gnecqozrg.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.hesvh.cn/Article/details/gwszdkrnq.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.zdbjq.cn/Article/details/geyrvxkzy.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.zdbjq.cn/Article/details/ggobrcntn.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.zdbjq.cn/Article/details/gpqfhlugs.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.zdbjq.cn/Article/details/gbowwqhmd.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.zdbjq.cn/Article/details/gamgnykfy.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.zdbjq.cn/Article/details/gwfrtedhy.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.hesvh.cn/Article/details/ggtqapzay.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.fehbvm.com/Article/details/gfbvuxozn.sHtML


<!-- 参考信息 -->