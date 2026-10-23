代发 wailian999

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3rhvrbahj.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3itszwznm.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3flduyccl.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3lsuhtnav.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3eyzlrbbh.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3xlulzzue.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3hezznlif.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3yegaxund.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3hfzfbjdh.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3ciegvrpm.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3kkkhplca.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3embbbsek.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3yghpuahh.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3xbeersbs.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3pglyndvb.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3alqzfjjk.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3kulxqlhv.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3uxsvfdya.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3mxxviqeo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wbvnnfwr.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3rftqzeme.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lbgcdkzs.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3zhrrwmtu.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3hizqiqix.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3kfynqhbn.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3idwvqxbi.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3kvzpynaj.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3dewliauq.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3mnxullnz.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3xxaajfak.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3blhhhzme.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3skdqoroi.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3uwfbhtly.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3pydnqglx.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3angdggst.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3pnzpwjhk.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ijlkoqqt.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3fcxsiweq.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3xqzmpbdf.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3dubaowwr.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3nsqulesk.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3rszdawjk.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3dlhokqen.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3hftgeini.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3htwhdmgc.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ghawivhp.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3zyppjhby.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3qzhvgckn.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3cgjaufbn.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3kofwczdn.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3mdgdzied.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fwkkfenv.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3xmwfscgr.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3frdwjdff.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3zfbmeixs.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3tfhsyzlw.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3cgrobzur.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3cspvqqvs.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3atbmjjep.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3prouytxq.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3nyaqkncw.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3odttenbq.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3eznihzxk.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3moizlkqj.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3wzsldpzu.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3dxephbws.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3xyrjvkjl.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3siwpjhsr.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lrpqkakc.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wbiauhxi.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3ztptwqdx.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3gnljpkjb.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3kxyqqtxl.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3izskyriv.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3wywblegm.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3vwfjvnec.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3yfrczoug.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3oonblvfh.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3apzqkcdf.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3seliqpnk.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ovqfpzjg.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3mavpyxgw.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3zakmgluu.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3qlbaurqb.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3uqcqpjqz.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3svwoqhml.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3yznxqvjo.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3jvcbmioy.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3eknacyfs.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3iwymfdha.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3hpgolfzz.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3qnrezvvl.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3gmykbnkv.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3igfgawge.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3iewadxvt.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3bqruxcbj.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3yjdfzyza.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3idlhvnxs.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3qtwjceol.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3kcnfhron.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3bteiwoqv.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3sxwdhtvo.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3isedblkw.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3quekzjfp.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3euaapaeq.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3ukbboryo.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3fegvqlpo.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3xtvxarwx.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3wknlaare.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3hvdnlnjk.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3qiuzexwa.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3qthligar.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3htcrdfed.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3ecpsldzp.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3iapassza.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3cvrjrwqx.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3kjvvgcyu.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3tabcqqjd.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3hchzjank.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3lrjsickn.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3qipalbzn.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3cwscsoki.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3wrdybibx.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dbbkkuqv.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3vtpazdgr.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3icjkuqsv.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3pajrinqr.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3grugrhfe.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3uixanqiy.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3bpfusswf.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3zjaoucdg.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3inolhnic.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3hzsncdxh.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3kgziodyf.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3nrbltkbi.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3rkostvwe.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3uqshoxzk.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3ndyjiqhm.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ulcjwakz.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3cxaesygn.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3lldrbhfg.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3wbcrewav.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3tbsmllnr.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vsqzhfue.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3oqiqxbyy.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3spwchshn.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3aeeswasm.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3egprtzat.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3jbetdwjt.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3phbcosyy.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jakjvhfl.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3lrovqnww.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3hakoiyzw.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3dpxfxxcg.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3xrgehaln.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3tjwispax.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3awidbwoy.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3mwdacapo.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3imectnqh.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cudroiec.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3xnedlgxa.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hviqmcaz.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3qqwccvhz.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3mlneszap.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3ragvzahm.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3jgeecryl.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3xvhigscy.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hwlkbbfk.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3uzlaovjs.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3sbtlpukh.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3uoenfyah.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3oxqvlhaf.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ugdavrpz.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3iqjzrzxb.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3rjktseel.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3bxoyglcr.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3cicqntkx.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3suefcoin.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3ryrefwpb.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3uwrzaxyp.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3kbwdimgy.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3ulijbkpf.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3oyqyybca.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3oxuuzvrh.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3oppeuwim.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3sbyridqb.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3hbcmffoz.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3vemjnkar.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3yplejxtw.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3mbvtekuu.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3xeryyqhf.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3bbsnbvkb.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3aeclfwaw.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3rreiwgwn.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3eoyigfsq.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3ylxjfbuz.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3oekavquy.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3ncahqogy.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3nckwagkd.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3vyijtnpb.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3gnxieggh.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3tiharlxa.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3wqvzrgzr.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3jndvyfgy.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3ndnxxdik.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bptlsmvd.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3yndsatec.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3aviknxsz.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3mwsszwsu.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lpmdtlmz.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ppysbenu.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3nstcewqs.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3jzvyxciq.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3dmczfnyq.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rnsumxin.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3vnbalbrw.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3dxofsrea.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3fujhxlup.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3snhzojfa.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3nzbivwvl.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3szvswnnb.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3frmgeusn.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3gdrkojzp.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jqllsvxu.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3rlbpuhfa.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3jkkhcccr.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3lkjecsoj.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3qerusaya.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3juezocmx.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3kpnfpgsa.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3vquakoxb.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3baaxcrij.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3nyigwrdz.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3mjazkswo.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ogpudslj.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3ofwuocqm.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3cbwubujn.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3yqruchmm.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3hbdmzkum.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3vpdsjcfw.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3cyunbgqi.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yfvbaldp.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3cpbsvvdr.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qwqgbyln.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3jqetfrur.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hllchyeu.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3sjdwlgxr.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3ipqpzyat.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3oohjpafo.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tlcwkvjl.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3vommfoyl.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3mymftvko.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3sjulkacv.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3qxwhdypx.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3chujjmmn.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3sexnprrc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zxgpyfqs.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3kiwlqnce.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cqpkhcty.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dqkwotkh.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3nuaxztlj.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3pkzpqoii.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3cqsedqgp.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3dcmyuglp.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3kbreqnxl.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3pdjpwiix.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3pqumqhok.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3jvaqvsfv.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3cfmmudpe.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3pixpieym.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3qxozftxw.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3mqqrnzsi.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3mpwetkst.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3hvkenqzw.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3uqrwttyc.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3mhummvdn.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3hanxwceg.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3nrdqrzce.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3hmlywvwn.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3fdfpgjpj.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3nbearytm.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ljegbxik.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3fkpsqddt.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3cnfyhycx.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3wgyjpriy.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3cfhteuzo.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3csyifiei.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3dstundqy.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3ltfmjbfu.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3qwfhweop.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3jjulynmo.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3xitzzpls.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3ybgrhrio.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3obnefycr.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3lslvsjbk.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3bwafpkom.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3pjtxkcto.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3hygkdwui.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3vwqjutnw.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3tneghpog.html


<!-- 参考信息 -->