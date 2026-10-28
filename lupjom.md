代发 wailian999

find . -name "*.tmp" -delete
来源：http://hz.gzhubu.top/gtreuaduol.html

[R46] 递归替换文件内容
来源：http://hz.yuxming.cn/gtewrtacjk.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.fzhhl.top/gtgjlivgat.html

[R47] sed 单行替换
来源：http://hz.0kj1m.cn/gtvdabyabh.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.fzhhl.top/gtjxzdwaij.html

[R48] awk 取指定列
来源：http://hz.pycfn.com/gtcpnpwssx.html

awk '{print $1, $3}' a.txt
来源：http://hz.hywenlv.cn/gtdzhvnlak.html

[R49] awk 带条件
来源：http://hz.aizwys.cn/gtzhtpnhgq.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.cdnleiting.top/gtmmnosvfy.html

[R50] awk 求和
来源：http://hz.nwbrower.top/gtjfeqrvpn.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.guannengcc.top/gtqjmltggt.html

[R51] 排序去重取前几
来源：http://hz.mhx1999.top/gtiupmxfhi.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.pengpengdd.cyou/gtohkzqaef.html

[R52] 统计行数
来源：http://hz.birdmap.top/gtsiijdmsc.html

wc -l a.txt
来源：http://hz.zhijiandao.cn/gtwdkelucn.html

[R53] 查看文件头与实时尾
来源：http://hz.kuanghao11.cn/gtvjcaseje.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.dianchejie.cn/gtvuawoojz.html

[R54] 比较两个文件
来源：http://hz.zycfv.cn/gtcidgedbs.html

diff a.txt b.txt
来源：http://hz.ppjwa.cn/gtqmhaohof.html

[R55] 压缩与解压
来源：http://hz.hysaishi.cn/gtuzstmrti.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.nwbrower.top/gtbzwlnusz.html

[R56] 远程拷贝
来源：http://hz.pengpengdd.cyou/gtmoofcwfg.html

scp file user@host:/path/
来源：http://hz.wangdashe.top/gthspuzbru.html

[R57] 远程执行命令
来源：http://hz.jianghu66.top/gtzpesjhfj.html

ssh user@host 'uptime'
来源：http://hz.yongpay.top/gtumroohth.html

[R58] 下载文件
来源：http://hz.snrcjt.cn/gtaxkvmmkq.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.aizwys.cn/gtezrylxsy.html

[R59] 发 POST JSON
来源：http://hz.iojbl.cn/gtdziesmrv.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.xingfuxueyuan.xyz/gtxruafkov.html

[R60] 只看 HTTP 状态码
来源：http://hz.xylfe.cn/gtprfcptyl.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.zhaomingkeji.xyz/gtyxtwyerw.html

[R61] 磁盘占用
来源：http://hz.zhiwuduotai.top/gtkocsycom.html

df -h;  du -sh *
来源：http://hz.zycfv.cn/gtmvefbgmc.html

[R62] 找最占空间的文件
来源：http://hz.yueranfly.top/gtrwgdqusw.html

du -ah . | sort -rh | head -10
来源：http://hz.52xcode.cn/gtctpkhhbf.html

[R63] 内存与进程
来源：http://hz.yj20258888.top/gtfejkztxw.html

free -h;  ps aux | grep nginx
来源：http://hz.ppjwa.cn/gtxazfkfhg.html

[R64] 结束进程
来源：http://hz.cheryme.top/gtgjtmtlpj.html

kill -9 $(pgrep -f app.py)
来源：http://hz.c1oappe.top/gtykmxsfct.html

[R65] 查看端口占用
来源：http://hz.jinyuanbaomall.cn/gtdcyojjye.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.fengsongda.top/gtwlaghwaw.html

[R66] 定时任务
来源：http://hz.cheryme.top/gtpgzhfbvc.html

crontab -e;  crontab -l
来源：http://hz.xuetiantiany.cn/gtzxyxymai.html

[R67] 生成随机十六进制串
来源：http://hz.nanxinkj.top/gtvyqrmbvi.html

openssl rand -hex 16
来源：http://hz.yanxiufei.cn/gtxqoptbfk.html

[R68] 计算文件校验值
来源：http://hz.yj202588.top/gtfyagjplm.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.jqgufenzy.top/gtpcxrmhxt.html

[R69] 生成随机密码
来源：http://hz.zhiwuduotai.top/gtnanwhtac.html

head -c 16 /dev/urandom | base64
来源：http://hz.hongshengwenyu.top/gttttsjosl.html

[R70] 时间戳与互转
来源：http://hz.yuanzhike.top/gtexqasyci.html

date +%s;  date -d @1700000000
来源：http://hz.tian-w.cn/gtkdamomun.html

[R71] 日期格式化
来源：http://hz.jianghu66.top/gtcznrtytv.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.9152youxi.cn/gtmqjuifha.html

[R72] 等待端口就绪
来源：http://hz.gotoacloud.top/gtsctpwopn.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.hongshengwenyu.top/gtrtlnneum.html

[R73] 分割大日志
来源：http://hz.havefunace.top/gthjcdpsgu.html

split -l 1000 big.log part_
来源：http://hz.jinqigufen.top/gtgwnnfbyy.html

[R74] 批量重命名
来源：http://hz.sufxvd.cn/gtydyjzzte.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.jinyuanbaomall.cn/gtqgqhqwlh.html

[R75] 导出环境变量
来源：http://hz.sysykeji.top/gtxflnukzv.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.birdmap.top/gtkqfqgjgx.html

[R76] 使用临时文件
来源：http://hz.mhx1999.top/gtjcvmbjut.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.yuxming.cn/gtdsbpklss.html

[R77] 读取用户输入
来源：http://hz.daxiang520.top/gtofqnwrgd.html

read -rp "请输入: " ans
来源：http://hz.havefunace.top/gtmyfwobud.html

[R78] 交互式菜单
来源：http://hz.pycfn.com/gtesknklrg.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.gaohongyu789.top/gtdehqpejv.html

[R79] 解析命令行选项
来源：http://hz.smart0.xyz/gtkjbogjpw.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.daxiang520.top/gtwuxtlrtt.html

[R80] 查看脚本执行耗时
来源：http://hz.chenlongwang.top/gtibvefqwq.html

time ./run.sh
来源：http://hz.daria6918.cn/gttbulvljm.html

================================================================================
来源：http://hz.wangdashe.top/gtwemnnqyn.html

S. C / C++ 专题
来源：http://hz.cdnleiting.top/gtpvtsywki.html

================================================================================
来源：http://hz.chenlongwang.top/gtioaxukhz.html

[S01] C：Hello World
来源：http://hz.0kj1m.cn/gtcflvmsaz.html

#include <stdio.h>
来源：http://hz.jinqigfzy.top/gtzrxnsgrc.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.zhongyouzk.top/gttyjlfoqn.html

[S02] C：变量与格式化输出
来源：http://hz.jianghu66.top/gtvxcaqjoj.html

int a = 10; printf("%d\n", a);
来源：http://hz.xinyue.icu/gtiljqlfsb.html

[S03] C：读入整数
来源：http://hz.redwolf501.top/gtnhxtohfk.html

int x; scanf("%d", &x);
来源：http://hz.shzxlz.cn/gtuakbczew.html

[S04] C：字符串复制
来源：http://hz.redwolf501.top/gtneciancz.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.jqgfzy.top/gtutpsojce.html

[S05] C：字符串长度
来源：http://hz.meibo888.top/gtgfniajem.html

strlen(s)
来源：http://hz.yuxming.cn/gtyjrcvwpn.html

[S06] C：字符串比较
来源：http://hz.jinqigfzy.top/gtrbtujdvu.html

strcmp(a, b) == 0
来源：http://hz.sxryk.cn/gtaayjtisv.html

[S07] C：数组遍历求和
来源：http://hz.xuetiantiany.cn/gtxdveyhhv.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.pengpengdd.cyou/gtkkhyvpaj.html

[S08] C：动态内存分配与释放
来源：http://hz.sweek.top/gtzwldhqga.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.cucudq.cn/gtklekskta.html

[S09] C：结构体定义与初始化
来源：http://hz.xziqi.cn/gtkazfyrtl.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.cucudq.cn/gtgxdqqhbw.html

[S10] C：指针与解引用
来源：http://hz.andypj.xyz/gtnhquldby.html

int *p = &a;  *p = 5;
来源：http://hz.zhijiandao.cn/gttxgjoehl.html

[S11] C：逐行读文件
来源：http://hz.xinyue.icu/gtgcdvclqw.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.ppjwa.cn/gtuyxsganx.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.guannengcc.top/gtrohggmny.html

fclose(f);
来源：http://hz.feifeiyinyue.top/gtgojdpbji.html

[S12] C：写文件
来源：http://hz.pycfn.com/gtuafseamb.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.cqqwz.cn/gtjewzpdgo.html

[S13] C：宏定义
来源：http://hz.wangdashe.top/gtidxdfqsa.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.iojbl.cn/gtphfelhwp.html

[S14] C：枚举
来源：http://hz.sufxvd.cn/gtzdzdmfqc.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.fzhhl.top/gthfeoloox.html

[S15] C：类型转换
来源：http://hz.dianchejie.cn/gtzdtlqglr.html

(double) a / b
来源：http://hz.nanxinkj.top/gtjeyitzzl.html

[S16] C：位操作置位
来源：http://hz.quarkkingdee.top/gtzjhyddsp.html

x |= (1 << 3);
来源：http://hz.xylfe.cn/gtzdtjgjxk.html

[S17] C：安全拼接字符串
来源：http://hz.zhengqikj.top/gtauhpbbuw.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.jinyuanbaomall.cn/gtozfwcxrx.html

[S18] C：命令行参数
来源：http://hz.iojbl.cn/gtquezqlfm.html

int main(int argc, char **argv)
来源：http://hz.smart0.xyz/gtjladvxpi.html

[S19] C：快速排序
来源：http://hz.wangshuangyany.cn/gtglqurffw.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.shanyushiyangtech.top/gtfshbeohh.html

[S20] C：二分查找
来源：http://hz.yonumen.top/gttikejtvl.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.redwolf501.top/gtfecpadka.html

[S21] C：字符类别判断
来源：http://hz.aizwys.cn/gtmxbfhsst.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.havefunace.top/gtxavbcltj.html

[S22] C：字符串转数字
来源：http://hz.zhiwuduotai.top/gtjkgsgvis.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.cashguo.top/gtljqmuhwm.html

[S23] C：随机数
来源：http://hz.ivvv.top/gtywuzlndd.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.meibo888.top/gtxtlkuvoh.html

[S24] C：获取本地时间
来源：http://hz.birdmap.top/gthrtqwhug.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.hnxiangtu.top/gtuqsmclzh.html

[S25] C：内存拷贝
来源：http://hz.wangdashe.top/gtnxrbxymi.html

memcpy(dst, src, n);
来源：http://hz.yonumen.top/gtizggrorp.html

[S26] C：内存清零
来源：http://hz.quarkkingdee.top/gtdckzgkbe.html

memset(a, 0, sizeof a);
来源：http://hz.yanxiufei.cn/gtfhrzeewy.html

[S27] C：定义常量
来源：http://hz.yj202588.top/gtpvyyeety.html

const double PI = 3.14159;
来源：http://hz.meibo888.top/gtqsxoxkho.html

[S28] C：静态变量
来源：http://hz.shanyushiyangkeji.top/gtqaguciml.html

static int counter = 0;
来源：http://hz.guowangkeji.top/gtpuricdnm.html

[S29] C：变参函数
来源：http://hz.svipenyu.cn/gthcdwedec.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.gogol.net.cn/gtfveajgcc.html

[S30] C：头文件保护
来源：http://hz.zhengqikj.top/gtxndqhthv.html

#ifndef X_H
来源：http://hz.yj20258.top/gtvuvxzthd.html

#define X_H
来源：http://hz.jyoumei.cn/gtylmpcsvo.html

#endif
来源：http://hz.ybcxt.top/gtchacelxc.html

[S31] C++：Hello World
来源：http://hz.cdnleiting.top/gtfaekwyvw.html

#include <iostream>
来源：http://hz.xingfuxueyuan.xyz/gtkpveoacb.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.shuidangran.top/gtgyskiftt.html

[S32] C++：字符串
来源：http://hz.zhixingplan.top/gtsmjzdzfi.html

std::string s = "hi";  s += "!";
来源：http://hz.ywan-chungtsiang.top/gtnrkvsqvi.html

[S33] C++：vector 增删
来源：http://hz.ivvv.top/gtjrclkceq.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.chenlongwang.top/gtgstzlxcy.html

[S34] C++：遍历 vector
来源：http://hz.shanyushiyangtech.top/gtkenssldz.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.wangshuangyany.cn/gtotyctdty.html

[S35] C++：map
来源：http://hz.ybcxt.top/gtgqwchidv.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.hywenlv.cn/gtpzzxzdcy.html

[S36] C++：unordered_map
来源：http://hz.sxryk.cn/gtjmrdksjx.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.316326.xyz/gtlldrqxtr.html

[S37] C++：set
来源：http://hz.cheryme.top/gtloqacgvs.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.fengsongda.top/gtuuzbwsoq.html

[S38] C++：排序
来源：http://hz.yongpay.top/gtphpwlfvq.html

std::sort(v.begin(), v.end());
来源：http://hz.tianlin.xyz/gttgajrujb.html

[S39] C++：自定义比较器排序
来源：http://hz.jyoumei.cn/gtcrjjxdlz.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.jinqigfzy.top/gtcxrmvscd.html

[S40] C++：查找元素
来源：http://hz.fzhhl.top/gtwjdxwldk.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.jianghu66.top/gthzsandqa.html

[S41] C++：类与构造函数
来源：http://hz.zdqjudy.top/gtfescirpl.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.hysaishi.cn/gtsxfrmffo.html

[S42] C++：继承与虚函数
来源：http://hz.zhiwuduotai.top/gtupzjswqe.html

class B : public Base { public: void f() override {} };
来源：http://hz.yj20258888.top/gtojocfyem.html

[S43] C++：智能指针
来源：http://hz.xingfuxueyuan.xyz/gtzejucirn.html

auto p = std::make_unique<int>(5);
来源：http://hz.jqgufenzy.top/gtrgkdpmfl.html

[S44] C++：引用传参
来源：http://hz.cucudq.cn/gtamzhtyxy.html

void inc(int &x) { ++x; }
来源：http://hz.zhiwuduotai.top/gtrnferpky.html

[S45] C++：lambda
来源：http://hz.zhiwuduotai.top/gtnlumnoly.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.jinyuanbaomall.cn/gthtdkffqd.html

[S46] C++：函数模板
来源：http://hz.dianchejie.cn/gtnpqetgsw.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.shanyushiyangtech.top/gtjfilcuiz.html

[S47] C++：结构化绑定遍历
来源：http://hz.ydjk.org.cn/gtnfsqyubm.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.yanxiufei.cn/gtjtqowaiv.html

[S48] C++：逐行读文件
来源：http://hz.hnxiangtu.top/gtwpignski.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.gzhubu.top/gtfbkybcjj.html

while (std::getline(in, line)) { }
来源：http://hz.aizwys.cn/gtgpirkxyh.html

[S49] C++：写文件
来源：http://hz.jlsjyb.cn/gthkwnndla.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.shuidangran.top/gtftpmggfl.html

[S50] C++：格式化数字
来源：http://hz.shuidangran.top/gtgzkhhexm.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.hammf.cn/gtavxtdlak.html

[S51] C++：显式类型转换
来源：http://hz.guannengcc.top/gtzqsltuoc.html

static_cast<double>(a) / b
来源：http://hz.hammf.cn/gtqnhwsoiw.html

[S52] C++：const 与 noexcept
来源：http://hz.meibo888.top/gtzszglsch.html

int size() const noexcept { return n_; }
来源：http://hz.daxiang520.top/gtrnondurd.html

[S53] C++：移动语义
来源：http://hz.kuanghao11.cn/gtnkvldlfz.html

std::vector<int> w = std::move(v);
来源：http://hz.jqgfzy.top/gttgggdunl.html

[S54] C++：异常处理
来源：http://hz.yanxiufei.cn/gtcctxlamv.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.shanyushiyangkeji.top/gtpnvyomge.html

[S55] C++：结构化绑定
来源：http://hz.nanxuanxn.top/gtfdzxsmhj.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.ydzc1.top/gtmqjmbedo.html

[S56] C++：optional
来源：http://hz.birdmap.top/gtutlvxmkr.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.ehwqpu.com/gtyourshtf.html

[S57] C++：编译期常量
来源：http://hz.iojbl.cn/gtqjcatdvi.html

constexpr int N = 10;
来源：http://hz.ehwqpu.com/gtabwyhbop.html

[S58] C++：命名空间
来源：http://hz.yonumen.top/gtxyfsyewb.html

namespace ns { int f() { return 1; } }
来源：http://hz.guannengcc.top/gtxglpefbd.html

[S59] C++：静态断言
来源：http://hz.chenjidiqi.icu/gtdldehmeq.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.nanxuanxn.top/gtnlmptufr.html

[S60] C++：遍历并删除元素
来源：http://hz.jyoumei.cn/gtkvaesvkd.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.yanxiufei.cn/gtrtjxxykr.html

================================================================================
来源：http://hz.xziqi.cn/gttdlsbstu.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.xuanzx.com/gtqplevmnl.html

================================================================================
来源：http://hz.yangfankeji.com/gtksggvsgt.html

[T01] Kotlin：Hello World
来源：http://hz.yueranfly.top/gtnkgkdwse.html

println("Hello")
来源：http://hz.kuanghao11.cn/gttgcfdeec.html

[T02] Kotlin：变量
来源：http://hz.316326.xyz/gtejhwdlfq.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.yanxiufei.cn/gtrunurdum.html

[T03] Kotlin：字符串模板
来源：http://hz.nwbrower.top/gtpiedyxgs.html

"值: $b"
来源：http://hz.ppjwa.cn/gtqgdkvwmy.html

[T04] Kotlin：空安全
来源：http://hz.ydjk.org.cn/gtuhkeohma.html

val n: String? = null;  n?.length
来源：http://hz.ywan-chungtsiang.top/gtncjtmonr.html

[T05] Kotlin：when 表达式
来源：http://hz.meibo888.top/gteinmyrpf.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.pycfn.com/gtghboucmd.html

[T06] Kotlin：集合映射
来源：http://hz.nwbrower.top/gtiiacullq.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.yanxiufei.cn/gtiylcwpym.html

[T07] Kotlin：集合过滤
来源：http://hz.tanke756.top/gttdmjewzo.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.meibo888.top/gthdbcmbeh.html

[T08] Kotlin：数据类
来源：http://hz.jinqigfzy.top/gtzvngvznx.html

data class User(val name: String, val age: Int)
来源：http://hz.zhengqikj.top/gtvideuvbi.html

[T09] Kotlin：扩展函数
来源：http://hz.hnxiangtu.top/gtjhhwdxft.html

fun String.exclaim() = this + "!"
来源：http://hz.jqgfzy.top/gtqpbcvuxd.html

[T10] Kotlin：默认参数
来源：http://hz.zhijiandao.cn/gtpnzeuhsg.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.feifeiyinyue.top/gtsujonrgb.html

[T11] Kotlin：协程
来源：http://hz.mhx1999.top/gtgeonqsgu.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.jinqigufen.top/gtntorfbri.html

[T12] Kotlin：解构声明
来源：http://hz.vqdsnc.cn/gtghmpllax.html

val (a, b) = Pair(1, 2)
来源：http://hz.jinyuanbaomall.cn/gtczxmyjkl.html

[T13] Kotlin：只读 Map
来源：http://hz.kuanghao11.cn/gtjolyhpol.html

val m = mapOf("a" to 1)
来源：http://hz.tanke756.top/gtvunbretp.html

[T14] Kotlin：循环
来源：http://hz.yj20258.top/gtloouamjk.html

for (i in 1..10) println(i)
来源：http://hz.shuidangran.top/gtimbvshky.html

[T15] Kotlin：接口
来源：http://hz.jianghu66.top/gtxibkyibj.html

interface Shape { fun area(): Double }
来源：http://hz.yuanzhike.top/gtulsksibe.html

[T16] Swift：Hello World
来源：http://hz.9152youxi.cn/gtbmkurabe.html

print("Hello")
来源：http://hz.shanyushiyangkeji.top/gtgftooaob.html

[T17] Swift：变量与常量
来源：http://hz.0kj1m.cn/gtweeftvrb.html

var a = 1;  let b = 2
来源：http://hz.aizwys.cn/gtxyehicub.html

[T18] Swift：字符串插值
来源：http://hz.yuxming.cn/gtbemvkkvk.html

"值: \(b)"
来源：http://hz.mhx1999.top/gtcljtmtlz.html

[T19] Swift：可选绑定
来源：http://hz.xinyue.icu/gtwykiytcr.html

if let n = opt { print(n) }
来源：http://hz.zhiwuduotai.top/gtpbkmvyug.html

[T20] Swift：数组操作
来源：http://hz.yvedp.cn/gtadalstvf.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.shanyushiyangkeji.top/gtbwmsjfpv.html

[T21] Swift：遍历
来源：http://hz.jyoumei.cn/gteljamear.html

for x in a { print(x) }
来源：http://hz.zhoulong.xyz/gtabztpyqt.html

[T22] Swift：字典
来源：http://hz.zdqjudy.top/gtrnrbokku.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.aibaodan.cn/gtqyggxgla.html

[T23] Swift：函数
来源：http://hz.iojbl.cn/gtlvahaouq.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.redwolf501.top/gtzhwhtcdd.html

[T24] Swift：闭包
来源：http://hz.gotoacloud.top/gttwgllbtv.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.sysykeji.top/gtbrmbwnca.html

[T25] Swift：结构体
来源：http://hz.xuetiantiany.cn/gtutfhnpwj.html

struct P { var x: Int }
来源：http://hz.zhongyouzk.top/gtcpuxlikr.html

[T26] Swift：类与重写
来源：http://hz.ppjwa.cn/gtaqyolzbv.html

class A: Base { override func f() {} }
来源：http://hz.yanxiufei.cn/gtdpfswnpg.html

[T27] Swift：错误处理
来源：http://hz.52xcode.cn/gtgemciddv.html

do { try f() } catch { print(error) }
来源：http://hz.jqgfzy.top/gttryokirc.html

[T28] Swift：枚举
来源：http://hz.vqdsnc.cn/gtzugwanis.html

enum Color { case red, green }
来源：http://hz.fzhhl.top/gteshvtouy.html

[T29] Swift：guard 提前返回
来源：http://hz.xziqi.cn/gtrhjvlleq.html

guard let x = opt else { return }
来源：http://hz.dianchejie.cn/gtwxrmljat.html

[T30] Swift：协议
来源：http://hz.hammf.cn/gtysidlxki.html

protocol Shape { func area() -> Double }
来源：http://hz.sweek.top/gtioibcnsk.html

[T31] Lua：Hello World
来源：http://hz.hnqzz.top/gteytkrqwa.html

print("Hello")
来源：http://hz.jinqigufen.top/gtgsgjcxxh.html

[T32] Lua：局部变量
来源：http://hz.hnqzz.top/gtfavjrkpf.html

local a = 1
来源：http://hz.meibo888.top/gtkpvvwrcp.html

[T33] Lua：表（数组）
来源：http://hz.gzhubu.top/gtblszihpg.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.ybcxt.top/gtsbtrzshp.html

[T34] Lua：遍历表
来源：http://hz.shangyingyoupin.top/gtamevnqfd.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.sufxvd.cn/gtlchljdxi.html

[T35] Lua：字典表
来源：http://hz.jqgfzy.top/gtpsvvawpx.html

local d = { a = 1 };  d.b = 2
来源：http://hz.ywan-chungtsiang.top/gttubzskwm.html

[T36] Lua：函数
来源：http://hz.cheryme.top/gteernkocf.html

function add(a, b) return a + b end
来源：http://hz.xziqi.cn/gturynwzvo.html

[T37] Lua：字符串拼接
来源：http://hz.gaohongyu789.top/gtykgrvpkn.html

"a" .. "b"
来源：http://hz.yj202588.top/gtrrzanvxr.html

[T38] Lua：条件
来源：http://hz.jqgufenzy.top/gtscenghkk.html

if x > 0 then print("正") end
来源：http://hz.cheryme.top/gtqqurwkor.html

[T39] Lua：模式匹配
来源：http://hz.andypj.xyz/gthkbqmtqv.html

string.find(s, "%d+")
来源：http://hz.xinyue.icu/gtexwkptng.html

[T40] Lua：元表
来源：http://hz.gotoacloud.top/gtjinhaaxt.html

setmetatable({}, { __index = base })
来源：http://hz.haohaochexian.top/gtucrbihzz.html

[T41] Perl：Hello World
来源：http://hz.xuanzx.com/gtgdonnzbe.html

print "Hello\n";
来源：http://hz.sxryk.cn/gtumznqvvh.html

[T42] Perl：变量类型
来源：http://hz.fzhhl.top/gtqjdewria.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.iojbl.cn/gtmcqvnqwb.html

[T43] Perl：字符串插值
来源：http://hz.zycfv.cn/gtbrlahrwi.html

"值: $a"
来源：http://hz.ydjk.org.cn/gtgbatwubw.html

[T44] Perl：条件
来源：http://hz.daxiang520.top/gtajbkrsdz.html

if ($a > 0) { print "正"; }
来源：http://hz.snrcjt.cn/gtwxnppsfb.html

[T45] Perl：数组遍历
来源：http://hz.nanxuanxn.top/gtoeoguyqz.html

for my $x (@arr) { print $x; }
来源：http://hz.zhaomingkeji.xyz/gtmoswbhov.html

[T46] Perl：哈希操作
来源：http://hz.hysaishi.cn/gtwnvwmgra.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.pycfn.com/gthvtusqyx.html

[T47] Perl：正则捕获
来源：http://hz.yongpay.top/gtdgqbounn.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.ybcxt.top/gtzuaquziu.html

[T48] Perl：正则替换
来源：http://hz.meibo888.top/gttppmizbt.html

$s =~ s/old/new/g;
来源：http://hz.andypj.xyz/gteixgkcuz.html


<!-- 参考信息 -->