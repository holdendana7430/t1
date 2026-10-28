代发 wailian999

ssh user@host 'uptime'
来源：http://hz.ybcxt.top/gtljypsheb.html

[R58] 下载文件
来源：http://hz.guowangkeji.top/gtazhhjbfo.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.wangdashe.top/gteuwvmsmj.html

[R59] 发 POST JSON
来源：http://hz.snrcjt.cn/gttjvianvf.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.shzxlz.cn/gtwlygzwbj.html

[R60] 只看 HTTP 状态码
来源：http://hz.yangfankeji.com/gtvnzmrsdz.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.xylfe.cn/gtlvyvypns.html

[R61] 磁盘占用
来源：http://hz.jinghuilouyu.cn/gtdphkgbtc.html

df -h;  du -sh *
来源：http://hz.52xcode.cn/gtltyfdhfp.html

[R62] 找最占空间的文件
来源：http://hz.zycfv.cn/gtbonfebqq.html

du -ah . | sort -rh | head -10
来源：http://hz.yueranfly.top/gteqhclqfg.html

[R63] 内存与进程
来源：http://hz.shangyingyoupin.top/gthbcmspsf.html

free -h;  ps aux | grep nginx
来源：http://hz.kuanghao11.cn/gtnellfcwe.html

[R64] 结束进程
来源：http://hz.haohaochexian.top/gteukcowbv.html

kill -9 $(pgrep -f app.py)
来源：http://hz.guowangkeji.top/gtwzcqxqge.html

[R65] 查看端口占用
来源：http://hz.yonumen.top/gtjgwjytgc.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.redwolf501.top/gtygcfewsr.html

[R66] 定时任务
来源：http://hz.gogol.net.cn/gtrrbwdwpy.html

crontab -e;  crontab -l
来源：http://hz.gotoacloud.top/gttebehfvf.html

[R67] 生成随机十六进制串
来源：http://hz.birdmap.top/gtrsckqisv.html

openssl rand -hex 16
来源：http://hz.xinyue.icu/gtrqqbvszy.html

[R68] 计算文件校验值
来源：http://hz.wangdashe.top/gtpdffadeb.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.dianchejie.cn/gtpvxnqjtd.html

[R69] 生成随机密码
来源：http://hz.tian-w.cn/gtxvclzvcx.html

head -c 16 /dev/urandom | base64
来源：http://hz.jyoumei.cn/gtvhoxfoqc.html

[R70] 时间戳与互转
来源：http://hz.hnxiangtu.top/gtgjuzwpxh.html

date +%s;  date -d @1700000000
来源：http://hz.zhixingplan.top/gtcdejlpnk.html

[R71] 日期格式化
来源：http://hz.shangyingyoupin.top/gthecflasd.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.nanxuanxn.top/gtpqvkuxmf.html

[R72] 等待端口就绪
来源：http://hz.zdqjudy.top/gtdzoreunk.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.daxiang520.top/gttrepvsyb.html

[R73] 分割大日志
来源：http://hz.shanyushiyangkeji.top/gtmabcdsqf.html

split -l 1000 big.log part_
来源：http://hz.ybcxt.top/gtpypfaibp.html

[R74] 批量重命名
来源：http://hz.aizwys.cn/gtqwtiqrxv.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.hysaishi.cn/gtemnlgviv.html

[R75] 导出环境变量
来源：http://hz.chenzaomai.com/gtlzvsyiww.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.tianlin.xyz/gtxaqjrexl.html

[R76] 使用临时文件
来源：http://hz.shzxlz.cn/gtkmifzvto.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.shanyushiyangkeji.top/gtegsoobzn.html

[R77] 读取用户输入
来源：http://hz.zhiwuduotai.top/gtlabohrvo.html

read -rp "请输入: " ans
来源：http://hz.yanxiufei.cn/gtrsacnflo.html

[R78] 交互式菜单
来源：http://hz.pengpengdd.cyou/gtzsfkpbjl.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.cashguo.top/gtkqoqjagt.html

[R79] 解析命令行选项
来源：http://hz.cucudq.cn/gtmdmqlrae.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.guannengcc.top/gteblfjrkm.html

[R80] 查看脚本执行耗时
来源：http://hz.yvedp.cn/gtraiopugb.html

time ./run.sh
来源：http://hz.fengsongda.top/gtqdbeywqk.html

================================================================================
来源：http://hz.gotoacloud.top/gtwavbboei.html

S. C / C++ 专题
来源：http://hz.feifeiyinyue.top/gtuwojtesb.html

================================================================================
来源：http://hz.xinyue.icu/gtgfqzwjpp.html

[S01] C：Hello World
来源：http://hz.yangfankeji.com/gtsddxervc.html

#include <stdio.h>
来源：http://hz.dianchejie.cn/gtsjpuwbwd.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.mhx1999.top/gtpttxeezl.html

[S02] C：变量与格式化输出
来源：http://hz.wangshuangyany.cn/gtxwxuxomh.html

int a = 10; printf("%d\n", a);
来源：http://hz.sysykeji.top/gtleashpiy.html

[S03] C：读入整数
来源：http://hz.nanxuanxn.top/gtktxnrlhj.html

int x; scanf("%d", &x);
来源：http://hz.jqgfzy.top/gtpoeeihhq.html

[S04] C：字符串复制
来源：http://hz.daria6918.cn/gtxnrjswru.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.dianchejie.cn/gtuhvgdiyq.html

[S05] C：字符串长度
来源：http://hz.snrcjt.cn/gtisyrxykd.html

strlen(s)
来源：http://hz.yj202588.top/gtkztejyvc.html

[S06] C：字符串比较
来源：http://hz.zhongyouzk.top/gtglkszllp.html

strcmp(a, b) == 0
来源：http://hz.zhijiandao.cn/gticqvxefi.html

[S07] C：数组遍历求和
来源：http://hz.zhongyouzk.top/gtlgrseyec.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.sweek.top/gtivjrcfhh.html

[S08] C：动态内存分配与释放
来源：http://hz.zhengqikj.top/gtsvlyzsik.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.zhiwuduotai.top/gtazpkmesr.html

[S09] C：结构体定义与初始化
来源：http://hz.jinqigufen.top/gtabuyqzdo.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.hysaishi.cn/gthdrbushm.html

[S10] C：指针与解引用
来源：http://hz.chenjidiqi.icu/gtadkpqamh.html

int *p = &a;  *p = 5;
来源：http://hz.xuanzx.com/gtxvtlwvof.html

[S11] C：逐行读文件
来源：http://hz.smart0.xyz/gtmprustdp.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.shangyingyoupin.top/gtbgqcdlya.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.nanxuanxn.top/gtwjkxiwst.html

fclose(f);
来源：http://hz.cdnleiting.top/gttxcssmcv.html

[S12] C：写文件
来源：http://hz.cdnleiting.top/gtnjoxffpn.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.jinyuanbaomall.cn/gtlqzurwld.html

[S13] C：宏定义
来源：http://hz.cheryme.top/gtapkzqglt.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.yvedp.cn/gtdskktuvo.html

[S14] C：枚举
来源：http://hz.nanxuanxn.top/gtrrespdms.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.ywan-chungtsiang.top/gtyzscadwy.html

[S15] C：类型转换
来源：http://hz.andypj.xyz/gtktztnytl.html

(double) a / b
来源：http://hz.daxiang520.top/gthaimyxqe.html

[S16] C：位操作置位
来源：http://hz.guowangkeji.top/gtmpcbuska.html

x |= (1 << 3);
来源：http://hz.pengpengdd.cyou/gtsdzgkzij.html

[S17] C：安全拼接字符串
来源：http://hz.tanke756.top/gtqdvbaqay.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.ydzc1.top/gthtuwaitk.html

[S18] C：命令行参数
来源：http://hz.cucudq.cn/gtatdhhpcc.html

int main(int argc, char **argv)
来源：http://hz.yanxiufei.cn/gtokezlfpy.html

[S19] C：快速排序
来源：http://hz.9152youxi.cn/gtlhyplavu.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.zhaomingkeji.xyz/gtjbyvcrov.html

[S20] C：二分查找
来源：http://hz.jyoumei.cn/gtdzgbfxda.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.sxryk.cn/gtkypspxzr.html

[S21] C：字符类别判断
来源：http://hz.aibaodan.cn/gtwkdqbqhy.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.jqgufenzy.top/gtrfzofxul.html

[S22] C：字符串转数字
来源：http://hz.9152youxi.cn/gtxoxjdhek.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.jyoumei.cn/gtsppmzblv.html

[S23] C：随机数
来源：http://hz.zhixingplan.top/gttmvrgujj.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.daria6918.cn/gtssukmubt.html

[S24] C：获取本地时间
来源：http://hz.52xcode.cn/gtlyhgexhl.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.gogol.net.cn/gttlgrmxkq.html

[S25] C：内存拷贝
来源：http://hz.hfpthk.cn/gthyguegqd.html

memcpy(dst, src, n);
来源：http://hz.ehwqpu.com/gtdgmvjjhd.html

[S26] C：内存清零
来源：http://hz.shanyushiyangkeji.top/gtuirsdpcs.html

memset(a, 0, sizeof a);
来源：http://hz.quarkkingdee.top/gtmiofgicp.html

[S27] C：定义常量
来源：http://hz.fzhhl.top/gtwfududhq.html

const double PI = 3.14159;
来源：http://hz.jinqigufen.top/gtgyspgzuv.html

[S28] C：静态变量
来源：http://hz.yj20258.top/gtilssqpnh.html

static int counter = 0;
来源：http://hz.shanyushiyangkeji.top/gtprcqpqra.html

[S29] C：变参函数
来源：http://hz.zhongyouzk.top/gtnezpuqfx.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.ywan-chungtsiang.top/gtxwsgmdww.html

[S30] C：头文件保护
来源：http://hz.jinghuilouyu.cn/gtgknlkczc.html

#ifndef X_H
来源：http://hz.ppjwa.cn/gtszdygvsy.html

#define X_H
来源：http://hz.zhaomingkeji.xyz/gtribivxib.html

#endif
来源：http://hz.zhaomingkeji.xyz/gteypxrmzi.html

[S31] C++：Hello World
来源：http://hz.shzxlz.cn/gtwsylupxu.html

#include <iostream>
来源：http://hz.snrcjt.cn/gtppmrvjbv.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.jianghu66.top/gtzqxujgbb.html

[S32] C++：字符串
来源：http://hz.mhx1999.top/gtvdumkvax.html

std::string s = "hi";  s += "!";
来源：http://hz.jinqigufen.top/gtajpeorbw.html

[S33] C++：vector 增删
来源：http://hz.meibo888.top/gtivzlarlk.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.cdnleiting.top/gtcpdkrase.html

[S34] C++：遍历 vector
来源：http://hz.jinyuanbaomall.cn/gtfdqfhjyj.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.52xcode.cn/gtjbsqthyi.html

[S35] C++：map
来源：http://hz.guowangkeji.top/gtxwkcdawl.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.xingfuxueyuan.xyz/gtqzxpvxco.html

[S36] C++：unordered_map
来源：http://hz.daria6918.cn/gtbmtwizdk.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.shzxlz.cn/gtoiwqvwcd.html

[S37] C++：set
来源：http://hz.yj20258888.top/gttsntyptq.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.jlsjyb.cn/gtpccrqmll.html

[S38] C++：排序
来源：http://hz.jianghu66.top/gtbbfodqth.html

std::sort(v.begin(), v.end());
来源：http://hz.snrcjt.cn/gtdfdjtdpg.html

[S39] C++：自定义比较器排序
来源：http://hz.chenzaomai.com/gtrhwlqvau.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.hammf.cn/gtxppxkfrv.html

[S40] C++：查找元素
来源：http://hz.0kj1m.cn/gtoozhrvrp.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.zhengqikj.top/gtjnbtyigc.html

[S41] C++：类与构造函数
来源：http://hz.jqgufenzy.top/gtvrnsrfjw.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.jyoumei.cn/gtjxxdolut.html

[S42] C++：继承与虚函数
来源：http://hz.havefunace.top/gtjlinyind.html

class B : public Base { public: void f() override {} };
来源：http://hz.nwbrower.top/gtbrfuskav.html

[S43] C++：智能指针
来源：http://hz.jiagoushi.top/gtgnlzixrg.html

auto p = std::make_unique<int>(5);
来源：http://hz.zdqjudy.top/gtyllrhxgs.html

[S44] C++：引用传参
来源：http://hz.52xcode.cn/gtajefkfwf.html

void inc(int &x) { ++x; }
来源：http://hz.sufxvd.cn/gtqudrhypt.html

[S45] C++：lambda
来源：http://hz.sxryk.cn/gtxcqrpekm.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.daria6918.cn/gtivdbaoab.html

[S46] C++：函数模板
来源：http://hz.hammf.cn/gtbmkkaotm.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.jinqigufen.top/gtbgujfzxs.html

[S47] C++：结构化绑定遍历
来源：http://hz.tianlin.xyz/gtnygabxfr.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.havefunace.top/gtkrzroxcc.html

[S48] C++：逐行读文件
来源：http://hz.tanke756.top/gtkftjngcr.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.shzxlz.cn/gtlssyxozn.html

while (std::getline(in, line)) { }
来源：http://hz.hywenlv.cn/gtfndcizkj.html

[S49] C++：写文件
来源：http://hz.svipenyu.cn/gtosnesvlf.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.yueranfly.top/gtsfrmazfi.html

[S50] C++：格式化数字
来源：http://hz.jinqigufen.top/gtwhaxukqk.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.c1oappe.top/gtmmymfohe.html

[S51] C++：显式类型转换
来源：http://hz.pengpengdd.cyou/gtnyqduacm.html

static_cast<double>(a) / b
来源：http://hz.tian-w.cn/gtnxfhbbfp.html

[S52] C++：const 与 noexcept
来源：http://hz.zhengqikj.top/gtmseorafh.html

int size() const noexcept { return n_; }
来源：http://hz.hongshengwenyu.top/gtzrrtbmid.html

[S53] C++：移动语义
来源：http://hz.vqdsnc.cn/gtihlnhdpz.html

std::vector<int> w = std::move(v);
来源：http://hz.ydjk.org.cn/gtaohvpwus.html

[S54] C++：异常处理
来源：http://hz.vqdsnc.cn/gtnrenrtwm.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.yj202588.top/gtujluited.html

[S55] C++：结构化绑定
来源：http://hz.jianghu66.top/gtgrdlvjbo.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.jianghu66.top/gtvlopwnkf.html

[S56] C++：optional
来源：http://hz.chenjidiqi.icu/gtmxbcnzna.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.xziqi.cn/gtxfeslnln.html

[S57] C++：编译期常量
来源：http://hz.ehwqpu.com/gtkdegezov.html

constexpr int N = 10;
来源：http://hz.pengpengdd.cyou/gtcuskbxcn.html

[S58] C++：命名空间
来源：http://hz.vqdsnc.cn/gtpjntylut.html

namespace ns { int f() { return 1; } }
来源：http://hz.xylfe.cn/gtqrabeefw.html

[S59] C++：静态断言
来源：http://hz.mhx1999.top/gtnrjpycks.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.zhongyouzk.top/gtmvcyoumr.html

[S60] C++：遍历并删除元素
来源：http://hz.cashguo.top/gttkksrdpj.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.zhijiandao.cn/gtrmxqfugd.html

================================================================================
来源：http://hz.quarkkingdee.top/gtkwtceqbt.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.meibo888.top/gtafrbfipd.html

================================================================================
来源：http://hz.hammf.cn/gtcgwirwdc.html

[T01] Kotlin：Hello World
来源：http://hz.zhongyouzk.top/gtciqqltza.html

println("Hello")
来源：http://hz.zhixingplan.top/gtxsjivora.html

[T02] Kotlin：变量
来源：http://hz.gzhubu.top/gtbhfmmrmf.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.ybcxt.top/gtkyexgxym.html

[T03] Kotlin：字符串模板
来源：http://hz.cdnleiting.top/gtbiazdroh.html

"值: $b"
来源：http://hz.andypj.xyz/gthvfuppyl.html

[T04] Kotlin：空安全
来源：http://hz.pycfn.com/gtugcbnenb.html

val n: String? = null;  n?.length
来源：http://hz.smart0.xyz/gtebvrkzoj.html

[T05] Kotlin：when 表达式
来源：http://hz.sxryk.cn/gtdykagtkj.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.zdqjudy.top/gtvjujnjxb.html

[T06] Kotlin：集合映射
来源：http://hz.hammf.cn/gtscgidiwl.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.nanxinkj.top/gtrkneagwi.html

[T07] Kotlin：集合过滤
来源：http://hz.iojbl.cn/gtkaknkyyj.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.hnxiangtu.top/gtovxzryub.html

[T08] Kotlin：数据类
来源：http://hz.ehwqpu.com/gtpghetqeq.html

data class User(val name: String, val age: Int)
来源：http://hz.ydjk.org.cn/gtsrdybpdx.html

[T09] Kotlin：扩展函数
来源：http://hz.xziqi.cn/gtktnaebfy.html

fun String.exclaim() = this + "!"
来源：http://hz.hywenlv.cn/gteipkgyvp.html

[T10] Kotlin：默认参数
来源：http://hz.hongshengwenyu.top/gtbotofekn.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.yuanzhike.top/gtevrhksjq.html

[T11] Kotlin：协程
来源：http://hz.bjfxy.top/gthilpgxto.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.birdmap.top/gtbhobjbpf.html

[T12] Kotlin：解构声明
来源：http://hz.xinyue.icu/gtekggfjpw.html

val (a, b) = Pair(1, 2)
来源：http://hz.snrcjt.cn/gtzvyfnuwo.html

[T13] Kotlin：只读 Map
来源：http://hz.shuidangran.top/gtyjvpbymp.html

val m = mapOf("a" to 1)
来源：http://hz.jinqigfzy.top/gtezhzdfum.html

[T14] Kotlin：循环
来源：http://hz.gogol.net.cn/gtrqxisadq.html

for (i in 1..10) println(i)
来源：http://hz.yuxming.cn/gturmgufcq.html

[T15] Kotlin：接口
来源：http://hz.svipenyu.cn/gtkdgxdeyb.html

interface Shape { fun area(): Double }
来源：http://hz.xingfuxueyuan.xyz/gtcbxnuagz.html

[T16] Swift：Hello World
来源：http://hz.shanyushiyangtech.top/gtygfmhlbk.html

print("Hello")
来源：http://hz.dashuyun.cn/gtjbjckfuh.html

[T17] Swift：变量与常量
来源：http://hz.svipenyu.cn/gtbeoxwrdc.html

var a = 1;  let b = 2
来源：http://hz.jyoumei.cn/gtstqsqlrh.html

[T18] Swift：字符串插值
来源：http://hz.jinyuanbaomall.cn/gtjkululod.html

"值: \(b)"
来源：http://hz.tianlin.xyz/gtzjlkawlo.html

[T19] Swift：可选绑定
来源：http://hz.xingfuxueyuan.xyz/gtpjyxyxpe.html

if let n = opt { print(n) }
来源：http://hz.yanxiufei.cn/gtqphoaxsf.html

[T20] Swift：数组操作
来源：http://hz.jiagoushi.top/gtveqpeipo.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.aibaodan.cn/gtwnbwkfyu.html

[T21] Swift：遍历
来源：http://hz.tanke756.top/gteebuejlu.html

for x in a { print(x) }
来源：http://hz.hysaishi.cn/gtznngfbvr.html

[T22] Swift：字典
来源：http://hz.birdmap.top/gtcuciihur.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.ywan-chungtsiang.top/gtarymnhwf.html

[T23] Swift：函数
来源：http://hz.zhongyouzk.top/gtvxobuujx.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.hammf.cn/gtlbjfnape.html

[T24] Swift：闭包
来源：http://hz.jinyuanbaomall.cn/gtqntqaaqi.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.ybcxt.top/gtqfnruizi.html

[T25] Swift：结构体
来源：http://hz.yanxiufei.cn/gtanbojveb.html

struct P { var x: Int }
来源：http://hz.yangfankeji.com/gtelujnzjv.html

[T26] Swift：类与重写
来源：http://hz.ydzc1.top/gtkokjkbws.html

class A: Base { override func f() {} }
来源：http://hz.ivvv.top/gtfwpyxfnb.html

[T27] Swift：错误处理
来源：http://hz.mhx1999.top/gtxluwfzna.html

do { try f() } catch { print(error) }
来源：http://hz.yuxming.cn/gtbwgmvydd.html

[T28] Swift：枚举
来源：http://hz.shangyingyoupin.top/gtpwyknkox.html

enum Color { case red, green }
来源：http://hz.yanxiufei.cn/gtxaiaqkaz.html

[T29] Swift：guard 提前返回
来源：http://hz.xuanzx.com/gtoejdfmaz.html

guard let x = opt else { return }
来源：http://hz.nanxuanxn.top/gtamhadieg.html

[T30] Swift：协议
来源：http://hz.gaohongyu789.top/gtztsnbmdr.html

protocol Shape { func area() -> Double }
来源：http://hz.jinqigufen.top/gtonfngrct.html

[T31] Lua：Hello World
来源：http://hz.nanxuanxn.top/gtigvuilxq.html

print("Hello")
来源：http://hz.sxryk.cn/gtheydwbds.html

[T32] Lua：局部变量
来源：http://hz.52xcode.cn/gtmstteovb.html

local a = 1
来源：http://hz.tianlin.xyz/gtgzvcukfs.html

[T33] Lua：表（数组）
来源：http://hz.haohaochexian.top/gtyjsvfunu.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.hongshengwenyu.top/gtwtjjgxpm.html

[T34] Lua：遍历表
来源：http://hz.xuanzx.com/gtbtrgmyof.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.nwbrower.top/gtukgbmhaa.html

[T35] Lua：字典表
来源：http://hz.hnqzz.top/gtilelvubq.html

local d = { a = 1 };  d.b = 2
来源：http://hz.wangdashe.top/gtnhnegvkv.html

[T36] Lua：函数
来源：http://hz.tanke756.top/gtfnagqujz.html

function add(a, b) return a + b end
来源：http://hz.shangyingyoupin.top/gtqkqlvkdz.html

[T37] Lua：字符串拼接
来源：http://hz.kuanghao11.cn/gtpeykoquh.html

"a" .. "b"
来源：http://hz.sxryk.cn/gttchldjbg.html

[T38] Lua：条件
来源：http://hz.chenjidiqi.icu/gtiiglyvmr.html

if x > 0 then print("正") end
来源：http://hz.kuanghao11.cn/gtspmwzdgg.html

[T39] Lua：模式匹配
来源：http://hz.nwbrower.top/gtzloipfkp.html

string.find(s, "%d+")
来源：http://hz.xylfe.cn/gtyrjonera.html

[T40] Lua：元表
来源：http://hz.sxryk.cn/gtogwzqskb.html

setmetatable({}, { __index = base })
来源：http://hz.yanxiufei.cn/gtsfgbkgyl.html

[T41] Perl：Hello World
来源：http://hz.cucudq.cn/gtetsafpoi.html

print "Hello\n";
来源：http://hz.dashuyun.cn/gtikmjbfke.html

[T42] Perl：变量类型
来源：http://hz.ybcxt.top/gtytcnqxwm.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.feifeiyinyue.top/gtglppypdh.html

[T43] Perl：字符串插值
来源：http://hz.nanxuanxn.top/gtqppjgkok.html

"值: $a"
来源：http://hz.cheryme.top/gtaslgnnbl.html

[T44] Perl：条件
来源：http://hz.cqqwz.cn/gtzkxatiff.html

if ($a > 0) { print "正"; }
来源：http://hz.xinyue.icu/gtzrfynbej.html

[T45] Perl：数组遍历
来源：http://hz.hammf.cn/gtphwjoocn.html

for my $x (@arr) { print $x; }
来源：http://hz.hywenlv.cn/gtyqgucadb.html

[T46] Perl：哈希操作
来源：http://hz.fengsongda.top/gtvwdpfcqq.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.cqqwz.cn/gtzznxhbmf.html

[T47] Perl：正则捕获
来源：http://hz.shangyingyoupin.top/gtltbfagbg.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.jianghu66.top/gtkvuulcrh.html

[T48] Perl：正则替换
来源：http://hz.zycfv.cn/gtdakpszom.html

$s =~ s/old/new/g;
来源：http://hz.tian-w.cn/gtfwtutkdf.html

[T49] Perl：函数
来源：http://hz.ybcxt.top/gtbyautpms.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.52xcode.cn/gtehrtoegh.html

[T50] Perl：逐行读文件
来源：http://hz.52xcode.cn/gtekcvgmsk.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.yj20258888.top/gtrizyguga.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.zhijiandao.cn/gtyanunprf.html

[T51] Scala：Hello World
来源：http://hz.ehwqpu.com/gtonomyzbu.html

println("Hello")
来源：http://hz.kuanghao11.cn/gtagokamio.html

[T52] Scala：变量
来源：http://hz.tian-w.cn/gtxtcecdat.html

val a = 1;  var b = 2
来源：http://hz.guannengcc.top/gttxkyyozi.html

[T53] Scala：字符串插值
来源：http://hz.yj202588.top/gtpifxhfws.html

s"值: $b"
来源：http://hz.zhiwuduotai.top/gtowgbtqti.html

[T54] Scala：集合映射
来源：http://hz.shanyushiyangkeji.top/gtzieqlxsi.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.fengsongda.top/gtkrododji.html

[T55] Scala：集合过滤
来源：http://hz.0kj1m.cn/gtlvjlwlqa.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.jinghuilouyu.cn/gtlzwlweqi.html

[T56] Scala：样例类
来源：http://hz.dianchejie.cn/gtyhbtrkjr.html

case class User(name: String, age: Int)
来源：http://hz.sysykeji.top/gtaivqfyfn.html

[T57] Scala：模式匹配
来源：http://hz.svipenyu.cn/gtxjcwzgpr.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.haohaochexian.top/gtazajkdyl.html

[T58] Scala：函数定义
来源：http://hz.dashuyun.cn/gtfirgxreu.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.zhijiandao.cn/gtlsfxkdsu.html

[T59] Scala：循环
来源：http://hz.yvedp.cn/gtwgyfxrww.html

for (i <- 1 to 10) println(i)
来源：http://hz.jlsjyb.cn/gtrnugfraj.html

[T60] Scala：折叠
来源：http://hz.hammf.cn/gtcufvgarb.html


<!-- 参考信息 -->