代发 wailian999

ssh user@host 'uptime'
来源：http://hz.dashuyun.cn/gtcvfuszrv.html

[R58] 下载文件
来源：http://hz.yuanzhike.top/gtvnumtbrp.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.feifeiyinyue.top/gtcvoyoodb.html

[R59] 发 POST JSON
来源：http://hz.zhoulong.xyz/gthfmzzcir.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.gzhubu.top/gtqmscghhj.html

[R60] 只看 HTTP 状态码
来源：http://hz.yuxming.cn/gtiiqtkias.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.gzhubu.top/gtuvogngbb.html

[R61] 磁盘占用
来源：http://hz.0kj1m.cn/gtjvejgjtn.html

df -h;  du -sh *
来源：http://hz.nanxuanxn.top/gtaxehwsau.html

[R62] 找最占空间的文件
来源：http://hz.jqgufenzy.top/gtcskzsezf.html

du -ah . | sort -rh | head -10
来源：http://hz.xingfuxueyuan.xyz/gtaplgvzpf.html

[R63] 内存与进程
来源：http://hz.shanyushiyangkeji.top/gtdfzmritx.html

free -h;  ps aux | grep nginx
来源：http://hz.pengpengdd.cyou/gtcxbltees.html

[R64] 结束进程
来源：http://hz.316326.xyz/gtiavjxmza.html

kill -9 $(pgrep -f app.py)
来源：http://hz.zhijiandao.cn/gtobizrupk.html

[R65] 查看端口占用
来源：http://hz.jinghuilouyu.cn/gtlkzflcyw.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.tanke756.top/gtjswvehhl.html

[R66] 定时任务
来源：http://hz.yongpay.top/gtnwzfidha.html

crontab -e;  crontab -l
来源：http://hz.wangdashe.top/gtxevsdott.html

[R67] 生成随机十六进制串
来源：http://hz.zycfv.cn/gtkngznfus.html

openssl rand -hex 16
来源：http://hz.tanke756.top/gtjyffrscg.html

[R68] 计算文件校验值
来源：http://hz.guannengcc.top/gtcxlomxwf.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.redwolf501.top/gtwcunynkm.html

[R69] 生成随机密码
来源：http://hz.meibo888.top/gtqykubphw.html

head -c 16 /dev/urandom | base64
来源：http://hz.ywan-chungtsiang.top/gtuvwqjcmk.html

[R70] 时间戳与互转
来源：http://hz.yvedp.cn/gtlvspgccm.html

date +%s;  date -d @1700000000
来源：http://hz.shanyushiyangtech.top/gthpdvcazn.html

[R71] 日期格式化
来源：http://hz.cucudq.cn/gtyxhbpcjy.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.c1oappe.top/gtohauwsdp.html

[R72] 等待端口就绪
来源：http://hz.pycfn.com/gtfsymremj.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.vqdsnc.cn/gtcevcmvfw.html

[R73] 分割大日志
来源：http://hz.chenlongwang.top/gtyeclstup.html

split -l 1000 big.log part_
来源：http://hz.gogol.net.cn/gtuqrrdldt.html

[R74] 批量重命名
来源：http://hz.yongpay.top/gtqnhioalq.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.yueranfly.top/gtkrizjazt.html

[R75] 导出环境变量
来源：http://hz.snrcjt.cn/gtoucmczkc.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.jiagoushi.top/gtpmupxkny.html

[R76] 使用临时文件
来源：http://hz.jyoumei.cn/gtthuqsyjl.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.zhijiandao.cn/gtbftilics.html

[R77] 读取用户输入
来源：http://hz.jinqigfzy.top/gtzmlsjtbp.html

read -rp "请输入: " ans
来源：http://hz.9152youxi.cn/gtgiuijdwq.html

[R78] 交互式菜单
来源：http://hz.bjfxy.top/gtauuoblke.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.meibo888.top/gtsbkwnhvs.html

[R79] 解析命令行选项
来源：http://hz.ybcxt.top/gtziqmlivq.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.gotoacloud.top/gtjlhfgela.html

[R80] 查看脚本执行耗时
来源：http://hz.cheryme.top/gtktlchwqf.html

time ./run.sh
来源：http://hz.wangshuangyany.cn/gtnhmnqhek.html

================================================================================
来源：http://hz.bjfxy.top/gteajldfaw.html

S. C / C++ 专题
来源：http://hz.yangfankeji.com/gteqvixigi.html

================================================================================
来源：http://hz.mhx1999.top/gtwcuxepgp.html

[S01] C：Hello World
来源：http://hz.ppjwa.cn/gtdpokoeaa.html

#include <stdio.h>
来源：http://hz.ydjk.org.cn/gtwqmfobob.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.yueranfly.top/gtojzsnuyw.html

[S02] C：变量与格式化输出
来源：http://hz.cdnleiting.top/gtfzvozbcg.html

int a = 10; printf("%d\n", a);
来源：http://hz.yuxming.cn/gtawurhjef.html

[S03] C：读入整数
来源：http://hz.jlsjyb.cn/gttzrtasrd.html

int x; scanf("%d", &x);
来源：http://hz.tian-w.cn/gtlrrxwgjx.html

[S04] C：字符串复制
来源：http://hz.haohaochexian.top/gtwieavlak.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.zhengqikj.top/gtnuejdixi.html

[S05] C：字符串长度
来源：http://hz.yvedp.cn/gtnlfhxgra.html

strlen(s)
来源：http://hz.yangfankeji.com/gtnrlhawur.html

[S06] C：字符串比较
来源：http://hz.chenlongwang.top/gtkoxjnfsf.html

strcmp(a, b) == 0
来源：http://hz.jianghu66.top/gtenhhofbj.html

[S07] C：数组遍历求和
来源：http://hz.jinghuilouyu.cn/gtpoiuizsc.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.ydzc1.top/gtrkbiikgo.html

[S08] C：动态内存分配与释放
来源：http://hz.zhiwuduotai.top/gtyzpoqcko.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.yj20258888.top/gtdpqtwcmb.html

[S09] C：结构体定义与初始化
来源：http://hz.zhongyouzk.top/gtmpjmgdqg.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.zhoulong.xyz/gtplnzplfm.html

[S10] C：指针与解引用
来源：http://hz.jinyuanbaomall.cn/gtvefgpqbd.html

int *p = &a;  *p = 5;
来源：http://hz.zhoulong.xyz/gtrljkmzuw.html

[S11] C：逐行读文件
来源：http://hz.c1oappe.top/gtujqidccn.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.hfpthk.cn/gtoynxsjqu.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.shuidangran.top/gtybxzaqqz.html

fclose(f);
来源：http://hz.shanyushiyangtech.top/gtaooujsqw.html

[S12] C：写文件
来源：http://hz.zycfv.cn/gtbswekhri.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.nwbrower.top/gtazceepov.html

[S13] C：宏定义
来源：http://hz.yueranfly.top/gtatgaetpq.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.jinghuilouyu.cn/gtxyxmvlmn.html

[S14] C：枚举
来源：http://hz.zhongyouzk.top/gtydocjypx.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.cdnleiting.top/gtmbrjycmp.html

[S15] C：类型转换
来源：http://hz.zhaomingkeji.xyz/gtiwxpaqva.html

(double) a / b
来源：http://hz.hysaishi.cn/gtxatfztgc.html

[S16] C：位操作置位
来源：http://hz.xziqi.cn/gtfzfmiamb.html

x |= (1 << 3);
来源：http://hz.dianchejie.cn/gtfjyrkhhw.html

[S17] C：安全拼接字符串
来源：http://hz.zhoulong.xyz/gttachfgaa.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.aizwys.cn/gtvvbrldox.html

[S18] C：命令行参数
来源：http://hz.yonumen.top/gtitybwtao.html

int main(int argc, char **argv)
来源：http://hz.gotoacloud.top/gtmjplfnvf.html

[S19] C：快速排序
来源：http://hz.sufxvd.cn/gtdleaextw.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.shuidangran.top/gtwqbjuetm.html

[S20] C：二分查找
来源：http://hz.aizwys.cn/gtvirsjhan.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.ydzc1.top/gtjjwweyal.html

[S21] C：字符类别判断
来源：http://hz.shangyingyoupin.top/gtkcadttbg.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.ydjk.org.cn/gtyozrcfyc.html

[S22] C：字符串转数字
来源：http://hz.hammf.cn/gtpuyimdst.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.sysykeji.top/gtidzyyypp.html

[S23] C：随机数
来源：http://hz.tanke756.top/gtipwibasu.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.cashguo.top/gtvjinmbcd.html

[S24] C：获取本地时间
来源：http://hz.hongshengwenyu.top/gtbjmnboxk.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.yj20258.top/gthznosmkj.html

[S25] C：内存拷贝
来源：http://hz.aizwys.cn/gtjfnhgeus.html

memcpy(dst, src, n);
来源：http://hz.xylfe.cn/gtkfitufvk.html

[S26] C：内存清零
来源：http://hz.yj20258.top/gtgjyairpu.html

memset(a, 0, sizeof a);
来源：http://hz.c1oappe.top/gthukfmoff.html

[S27] C：定义常量
来源：http://hz.wangdashe.top/gtvecstcgh.html

const double PI = 3.14159;
来源：http://hz.wangdashe.top/gthpiyhhbw.html

[S28] C：静态变量
来源：http://hz.pycfn.com/gtvkglweff.html

static int counter = 0;
来源：http://hz.fzhhl.top/gtvwsfavot.html

[S29] C：变参函数
来源：http://hz.ydjk.org.cn/gtpxwtgjor.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.gzhubu.top/gtnmiqgpqu.html

[S30] C：头文件保护
来源：http://hz.mhx1999.top/gtmlztanwc.html

#ifndef X_H
来源：http://hz.iojbl.cn/gtyufteart.html

#define X_H
来源：http://hz.sxryk.cn/gtmpkxqvox.html

#endif
来源：http://hz.yj202588.top/gtdjjwrmak.html

[S31] C++：Hello World
来源：http://hz.zhixingplan.top/gtftuqnplc.html

#include <iostream>
来源：http://hz.shuidangran.top/gtwukflybk.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.aibaodan.cn/gtcwdadjtx.html

[S32] C++：字符串
来源：http://hz.sweek.top/gtncadukzx.html

std::string s = "hi";  s += "!";
来源：http://hz.yj202588.top/gtwouyecge.html

[S33] C++：vector 增删
来源：http://hz.smart0.xyz/gtjmesjafd.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.ehwqpu.com/gtvxdnurpf.html

[S34] C++：遍历 vector
来源：http://hz.cashguo.top/gtcfewqgfq.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.cashguo.top/gtvtutdmve.html

[S35] C++：map
来源：http://hz.quarkkingdee.top/gtcyjxevce.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.quarkkingdee.top/gtobzdcuqz.html

[S36] C++：unordered_map
来源：http://hz.sweek.top/gtucwpeedm.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.redwolf501.top/gtvjnrimlm.html

[S37] C++：set
来源：http://hz.svipenyu.cn/gtaiotmikt.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.fzhhl.top/gtxmsxaabf.html

[S38] C++：排序
来源：http://hz.shzxlz.cn/gtiargqcfn.html

std::sort(v.begin(), v.end());
来源：http://hz.52xcode.cn/gttumnpgfk.html

[S39] C++：自定义比较器排序
来源：http://hz.yuxming.cn/gthzlacwyb.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.yj20258888.top/gtwrgqtmeg.html

[S40] C++：查找元素
来源：http://hz.chenjidiqi.icu/gtiokjoaea.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.smart0.xyz/gtduvqlzod.html

[S41] C++：类与构造函数
来源：http://hz.yangfankeji.com/gtukxhvmag.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.yangfankeji.com/gtbqjbyoxn.html

[S42] C++：继承与虚函数
来源：http://hz.shangyingyoupin.top/gtffmlhjag.html

class B : public Base { public: void f() override {} };
来源：http://hz.hywenlv.cn/gtwzbxxybt.html

[S43] C++：智能指针
来源：http://hz.yueranfly.top/gtwzfzqtuv.html

auto p = std::make_unique<int>(5);
来源：http://hz.guowangkeji.top/gtjazbuats.html

[S44] C++：引用传参
来源：http://hz.nanxuanxn.top/gtchymvxbr.html

void inc(int &x) { ++x; }
来源：http://hz.cashguo.top/gthizbvkvo.html

[S45] C++：lambda
来源：http://hz.yangfankeji.com/gttplpcifh.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.xuetiantiany.cn/gtgaaogmjj.html

[S46] C++：函数模板
来源：http://hz.snrcjt.cn/gtgejqubro.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.tanke756.top/gtjjizfpqg.html

[S47] C++：结构化绑定遍历
来源：http://hz.shuidangran.top/gtfiappiug.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.gzhubu.top/gtosandros.html

[S48] C++：逐行读文件
来源：http://hz.xuanzx.com/gtzscgylvb.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.havefunace.top/gtygadvwiz.html

while (std::getline(in, line)) { }
来源：http://hz.mhx1999.top/gtworqabjy.html

[S49] C++：写文件
来源：http://hz.c1oappe.top/gtfqtfvedq.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.daria6918.cn/gttimxmqsa.html

[S50] C++：格式化数字
来源：http://hz.mhx1999.top/gtplyfwxlj.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.shuidangran.top/gtscxnnqom.html

[S51] C++：显式类型转换
来源：http://hz.tianlin.xyz/gtmobisaud.html

static_cast<double>(a) / b
来源：http://hz.jqgufenzy.top/gtfjgqjglg.html

[S52] C++：const 与 noexcept
来源：http://hz.xuanzx.com/gtbwxmgiqv.html

int size() const noexcept { return n_; }
来源：http://hz.yueranfly.top/gtjapkywjp.html

[S53] C++：移动语义
来源：http://hz.0kj1m.cn/gtmnswkyqh.html

std::vector<int> w = std::move(v);
来源：http://hz.yj20258888.top/gtjkuuqofi.html

[S54] C++：异常处理
来源：http://hz.sweek.top/gtorvdfutl.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.hammf.cn/gtqlnnaraf.html

[S55] C++：结构化绑定
来源：http://hz.jyoumei.cn/gtykbnnuso.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.chenjidiqi.icu/gtcifxvbdv.html

[S56] C++：optional
来源：http://hz.yj20258888.top/gtnpnnvise.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.jqgfzy.top/gtpilubxly.html

[S57] C++：编译期常量
来源：http://hz.wangdashe.top/gtetikdoqz.html

constexpr int N = 10;
来源：http://hz.nanxuanxn.top/gtbtbmyaci.html

[S58] C++：命名空间
来源：http://hz.bjfxy.top/gtkngnotuo.html

namespace ns { int f() { return 1; } }
来源：http://hz.jinyuanbaomall.cn/gtrvsqlqtl.html

[S59] C++：静态断言
来源：http://hz.dashuyun.cn/gtnuvpfiqo.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.shuidangran.top/gtkcvspses.html

[S60] C++：遍历并删除元素
来源：http://hz.yonumen.top/gtiswgvzje.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.vqdsnc.cn/gtnsrabbao.html

================================================================================
来源：http://hz.c1oappe.top/gtweqpglhn.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.gzhubu.top/gtupswtczl.html

================================================================================
来源：http://hz.yuxming.cn/gtljfqloch.html

[T01] Kotlin：Hello World
来源：http://hz.haohaochexian.top/gtqrccrpvq.html

println("Hello")
来源：http://hz.iojbl.cn/gtsdzsnurh.html

[T02] Kotlin：变量
来源：http://hz.jyoumei.cn/gthjktbmcf.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.chenlongwang.top/gtcudfqadf.html

[T03] Kotlin：字符串模板
来源：http://hz.meibo888.top/gtfclakfmb.html

"值: $b"
来源：http://hz.fengsongda.top/gthinuqoyk.html

[T04] Kotlin：空安全
来源：http://hz.gzhubu.top/gtgoznozuj.html

val n: String? = null;  n?.length
来源：http://hz.cdnleiting.top/gtdufuwtls.html

[T05] Kotlin：when 表达式
来源：http://hz.fzhhl.top/gtlsgcejze.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.vqdsnc.cn/gtlzlqxbsu.html

[T06] Kotlin：集合映射
来源：http://hz.ybcxt.top/gtigsqkndr.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.yanxiufei.cn/gtawhjhwjl.html

[T07] Kotlin：集合过滤
来源：http://hz.zhijiandao.cn/gtibomdxjr.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.yonumen.top/gtdmtyvclt.html

[T08] Kotlin：数据类
来源：http://hz.yuxming.cn/gtsavzdesb.html

data class User(val name: String, val age: Int)
来源：http://hz.andypj.xyz/gttryssrlj.html

[T09] Kotlin：扩展函数
来源：http://hz.xinyue.icu/gtcghqqrih.html

fun String.exclaim() = this + "!"
来源：http://hz.iojbl.cn/gtbdmsliex.html

[T10] Kotlin：默认参数
来源：http://hz.yonumen.top/gtqcfljnqd.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.jinqigfzy.top/gtgcucmtrz.html

[T11] Kotlin：协程
来源：http://hz.iojbl.cn/gtocxkazmd.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.guowangkeji.top/gtwihnacbv.html

[T12] Kotlin：解构声明
来源：http://hz.xuanzx.com/gtzupbhorf.html

val (a, b) = Pair(1, 2)
来源：http://hz.hfpthk.cn/gthvljsqzi.html

[T13] Kotlin：只读 Map
来源：http://hz.cheryme.top/gturprzjwy.html

val m = mapOf("a" to 1)
来源：http://hz.hnxiangtu.top/gtglhxewtj.html

[T14] Kotlin：循环
来源：http://hz.dashuyun.cn/gtfzcgcpxw.html

for (i in 1..10) println(i)
来源：http://hz.xziqi.cn/gtwxkuluuk.html

[T15] Kotlin：接口
来源：http://hz.hfpthk.cn/gthwyupsmw.html

interface Shape { fun area(): Double }
来源：http://hz.zhengqikj.top/gtyuxgfssp.html

[T16] Swift：Hello World
来源：http://hz.jqgfzy.top/gtlbqbvqhf.html

print("Hello")
来源：http://hz.chenzaomai.com/gtflfgslea.html

[T17] Swift：变量与常量
来源：http://hz.redwolf501.top/gtwnqzcyqa.html

var a = 1;  let b = 2
来源：http://hz.jinyuanbaomall.cn/gtmrzxiiqb.html

[T18] Swift：字符串插值
来源：http://hz.shanyushiyangtech.top/gtbrgebzrj.html

"值: \(b)"
来源：http://hz.zhiwuduotai.top/gtanurxxbp.html

[T19] Swift：可选绑定
来源：http://hz.vqdsnc.cn/gtsvefqytr.html

if let n = opt { print(n) }
来源：http://hz.xinyue.icu/gtlswibgle.html

[T20] Swift：数组操作
来源：http://hz.shzxlz.cn/gtzwoebcgm.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.kuanghao11.cn/gthvtkwdvq.html

[T21] Swift：遍历
来源：http://hz.meibo888.top/gtlawdrcik.html

for x in a { print(x) }
来源：http://hz.tianlin.xyz/gtioauvfry.html

[T22] Swift：字典
来源：http://hz.jlsjyb.cn/gtukpeyckk.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.vqdsnc.cn/gtvsglwaji.html

[T23] Swift：函数
来源：http://hz.zhijiandao.cn/gtnksrfkye.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.svipenyu.cn/gttoxpzprl.html

[T24] Swift：闭包
来源：http://hz.quarkkingdee.top/gtambyikaw.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.kuanghao11.cn/gtadomqvdu.html

[T25] Swift：结构体
来源：http://hz.meibo888.top/gtcdgrkojf.html

struct P { var x: Int }
来源：http://hz.yueranfly.top/gtneujcgow.html

[T26] Swift：类与重写
来源：http://hz.zhiwuduotai.top/gtrhdnnsjm.html

class A: Base { override func f() {} }
来源：http://hz.shangyingyoupin.top/gtonmznokm.html

[T27] Swift：错误处理
来源：http://hz.dashuyun.cn/gtteufctaj.html

do { try f() } catch { print(error) }
来源：http://hz.tianlin.xyz/gtxryxtklp.html

[T28] Swift：枚举
来源：http://hz.smart0.xyz/gtucfkwuze.html

enum Color { case red, green }
来源：http://hz.hnxiangtu.top/gtjbszhciv.html

[T29] Swift：guard 提前返回
来源：http://hz.ydzc1.top/gtsvstyxwn.html

guard let x = opt else { return }
来源：http://hz.ppjwa.cn/gtlyrixmoa.html

[T30] Swift：协议
来源：http://hz.wangdashe.top/gtobqtzhvd.html

protocol Shape { func area() -> Double }
来源：http://hz.guowangkeji.top/gtbbzapwbb.html

[T31] Lua：Hello World
来源：http://hz.ehwqpu.com/gtmxtbiini.html

print("Hello")
来源：http://hz.nanxinkj.top/gtesfuijsb.html

[T32] Lua：局部变量
来源：http://hz.wangdashe.top/gtjfxvbulg.html

local a = 1
来源：http://hz.ydjk.org.cn/gtckvxvxec.html

[T33] Lua：表（数组）
来源：http://hz.nanxinkj.top/gtxkzjutou.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.xingfuxueyuan.xyz/gtfwdnugze.html

[T34] Lua：遍历表
来源：http://hz.cdnleiting.top/gtbjkycrhd.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.jqgfzy.top/gtotqatkui.html

[T35] Lua：字典表
来源：http://hz.dashuyun.cn/gtnxgwxfnk.html

local d = { a = 1 };  d.b = 2
来源：http://hz.ivvv.top/gtohqwqbis.html

[T36] Lua：函数
来源：http://hz.jianghu66.top/gtuwsjtxlr.html

function add(a, b) return a + b end
来源：http://hz.gotoacloud.top/gtqmobvfsc.html

[T37] Lua：字符串拼接
来源：http://hz.gotoacloud.top/gtjvluvjyx.html

"a" .. "b"
来源：http://hz.yangfankeji.com/gthhqgtejx.html

[T38] Lua：条件
来源：http://hz.hammf.cn/gttolxhttn.html

if x > 0 then print("正") end
来源：http://hz.snrcjt.cn/gtbnepkgrx.html

[T39] Lua：模式匹配
来源：http://hz.sufxvd.cn/gtqicnsqpk.html

string.find(s, "%d+")
来源：http://hz.cucudq.cn/gtfpeiahwr.html

[T40] Lua：元表
来源：http://hz.jiagoushi.top/gtestnwxsv.html

setmetatable({}, { __index = base })
来源：http://hz.mhx1999.top/gtsomgqkqi.html

[T41] Perl：Hello World
来源：http://hz.xuetiantiany.cn/gtvsmboxcr.html

print "Hello\n";
来源：http://hz.gogol.net.cn/gthfhyqjwp.html

[T42] Perl：变量类型
来源：http://hz.fengsongda.top/gtdkpteall.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.yj20258888.top/gtovvtjjyt.html

[T43] Perl：字符串插值
来源：http://hz.shzxlz.cn/gttsflkiha.html

"值: $a"
来源：http://hz.sxryk.cn/gtjsoujohq.html

[T44] Perl：条件
来源：http://hz.nanxinkj.top/gtzqefjhvz.html

if ($a > 0) { print "正"; }
来源：http://hz.316326.xyz/gtfvrbvjlm.html

[T45] Perl：数组遍历
来源：http://hz.sxryk.cn/gtnlhhxrzl.html

for my $x (@arr) { print $x; }
来源：http://hz.tianlin.xyz/gtvwrsthgz.html

[T46] Perl：哈希操作
来源：http://hz.pengpengdd.cyou/gtnacxywgw.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.9152youxi.cn/gtnnsbifvs.html

[T47] Perl：正则捕获
来源：http://hz.guowangkeji.top/gtpzkwgpcb.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.kuanghao11.cn/gtnmonjbxh.html

[T48] Perl：正则替换
来源：http://hz.zhixingplan.top/gtbtgxadgs.html

$s =~ s/old/new/g;
来源：http://hz.cdnleiting.top/gtxisrlwsz.html

[T49] Perl：函数
来源：http://hz.shanyushiyangtech.top/gtdcvgmnmb.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.meibo888.top/gtmqikxfeb.html

[T50] Perl：逐行读文件
来源：http://hz.ppjwa.cn/gtzqefdphw.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.hongshengwenyu.top/gtfcwxfqsr.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.jianghu66.top/gtkyemjkdc.html

[T51] Scala：Hello World
来源：http://hz.sxryk.cn/gtpvfybodg.html

println("Hello")
来源：http://hz.zhijiandao.cn/gtwbmmdpyp.html

[T52] Scala：变量
来源：http://hz.sweek.top/gtxxvcqdzn.html

val a = 1;  var b = 2
来源：http://hz.ppjwa.cn/gtnytpgjph.html

[T53] Scala：字符串插值
来源：http://hz.ydjk.org.cn/gtgjzkzrmk.html

s"值: $b"
来源：http://hz.yangfankeji.com/gtpjvinnid.html

[T54] Scala：集合映射
来源：http://hz.xingfuxueyuan.xyz/gtznnvhyij.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.sufxvd.cn/gtxgjqxsgo.html

[T55] Scala：集合过滤
来源：http://hz.zycfv.cn/gtnqsqhzbd.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.hongshengwenyu.top/gteanyjilz.html

[T56] Scala：样例类
来源：http://hz.xuetiantiany.cn/gtpqinghbv.html

case class User(name: String, age: Int)
来源：http://hz.tianlin.xyz/gtudnnxbug.html

[T57] Scala：模式匹配
来源：http://hz.zdqjudy.top/gttbiyfnvc.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.guannengcc.top/gtsqwxpfsm.html

[T58] Scala：函数定义
来源：http://hz.xingfuxueyuan.xyz/gtzdjqsrjo.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.nanxinkj.top/gtwepetihd.html

[T59] Scala：循环
来源：http://hz.wangdashe.top/gtanlnetmn.html

for (i <- 1 to 10) println(i)
来源：http://hz.meibo888.top/gtzhfbfsvx.html

[T60] Scala：折叠
来源：http://hz.pycfn.com/gtbfwcpeom.html


<!-- 参考信息 -->