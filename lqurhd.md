代发 wailian999

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3wwaqgrlj.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3qiaoheke.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3hmrzggrf.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3ymgkcpsn.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3xueeelsl.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3kowdfpep.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3vqkszcch.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3cjoudzqf.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ibhpkfep.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3ybexglyp.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3qxcyumaq.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3fhpusiag.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3qaasjzxj.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3boabyslh.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3benmcqvs.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3okwyrqrz.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xezfanek.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3ypdgnafy.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3hyyqxnea.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3mlasunrr.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3cifthjxc.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3qeykxkhk.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3pqphwsus.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3mixaiizv.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3dylwseqo.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3pkckopsi.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3djgxalgq.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3wtsymjdd.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3rrcacqlh.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3jvowvqyi.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3hglsbfbi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kmyruehb.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3mlocbocb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xemhtaaf.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3vpgafaws.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3isndurqg.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3mepbqmbn.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3fegcuevq.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3tiqucffo.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3mfnsdjpm.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3czwdkdvr.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3orzgzxtd.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3qtwfoqic.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3nhctkvjs.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3mryedbyk.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3pfikzyur.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3svfkdkdn.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3rltybqgh.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3ubrpcfia.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3zqwtnbbl.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3guwxmsly.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3itdlhodw.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3umrgnocj.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3tuwmcrxm.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3mwuttqzw.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3chhbomav.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3klxyjxxq.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3npqyjkqn.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3uohzmcqa.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3mutlnaiv.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3vopggycx.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3aqnkzmzb.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3enzskozj.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rootgwzt.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3jindtble.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3czboceiu.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3mdutzuln.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3btkxcdet.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3vjckwoda.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3vwrvnbiv.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3qwhfnibg.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3rrknlgre.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3mixwntks.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3afiecqnz.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3edcewksx.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3hfdgsncl.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3rprccpkf.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3zpbczope.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3kvjyaofv.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3bgpitfky.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3whnltspc.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3ftzednes.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3eqxvtmrf.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3drklywhy.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3uzwfnghj.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zxxpxytq.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3xfmjzwap.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3dltaksrz.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3qnqlnztj.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3nkrngnfr.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ohxburrs.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ljicstwx.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3wshvbeeq.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3boneumow.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3uztgyjya.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3jiszawet.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3dqfgkaui.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3qqtyrjkk.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3gwdnzxqr.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3nxrnvigk.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3ddjiqcyj.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3aoxduynv.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3twblnjbs.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3qjmaadkx.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3kpeudoku.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3thvzibpk.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3cwmekhvi.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3qrnowhfe.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pjhvfikx.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3wuopwsec.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3iiaxwcqy.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3zxtjyrae.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fevkuigt.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3sjdsrutg.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3atzdhtae.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3iauyalrj.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3pkcrutkg.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3hqmtjaoi.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3gwepcjup.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3sequkjrd.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3kxfkotxs.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3pmyhayzf.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3tgwuikdc.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3sqxetmst.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3mzlikkkr.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3osqitdfz.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wjfwyrcs.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3mbsdfgaj.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3irbadqpz.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3ngsnnsdk.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3syvrkazl.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3pghiszae.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3bgjqmmyv.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3jdtxojxu.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3hbahnhlx.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3yvzdtgtt.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3lzbgoeso.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3dcblptwl.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3fylnazhd.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3pibavknk.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3aqpjagur.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3qujzzgka.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3gicwhozr.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3rsrlehlf.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3uyzbwbxg.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3dgdurqrg.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3qsopkrmp.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3tfqokebw.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3iuoagaeq.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3kmrpwwle.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3tmjmfnqo.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3sqyeprqr.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3drtexcyf.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3uccndfwy.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3xwhvwkmy.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3nsrxotsw.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3cprnddsj.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3mvfdeujm.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3vmmvaxcn.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ijaectlj.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3xlcsslxn.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3xvtsdpzl.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3airmzdss.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3zsingevw.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3eskabuft.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3jtopcsip.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3tvqnraux.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3iebdogja.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3dhomkhwz.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3utbvrxyd.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3tuxvrfsv.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3odxmycfw.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3vllkzhsb.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3orztbocj.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3xbmamcjs.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3ugjmkgjs.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3nitxeztn.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3asrhkrcu.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3mvpbagtv.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3cuenyqda.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nlqrnkmi.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3honmxifb.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3xbnfzwfq.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3ofmlzzqe.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3acihekxu.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3aqdampwm.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3kcuhllby.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3bejwsfst.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3orqbhprl.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3xsyyenal.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3opljdfcf.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3ztmilsyt.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3fkjvicxd.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3hvkztkwr.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3facyyybh.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3diasnrtc.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3psvtyfde.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ckisvlmq.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3vnbxlaqx.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3ktuynyvi.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3iygaahjz.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3llsxqyun.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3xstrxrwt.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3qvntusxp.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3yxdunqtn.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3pzxzhogb.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3usbxsgfv.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ioxrcuhy.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3jsjbowhg.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3mlslehfx.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3gqkyhxdl.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3jqzvqcvg.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3bybmeyww.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3rteomdno.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3xlnzfdjt.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3gspxrags.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3nztmcrum.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wejmovfn.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3yulkdnhs.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3juecvrtu.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3natabdkd.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xurhfzxo.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kpskpmyq.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3jsxgrupi.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rkonrkoy.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3ouankiex.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hbopohvi.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3tfxtfrol.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3shnhgsmx.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3cjbehlxo.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3ogrudgbg.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3gmgiarve.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3ikquouad.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3iecmkfvg.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ooyfobep.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3dtqbwgri.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3gakexgpi.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3glemrucf.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3sqputfny.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3porcaxnq.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3wfgzowjv.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3vhcsntdq.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3toacppst.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3iohxneuj.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3zphshaqi.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3enulceaw.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3aqbrnabo.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3yzzidljn.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3spziayez.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3cahfyzsf.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3kjzpidcq.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3xxwimxkh.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3wwtsxvwf.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3uejxjdbz.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3iojielim.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3kefjiquq.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3mnmhxupi.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3vpnxcllt.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gdpuoegp.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3akbppeut.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3osrsuwic.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wytxqjbt.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3pzzxxyfq.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3nnepeluc.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3wywevrhi.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3kcgitlxe.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3tebuaggl.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3diqbrimt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3joylvaoo.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3agkxgafy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yxbvdeap.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3xdmufijy.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3hfsnbosf.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3cnahfvdu.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3uufpuzic.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xacmfojl.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3vldyrgoe.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3icwlpmtx.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3xdvdqjee.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3gsazcnha.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3iidsvzeg.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3svqvajso.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3cswatsmm.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3vngomcrv.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3kblzfevb.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3lxlzdlmp.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3pchzckia.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3zizpwskl.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3mkcpefei.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3hjttvorz.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3achqywyi.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3dausbuxz.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3yhucsirl.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3npqgltdp.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3rjroyfxy.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3woutjltu.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3timjorvd.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3wilwyjkm.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3uiwcjylw.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3oybhroqi.html


<!-- 参考信息 -->