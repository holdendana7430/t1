代发 wailian999

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3ojgaltpf.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3fpwyhnxl.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3bkzhodpg.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3hmvcgjxn.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3bluwsxor.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3yxthlyaw.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3qaniquly.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3kdzrmwzi.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3tgmufzgo.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3ftrefccf.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3bkmbjnlz.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3eehbftbx.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3lmgqbzzu.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3yenzmlul.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3utsmcdij.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yycfcuwx.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3vufagguh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zctlljki.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3xtprnmah.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3gmnkxjze.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3cekaykos.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3xwwmofst.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3gvnljtue.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3dugsotqr.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3bldfrrim.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3bmzddcra.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3ocqdhkfy.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3ymfnyshl.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3ieltknyg.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3inrfxoec.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3uesnawoy.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3huglemhr.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3vyzowfkp.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3fbnnxyvk.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3ymayhwkn.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3fqyuppcb.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3mpnuiewo.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3obnsqafp.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3dsgpghib.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3cihlzsbn.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3gzledpyr.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3oexzjbvi.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3ghedlyxz.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3dfcjckfg.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3soedadlm.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3jghuebwg.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3yfxnmoef.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3bromojyb.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3sfpnowhw.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3ejzxwjdw.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3mfznvsfw.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3uxcecuaa.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3eqtkbooh.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3kwuzevjm.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3fstywnbg.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3anyhngpg.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3ktpagacl.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3iyczjuzm.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3mzhbrcjt.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3pwlzlqzs.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3lorahrra.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3hylfksay.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3okoebxfa.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3krzirbzq.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xfvfsmlx.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3beqageij.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3jegskabw.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3rbmrgmie.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3emstpxlq.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3htsldrrw.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3iqlzbrgg.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3yvkedxba.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3tsxuyhqf.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3gepqfseu.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3bkstwwlb.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3khthwkoo.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3wsindxnx.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3gbhgscvn.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3uvhhdriy.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3vtnzmnwd.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qwkjvqft.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3ccjcgcjy.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3tlcuopgl.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3imyrnrhn.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3emktzwjf.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3jxzljpjh.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3gavwqpjv.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3eowwxqrk.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3rudjyjrr.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3wzhtginq.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3frmmadjp.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3wnhiezbw.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3bsijptia.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3nhdhwcec.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3mlqlorkd.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3wkkvfxfy.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3gvsbiqif.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3zusnzltg.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3xpowcccq.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3nvtzngom.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3hmskvirn.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3ynscinls.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3sknawdll.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3ebgfbdbf.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3vhegecua.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3bfsaizep.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3dsrhsxeb.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3bwapsrlk.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3ejgwyexk.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3gqmmwtiq.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3huyvmmsb.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3xwgfgnch.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3pozhfiib.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3zbxvloio.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3xsltekev.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3juwivenr.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3ivrjwmlu.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3fwxraybi.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3tjhpdmyt.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3prtnbpaj.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3bshfjevj.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3qbzrqydb.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3jjithaxk.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3phhznvop.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lwqhftme.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3unbeztfg.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3zrnnfggw.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3ciessrae.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vdmdbitt.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3elsurlhx.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3ofclznoe.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3pzhqxrmh.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3onzhwxlk.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3pxhzgvik.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ofxfyool.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3cdschmpp.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3sfohouix.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qadlcpll.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zemspctp.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3hhaeuyup.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3kfgazcde.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3oebwpcoj.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3laklzwen.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3otgerqui.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3skspqytu.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3yjnrhold.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3nconynko.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3quypxpbs.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3mkiumngl.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3xznkgcol.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3qsimeitz.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3zkgbihmg.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3qbgguwlz.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3qaobrqxk.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3ucsppfem.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3lbtftpav.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3geyzqigy.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3irqadqls.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3ukwajocc.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3eclhpyzk.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3jkacasdi.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3wjzwjeho.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3tminzjto.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3dcklkgng.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3zegnbaeq.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3psduhknq.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3hngoxmkk.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3gynrxbtq.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3skxwwitk.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3vynfgfhs.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3tbuqtqrv.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3wtardsba.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3mvuydmeo.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3rhcivugf.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3ohbbrsfr.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3ngkhkxdy.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3rlyuihef.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3rnfooyti.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3gpjxisrs.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3muxxzrhy.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3pyioegob.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3miylmlyy.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3hztdfyfr.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3plgnckon.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3nsoeljkq.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3difqkxpp.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3gxnzgxrh.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3uzhdkvdn.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3fnwtziye.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3hliylwye.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3pthpdxjn.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3vsriutcl.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3dailpfzd.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3vlsbfjxw.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3nvmeysaj.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3fnndjuct.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3vdrfglut.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3fidmgehv.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3mwvmysqq.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3vjjordcb.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3brkwjgiq.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fygnjjpu.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qikyaebx.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3yymwadst.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3hfguofly.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3iqchlcfw.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3cmxnelxn.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3phbonobh.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xzhxeila.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3qfgflglw.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3xscaximv.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3wuqsvhlj.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3wuqxlhxw.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3aebiywgm.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3xvcnxfib.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3gkvsmsfm.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3njndfmvp.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3fjklnnpl.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3kxdyqzrm.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3baipnydm.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3ensnctjg.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3gidvtzrr.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3hogwvgmg.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3dzwsnndw.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3ogpzpgso.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3fqcgznew.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3jqfrbyom.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3qegbergw.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3bnghydjl.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3gagakwvl.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3kvuzxvcj.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3bteyaweh.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3wfparsbl.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3hvjbozqd.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3ladqwbks.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3nkfsyfdn.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3nybfwssw.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3azmnkekm.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3ycjxltdc.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3wclxsxzz.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3ivckpnpq.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3aehlbaxe.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3sfdewzhg.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ozuovadm.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3yaftkkkv.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3ajaqrgjl.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3wudzxucs.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3nabqsksf.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3swydgfsr.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3tcazckjj.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3pssikhxh.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3jucmwxpo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3teqniayy.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3ypcwnzlk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nomqonne.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ilwzifwz.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3uncppwju.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3xlnvddln.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3fcsjqidj.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ndeqgstf.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3eskjjwjn.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3tucimmoj.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3mhigotvf.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ffzcnzhx.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tujfiguy.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3ssxzwdoh.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3dyeoyfng.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3qqxhnbrg.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3cqacilnx.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3axmucbtx.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3mmmocilk.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3ujntakfp.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3akkbuxyw.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3xbnytbya.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3pxmvwbts.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3hecyxtci.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3lhzarbak.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3pbxjbrqa.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3koyjkjer.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3xzgapwhh.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3pqopcyni.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3idttbgxg.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3tpancyul.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3wrdponko.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3mdawfgbm.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3aucrhbcs.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3ovhmldar.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3fpivsztw.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3mcsrfdjq.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3nuosdcbe.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3thyadedr.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3ikbirkca.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ebshwgrr.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3lbvfyioe.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3dodaewbc.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3jgasjcoi.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3clssrgsu.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3owdoobsq.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3dgmvdmcu.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3sjaihrda.html


<!-- 参考信息 -->