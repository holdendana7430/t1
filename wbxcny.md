代发 wailian999

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3olshgxmq.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3lqmjvgur.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3uemzbynv.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3tvyysofz.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3yqqmoiyh.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3eayvmjaw.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pagfunkv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3amkdqvwg.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3nnhsuekz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lfigejom.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3hfwomoaz.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3mxcnktje.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3unevjmgj.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3hoonrulx.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3hbekjknj.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3hoqgvkeh.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3pblrmwke.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3dqxtvkzl.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3eshwnawl.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3bhvodvys.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3cmhnunxc.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3cexbqjbn.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3sxbxidli.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3jwvttpbh.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3ryxykgnm.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3molavdih.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3cspzztbi.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3enemqtvm.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3gpbgnqvj.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3fbwfpeam.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3pxkyucas.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3wkezettn.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3edocxkdn.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3mekukzki.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3cbueudtb.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3bqixwctp.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ivhwglom.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3yvcpgznn.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3wmzcczuo.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wnluzslj.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3efdnnxpc.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3tlftmdyi.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3wlbqjdab.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3hyvfkwua.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3avxjmoof.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3xnvqisud.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3rwewqmyj.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3fdvxajtt.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3xqtdcifz.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3gmeyiefn.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3vxzgezlg.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3nprbzdzs.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3oiqyyqal.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3xuwmzlxs.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3vevhchuv.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3fxpdognx.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3pkomkbpd.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3ealwltmj.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3lzqsielh.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3uwzkottt.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3rhzkxzdp.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3cuoampzn.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3qbvtkicx.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3htblqenp.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3cuucybpj.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3wyebtjdv.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ofwzukgh.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3nixaoyaz.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3mzpqqdee.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3mwkrxkkn.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3nwkxqxsp.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3qkhlsziu.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3laqbaqxt.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3svcdpbpc.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3bnthpsqq.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3cvtiicqy.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3pxwalkdl.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3rykxgbpt.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ppxqespx.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3ubmsqquc.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3cigukyin.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3xagvqedd.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3bctbnice.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3zuscmgfp.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ktqdjuyc.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3zpgdsnop.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3qbdvewvw.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3rykvkhho.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3teozbctj.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3tgpheaph.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3ruwneifg.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3kfutyaxv.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3xeejbsdz.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3nczfqtpe.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3fccvcmyn.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3ridouhnu.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3gmkpessp.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3vfenorig.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3lqrddnvv.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3gqcsmqua.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3alutnffi.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3pykbavwa.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xercwhzg.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3nvxvmyic.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3phddnizw.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3fopnptgx.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3hrefzllg.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3qvwwvfye.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3blzuxbjc.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3lpcjhgvj.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3ezbbclfw.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3nqadupnw.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3lbipwgjw.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3rrxkwctz.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3bulrwxtj.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3xqxozjxi.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3spjsqvjn.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3iiqgtacr.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3gctrlggo.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3jiwmgwls.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3ecqfyykn.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3enloodha.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3wdgjthoe.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3samkjhqq.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3vxcstzci.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3ptihmxll.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3fflwxssf.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3kvxohfge.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3qzwkbkhb.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mskdezgu.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3iyqykgak.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3nwhiopnz.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3gjdmazet.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3xocrxkmk.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3lwuwugvy.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ajzoyagw.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3bqoqdjcw.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3cjvlofhc.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3uoyvnidd.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3nrwraara.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3oecuupqm.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3qjhntlzr.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3lqctxfbi.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3iicodcxz.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3jfbwftgg.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3sjmrwdli.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3ruwwhicp.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3uvlvokng.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3xnnfcsei.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3gtbswwen.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3myeikrwu.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3xcuydrym.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3ckgkxazc.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3nvstgqec.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3enajgxlv.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rbjswjsa.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3pfamamld.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3aiocxrxd.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3cycsrzna.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ifouvssh.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3lmmeivub.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3uequypwe.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3ipcptfhu.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3updujkwh.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3bsqijktw.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3lhcrsmfm.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3gpsbihxw.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3rnwickmi.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3bwsncgmb.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3rbapiokv.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3ioioevkh.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3owlxvhbb.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3ckwcmppd.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3keprbnbu.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3ojykposa.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3oldulvid.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3wbrzfcxx.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3mkgxxkxo.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3uvqiuljo.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3upjijcim.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3sowexlcn.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3brlqkgcv.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3grlfolre.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3shmayldc.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3ohtfryqn.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3eupmlkxo.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3qtbumerj.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3tijzbyoo.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3jjilgptk.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3ewkwcgoc.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3jzrcowht.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3pkksdzlo.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3dwrinauh.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3kiglbatm.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3pqhgpccb.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3fdlmwshg.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3lhqjskcy.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3erfwntqd.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3tjrvdocn.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3kysukoeu.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3uljsvxlw.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3npiezjek.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3qkqfsolg.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3xdxrclhy.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ttksyisx.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3suhnjsiw.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3cojvzxmf.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3mccnyych.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3myybqkub.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3bnktbgei.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3fugrgkmb.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3rnsftpyu.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3yuohlzml.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3masxopnc.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3nknogppw.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3sucmiwuw.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3mbsontpy.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3jaopghtw.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3saukedel.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3xbtmatrk.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3yfiumzqq.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ykuhubfb.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3duuevexy.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3zdhvpsrm.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3wvvwlsee.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3glcqlnox.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3nbdxiuvc.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3jwilkkbk.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3jjmqhmly.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xuwghivf.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3enirvzwv.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jsqcbthz.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3dehqfrok.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3etpxjxax.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3rxamfxox.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3tdhcrdhp.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3hzlnpque.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3dgjxvlwg.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3wpdiqbqk.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3atrlexgn.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3icombbox.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3zwtehnfo.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3jrjsbdhb.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3vuewrhxt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ladiiajf.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3ldoobjfn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jgptesjz.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kcojpfdb.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3jqjzqrnt.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3trdczvzm.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3muivcxbz.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3qkuyauxl.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3rahaaitw.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3xkrijodj.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3iwziasxx.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3znnlvynj.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ttejcfkg.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3hfebpimy.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3tgmbgnbl.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3bsdmrjfo.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3yibxutzz.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3xsltdrwa.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3vzwdkwwt.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3rwszsqrg.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3qxddysdt.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3yftlcumt.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3lvfkxqzf.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3myblajvn.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3uqgbcinv.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ftvwbqru.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3yaxmtnbu.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3dlpxvxwv.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3ksukphji.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3nwktxwzu.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3aenzmvfx.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3pogozdtg.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3qndaxids.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3hmrchkil.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3dgqixhrv.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3lqxiptkj.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3arvxfmko.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3gqzerrdb.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3dgrgrzvq.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3vzmkfzkn.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3awohcrrw.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3vixxggul.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3gzriuabr.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3wqlfqalg.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3gsmmpvqe.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3ptchffrm.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3moswhkcg.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3pamsqjpb.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3jofkjhgd.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3dwbbhvpa.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3vxnjngez.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3uaerwqfm.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3didrbhvi.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3pywljllo.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vusnsbnn.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3aubmweyd.html


<!-- 参考信息 -->