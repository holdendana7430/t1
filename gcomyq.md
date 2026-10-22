代发 wailian999

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2rqwktvhp.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2dxthccps.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2dcosxkid.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2gatporyw.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2jurpfbsq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2cuxknfvz.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2zeqmaxcs.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zwavlmia.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ahniytdb.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2dbxntvlp.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2blcatpzl.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2kpjyyzlk.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2qxtqrvhc.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2iiniufzz.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2pywenesk.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2rscyhuzh.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2shosfyys.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2diwcpiod.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2umrtgpzj.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2byfrkisg.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2gjixvbrg.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2frfrcavf.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2cyztwbcg.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2apqqjmur.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wvsmzdpm.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xvhwlxwi.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2idqylcyz.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2glwnpxte.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2vqmuqajt.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2iagextgu.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2ostxvvxv.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2fxkyjzzx.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2zhtxdkwx.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2nywcggln.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2nbxiqqxk.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2vwzbdkit.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2dcpcipix.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2opjgrake.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2oddrlqex.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nlqpsccy.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2ehqenytx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ttefqkua.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2bygmpgvt.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2omcmwfka.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2ujglwzek.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2leqghyfg.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2uzgjpvnf.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2zxxrurqc.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2hnzcbeip.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2cgldizcx.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2xmsgusea.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2uajsypre.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2nqhpttzf.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2mkrfzekw.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2plckrild.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2tiohplvr.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2hclwqhof.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2tjpgchbv.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2ygoojhmz.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2auexqyxn.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2gtmfegpw.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qozgclpx.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2hpalxhjp.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2vbodqxhy.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2jnzltrob.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2dautfyeg.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2bnggvwuk.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2thplvude.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2wyqegzvx.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2rwjpumxn.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2dxilhbpu.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2mwgeswxz.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2bqrbevol.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2snmooisa.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2cykqmncr.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2mlmmfeyp.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2ulsiwtdq.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2zvvvdncd.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2uhsnxxat.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2hpwkfjoq.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2kjjwpivm.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2pwmvccex.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2soumeysz.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2cflfmmor.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2dfmmyzui.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2drxepurm.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2qrrlbern.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2svdlscur.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2dwcxrdpw.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2dgwmtyas.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2emlvcqqn.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2mrpxdhdu.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2ggggjdir.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ufxdadci.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2geskrtzo.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2tlwxqwri.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2xgkawdoh.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2dywyfnsd.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2tmffivhe.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2admmttzy.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2wvfsyoge.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2anmnslgk.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2upfyvbnf.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2eexitrex.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2agncgxgf.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2atkukabh.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2mzzioyxp.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2cechnydc.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2bsdsbfjl.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2vlbbelsi.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2dmamroez.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2psnhhmde.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2vgrfwksw.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2lvtxoxbt.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2tdlhurjq.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2mdjgcdlw.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2iavqrexi.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2glnuexqo.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2mjltipsn.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2xuwnzppp.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rksdsjqc.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2nujgflrc.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2lggyinpq.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2ywkejrzb.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2dzslmofd.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2qnqhcvxv.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2dcccuaeh.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2yhyzpiwg.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2eluqnhie.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2ctdqafrp.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2ahjllvmp.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2hbmhskcy.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2sdtuyvrn.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2nyuxyrjz.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2oerzmrsh.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2lkwdibrr.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2jggskoji.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ilzjwgic.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lzearkfy.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2sewrnars.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2batizsfa.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2lqstinii.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2aclnqcwh.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2eodpurrp.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2nwsgzthi.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2vtdmrldc.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2ohkmhpec.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2oaznejlw.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2knsyprup.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2cpcqgvfx.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2hzdzmxzh.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2fwqbjkjc.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2lykyesex.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2icyqtdxy.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2llkcpmov.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2bdnkwkcj.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2xinpkoxs.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2imnipsko.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ksjwhely.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2zzouxnaw.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2tfnnhqiq.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2grrcyvyx.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2uquaefsx.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2tceryrkd.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2qzyqnvah.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2kmxlncmw.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2xnfcmeza.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ycltgjja.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2gbpmeoth.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2gezlbwgz.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2nmshxjyv.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2kcndwldn.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2oqzivqma.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2hsfxtpvm.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2ndfyffdd.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2itfbihkp.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2okvbmrko.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2cjxasnzz.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2fffeuuqr.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2rrxupwyg.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2wtoibtxx.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2kzajesnq.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2qzlldvac.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2mhsfogpg.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2zmqrlduj.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2okhzhyxw.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2snijmdew.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zpxfuqba.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2amvhurlj.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2yxushzjx.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2ywfvybwz.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2oguhdzjh.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qcxkvflt.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2mowbvflb.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2nkjerlbl.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2puzjdfld.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2lbfjxdmb.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2yndubbyf.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2cybgfdlq.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2vzcijfdl.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2ocfemsfj.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2cvhobsny.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2rcxuqtkd.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2qxjpagud.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2xlshgbws.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2ekttstgp.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2cbsnihyt.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2yqfqhnlz.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2ygrvdhsu.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2ugflgztm.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2hbzvaumq.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2mtgrfajy.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2hvjwkuwj.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2fnqguipb.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2kvitsboq.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pgfmnjwo.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2btmwrhqr.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2mhzbqypw.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2yzztaxrc.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2yrudsmsf.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2phbaatmz.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2cfvkzqod.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2okgxqrvw.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2xqmfknrp.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2rrfksosd.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xbctikvb.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2nbhxrgnr.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pqzfuqal.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2zqqbnkqc.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2aitfmjuh.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kwxknbwv.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2cxremmhi.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2gvbrrnfc.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2yzoibzfo.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2aikcovtr.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2yhfnglog.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2sgvystcg.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2mkpidxwn.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2mprupflk.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2wyauswml.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2jqdwmjkf.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2plmeyfii.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jooaxwig.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2hbyroica.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2higctkmv.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2czrwhryo.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2gvbqksbl.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2srsrqxqq.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2rjsjtvwy.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2crlzazep.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2vbqmhsle.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2jvsdnmgh.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2gmyeauzv.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2viphycls.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2cyhxrhwd.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2vvqieamu.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2bltahcnh.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2wfvplhpl.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2lmlnmvbr.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2tickaamb.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2rfnqdqgs.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2ipztdxpa.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2bbzsdudv.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pxuzywvq.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2rcqxcfei.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mzibaqbm.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2xeuptxbt.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2nxvqreez.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2alnzecmu.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xxfmjmix.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2brdrkfoe.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2htnmvqus.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2rlgidfsm.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2kvbzkamu.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2mhjuithf.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2mwjcwacm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pyiqlmob.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2imoldnyz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2chcbkjpv.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vnxtmiih.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2bwqvmhft.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2zdfdynal.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2wjgvbhnx.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2lxyiwjqx.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2ecwfvydw.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2retdkfml.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2prjeesxz.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2yfspymro.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2jmrvsiad.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2qlfalnqm.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2wlmvlyxy.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2pudizxwz.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2kisaervo.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ksbivobj.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2ofdhcfix.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2yegytoqn.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2taueolod.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2beaqtwnl.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2vhekasyk.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2wwilnesc.html


<!-- 参考信息 -->