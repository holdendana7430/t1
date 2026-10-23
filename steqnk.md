代发 wailian999

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3acednvrm.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3ieiejaqf.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3havppyci.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3xgzmartb.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3ymuprszz.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3otrqaxqt.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3abgiwoxa.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3xjqzuvje.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ysjxhzhs.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iyudepfq.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3ivhtluzm.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3jbalblbb.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3ohktyhgg.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3xulcmvru.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3yczzdjwq.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3jwjogtzd.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3sdgmbkmq.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3rfkvakbu.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3dqcsxgul.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ubloqksm.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3fgslwmvt.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3hdrzojeb.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3gfuezpen.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gncugmlj.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3ofbgqrri.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zudzkrpy.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3wgfvokho.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3doqdimjt.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3swvhemmd.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3yxnvwipw.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3uyzxrlrb.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3brvzasbg.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3gujwpqsy.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3owyxbccl.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3fhclkglv.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3guxnunkw.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3hkjpgaet.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3csgaddqq.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3feqkfsvs.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3lrkccssd.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3blbwyozk.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3uiqniehu.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3wbrjfvmb.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3qdncdtkg.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3hbhieeqt.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3fnjetkwy.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3miyucuei.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3xecabvmg.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3uvryyduk.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3rsrbtglm.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3gamgzmkp.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3jbkbpghb.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3fklqxzvp.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3lyoxfqkm.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3svexgain.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3mwbacxgl.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3zfnstqbl.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3jrzukkgy.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3lhtvigby.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3pwqtmmcg.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3aphcaitf.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3wcnpkiyj.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3ftclsxkj.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3xsgylehv.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3zpsixihw.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3dzdzazxx.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3dvpbjwdi.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3upfkrflh.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3mtuxqeyb.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3iglykiru.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3jeimucbw.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3hqndogqv.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hmitxwhz.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3itwshfcj.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3djqcsjdu.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3ayyrmnif.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3ycyeaceg.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3cxkdijiu.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3bowuuixu.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3lmiyvfva.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3wpuymdlv.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3rrqlbfzb.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3vfjokgdc.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3iijrugcd.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3bvcafrxj.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3imyhvoge.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3ssdoaayv.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3dyzpzcde.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3yztorsfn.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3zubgeuae.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3yinfapwg.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3whionnxh.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3ssuxqhpx.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3lvqqisyp.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3vylehhca.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3qpxxkffd.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3zjmboxeb.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3sgornxif.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3iwzmcjci.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3nofowikr.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hcuolkpd.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3bgxxxfwm.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3pxyagheo.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3nfcfvuts.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tjvmncmi.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3nioqfcxl.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3byyyxvgo.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3qbblyfvb.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3kovhutjm.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3swhuktpc.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3cgdbhdzy.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3mvajheql.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3xruyjqcd.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3ukuofuil.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3mwnirbas.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3pmstlcuk.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3shzuygak.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3xaipfzot.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3pxjuoqjj.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3iqpwyowr.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3ypyokrck.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3dowpaovh.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3frhrdywn.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3ocbcbnbp.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3udyvljgx.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3mthpzenz.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3bpbmdnmm.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3tucackrr.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3anoxoxlg.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3gfgzfsuk.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3yrehuqba.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3aaskruni.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3icmydjvm.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3hhjblqur.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3xbrjqhml.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3llarjmkl.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3uopbxaer.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3dilngseh.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ozahkcjm.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3zabxqfdf.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3vmtuwdzb.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3chjbdefa.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ugaddwtr.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3gowwkcvu.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3vsjswten.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3lamioweh.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3clfoodsg.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3skiratxu.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3gsrvuind.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3sbsvvciv.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3oqoygicf.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3lmkxiygl.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3elzpbpeq.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3uhhcissd.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3kqgjgxpl.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3yyupogdh.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3xddqmvzx.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3ptrbvoii.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3pnpvinko.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3jaftqmym.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3uyqsxnhs.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3cbyuxxsa.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dvskvrze.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3keghpfef.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3kdwbdzrx.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3qvamcjar.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3zeopnebv.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3zrzjljsz.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3vxzrjugf.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3utbphnyz.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3mdeiglis.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3akwfvzpz.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3cjkkupav.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3pabrabnf.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tqbaprnb.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3kjioxyrn.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3vhmdnaor.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3ievsscee.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3iuqpscta.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3zkhfrzmo.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3manqhome.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3fmdssnbp.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3dklkaycy.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3rstqjoqa.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3ybndciwn.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3avwjpwnz.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3icssilab.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3kbjlgwzd.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3ylytcgpn.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3snefoxou.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3casggvxb.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3ffquyfwj.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3fxojvmxt.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3qhejpozk.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3zvfcmghe.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3lnlraeeu.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3wuiedidn.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3ezkoxurk.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3oovxjcol.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3edufekeq.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3dvoizojy.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3sqnoxsyx.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3rwoljjkn.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3qpieranm.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3tojutdzp.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3wrwpdldw.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3lfcrawit.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3phvomxij.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3jgdhmocy.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ewlojykp.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rukpfrfz.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3merrquav.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3xzwlhbqb.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gpsbaqyg.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3onrhpwin.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3fulpkeal.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nbgfsybo.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3xohklzhx.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3krydlfny.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3zwkahyda.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3tdrvpvcx.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3dflvatgt.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3vtwtohse.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3oelndgqd.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3izsuboyl.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3mhgrjfxn.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ipoghoxe.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3aqwyjimz.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3kutqlqmv.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3bpuvjouw.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3isercypk.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3hlmemrca.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3utrpbjjh.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3ptnlumhd.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3yomedxoa.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3hvwrtrdr.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3wbddaswf.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ygldebbs.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3ydicykfh.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3vflurobn.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3gjoyuzyq.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3baxfrydv.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3hagqsbzz.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3wmxghykn.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3ovjncyka.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3zhklsulj.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3ddseirkj.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hbtngqpa.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3janepepb.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pzwrkpbe.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3rowkyljg.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nshxtcec.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3rabgjest.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qolfqewx.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3fcgdxefj.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3pxtopcbq.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3tzttpote.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3chnqaavj.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3bkxdsyrk.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3movylrdv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3amxirnoe.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3rgeweroo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ygmpmlku.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3pamrzroq.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3hluwtuhc.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3acovurds.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3hjgemwow.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ewoniswh.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3rdxszmau.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3wooclvaw.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3mlhtfjqq.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3vvcufszq.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3chhohtvs.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3dzavftpn.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3biclgttc.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3bovluyuu.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3vdlcjryd.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3mbhrxfqk.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3fwrovysv.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3skytrcsu.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3rslocgmk.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3knojunnd.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3wcfimqnh.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3qfwcsryo.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3srtilgas.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ycehxxsm.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3xcjmzmzj.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3jdlhonzs.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3wuqkcqtb.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3fispetnt.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3fblebgqz.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3ivkexxgu.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3ydkkwvmb.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3vicgqxqq.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3qzcemejo.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3nmpdbmbc.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3qskjjvgy.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3xakqimoo.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3ckrngcwh.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3uzicqwkx.html


<!-- 参考信息 -->