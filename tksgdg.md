代发 wailian999

ssh user@host 'uptime'
来源：http://hz.chenjidiqi.icu/gtmimmeguf.html

[R58] 下载文件
来源：http://hz.cheryme.top/gtzajhkrxf.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.cqqwz.cn/gteihwkuab.html

[R59] 发 POST JSON
来源：http://hz.cdnleiting.top/gtywsehuwk.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.zhixingplan.top/gteocdeyie.html

[R60] 只看 HTTP 状态码
来源：http://hz.svipenyu.cn/gttrhqcrix.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.shanyushiyangkeji.top/gtvbpywffc.html

[R61] 磁盘占用
来源：http://hz.pengpengdd.cyou/gtbqofpnya.html

df -h;  du -sh *
来源：http://hz.gotoacloud.top/gtutwhkphm.html

[R62] 找最占空间的文件
来源：http://hz.wangshuangyany.cn/gtkbmxiddv.html

du -ah . | sort -rh | head -10
来源：http://hz.shuidangran.top/gtykeqwnsh.html

[R63] 内存与进程
来源：http://hz.xinyue.icu/gtumljishb.html

free -h;  ps aux | grep nginx
来源：http://hz.dianchejie.cn/gtiydsnlof.html

[R64] 结束进程
来源：http://hz.pycfn.com/gtqqehrypb.html

kill -9 $(pgrep -f app.py)
来源：http://hz.gzhubu.top/gtbnphoksh.html

[R65] 查看端口占用
来源：http://hz.wangshuangyany.cn/gtjwraqslr.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.yueranfly.top/gthlbsbygg.html

[R66] 定时任务
来源：http://hz.gaohongyu789.top/gtnyhukfkn.html

crontab -e;  crontab -l
来源：http://hz.gogol.net.cn/gtpvynxsow.html

[R67] 生成随机十六进制串
来源：http://hz.gaohongyu789.top/gtgjgctwna.html

openssl rand -hex 16
来源：http://hz.zhiwuduotai.top/gtuqcdkwxy.html

[R68] 计算文件校验值
来源：http://hz.yangfankeji.com/gtxywmmcvq.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.svipenyu.cn/gtkqftfqtn.html

[R69] 生成随机密码
来源：http://hz.havefunace.top/gttwivihog.html

head -c 16 /dev/urandom | base64
来源：http://hz.hfpthk.cn/gtfjyyuorl.html

[R70] 时间戳与互转
来源：http://hz.sysykeji.top/gtoemoyfmk.html

date +%s;  date -d @1700000000
来源：http://hz.jqgufenzy.top/gtofakyllp.html

[R71] 日期格式化
来源：http://hz.xinyue.icu/gtcebipujb.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.hnxiangtu.top/gtsrmhbxfs.html

[R72] 等待端口就绪
来源：http://hz.xuetiantiany.cn/gtsjrlzmqn.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.aizwys.cn/gtdtheipts.html

[R73] 分割大日志
来源：http://hz.sxryk.cn/gtdhgqbfdp.html

split -l 1000 big.log part_
来源：http://hz.dianchejie.cn/gtoaextshs.html

[R74] 批量重命名
来源：http://hz.ybcxt.top/gtwosboryh.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.shangyingyoupin.top/gtlbwsphis.html

[R75] 导出环境变量
来源：http://hz.zhaomingkeji.xyz/gtuycwslbg.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.cqqwz.cn/gtbqegwsju.html

[R76] 使用临时文件
来源：http://hz.tian-w.cn/gttsbvbobh.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.fengsongda.top/gtbszhepcg.html

[R77] 读取用户输入
来源：http://hz.hfpthk.cn/gtgcnaoury.html

read -rp "请输入: " ans
来源：http://hz.hywenlv.cn/gtwjgdzecy.html

[R78] 交互式菜单
来源：http://hz.cashguo.top/gtucjaikhh.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.hnqzz.top/gtegvcizdt.html

[R79] 解析命令行选项
来源：http://hz.zhiwuduotai.top/gtdnxgcnqf.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.jiagoushi.top/gtfjribndo.html

[R80] 查看脚本执行耗时
来源：http://hz.nanxinkj.top/gtqcoysxvp.html

time ./run.sh
来源：http://hz.jqgufenzy.top/gtytapztwg.html

================================================================================
来源：http://hz.ydjk.org.cn/gtqgxumotu.html

S. C / C++ 专题
来源：http://hz.zhixingplan.top/gtmtfuazsw.html

================================================================================
来源：http://hz.ehwqpu.com/gtnpvbhfth.html

[S01] C：Hello World
来源：http://hz.ywan-chungtsiang.top/gtbjghyuci.html

#include <stdio.h>
来源：http://hz.fengsongda.top/gtblzcjgky.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.52xcode.cn/gtmhyaubpx.html

[S02] C：变量与格式化输出
来源：http://hz.xylfe.cn/gtktrwiuom.html

int a = 10; printf("%d\n", a);
来源：http://hz.nanxinkj.top/gteobtgfbd.html

[S03] C：读入整数
来源：http://hz.xuetiantiany.cn/gtiokbjxsh.html

int x; scanf("%d", &x);
来源：http://hz.andypj.xyz/gtvrniqcla.html

[S04] C：字符串复制
来源：http://hz.shanyushiyangkeji.top/gtuzdjriki.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.zhiwuduotai.top/gtodnmyhnu.html

[S05] C：字符串长度
来源：http://hz.xziqi.cn/gtukdiznis.html

strlen(s)
来源：http://hz.jyoumei.cn/gtvepoebdk.html

[S06] C：字符串比较
来源：http://hz.gotoacloud.top/gttfpobker.html

strcmp(a, b) == 0
来源：http://hz.hfpthk.cn/gtzdybrvqp.html

[S07] C：数组遍历求和
来源：http://hz.zhijiandao.cn/gtcopyecre.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.yueranfly.top/gtavqgsfdl.html

[S08] C：动态内存分配与释放
来源：http://hz.hysaishi.cn/gtuqwpxqcc.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.yuxming.cn/gterqrphuf.html

[S09] C：结构体定义与初始化
来源：http://hz.jinqigufen.top/gtoawcgaoa.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.meibo888.top/gtayrmzeak.html

[S10] C：指针与解引用
来源：http://hz.cqqwz.cn/gtdnypgxvy.html

int *p = &a;  *p = 5;
来源：http://hz.jinqigfzy.top/gtjxcfjtfz.html

[S11] C：逐行读文件
来源：http://hz.dianchejie.cn/gtqrdzpdrn.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.c1oappe.top/gtkqtwloth.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.hfpthk.cn/gtvenbxqxs.html

fclose(f);
来源：http://hz.yvedp.cn/gtxcummekt.html

[S12] C：写文件
来源：http://hz.aizwys.cn/gtfjpvgrbj.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.shuidangran.top/gtbzprnrrv.html

[S13] C：宏定义
来源：http://hz.yangfankeji.com/gtnenoyawn.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.xinyue.icu/gtcboalywy.html

[S14] C：枚举
来源：http://hz.xziqi.cn/gtfadskgrl.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.yj20258888.top/gtdvlqsqrm.html

[S15] C：类型转换
来源：http://hz.yueranfly.top/gthqzumkry.html

(double) a / b
来源：http://hz.zhoulong.xyz/gttpvvqmja.html

[S16] C：位操作置位
来源：http://hz.cdnleiting.top/gtllixhlij.html

x |= (1 << 3);
来源：http://hz.gaohongyu789.top/gtxxlgcdob.html

[S17] C：安全拼接字符串
来源：http://hz.ivvv.top/gtlbzxpiix.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.zycfv.cn/gtdczicscn.html

[S18] C：命令行参数
来源：http://hz.yuanzhike.top/gthhgghgxx.html

int main(int argc, char **argv)
来源：http://hz.tian-w.cn/gtincbjvxk.html

[S19] C：快速排序
来源：http://hz.fengsongda.top/gtwcjlyrib.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.yj20258.top/gtjyouxnwd.html

[S20] C：二分查找
来源：http://hz.ydzc1.top/gtifrxedng.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.ybcxt.top/gtergobuvy.html

[S21] C：字符类别判断
来源：http://hz.ywan-chungtsiang.top/gtyyrtznoo.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.jlsjyb.cn/gtqethtuvp.html

[S22] C：字符串转数字
来源：http://hz.yangfankeji.com/gtjjvfgjmy.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.cheryme.top/gttzdihvhi.html

[S23] C：随机数
来源：http://hz.yongpay.top/gtpccfdbiu.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.wangshuangyany.cn/gtrkdnknfa.html

[S24] C：获取本地时间
来源：http://hz.zhoulong.xyz/gtinxvjbnx.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.hfpthk.cn/gttbdsawki.html

[S25] C：内存拷贝
来源：http://hz.yj202588.top/gtqoecydzt.html

memcpy(dst, src, n);
来源：http://hz.aizwys.cn/gtqvwffkoh.html

[S26] C：内存清零
来源：http://hz.jianghu66.top/gtbrgnlril.html

memset(a, 0, sizeof a);
来源：http://hz.yangfankeji.com/gtmhpvxpyv.html

[S27] C：定义常量
来源：http://hz.zhiwuduotai.top/gtfzhynobm.html

const double PI = 3.14159;
来源：http://hz.sufxvd.cn/gtzauhifbn.html

[S28] C：静态变量
来源：http://hz.meibo888.top/gtbxjmximv.html

static int counter = 0;
来源：http://hz.hammf.cn/gtzoyavgkw.html

[S29] C：变参函数
来源：http://hz.shanyushiyangtech.top/gtxdfnabvc.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.nanxinkj.top/gtqpswvoou.html

[S30] C：头文件保护
来源：http://hz.aizwys.cn/gtdedrvswu.html

#ifndef X_H
来源：http://hz.nanxinkj.top/gtzsumxunz.html

#define X_H
来源：http://hz.cucudq.cn/gtwvxnataz.html

#endif
来源：http://hz.kuanghao11.cn/gtkwqjevtd.html

[S31] C++：Hello World
来源：http://hz.yuanzhike.top/gthshcfwfi.html

#include <iostream>
来源：http://hz.chenzaomai.com/gtdrbvptgf.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.zhijiandao.cn/gtkcltxmmj.html

[S32] C++：字符串
来源：http://hz.zhixingplan.top/gtbelxkqrz.html

std::string s = "hi";  s += "!";
来源：http://hz.fzhhl.top/gtylndlueq.html

[S33] C++：vector 增删
来源：http://hz.ydjk.org.cn/gtfjyezqaq.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.xziqi.cn/gtvhfzumjg.html

[S34] C++：遍历 vector
来源：http://hz.shanyushiyangkeji.top/gttkfxfvhp.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.9152youxi.cn/gtxzgkmjhm.html

[S35] C++：map
来源：http://hz.cqqwz.cn/gtrwauopra.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yanxiufei.cn/gtytrpiwcj.html

[S36] C++：unordered_map
来源：http://hz.jinghuilouyu.cn/gtfrwngihm.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.pengpengdd.cyou/gtfkozmmyo.html

[S37] C++：set
来源：http://hz.zhengqikj.top/gtsvsigowq.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.sufxvd.cn/gtelioysvm.html

[S38] C++：排序
来源：http://hz.pengpengdd.cyou/gtyenfngqn.html

std::sort(v.begin(), v.end());
来源：http://hz.cheryme.top/gtzrbmztxc.html

[S39] C++：自定义比较器排序
来源：http://hz.xziqi.cn/gtgbcgfkwc.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.chenlongwang.top/gtievuwwkw.html

[S40] C++：查找元素
来源：http://hz.hfpthk.cn/gtzismvalq.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.9152youxi.cn/gtvxcgbptl.html

[S41] C++：类与构造函数
来源：http://hz.nwbrower.top/gtqsciifgw.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.yj20258888.top/gtxtxraixt.html

[S42] C++：继承与虚函数
来源：http://hz.ehwqpu.com/gtodzkcwoc.html

class B : public Base { public: void f() override {} };
来源：http://hz.yj20258.top/gtefexwkfc.html

[S43] C++：智能指针
来源：http://hz.havefunace.top/gtsgqqmwlt.html

auto p = std::make_unique<int>(5);
来源：http://hz.jyoumei.cn/gthgqwraav.html

[S44] C++：引用传参
来源：http://hz.daxiang520.top/gthfwxzilt.html

void inc(int &x) { ++x; }
来源：http://hz.jianghu66.top/gttomlljru.html

[S45] C++：lambda
来源：http://hz.zdqjudy.top/gtviuelvoi.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.daxiang520.top/gtrkcufxiy.html

[S46] C++：函数模板
来源：http://hz.52xcode.cn/gtbsobnwyc.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.jinyuanbaomall.cn/gtyuqrakfk.html

[S47] C++：结构化绑定遍历
来源：http://hz.svipenyu.cn/gtbcsvdkff.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.aizwys.cn/gtlmxfsvbv.html

[S48] C++：逐行读文件
来源：http://hz.hysaishi.cn/gtrmhbqpua.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.yj20258888.top/gtwihdkehr.html

while (std::getline(in, line)) { }
来源：http://hz.zhoulong.xyz/gtyyxdcroy.html

[S49] C++：写文件
来源：http://hz.guannengcc.top/gtlussdfcp.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.ydjk.org.cn/gtypjrkpij.html

[S50] C++：格式化数字
来源：http://hz.jlsjyb.cn/gtnfoiebek.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.jinqigufen.top/gtmsdqkucx.html

[S51] C++：显式类型转换
来源：http://hz.vqdsnc.cn/gthuitvyhl.html

static_cast<double>(a) / b
来源：http://hz.ybcxt.top/gtfxcfwomk.html

[S52] C++：const 与 noexcept
来源：http://hz.daria6918.cn/gtvoeptudd.html

int size() const noexcept { return n_; }
来源：http://hz.shanyushiyangtech.top/gtokoxxguh.html

[S53] C++：移动语义
来源：http://hz.dianchejie.cn/gtoxhxfobp.html

std::vector<int> w = std::move(v);
来源：http://hz.meibo888.top/gtccllbbgy.html

[S54] C++：异常处理
来源：http://hz.316326.xyz/gteybtruqb.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.ppjwa.cn/gtwjrougvj.html

[S55] C++：结构化绑定
来源：http://hz.zhiwuduotai.top/gtxnnxhczc.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.hnqzz.top/gtcyqxbwgd.html

[S56] C++：optional
来源：http://hz.kuanghao11.cn/gtptrtfqgd.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.quarkkingdee.top/gtxhecfjkf.html

[S57] C++：编译期常量
来源：http://hz.jqgufenzy.top/gtqzjmwjwv.html

constexpr int N = 10;
来源：http://hz.iojbl.cn/gtzsdukycy.html

[S58] C++：命名空间
来源：http://hz.xuanzx.com/gtgmrtbrrz.html

namespace ns { int f() { return 1; } }
来源：http://hz.xylfe.cn/gtmcjvrqfl.html

[S59] C++：静态断言
来源：http://hz.hfpthk.cn/gtdikfhdxx.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.zhoulong.xyz/gtjmhufqbl.html

[S60] C++：遍历并删除元素
来源：http://hz.zhijiandao.cn/gtytvmtqat.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.snrcjt.cn/gtwtdismsh.html

================================================================================
来源：http://hz.jqgufenzy.top/gttpppgppc.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.cashguo.top/gtqsqhnjzj.html

================================================================================
来源：http://hz.yuxming.cn/gteuujxryb.html

[T01] Kotlin：Hello World
来源：http://hz.shanyushiyangkeji.top/gtkcgksmua.html

println("Hello")
来源：http://hz.sxryk.cn/gtyhqdanzh.html

[T02] Kotlin：变量
来源：http://hz.pycfn.com/gtnxjkybms.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.zycfv.cn/gtsqvnabpf.html

[T03] Kotlin：字符串模板
来源：http://hz.hfpthk.cn/gtqbrubkvv.html

"值: $b"
来源：http://hz.birdmap.top/gtnnwyvesb.html

[T04] Kotlin：空安全
来源：http://hz.yueranfly.top/gtxqjlqlzw.html

val n: String? = null;  n?.length
来源：http://hz.zhaomingkeji.xyz/gtxtjwgiiu.html

[T05] Kotlin：when 表达式
来源：http://hz.redwolf501.top/gtbtibdwki.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.nanxuanxn.top/gttrmprlhl.html

[T06] Kotlin：集合映射
来源：http://hz.daria6918.cn/gtzkchnoqf.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.hammf.cn/gtqpmhovek.html

[T07] Kotlin：集合过滤
来源：http://hz.daxiang520.top/gttfvhzpii.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.jyoumei.cn/gtahmussfo.html

[T08] Kotlin：数据类
来源：http://hz.zhongyouzk.top/gtxnipqctz.html

data class User(val name: String, val age: Int)
来源：http://hz.gzhubu.top/gtpobcdacz.html

[T09] Kotlin：扩展函数
来源：http://hz.cashguo.top/gtujiujtgy.html

fun String.exclaim() = this + "!"
来源：http://hz.zhixingplan.top/gtniropprm.html

[T10] Kotlin：默认参数
来源：http://hz.aibaodan.cn/gtrjwsalav.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.jinqigfzy.top/gtzcwelryu.html

[T11] Kotlin：协程
来源：http://hz.cheryme.top/gtdxrwxayg.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.jinqigfzy.top/gtctqxchbp.html

[T12] Kotlin：解构声明
来源：http://hz.yuanzhike.top/gticofebvu.html

val (a, b) = Pair(1, 2)
来源：http://hz.wangdashe.top/gthqyfydtw.html

[T13] Kotlin：只读 Map
来源：http://hz.jyoumei.cn/gthcemslpd.html

val m = mapOf("a" to 1)
来源：http://hz.zhiwuduotai.top/gtopfbsegp.html

[T14] Kotlin：循环
来源：http://hz.ivvv.top/gtqmrkpham.html

for (i in 1..10) println(i)
来源：http://hz.shanyushiyangtech.top/gtffwhllln.html

[T15] Kotlin：接口
来源：http://hz.vqdsnc.cn/gtkqlqwkan.html

interface Shape { fun area(): Double }
来源：http://hz.vqdsnc.cn/gtonmoqoci.html

[T16] Swift：Hello World
来源：http://hz.hywenlv.cn/gtkmglsjux.html

print("Hello")
来源：http://hz.cashguo.top/gtklokpwha.html

[T17] Swift：变量与常量
来源：http://hz.sweek.top/gtgipzgpsp.html

var a = 1;  let b = 2
来源：http://hz.shzxlz.cn/gtzhdtesup.html

[T18] Swift：字符串插值
来源：http://hz.vqdsnc.cn/gtfowttmbz.html

"值: \(b)"
来源：http://hz.dianchejie.cn/gtlikbesrn.html

[T19] Swift：可选绑定
来源：http://hz.cucudq.cn/gtzthkuyhd.html

if let n = opt { print(n) }
来源：http://hz.shuidangran.top/gtbrckrjzz.html

[T20] Swift：数组操作
来源：http://hz.shzxlz.cn/gtmzufzldv.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.fzhhl.top/gtoridmzag.html

[T21] Swift：遍历
来源：http://hz.yvedp.cn/gteafmtvha.html

for x in a { print(x) }
来源：http://hz.gaohongyu789.top/gttdndmdmi.html

[T22] Swift：字典
来源：http://hz.tianlin.xyz/gtwijwshyj.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.zhijiandao.cn/gthqpfakim.html

[T23] Swift：函数
来源：http://hz.ybcxt.top/gtjkavyezn.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.pengpengdd.cyou/gtitbsipbs.html

[T24] Swift：闭包
来源：http://hz.fengsongda.top/gtcbyrcsws.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.tianlin.xyz/gtzvlrlbam.html

[T25] Swift：结构体
来源：http://hz.ydzc1.top/gtizdyqgok.html

struct P { var x: Int }
来源：http://hz.daxiang520.top/gtjeskjhuq.html

[T26] Swift：类与重写
来源：http://hz.0kj1m.cn/gtbxlfszjg.html

class A: Base { override func f() {} }
来源：http://hz.feifeiyinyue.top/gtaanbtspj.html

[T27] Swift：错误处理
来源：http://hz.nwbrower.top/gtnjoaxegn.html

do { try f() } catch { print(error) }
来源：http://hz.snrcjt.cn/gtpnqiqvrc.html

[T28] Swift：枚举
来源：http://hz.jinghuilouyu.cn/gtznkjnlzk.html

enum Color { case red, green }
来源：http://hz.nanxuanxn.top/gtuyeuvrwn.html

[T29] Swift：guard 提前返回
来源：http://hz.pycfn.com/gtohdhgpaw.html

guard let x = opt else { return }
来源：http://hz.ywan-chungtsiang.top/gtydijxqwh.html

[T30] Swift：协议
来源：http://hz.gotoacloud.top/gtujukedyc.html

protocol Shape { func area() -> Double }
来源：http://hz.gogol.net.cn/gtfigcqsoe.html

[T31] Lua：Hello World
来源：http://hz.hysaishi.cn/gtsaftokfm.html

print("Hello")
来源：http://hz.yanxiufei.cn/gtxktefmqm.html

[T32] Lua：局部变量
来源：http://hz.jyoumei.cn/gtxsadyosk.html

local a = 1
来源：http://hz.jinghuilouyu.cn/gtiucqxhci.html

[T33] Lua：表（数组）
来源：http://hz.yuanzhike.top/gtddufajxx.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.haohaochexian.top/gtmntawhna.html

[T34] Lua：遍历表
来源：http://hz.tanke756.top/gtrbuvvlbl.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.cucudq.cn/gthkyfiemp.html

[T35] Lua：字典表
来源：http://hz.pengpengdd.cyou/gtrzltceey.html

local d = { a = 1 };  d.b = 2
来源：http://hz.svipenyu.cn/gttvrxgufy.html

[T36] Lua：函数
来源：http://hz.dianchejie.cn/gtgyfparfm.html

function add(a, b) return a + b end
来源：http://hz.meibo888.top/gtyqyshxbp.html

[T37] Lua：字符串拼接
来源：http://hz.yj20258.top/gtylmosnha.html

"a" .. "b"
来源：http://hz.sxryk.cn/gteambfxvy.html

[T38] Lua：条件
来源：http://hz.sysykeji.top/gtwqabyqqf.html

if x > 0 then print("正") end
来源：http://hz.chenzaomai.com/gtftlbnaoc.html

[T39] Lua：模式匹配
来源：http://hz.svipenyu.cn/gtpfnrorqn.html

string.find(s, "%d+")
来源：http://hz.ydzc1.top/gtmcxctdnr.html

[T40] Lua：元表
来源：http://hz.zhijiandao.cn/gtkpfjxmck.html

setmetatable({}, { __index = base })
来源：http://hz.redwolf501.top/gteilqmyoc.html

[T41] Perl：Hello World
来源：http://hz.smart0.xyz/gtfjmiyayb.html

print "Hello\n";
来源：http://hz.sysykeji.top/gtcolmvmka.html

[T42] Perl：变量类型
来源：http://hz.cheryme.top/gtszbfghkp.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.bjfxy.top/gtkbgoixgl.html

[T43] Perl：字符串插值
来源：http://hz.dianchejie.cn/gtvmzgrdpi.html

"值: $a"
来源：http://hz.jinqigufen.top/gtguypssrp.html

[T44] Perl：条件
来源：http://hz.tanke756.top/gtatoyhgzi.html

if ($a > 0) { print "正"; }
来源：http://hz.zhixingplan.top/gtwvjhcxns.html

[T45] Perl：数组遍历
来源：http://hz.jlsjyb.cn/gtterarxwf.html

for my $x (@arr) { print $x; }
来源：http://hz.gzhubu.top/gttwhwipzr.html

[T46] Perl：哈希操作
来源：http://hz.nanxuanxn.top/gtlajqqhrx.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.gaohongyu789.top/gtaptstrsr.html

[T47] Perl：正则捕获
来源：http://hz.shangyingyoupin.top/gtogmbcgmw.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.ydjk.org.cn/gtcotdpshd.html

[T48] Perl：正则替换
来源：http://hz.snrcjt.cn/gthijhphzx.html

$s =~ s/old/new/g;
来源：http://hz.cdnleiting.top/gtarpfiyaa.html

[T49] Perl：函数
来源：http://hz.fengsongda.top/gtkonqhwov.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.zhaomingkeji.xyz/gtoljvxvye.html

[T50] Perl：逐行读文件
来源：http://hz.aibaodan.cn/gttbhpqeur.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.xylfe.cn/gtfnszpajw.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.pengpengdd.cyou/gtmafpnqrw.html

[T51] Scala：Hello World
来源：http://hz.iojbl.cn/gtrgqrxyhi.html

println("Hello")
来源：http://hz.gotoacloud.top/gtoxgvuonb.html

[T52] Scala：变量
来源：http://hz.chenjidiqi.icu/gtboxfapsi.html

val a = 1;  var b = 2
来源：http://hz.9152youxi.cn/gtldfuktza.html

[T53] Scala：字符串插值
来源：http://hz.wangdashe.top/gtkumcvtso.html

s"值: $b"
来源：http://hz.tanke756.top/gtdzdndfsu.html

[T54] Scala：集合映射
来源：http://hz.cdnleiting.top/gtqkuosmph.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.guannengcc.top/gtcbdbdddg.html

[T55] Scala：集合过滤
来源：http://hz.quarkkingdee.top/gtnvqkuzbi.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.pengpengdd.cyou/gtsedultuq.html

[T56] Scala：样例类
来源：http://hz.hongshengwenyu.top/gtgibjzfmu.html

case class User(name: String, age: Int)
来源：http://hz.gogol.net.cn/gthirrsauf.html

[T57] Scala：模式匹配
来源：http://hz.pengpengdd.cyou/gtmtzamlqf.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.ydjk.org.cn/gtfpoctogv.html

[T58] Scala：函数定义
来源：http://hz.jiagoushi.top/gthrwknuwc.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.yvedp.cn/gtjohkwcxj.html

[T59] Scala：循环
来源：http://hz.svipenyu.cn/gtpflcbsaw.html

for (i <- 1 to 10) println(i)
来源：http://hz.xuetiantiany.cn/gtyzzzwcrj.html

[T60] Scala：折叠
来源：http://hz.hnxiangtu.top/gtvbqanabb.html


<!-- 参考信息 -->