代发 wailian999

PHP:  (function () { echo "run"; })();
来源：http://www.share.hesvh.cn/Article/details/gsoublouh.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.zdbjq.cn/Article/details/ggtorbtbe.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.hesvh.cn/Article/details/gtkjqgsil.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.zdbjq.cn/Article/details/gqslodaah.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.fehbvm.com/Article/details/gralmvews.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.fehbvm.com/Article/details/glwytnoab.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.hesvh.cn/Article/details/gvoqwpmke.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.fehbvm.com/Article/details/gxqagwscv.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.zdbjq.cn/Article/details/grkrnidnr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/gfxjrmzet.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.hesvh.cn/Article/details/gabzferxh.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gqrqbebsk.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gzfsbqblj.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.hesvh.cn/Article/details/gaccowolb.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.fehbvm.com/Article/details/gxtkytblr.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.fehbvm.com/Article/details/gbmbhvabr.sHtML

[C14] 泛型函数
来源：http://m.share.hesvh.cn/Article/details/glgcqfufc.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.zdbjq.cn/Article/details/gmsclqabl.sHtML

PHP:  // 无泛型
来源：http://mobile.hesvh.cn/Article/details/gmjlbkcob.sHtML

JS:   // 无泛型
来源：http://3g.zdbjq.cn/Article/details/gigwcblgl.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.zdbjq.cn/Article/details/getlgmbpj.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.fehbvm.com/Article/details/geiffbczb.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.hesvh.cn/Article/details/gcrvsbpgh.sHtML

Ruby: # 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/gbhccibzl.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.fehbvm.com/Article/details/glswsoccf.sHtML

[C15] 解构 / 展开参数
来源：http://blog.fehbvm.com/Article/details/gobcmnbyt.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.fehbvm.com/Article/details/gheaaykfv.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.fehbvm.com/Article/details/grdmjyznf.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gvomppuom.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.zdbjq.cn/Article/details/gpzeadtty.sHtML

Java: // 无解构
来源：http://3g.fehbvm.com/Article/details/gvdumveoi.sHtML

Go:   // 无解构
来源：http://wap.zdbjq.cn/Article/details/gcwmwfhtd.sHtML

Ruby: a, b = pair
来源：http://wap.fehbvm.com/Article/details/gwpiajjrx.sHtML

C#:   var (a, b) = pair;
来源：http://baike.fehbvm.com/Article/details/gmwayzoca.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.hesvh.cn/Article/details/gaejalhrp.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.fehbvm.com/Article/details/gphgwjqvb.sHtML

PHP:  // 无重载
来源：http://mobile.fehbvm.com/Article/details/gmyijcwbg.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.zdbjq.cn/Article/details/gzjapldfp.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.hesvh.cn/Article/details/gtvwvrryl.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.zdbjq.cn/Article/details/geovcizyq.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.zdbjq.cn/Article/details/gpxaxrmhs.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.hesvh.cn/Article/details/glchnnkio.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.fehbvm.com/Article/details/ghpwdqmvc.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gsgyltcdv.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.fehbvm.com/Article/details/gwxaxfifk.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/grvtgwwgp.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.hesvh.cn/Article/details/ggrukoniz.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.zdbjq.cn/Article/details/gmfdxwdnp.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.hesvh.cn/Article/details/gzzntvrnr.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.hesvh.cn/Article/details/gjfwiuuoe.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.hesvh.cn/Article/details/gqbjjimwo.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.hesvh.cn/Article/details/gejgmuvbb.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.hesvh.cn/Article/details/ggidojqmm.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.zdbjq.cn/Article/details/gwrodafys.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.fehbvm.com/Article/details/gwxwmuyyp.sHtML

[D02] 追加元素到末尾
来源：http://m.share.fehbvm.com/Article/details/gctyvyrop.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.hesvh.cn/Article/details/geekldyxr.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.fehbvm.com/Article/details/gxzqzfgyh.sHtML

JS:   arr.push(4);
来源：http://m.share.zdbjq.cn/Article/details/ggktpuqgp.sHtML

TS:   arr.push(4);
来源：http://www.m.share.hesvh.cn/Article/details/ggbaakiao.sHtML

Java: list.add(4);
来源：http://www.m.share.hesvh.cn/Article/details/glmdrpjwg.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.zdbjq.cn/Article/details/gltjavijo.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.fehbvm.com/Article/details/gawwaturn.sHtML

C#:   list.Add(4);
来源：http://wap.hesvh.cn/Article/details/grcaitufb.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.zdbjq.cn/Article/details/gjqkbijru.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.hesvh.cn/Article/details/ghsbgkgtu.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.zdbjq.cn/Article/details/gswkvxkqs.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.hesvh.cn/Article/details/gpcbbxjyp.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gqnxyqkfg.sHtML

Java: list.add(0, 0);
来源：http://mobile.hesvh.cn/Article/details/gehzwhtix.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.zdbjq.cn/Article/details/gsskbgnwb.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.zdbjq.cn/Article/details/gqukpgryr.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.fehbvm.com/Article/details/gstawrikp.sHtML

[D04] 删除元素
来源：http://blog.zdbjq.cn/Article/details/ghnqcjgtr.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.hesvh.cn/Article/details/gdlullczh.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.hesvh.cn/Article/details/gmgobxtuk.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.hesvh.cn/Article/details/grretjrfz.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.hesvh.cn/Article/details/gyclhihht.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.zdbjq.cn/Article/details/glffdsqdt.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.zdbjq.cn/Article/details/gufspmqbc.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.fehbvm.com/Article/details/grdgqjmvq.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.fehbvm.com/Article/details/gwoqdunwa.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.fehbvm.com/Article/details/gvukrrcvw.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/ghfqahylv.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/galfmeuaz.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/gwpsolbkw.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.fehbvm.com/Article/details/gxrwiqdor.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.fehbvm.com/Article/details/gjbsgqmvr.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/ghijaxtua.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/grqvjyefy.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gvsgqptkc.sHtML

[D06] 数组长度
来源：http://baike.hesvh.cn/Article/details/gmnvtzqmm.sHtML

Py:   len(arr)
来源：http://baike.fehbvm.com/Article/details/goyvmuwzm.sHtML

PHP:  count($arr);
来源：http://wap.hesvh.cn/Article/details/gyksribqs.sHtML

JS:   arr.length
来源：http://www.m.share.hesvh.cn/Article/details/gdurjasjb.sHtML

TS:   arr.length
来源：http://mobile.hesvh.cn/Article/details/gwhbxmrlm.sHtML

Java: list.size();
来源：http://wap.fehbvm.com/Article/details/gzqlmvoxe.sHtML

Go:   len(arr)
来源：http://blog.fehbvm.com/Article/details/gungedukg.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.fehbvm.com/Article/details/gcdigmtzx.sHtML

C#:   list.Count;
来源：http://read.share.fehbvm.com/Article/details/ggynorkvs.sHtML

[D07] 切片 / 取子数组
来源：http://baike.zdbjq.cn/Article/details/gejhhuilx.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.zdbjq.cn/Article/details/godyrzxft.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.fehbvm.com/Article/details/gompzqjrn.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.hesvh.cn/Article/details/gkukldfyw.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gbfxzlfqw.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/grvstudmv.sHtML

Go:   arr[1:4]
来源：http://blog.zdbjq.cn/Article/details/ghvgqbhpb.sHtML

Ruby: arr[1, 3]
来源：http://wap.hesvh.cn/Article/details/gnhvgomrq.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.zdbjq.cn/Article/details/gyidtfxsf.sHtML

[D08] 合并两个数组
来源：http://www.m.share.hesvh.cn/Article/details/gbuljbzfy.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.hesvh.cn/Article/details/gifahpbwt.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.hesvh.cn/Article/details/gqxjhcgdd.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.zdbjq.cn/Article/details/gwqlbgadg.sHtML

TS:   [...a, ...b];
来源：http://wap.hesvh.cn/Article/details/ggvugenmq.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.hesvh.cn/Article/details/gpsvmxgka.sHtML

Go:   append(a, b...)
来源：http://baike.fehbvm.com/Article/details/gvnzuartk.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.fehbvm.com/Article/details/gnfsrbfxp.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.fehbvm.com/Article/details/gtgaoqorq.sHtML

[D09] 排序（升序）
来源：http://www.blog.fehbvm.com/Article/details/gcawkyzmr.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.zdbjq.cn/Article/details/gjiictkcm.sHtML

PHP:  sort($arr);
来源：http://3g.zdbjq.cn/Article/details/glitebssn.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.fehbvm.com/Article/details/ghaxiebim.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.zdbjq.cn/Article/details/gusbyclxx.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.zdbjq.cn/Article/details/gzsocqrkm.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gmeoiflny.sHtML

Ruby: arr.sort
来源：http://www.m.share.fehbvm.com/Article/details/gguvvysds.sHtML

C#:   list.Sort();
来源：http://www.blog.zdbjq.cn/Article/details/gozbbexxn.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.zdbjq.cn/Article/details/gkieiolsd.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.hesvh.cn/Article/details/gnojpkyma.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fehbvm.com/Article/details/gmzuichle.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fehbvm.com/Article/details/gjutidspr.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fehbvm.com/Article/details/gyvmvjpxl.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.hesvh.cn/Article/details/gpbxiyuwr.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.hesvh.cn/Article/details/giertgmww.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.zdbjq.cn/Article/details/gjscmgkvw.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.hesvh.cn/Article/details/gxzzbzryq.sHtML

[D11] 反转数组
来源：http://3g.fehbvm.com/Article/details/gatuisaru.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.zdbjq.cn/Article/details/gelixherw.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.fehbvm.com/Article/details/gpdxoochh.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.hesvh.cn/Article/details/gijryoveh.sHtML

TS:   [...arr].reverse();
来源：http://blog.fehbvm.com/Article/details/gpmyrvueb.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.zdbjq.cn/Article/details/ggraxbygn.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.fehbvm.com/Article/details/ghulrzaza.sHtML

Ruby: arr.reverse
来源：http://wap.fehbvm.com/Article/details/gziovkzmv.sHtML

C#:   list.Reverse();
来源：http://mobile.zdbjq.cn/Article/details/ggqwhhkou.sHtML

[D12] 查找元素下标
来源：http://m.share.hesvh.cn/Article/details/gyecppjgw.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.zdbjq.cn/Article/details/gqgrygatd.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.zdbjq.cn/Article/details/goypxvmrh.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fehbvm.com/Article/details/gjxigaiok.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gjmemqlif.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.hesvh.cn/Article/details/gwddfeyxv.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gkmqjkhpb.sHtML

Ruby: arr.index(x)
来源：http://read.share.zdbjq.cn/Article/details/gntqlvatu.sHtML

C#:   list.IndexOf(x);
来源：http://3g.hesvh.cn/Article/details/gunjzazra.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.zdbjq.cn/Article/details/gocfgjcog.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.fehbvm.com/Article/details/gakggkapw.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.hesvh.cn/Article/details/gtitnordf.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.hesvh.cn/Article/details/gpubpglow.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.fehbvm.com/Article/details/gzdegilho.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.hesvh.cn/Article/details/gfjljcmvw.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.fehbvm.com/Article/details/gkctlvhmu.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.zdbjq.cn/Article/details/gtzzpsmgz.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gnurgpspm.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.zdbjq.cn/Article/details/gwpojmhrt.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.zdbjq.cn/Article/details/gxmkzzkga.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.fehbvm.com/Article/details/gwbuscuwb.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.zdbjq.cn/Article/details/gcojcueki.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.hesvh.cn/Article/details/gsnyhjrbr.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.zdbjq.cn/Article/details/gurucpopu.sHtML

Go:   // 手写循环
来源：http://www.share.zdbjq.cn/Article/details/gnxjiyldt.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.fehbvm.com/Article/details/gsjattaaw.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gacyknznk.sHtML

[D15] 去重
来源：http://wap.hesvh.cn/Article/details/gqrpvcluj.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.hesvh.cn/Article/details/gtewlzydj.sHtML

PHP:  array_unique($arr);
来源：http://blog.zdbjq.cn/Article/details/giedqfcqp.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.zdbjq.cn/Article/details/gzegrkkil.sHtML

TS:   [...new Set(arr)]
来源：http://baike.fehbvm.com/Article/details/gcvmaehde.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.zdbjq.cn/Article/details/gghiyjpxy.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.zdbjq.cn/Article/details/gqgsprnud.sHtML

Ruby: arr.uniq
来源：http://www.share.zdbjq.cn/Article/details/glbubiijc.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gxiobapdw.sHtML

[D16] 求和与平均值
来源：http://m.share.fehbvm.com/Article/details/gslwjrgbh.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gogoisjcy.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.fehbvm.com/Article/details/guwcwwdmd.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.hesvh.cn/Article/details/gotnnzdlp.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gprwgdbei.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.zdbjq.cn/Article/details/gqepajtby.sHtML

Go:   // 手写循环累加
来源：http://baike.fehbvm.com/Article/details/gsrhxjron.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.hesvh.cn/Article/details/gyacqqbxb.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.fehbvm.com/Article/details/gwwzscmgu.sHtML

[D17] 最大值与最小值
来源：http://m.share.fehbvm.com/Article/details/gyzblitnd.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.hesvh.cn/Article/details/gulmvspab.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.hesvh.cn/Article/details/glkjhhndw.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.zdbjq.cn/Article/details/gfquvxnnz.sHtML

TS:   Math.max(...arr);
来源：http://www.share.hesvh.cn/Article/details/gbyzueocu.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.hesvh.cn/Article/details/gztcgbzbk.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.zdbjq.cn/Article/details/gntethgas.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.zdbjq.cn/Article/details/gzsozrekc.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.hesvh.cn/Article/details/gkgsszzyu.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.hesvh.cn/Article/details/gqoosgihx.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.fehbvm.com/Article/details/gwucvpmqi.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.fehbvm.com/Article/details/gjjanjglq.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.hesvh.cn/Article/details/ghkhdunos.sHtML

TS:   nested.flat();
来源：http://baike.zdbjq.cn/Article/details/gcmnwbzzq.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.hesvh.cn/Article/details/gprbctohd.sHtML

Go:   // 手写双层循环
来源：http://m.share.zdbjq.cn/Article/details/gydzbvqyy.sHtML

Ruby: nested.flatten
来源：http://m.share.zdbjq.cn/Article/details/gmcfwjnpi.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.hesvh.cn/Article/details/gefochfuk.sHtML

[D19] 按字段分组
来源：http://blog.hesvh.cn/Article/details/gjamvkffg.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.zdbjq.cn/Article/details/gwkzfpqri.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.zdbjq.cn/Article/details/gmynhmokq.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.hesvh.cn/Article/details/gaclixxnu.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.fehbvm.com/Article/details/gslfbzukb.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.hesvh.cn/Article/details/gwxubgdbp.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.fehbvm.com/Article/details/gibgexrvy.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.zdbjq.cn/Article/details/grvzaxgeg.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.hesvh.cn/Article/details/gruveqmya.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.zdbjq.cn/Article/details/gapniqpay.sHtML

Py:   Counter(arr)
来源：http://baike.hesvh.cn/Article/details/gsxveatph.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.hesvh.cn/Article/details/gucyjrwuv.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.hesvh.cn/Article/details/gyfqarldp.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.zdbjq.cn/Article/details/ghsawyyyo.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.hesvh.cn/Article/details/giyrwqapf.sHtML

Go:   // 手写 map[T]int
来源：http://3g.hesvh.cn/Article/details/gagehjnbg.sHtML

Ruby: arr.tally
来源：http://wap.fehbvm.com/Article/details/gurcbxnzh.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.hesvh.cn/Article/details/giulzaujv.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.fehbvm.com/Article/details/gacstysbx.sHtML

Py:   x in arr
来源：http://m.share.hesvh.cn/Article/details/gjgunjwtq.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.zdbjq.cn/Article/details/gjngtpfet.sHtML

JS:   arr.includes(x)
来源：http://m.share.hesvh.cn/Article/details/gvkypvrkb.sHtML

TS:   arr.includes(x)
来源：http://www.blog.fehbvm.com/Article/details/ggtmwsbtq.sHtML

Java: list.contains(x)
来源：http://baike.hesvh.cn/Article/details/gxssmfhrm.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.fehbvm.com/Article/details/garofdgaw.sHtML

Ruby: arr.include?(x)
来源：http://www.share.hesvh.cn/Article/details/gmhvlkzlm.sHtML

C#:   list.Contains(x)
来源：http://blog.fehbvm.com/Article/details/gkbbbwwff.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.zdbjq.cn/Article/details/gqgcenpiu.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.fehbvm.com/Article/details/guqmrmwob.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.hesvh.cn/Article/details/glaxizgju.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gyyxnbmsl.sHtML

TS:   [...arr];
来源：http://read.share.hesvh.cn/Article/details/gjniyaohb.sHtML

Java: new ArrayList<>(list);
来源：http://baike.zdbjq.cn/Article/details/guckunqyl.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.hesvh.cn/Article/details/gydamsfne.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.hesvh.cn/Article/details/gyazrpvtd.sHtML

C#:   new List<int>(list);
来源：http://www.share.fehbvm.com/Article/details/ghafldvzp.sHtML

[D23] reduce 累积计算
来源：http://wap.fehbvm.com/Article/details/gzrklkjcm.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gfsoafgkq.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.hesvh.cn/Article/details/guekrmhzk.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gktmsjkqq.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gknosodhw.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.fehbvm.com/Article/details/gcwkoljse.sHtML

Go:   // 手写循环
来源：http://www.m.share.fehbvm.com/Article/details/gpwipdacz.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.zdbjq.cn/Article/details/gyamrjqys.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.fehbvm.com/Article/details/gqrznbetz.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.zdbjq.cn/Article/details/guhjwnexo.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.hesvh.cn/Article/details/gityywnxe.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.fehbvm.com/Article/details/gvbsdekwx.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.hesvh.cn/Article/details/gtvocjffe.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gdvviagom.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.fehbvm.com/Article/details/gyaertjww.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.hesvh.cn/Article/details/gbxyoklps.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.zdbjq.cn/Article/details/ggexwouts.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.zdbjq.cn/Article/details/gtriddjbi.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.zdbjq.cn/Article/details/gqeuhagud.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.zdbjq.cn/Article/details/gaglefybi.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.hesvh.cn/Article/details/gupflzotu.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.hesvh.cn/Article/details/gwwrhfwpm.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.hesvh.cn/Article/details/ghgpptmbz.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.fehbvm.com/Article/details/gheqmixmd.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.hesvh.cn/Article/details/glbvnqnqr.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.fehbvm.com/Article/details/gpsncnmha.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.zdbjq.cn/Article/details/gjsiakmvl.sHtML

[D26] 数组转字符串
来源：http://baike.fehbvm.com/Article/details/gpufdveiz.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.fehbvm.com/Article/details/gorgacsvb.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.zdbjq.cn/Article/details/gbudxfvyf.sHtML

JS:   arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/gmkzciiuc.sHtML

TS:   arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/grpefduzl.sHtML

Java: String.join(", ", list)
来源：http://www.blog.fehbvm.com/Article/details/gsrsxydtm.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.fehbvm.com/Article/details/gwsjffysy.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/gcfbhlfvv.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.zdbjq.cn/Article/details/gkrlgxguv.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gnerjqxyn.sHtML

E. 字符串处理
来源：http://www.blog.fehbvm.com/Article/details/gnypeonxy.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gziohnuwg.sHtML

[E01] 拼接字符串
来源：http://read.share.hesvh.cn/Article/details/gelinxmhx.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.fehbvm.com/Article/details/gknnyaypr.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.fehbvm.com/Article/details/gowwpbxgb.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.hesvh.cn/Article/details/govbwyrap.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.hesvh.cn/Article/details/gcllkcalf.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.hesvh.cn/Article/details/gboixoonp.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.hesvh.cn/Article/details/gbgdvqrdd.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.fehbvm.com/Article/details/gbybjbsur.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gdmrilopa.sHtML

[E02] 重复字符串
来源：http://3g.zdbjq.cn/Article/details/gfydrhnku.sHtML

Py:   "ab" * 3
来源：http://baike.hesvh.cn/Article/details/gbielsggv.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.hesvh.cn/Article/details/gffvauagu.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/gddijaxoj.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gsxgocafs.sHtML

Java: "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/gpdoejrfh.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.zdbjq.cn/Article/details/gxxfqtsjb.sHtML

Ruby: "ab" * 3
来源：http://m.share.zdbjq.cn/Article/details/gnrzwysvu.sHtML


<!-- 参考信息 -->