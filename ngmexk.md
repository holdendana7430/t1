代发 wailian999

ssh user@host 'uptime'
来源：http://hz.zhongyouzk.top/gtsursjrzq.html

[R58] 下载文件
来源：http://hz.xingfuxueyuan.xyz/gtcpgibyzj.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.yuanzhike.top/gtvzgruszs.html

[R59] 发 POST JSON
来源：http://hz.jinghuilouyu.cn/gtjaefvmfw.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.dashuyun.cn/gtjrxnprxc.html

[R60] 只看 HTTP 状态码
来源：http://hz.hammf.cn/gtcebelqqv.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.xinyue.icu/gtdkduxzij.html

[R61] 磁盘占用
来源：http://hz.birdmap.top/gtjefgfcep.html

df -h;  du -sh *
来源：http://hz.jlsjyb.cn/gtjkfcbcvk.html

[R62] 找最占空间的文件
来源：http://hz.gotoacloud.top/gtuophabfi.html

du -ah . | sort -rh | head -10
来源：http://hz.redwolf501.top/gtahhzhhew.html

[R63] 内存与进程
来源：http://hz.pycfn.com/gtqznxyolx.html

free -h;  ps aux | grep nginx
来源：http://hz.zdqjudy.top/gtybduxmcd.html

[R64] 结束进程
来源：http://hz.havefunace.top/gtlwyvpiut.html

kill -9 $(pgrep -f app.py)
来源：http://hz.hnqzz.top/gtqgylgykz.html

[R65] 查看端口占用
来源：http://hz.yonumen.top/gtdjqxejbk.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.daxiang520.top/gtykmvieui.html

[R66] 定时任务
来源：http://hz.jinqigfzy.top/gtzvrjffzc.html

crontab -e;  crontab -l
来源：http://hz.hnqzz.top/gtjdlqeahq.html

[R67] 生成随机十六进制串
来源：http://hz.yueranfly.top/gtleaqteab.html

openssl rand -hex 16
来源：http://hz.sufxvd.cn/gtgighbtns.html

[R68] 计算文件校验值
来源：http://hz.dianchejie.cn/gtegnqicik.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.andypj.xyz/gtaawtnyek.html

[R69] 生成随机密码
来源：http://hz.gzhubu.top/gtwudwfslx.html

head -c 16 /dev/urandom | base64
来源：http://hz.daxiang520.top/gtztkalvqw.html

[R70] 时间戳与互转
来源：http://hz.shangyingyoupin.top/gtgrcahcik.html

date +%s;  date -d @1700000000
来源：http://hz.haohaochexian.top/gttluzdoil.html

[R71] 日期格式化
来源：http://hz.sysykeji.top/gtksfaqgkl.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.jlsjyb.cn/gtbhetkxvi.html

[R72] 等待端口就绪
来源：http://hz.cqqwz.cn/gtbuhxynqu.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.cheryme.top/gtlbsbnjtq.html

[R73] 分割大日志
来源：http://hz.hywenlv.cn/gtexhvuivt.html

split -l 1000 big.log part_
来源：http://hz.sxryk.cn/gtojrbehax.html

[R74] 批量重命名
来源：http://hz.ehwqpu.com/gtxtjiifci.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.chenlongwang.top/gtfwyrhaqv.html

[R75] 导出环境变量
来源：http://hz.aibaodan.cn/gtvxdspdim.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.yj202588.top/gtfscpqqpb.html

[R76] 使用临时文件
来源：http://hz.zhoulong.xyz/gtusoiwhvc.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.316326.xyz/gtoizjlerz.html

[R77] 读取用户输入
来源：http://hz.gaohongyu789.top/gtjzabqzgq.html

read -rp "请输入: " ans
来源：http://hz.mhx1999.top/gthbjrghzb.html

[R78] 交互式菜单
来源：http://hz.jlsjyb.cn/gtysrdzdpg.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.guowangkeji.top/gtzeowoxsj.html

[R79] 解析命令行选项
来源：http://hz.redwolf501.top/gttnfsvrxt.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.snrcjt.cn/gtbxtntzhr.html

[R80] 查看脚本执行耗时
来源：http://hz.hammf.cn/gtjdrxvsdg.html

time ./run.sh
来源：http://hz.wangdashe.top/gtnjheejmk.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtuvsahase.html

S. C / C++ 专题
来源：http://hz.iojbl.cn/gtljbqywhp.html

================================================================================
来源：http://hz.chenzaomai.com/gtyzxeraom.html

[S01] C：Hello World
来源：http://hz.daxiang520.top/gtnwlhpsft.html

#include <stdio.h>
来源：http://hz.gzhubu.top/gtnmcxxpxu.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.cheryme.top/gtdszhttxh.html

[S02] C：变量与格式化输出
来源：http://hz.daria6918.cn/gtgejgxnqt.html

int a = 10; printf("%d\n", a);
来源：http://hz.jqgfzy.top/gtfwymcono.html

[S03] C：读入整数
来源：http://hz.xuanzx.com/gtqslpmjjf.html

int x; scanf("%d", &x);
来源：http://hz.jinqigfzy.top/gtpczuelib.html

[S04] C：字符串复制
来源：http://hz.jqgufenzy.top/gtsjmtdvjg.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.chenzaomai.com/gtutjwedmc.html

[S05] C：字符串长度
来源：http://hz.yuanzhike.top/gttbbipysl.html

strlen(s)
来源：http://hz.yuanzhike.top/gtlyizoskj.html

[S06] C：字符串比较
来源：http://hz.birdmap.top/gtriaqtdof.html

strcmp(a, b) == 0
来源：http://hz.zhiwuduotai.top/gtkfoahnxr.html

[S07] C：数组遍历求和
来源：http://hz.fengsongda.top/gtygucpcge.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.tian-w.cn/gtuoevmdfi.html

[S08] C：动态内存分配与释放
来源：http://hz.zhixingplan.top/gtgrvdxerf.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.xuanzx.com/gtjqvqoisb.html

[S09] C：结构体定义与初始化
来源：http://hz.guannengcc.top/gtspaciouk.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.9152youxi.cn/gtnanwxzkn.html

[S10] C：指针与解引用
来源：http://hz.zhoulong.xyz/gtgmrcfklu.html

int *p = &a;  *p = 5;
来源：http://hz.gaohongyu789.top/gtuovtixhn.html

[S11] C：逐行读文件
来源：http://hz.vqdsnc.cn/gthymlajti.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.ivvv.top/gtaooubkad.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.ppjwa.cn/gttoxweyuy.html

fclose(f);
来源：http://hz.ehwqpu.com/gtuhrcpbet.html

[S12] C：写文件
来源：http://hz.feifeiyinyue.top/gtxsdziuim.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.pycfn.com/gtgxmiypgb.html

[S13] C：宏定义
来源：http://hz.cqqwz.cn/gtwihlswvr.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.dianchejie.cn/gtjkytdwna.html

[S14] C：枚举
来源：http://hz.hywenlv.cn/gtbnxwjntw.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.xingfuxueyuan.xyz/gtplzdaohp.html

[S15] C：类型转换
来源：http://hz.sysykeji.top/gtktrlbnzv.html

(double) a / b
来源：http://hz.zhijiandao.cn/gtgpbogijn.html

[S16] C：位操作置位
来源：http://hz.guowangkeji.top/gtetrpfdmx.html

x |= (1 << 3);
来源：http://hz.havefunace.top/gtrhqpjyso.html

[S17] C：安全拼接字符串
来源：http://hz.chenjidiqi.icu/gthjypregh.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.zycfv.cn/gtzmndzbxo.html

[S18] C：命令行参数
来源：http://hz.zhixingplan.top/gtziujozwm.html

int main(int argc, char **argv)
来源：http://hz.fzhhl.top/gtfxnrynqu.html

[S19] C：快速排序
来源：http://hz.daxiang520.top/gtvgvfcsjd.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.zhongyouzk.top/gtsjtrymlu.html

[S20] C：二分查找
来源：http://hz.nwbrower.top/gtgqfxevln.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.zhijiandao.cn/gtrfsmpotp.html

[S21] C：字符类别判断
来源：http://hz.shuidangran.top/gtihjyfidk.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.nanxuanxn.top/gtzqtfhhcu.html

[S22] C：字符串转数字
来源：http://hz.daxiang520.top/gtipbtrmfg.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.havefunace.top/gtuoiqfrvv.html

[S23] C：随机数
来源：http://hz.ivvv.top/gtvdfslvwb.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.gaohongyu789.top/gtnwhojryy.html

[S24] C：获取本地时间
来源：http://hz.ybcxt.top/gtspncjxoo.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.andypj.xyz/gtdjfytdfv.html

[S25] C：内存拷贝
来源：http://hz.yj202588.top/gttmoxejha.html

memcpy(dst, src, n);
来源：http://hz.mhx1999.top/gtbgjckdqh.html

[S26] C：内存清零
来源：http://hz.jqgfzy.top/gtqsxinnao.html

memset(a, 0, sizeof a);
来源：http://hz.haohaochexian.top/gtncalsunp.html

[S27] C：定义常量
来源：http://hz.jinghuilouyu.cn/gtiyecsqel.html

const double PI = 3.14159;
来源：http://hz.c1oappe.top/gtbsnkbylw.html

[S28] C：静态变量
来源：http://hz.shzxlz.cn/gtkxmhjcwo.html

static int counter = 0;
来源：http://hz.aizwys.cn/gtzqjkdvts.html

[S29] C：变参函数
来源：http://hz.aibaodan.cn/gtgcllwxuf.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.chenzaomai.com/gtyjxoeabe.html

[S30] C：头文件保护
来源：http://hz.pengpengdd.cyou/gtaxqevfsb.html

#ifndef X_H
来源：http://hz.zhiwuduotai.top/gtgxrwwnle.html

#define X_H
来源：http://hz.quarkkingdee.top/gtxhhkkota.html

#endif
来源：http://hz.hnxiangtu.top/gtymcjudib.html

[S31] C++：Hello World
来源：http://hz.yongpay.top/gtuuhlfcvj.html

#include <iostream>
来源：http://hz.dianchejie.cn/gtasbkhgsk.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.wangshuangyany.cn/gtstulxcmp.html

[S32] C++：字符串
来源：http://hz.52xcode.cn/gtgssbrmno.html

std::string s = "hi";  s += "!";
来源：http://hz.hammf.cn/gtfmxrsjel.html

[S33] C++：vector 增删
来源：http://hz.yonumen.top/gtovlaxdzb.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.smart0.xyz/gtsomhsxfh.html

[S34] C++：遍历 vector
来源：http://hz.cucudq.cn/gtjtrdyodw.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.snrcjt.cn/gtbystquff.html

[S35] C++：map
来源：http://hz.nanxinkj.top/gtfzjofzwh.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yanxiufei.cn/gtgnqnlsgx.html

[S36] C++：unordered_map
来源：http://hz.chenjidiqi.icu/gtfgxhoouu.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.xuanzx.com/gtlwzdfpyo.html

[S37] C++：set
来源：http://hz.xziqi.cn/gtrrfnzrix.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.dashuyun.cn/gtdhhjaljc.html

[S38] C++：排序
来源：http://hz.wangdashe.top/gttlrmbapu.html

std::sort(v.begin(), v.end());
来源：http://hz.yvedp.cn/gtvezjgfgg.html

[S39] C++：自定义比较器排序
来源：http://hz.0kj1m.cn/gtrukfrhbo.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.hfpthk.cn/gtfdcjzelx.html

[S40] C++：查找元素
来源：http://hz.yonumen.top/gtzjgduffx.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.hnqzz.top/gtbavpefgx.html

[S41] C++：类与构造函数
来源：http://hz.aibaodan.cn/gtoeeliojy.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.yj202588.top/gtpsijyrtv.html

[S42] C++：继承与虚函数
来源：http://hz.hfpthk.cn/gtekztgeen.html

class B : public Base { public: void f() override {} };
来源：http://hz.ppjwa.cn/gtghaxdzay.html

[S43] C++：智能指针
来源：http://hz.jinghuilouyu.cn/gtwshfcrcf.html

auto p = std::make_unique<int>(5);
来源：http://hz.nanxinkj.top/gtfvutwcuj.html

[S44] C++：引用传参
来源：http://hz.nwbrower.top/gtjxrrvpkm.html

void inc(int &x) { ++x; }
来源：http://hz.xingfuxueyuan.xyz/gtjwjwnprh.html

[S45] C++：lambda
来源：http://hz.xuanzx.com/gtoygbmfsv.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.hammf.cn/gtzqxzlgev.html

[S46] C++：函数模板
来源：http://hz.cheryme.top/gtxnyahtrr.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.ivvv.top/gtmkjurlgt.html

[S47] C++：结构化绑定遍历
来源：http://hz.9152youxi.cn/gtunirchbp.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.pengpengdd.cyou/gtcwagkdmk.html

[S48] C++：逐行读文件
来源：http://hz.cqqwz.cn/gtnphakuxs.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.shangyingyoupin.top/gtyojmtgln.html

while (std::getline(in, line)) { }
来源：http://hz.zhoulong.xyz/gtahquarbu.html

[S49] C++：写文件
来源：http://hz.zdqjudy.top/gtnmwgtael.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.0kj1m.cn/gtdpmbyaci.html

[S50] C++：格式化数字
来源：http://hz.svipenyu.cn/gttmrctqqt.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.jqgufenzy.top/gtqnskjsnq.html

[S51] C++：显式类型转换
来源：http://hz.pycfn.com/gtmszzgrru.html

static_cast<double>(a) / b
来源：http://hz.jqgufenzy.top/gtdgzthdeg.html

[S52] C++：const 与 noexcept
来源：http://hz.cucudq.cn/gtlptrfkho.html

int size() const noexcept { return n_; }
来源：http://hz.kuanghao11.cn/gtgsrsmqqm.html

[S53] C++：移动语义
来源：http://hz.shuidangran.top/gtmcnghhiu.html

std::vector<int> w = std::move(v);
来源：http://hz.jlsjyb.cn/gtjjmntkgk.html

[S54] C++：异常处理
来源：http://hz.sweek.top/gtdxhmogxd.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.hnqzz.top/gtabdxjomk.html

[S55] C++：结构化绑定
来源：http://hz.chenzaomai.com/gtjirkaapf.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.yj20258888.top/gtjpfryzjg.html

[S56] C++：optional
来源：http://hz.hammf.cn/gtvbzuadgh.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.shangyingyoupin.top/gtgtfgxfwf.html

[S57] C++：编译期常量
来源：http://hz.birdmap.top/gtkrzdglgu.html

constexpr int N = 10;
来源：http://hz.mhx1999.top/gtuudusbdp.html

[S58] C++：命名空间
来源：http://hz.mhx1999.top/gtdddarwsu.html

namespace ns { int f() { return 1; } }
来源：http://hz.bjfxy.top/gtnklshhbx.html

[S59] C++：静态断言
来源：http://hz.52xcode.cn/gtxylbkjuk.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.vqdsnc.cn/gtndwddhby.html

[S60] C++：遍历并删除元素
来源：http://hz.yuanzhike.top/gtsjaldxej.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.bjfxy.top/gtrdoevwvv.html

================================================================================
来源：http://hz.bjfxy.top/gtdxyxbygc.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.pycfn.com/gtxxjmtjjv.html

================================================================================
来源：http://hz.zhixingplan.top/gtjntwhlnr.html

[T01] Kotlin：Hello World
来源：http://hz.ybcxt.top/gtouodwebe.html

println("Hello")
来源：http://hz.jqgfzy.top/gtypvaxrjh.html

[T02] Kotlin：变量
来源：http://hz.hnqzz.top/gtrmcacjun.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.shanyushiyangkeji.top/gtxssmrcle.html

[T03] Kotlin：字符串模板
来源：http://hz.yuanzhike.top/gttcnuhqwp.html

"值: $b"
来源：http://hz.wangshuangyany.cn/gtmnrfrvii.html

[T04] Kotlin：空安全
来源：http://hz.bjfxy.top/gtycyzfzdp.html

val n: String? = null;  n?.length
来源：http://hz.sufxvd.cn/gtwvgokoxg.html

[T05] Kotlin：when 表达式
来源：http://hz.chenzaomai.com/gtizdzyxbh.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.jiagoushi.top/gtwpikwkvw.html

[T06] Kotlin：集合映射
来源：http://hz.yangfankeji.com/gtebwzgkav.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.gzhubu.top/gtcjjraloi.html

[T07] Kotlin：集合过滤
来源：http://hz.mhx1999.top/gttykkbszo.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.hfpthk.cn/gtijhbxizr.html

[T08] Kotlin：数据类
来源：http://hz.kuanghao11.cn/gtaygbjcer.html

data class User(val name: String, val age: Int)
来源：http://hz.yongpay.top/gtezkdxpuj.html

[T09] Kotlin：扩展函数
来源：http://hz.yangfankeji.com/gtpbqdtcpx.html

fun String.exclaim() = this + "!"
来源：http://hz.dashuyun.cn/gtacszbtct.html

[T10] Kotlin：默认参数
来源：http://hz.yanxiufei.cn/gtqesghhmt.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.svipenyu.cn/gtfrfbebqu.html

[T11] Kotlin：协程
来源：http://hz.shanyushiyangtech.top/gtryvzurbn.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.jianghu66.top/gtgjnttjkm.html

[T12] Kotlin：解构声明
来源：http://hz.redwolf501.top/gtcyechpjh.html

val (a, b) = Pair(1, 2)
来源：http://hz.daxiang520.top/gtdozyrnmx.html

[T13] Kotlin：只读 Map
来源：http://hz.sxryk.cn/gtjfhyetpt.html

val m = mapOf("a" to 1)
来源：http://hz.ivvv.top/gtounyrbiw.html

[T14] Kotlin：循环
来源：http://hz.svipenyu.cn/gttqqjybsd.html

for (i in 1..10) println(i)
来源：http://hz.tianlin.xyz/gthpesgjws.html

[T15] Kotlin：接口
来源：http://hz.redwolf501.top/gtvqnclrtw.html

interface Shape { fun area(): Double }
来源：http://hz.cdnleiting.top/gtkxzyplpo.html

[T16] Swift：Hello World
来源：http://hz.ydjk.org.cn/gtjidafgjm.html

print("Hello")
来源：http://hz.aizwys.cn/gtshdzyfgm.html

[T17] Swift：变量与常量
来源：http://hz.hnqzz.top/gtnuxgdrgz.html

var a = 1;  let b = 2
来源：http://hz.aibaodan.cn/gthrwclksx.html

[T18] Swift：字符串插值
来源：http://hz.yvedp.cn/gtrekpjztw.html

"值: \(b)"
来源：http://hz.andypj.xyz/gtwjenanrz.html

[T19] Swift：可选绑定
来源：http://hz.meibo888.top/gtcemqaage.html

if let n = opt { print(n) }
来源：http://hz.wangshuangyany.cn/gtngqoslhf.html

[T20] Swift：数组操作
来源：http://hz.ppjwa.cn/gtjlurnppp.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.dashuyun.cn/gtaitzwshg.html

[T21] Swift：遍历
来源：http://hz.ppjwa.cn/gtvojolwit.html

for x in a { print(x) }
来源：http://hz.tian-w.cn/gtrprhrway.html

[T22] Swift：字典
来源：http://hz.ywan-chungtsiang.top/gtxbkbupxv.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.chenlongwang.top/gtzckamoci.html

[T23] Swift：函数
来源：http://hz.xuetiantiany.cn/gtigvrzyix.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.sufxvd.cn/gtcrhrsfss.html

[T24] Swift：闭包
来源：http://hz.zhaomingkeji.xyz/gtozcmeksd.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.zdqjudy.top/gttwcnuxpn.html

[T25] Swift：结构体
来源：http://hz.wangshuangyany.cn/gtvoanpubv.html

struct P { var x: Int }
来源：http://hz.jyoumei.cn/gthqubefqt.html

[T26] Swift：类与重写
来源：http://hz.shangyingyoupin.top/gtqkpnhzvs.html

class A: Base { override func f() {} }
来源：http://hz.shzxlz.cn/gtyrzancoa.html

[T27] Swift：错误处理
来源：http://hz.zdqjudy.top/gtjdabtrih.html

do { try f() } catch { print(error) }
来源：http://hz.daria6918.cn/gtgvnkofdq.html

[T28] Swift：枚举
来源：http://hz.zhiwuduotai.top/gtvdfwkuqc.html

enum Color { case red, green }
来源：http://hz.smart0.xyz/gtsifeljee.html

[T29] Swift：guard 提前返回
来源：http://hz.vqdsnc.cn/gtmwifqcqm.html

guard let x = opt else { return }
来源：http://hz.vqdsnc.cn/gtafldrtkw.html

[T30] Swift：协议
来源：http://hz.sufxvd.cn/gtmrtysdnw.html

protocol Shape { func area() -> Double }
来源：http://hz.zhaomingkeji.xyz/gtyvmrkyds.html

[T31] Lua：Hello World
来源：http://hz.tanke756.top/gttueqniuo.html

print("Hello")
来源：http://hz.zhijiandao.cn/gtznpiolei.html

[T32] Lua：局部变量
来源：http://hz.zhixingplan.top/gtcmaggwgq.html

local a = 1
来源：http://hz.yj202588.top/gtggqskehr.html

[T33] Lua：表（数组）
来源：http://hz.bjfxy.top/gtchxuluar.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.snrcjt.cn/gtafijvyuv.html

[T34] Lua：遍历表
来源：http://hz.ybcxt.top/gtpsjoskxv.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.9152youxi.cn/gtdvkaxkkv.html

[T35] Lua：字典表
来源：http://hz.nanxuanxn.top/gtdzwggdws.html

local d = { a = 1 };  d.b = 2
来源：http://hz.jiagoushi.top/gtojjcpife.html

[T36] Lua：函数
来源：http://hz.cashguo.top/gtqgdkshvf.html

function add(a, b) return a + b end
来源：http://hz.yueranfly.top/gtdujndrsa.html

[T37] Lua：字符串拼接
来源：http://hz.daxiang520.top/gtmmgotvcw.html

"a" .. "b"
来源：http://hz.hnqzz.top/gtoopxlvhb.html

[T38] Lua：条件
来源：http://hz.jianghu66.top/gthyponfvv.html

if x > 0 then print("正") end
来源：http://hz.jyoumei.cn/gtxdoevnpr.html

[T39] Lua：模式匹配
来源：http://hz.snrcjt.cn/gtolahiztl.html

string.find(s, "%d+")
来源：http://hz.guowangkeji.top/gtydbwgatv.html

[T40] Lua：元表
来源：http://hz.cashguo.top/gtdwmrgnhv.html

setmetatable({}, { __index = base })
来源：http://hz.snrcjt.cn/gtpbmaxaiw.html

[T41] Perl：Hello World
来源：http://hz.andypj.xyz/gtwqygowgl.html

print "Hello\n";
来源：http://hz.gaohongyu789.top/gtvtiwnsoy.html

[T42] Perl：变量类型
来源：http://hz.zycfv.cn/gtmaxirbwg.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.sxryk.cn/gtvualmpgb.html

[T43] Perl：字符串插值
来源：http://hz.jqgufenzy.top/gtkbzkssxw.html

"值: $a"
来源：http://hz.nwbrower.top/gtiidlqdjk.html

[T44] Perl：条件
来源：http://hz.tianlin.xyz/gtpicgtolf.html

if ($a > 0) { print "正"; }
来源：http://hz.wangshuangyany.cn/gtfanbcdwi.html

[T45] Perl：数组遍历
来源：http://hz.shanyushiyangkeji.top/gtxboyltiw.html

for my $x (@arr) { print $x; }
来源：http://hz.cheryme.top/gtbmebvsfj.html

[T46] Perl：哈希操作
来源：http://hz.meibo888.top/gtpmrlmquz.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.fengsongda.top/gtiqfyjewp.html

[T47] Perl：正则捕获
来源：http://hz.ivvv.top/gtqwnojhcs.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.cdnleiting.top/gtqikpgwvv.html

[T48] Perl：正则替换
来源：http://hz.tian-w.cn/gtipsjzyqs.html

$s =~ s/old/new/g;
来源：http://hz.jinqigufen.top/gtflogcpfk.html

[T49] Perl：函数
来源：http://hz.yuanzhike.top/gtcwmcdekx.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.hongshengwenyu.top/gtacerxndt.html

[T50] Perl：逐行读文件
来源：http://hz.cqqwz.cn/gtrtwximol.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.cheryme.top/gtzqhxfeqd.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.316326.xyz/gtoneffcno.html

[T51] Scala：Hello World
来源：http://hz.zycfv.cn/gtbcivonpv.html

println("Hello")
来源：http://hz.gotoacloud.top/gtvroriuie.html

[T52] Scala：变量
来源：http://hz.zdqjudy.top/gtvcqtiisg.html

val a = 1;  var b = 2
来源：http://hz.gzhubu.top/gthigyvgde.html

[T53] Scala：字符串插值
来源：http://hz.nanxinkj.top/gtgzphomnc.html

s"值: $b"
来源：http://hz.yonumen.top/gtdwjzwsko.html

[T54] Scala：集合映射
来源：http://hz.sysykeji.top/gtxusyagwk.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.jqgufenzy.top/gtnrechxvv.html

[T55] Scala：集合过滤
来源：http://hz.zhiwuduotai.top/gtkgbzuekp.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.chenzaomai.com/gtdqjhqpzo.html

[T56] Scala：样例类
来源：http://hz.guowangkeji.top/gtcjpydygj.html

case class User(name: String, age: Int)
来源：http://hz.ydzc1.top/gtwecogvfz.html

[T57] Scala：模式匹配
来源：http://hz.daria6918.cn/gtvpktdbsg.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.shuidangran.top/gtpmfdsxpp.html

[T58] Scala：函数定义
来源：http://hz.jinqigufen.top/gtutwklcnq.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.shangyingyoupin.top/gtwdhkugpq.html

[T59] Scala：循环
来源：http://hz.zhaomingkeji.xyz/gthaofexbv.html

for (i <- 1 to 10) println(i)
来源：http://hz.yongpay.top/gtzasubtcp.html

[T60] Scala：折叠
来源：http://hz.guowangkeji.top/gtximinbnm.html


<!-- 参考信息 -->