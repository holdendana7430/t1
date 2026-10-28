代发 wailian999

find . -name "*.tmp" -delete
来源：http://hz.guowangkeji.top/gtdhyxwkxy.html

[R46] 递归替换文件内容
来源：http://hz.havefunace.top/gtufhqhnuo.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.yangfankeji.com/gtcwndgyuc.html

[R47] sed 单行替换
来源：http://hz.shanyushiyangkeji.top/gtsasavhrp.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.jinyuanbaomall.cn/gtsdtmarin.html

[R48] awk 取指定列
来源：http://hz.cucudq.cn/gtbjpisiqz.html

awk '{print $1, $3}' a.txt
来源：http://hz.pengpengdd.cyou/gtvrencoze.html

[R49] awk 带条件
来源：http://hz.shangyingyoupin.top/gtkmlqojez.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.yonumen.top/gtsmetrhfx.html

[R50] awk 求和
来源：http://hz.cdnleiting.top/gtpmefgfsg.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.zhongyouzk.top/gtiwsshbdk.html

[R51] 排序去重取前几
来源：http://hz.shuidangran.top/gthisaukrn.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.guowangkeji.top/gtjfoovtbl.html

[R52] 统计行数
来源：http://hz.yanxiufei.cn/gtswebpsfh.html

wc -l a.txt
来源：http://hz.fzhhl.top/gtrnbwdqmu.html

[R53] 查看文件头与实时尾
来源：http://hz.hongshengwenyu.top/gtazrnxynn.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.sxryk.cn/gtmzfsdfmx.html

[R54] 比较两个文件
来源：http://hz.shuidangran.top/gtuyadaejq.html

diff a.txt b.txt
来源：http://hz.jqgufenzy.top/gtanrxhtjy.html

[R55] 压缩与解压
来源：http://hz.zhoulong.xyz/gtslwgmbrq.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.sweek.top/gtrvnxwfxk.html

[R56] 远程拷贝
来源：http://hz.yanxiufei.cn/gtduvhywlc.html

scp file user@host:/path/
来源：http://hz.zhaomingkeji.xyz/gtshgoejxn.html

[R57] 远程执行命令
来源：http://hz.jlsjyb.cn/gthipnivwv.html

ssh user@host 'uptime'
来源：http://hz.gotoacloud.top/gtynrlrexp.html

[R58] 下载文件
来源：http://hz.xylfe.cn/gtfgrregcm.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.vqdsnc.cn/gtkhathujn.html

[R59] 发 POST JSON
来源：http://hz.xinyue.icu/gtqfqikbmq.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.chenzaomai.com/gtrbvmjouf.html

[R60] 只看 HTTP 状态码
来源：http://hz.shuidangran.top/gtuwhytulr.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.zycfv.cn/gtwgejlafr.html

[R61] 磁盘占用
来源：http://hz.hammf.cn/gtzwlfxfwv.html

df -h;  du -sh *
来源：http://hz.zdqjudy.top/gteznynqqg.html

[R62] 找最占空间的文件
来源：http://hz.cqqwz.cn/gtnemyqyfd.html

du -ah . | sort -rh | head -10
来源：http://hz.gaohongyu789.top/gtgoeqmmvc.html

[R63] 内存与进程
来源：http://hz.xylfe.cn/gtmnohzqci.html

free -h;  ps aux | grep nginx
来源：http://hz.jinqigufen.top/gtzowdnwgk.html

[R64] 结束进程
来源：http://hz.yonumen.top/gtmjzxxqeb.html

kill -9 $(pgrep -f app.py)
来源：http://hz.cashguo.top/gtujdexzlc.html

[R65] 查看端口占用
来源：http://hz.jyoumei.cn/gttivwtjhy.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.yuanzhike.top/gtekicpjhh.html

[R66] 定时任务
来源：http://hz.feifeiyinyue.top/gtmeiubvkc.html

crontab -e;  crontab -l
来源：http://hz.sxryk.cn/gtcbrerswe.html

[R67] 生成随机十六进制串
来源：http://hz.ydzc1.top/gtslfdpgok.html

openssl rand -hex 16
来源：http://hz.jinghuilouyu.cn/gtsckxbddj.html

[R68] 计算文件校验值
来源：http://hz.aibaodan.cn/gtslpvykwn.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.ybcxt.top/gtbexipzxj.html

[R69] 生成随机密码
来源：http://hz.yuxming.cn/gttxgovnzg.html

head -c 16 /dev/urandom | base64
来源：http://hz.cdnleiting.top/gtjexarqtr.html

[R70] 时间戳与互转
来源：http://hz.cqqwz.cn/gtfrsqbvfw.html

date +%s;  date -d @1700000000
来源：http://hz.xuetiantiany.cn/gtwlbqztkx.html

[R71] 日期格式化
来源：http://hz.vqdsnc.cn/gthpserzgk.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.gotoacloud.top/gtskkqqeiu.html

[R72] 等待端口就绪
来源：http://hz.dianchejie.cn/gtzzkrfwvu.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.yonumen.top/gtyrgbwarr.html

[R73] 分割大日志
来源：http://hz.ivvv.top/gtxdkqzdxp.html

split -l 1000 big.log part_
来源：http://hz.wangshuangyany.cn/gtbvmpdotn.html

[R74] 批量重命名
来源：http://hz.xylfe.cn/gtmtmjysdn.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.wangdashe.top/gtvalpkqlz.html

[R75] 导出环境变量
来源：http://hz.bjfxy.top/gtslklrucy.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.cucudq.cn/gtjoboiyaj.html

[R76] 使用临时文件
来源：http://hz.bjfxy.top/gtyktjzldq.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.chenjidiqi.icu/gtliwawhgk.html

[R77] 读取用户输入
来源：http://hz.fengsongda.top/gtnobirkzc.html

read -rp "请输入: " ans
来源：http://hz.bjfxy.top/gtyhtzxqdy.html

[R78] 交互式菜单
来源：http://hz.zhongyouzk.top/gtjcpehsiz.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.tanke756.top/gtevqzptfb.html

[R79] 解析命令行选项
来源：http://hz.zhixingplan.top/gtsnvuafss.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.shzxlz.cn/gtsevpugqr.html

[R80] 查看脚本执行耗时
来源：http://hz.nanxinkj.top/gtouujgxyo.html

time ./run.sh
来源：http://hz.yangfankeji.com/gtyszbrtto.html

================================================================================
来源：http://hz.zhoulong.xyz/gtgngmctpk.html

S. C / C++ 专题
来源：http://hz.daxiang520.top/gtsqysrgpa.html

================================================================================
来源：http://hz.chenlongwang.top/gtrnxslxqf.html

[S01] C：Hello World
来源：http://hz.yueranfly.top/gtoszggeya.html

#include <stdio.h>
来源：http://hz.hnqzz.top/gtpweimcrp.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.wangdashe.top/gtkmgskspl.html

[S02] C：变量与格式化输出
来源：http://hz.sxryk.cn/gtrvdvntqq.html

int a = 10; printf("%d\n", a);
来源：http://hz.gogol.net.cn/gtfvfuhlgs.html

[S03] C：读入整数
来源：http://hz.zhijiandao.cn/gtemmgddpm.html

int x; scanf("%d", &x);
来源：http://hz.9152youxi.cn/gtqbprxnrk.html

[S04] C：字符串复制
来源：http://hz.feifeiyinyue.top/gtjutdzydy.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.sysykeji.top/gtjvtubozk.html

[S05] C：字符串长度
来源：http://hz.zhoulong.xyz/gttaxjqkzo.html

strlen(s)
来源：http://hz.redwolf501.top/gtckjuitcr.html

[S06] C：字符串比较
来源：http://hz.yongpay.top/gtkrvitexu.html

strcmp(a, b) == 0
来源：http://hz.ehwqpu.com/gtrbcltdwy.html

[S07] C：数组遍历求和
来源：http://hz.yanxiufei.cn/gtucqeitlr.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.dianchejie.cn/gtrhvfcqrt.html

[S08] C：动态内存分配与释放
来源：http://hz.sxryk.cn/gtliziakwy.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.aibaodan.cn/gtkkbvmzyk.html

[S09] C：结构体定义与初始化
来源：http://hz.sufxvd.cn/gtdwrcxdjn.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.0kj1m.cn/gtqatbmpuq.html

[S10] C：指针与解引用
来源：http://hz.birdmap.top/gtlpiqzvup.html

int *p = &a;  *p = 5;
来源：http://hz.jianghu66.top/gtmrducrbr.html

[S11] C：逐行读文件
来源：http://hz.dashuyun.cn/gtzmrekcov.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.daria6918.cn/gtluqsgesa.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.jlsjyb.cn/gthgypflvv.html

fclose(f);
来源：http://hz.nanxinkj.top/gtotsislyn.html

[S12] C：写文件
来源：http://hz.xziqi.cn/gtjjwafkuj.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.ydzc1.top/gtpikaqtjk.html

[S13] C：宏定义
来源：http://hz.vqdsnc.cn/gtolsapcbs.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.pengpengdd.cyou/gtpcpztinm.html

[S14] C：枚举
来源：http://hz.ybcxt.top/gtbskkcjkh.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.kuanghao11.cn/gtuotihndh.html

[S15] C：类型转换
来源：http://hz.kuanghao11.cn/gtsehkwpjp.html

(double) a / b
来源：http://hz.zhengqikj.top/gtvlgnkymi.html

[S16] C：位操作置位
来源：http://hz.sysykeji.top/gtarncdqvs.html

x |= (1 << 3);
来源：http://hz.yangfankeji.com/gtdoxszdlo.html

[S17] C：安全拼接字符串
来源：http://hz.zhixingplan.top/gtgwirnber.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.xinyue.icu/gtdjedzcaq.html

[S18] C：命令行参数
来源：http://hz.fengsongda.top/gtvberxecr.html

int main(int argc, char **argv)
来源：http://hz.cqqwz.cn/gtsytmrgmp.html

[S19] C：快速排序
来源：http://hz.sysykeji.top/gtfyviawgv.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.jiagoushi.top/gtszhhrate.html

[S20] C：二分查找
来源：http://hz.smart0.xyz/gtcavomczl.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.yuxming.cn/gtdkrxwbvs.html

[S21] C：字符类别判断
来源：http://hz.havefunace.top/gtufwdqwzx.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.hammf.cn/gtrrfozvnh.html

[S22] C：字符串转数字
来源：http://hz.ppjwa.cn/gtxtkdgetu.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.mhx1999.top/gtqzttlnnk.html

[S23] C：随机数
来源：http://hz.aibaodan.cn/gtczpwsajs.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.shanyushiyangtech.top/gtbxwiisjl.html

[S24] C：获取本地时间
来源：http://hz.shzxlz.cn/gtvxzkkoju.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.hfpthk.cn/gtxyfdeoql.html

[S25] C：内存拷贝
来源：http://hz.pycfn.com/gtngcszhca.html

memcpy(dst, src, n);
来源：http://hz.yuanzhike.top/gtnnjnzcwn.html

[S26] C：内存清零
来源：http://hz.guowangkeji.top/gtrhirzyao.html

memset(a, 0, sizeof a);
来源：http://hz.kuanghao11.cn/gtbplqqhlc.html

[S27] C：定义常量
来源：http://hz.yj20258888.top/gtecmievul.html

const double PI = 3.14159;
来源：http://hz.tianlin.xyz/gtdfpjzztp.html

[S28] C：静态变量
来源：http://hz.ydzc1.top/gtseymycko.html

static int counter = 0;
来源：http://hz.xinyue.icu/gtbooichjd.html

[S29] C：变参函数
来源：http://hz.hnqzz.top/gtemcsnoca.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.zhijiandao.cn/gtxeztuued.html

[S30] C：头文件保护
来源：http://hz.0kj1m.cn/gtfqbspcry.html

#ifndef X_H
来源：http://hz.zhixingplan.top/gtubiffedn.html

#define X_H
来源：http://hz.ppjwa.cn/gtbxodfapt.html

#endif
来源：http://hz.chenjidiqi.icu/gtwkdbnxmm.html

[S31] C++：Hello World
来源：http://hz.hnqzz.top/gtrpyxkdwa.html

#include <iostream>
来源：http://hz.shanyushiyangtech.top/gtaewlxgqx.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.yangfankeji.com/gtpbczszkk.html

[S32] C++：字符串
来源：http://hz.jqgfzy.top/gtjoszfvcs.html

std::string s = "hi";  s += "!";
来源：http://hz.dianchejie.cn/gtxyvjxlju.html

[S33] C++：vector 增删
来源：http://hz.ywan-chungtsiang.top/gthmmwlxpt.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.mhx1999.top/gtnlwdfdyt.html

[S34] C++：遍历 vector
来源：http://hz.zhoulong.xyz/gtxfhcxsss.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.hnxiangtu.top/gtojebrqoz.html

[S35] C++：map
来源：http://hz.yongpay.top/gtwnqbpmuw.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.cheryme.top/gtaljxxqum.html

[S36] C++：unordered_map
来源：http://hz.cdnleiting.top/gttdxjeiqq.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.pengpengdd.cyou/gthgwefekx.html

[S37] C++：set
来源：http://hz.nwbrower.top/gtmbbwhatk.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.quarkkingdee.top/gtcxwoertp.html

[S38] C++：排序
来源：http://hz.yueranfly.top/gtscfmvsnm.html

std::sort(v.begin(), v.end());
来源：http://hz.jlsjyb.cn/gtisjagdvn.html

[S39] C++：自定义比较器排序
来源：http://hz.hysaishi.cn/gtaalyyehy.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.wangshuangyany.cn/gthanueiwm.html

[S40] C++：查找元素
来源：http://hz.guowangkeji.top/gtnusvyfnj.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.haohaochexian.top/gtycqtmdsg.html

[S41] C++：类与构造函数
来源：http://hz.yj202588.top/gtwgeewnjv.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.sysykeji.top/gtfejfwyqx.html

[S42] C++：继承与虚函数
来源：http://hz.gogol.net.cn/gtfimauiyd.html

class B : public Base { public: void f() override {} };
来源：http://hz.gzhubu.top/gtvsyggfkr.html

[S43] C++：智能指针
来源：http://hz.jyoumei.cn/gtieeoiddk.html

auto p = std::make_unique<int>(5);
来源：http://hz.sufxvd.cn/gtootwqvxq.html

[S44] C++：引用传参
来源：http://hz.ydzc1.top/gthkjatgkl.html

void inc(int &x) { ++x; }
来源：http://hz.shuidangran.top/gtsbzoccai.html

[S45] C++：lambda
来源：http://hz.zhoulong.xyz/gtuzhziwip.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.ehwqpu.com/gtqzmsajtb.html

[S46] C++：函数模板
来源：http://hz.haohaochexian.top/gtjpoxzuji.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.jlsjyb.cn/gtcuvstvfh.html

[S47] C++：结构化绑定遍历
来源：http://hz.haohaochexian.top/gtyjybifif.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.mhx1999.top/gtrxdxxloj.html

[S48] C++：逐行读文件
来源：http://hz.dianchejie.cn/gtalumxvyx.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.snrcjt.cn/gtnxmahrhw.html

while (std::getline(in, line)) { }
来源：http://hz.tanke756.top/gtkiwegdar.html

[S49] C++：写文件
来源：http://hz.shuidangran.top/gtnyftfmzt.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.zhijiandao.cn/gtyshyplyp.html

[S50] C++：格式化数字
来源：http://hz.havefunace.top/gtsduvmwxd.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.yuxming.cn/gttnnczsuq.html

[S51] C++：显式类型转换
来源：http://hz.hammf.cn/gtvvuaimyq.html

static_cast<double>(a) / b
来源：http://hz.yanxiufei.cn/gtdbbfazij.html

[S52] C++：const 与 noexcept
来源：http://hz.0kj1m.cn/gtmpykxawp.html

int size() const noexcept { return n_; }
来源：http://hz.xylfe.cn/gtwikshqzo.html

[S53] C++：移动语义
来源：http://hz.daria6918.cn/gtvysjadas.html

std::vector<int> w = std::move(v);
来源：http://hz.andypj.xyz/gtogvebmwl.html

[S54] C++：异常处理
来源：http://hz.birdmap.top/gtcgkyudti.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.hywenlv.cn/gtejflnihl.html

[S55] C++：结构化绑定
来源：http://hz.jlsjyb.cn/gtalvaaatd.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.jqgfzy.top/gtrspfwkto.html

[S56] C++：optional
来源：http://hz.yongpay.top/gtdnhjiyfk.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.316326.xyz/gtishpeqyx.html

[S57] C++：编译期常量
来源：http://hz.ehwqpu.com/gtrqwbixxj.html

constexpr int N = 10;
来源：http://hz.cqqwz.cn/gtwmsjgytf.html

[S58] C++：命名空间
来源：http://hz.yongpay.top/gteqfroxyq.html

namespace ns { int f() { return 1; } }
来源：http://hz.xuanzx.com/gtqpjxzrhl.html

[S59] C++：静态断言
来源：http://hz.wangdashe.top/gtoxysdalj.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.pycfn.com/gtzchftdvb.html

[S60] C++：遍历并删除元素
来源：http://hz.yongpay.top/gtlosixecv.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.snrcjt.cn/gtpfgzujpm.html

================================================================================
来源：http://hz.ybcxt.top/gtfshpcfam.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.tanke756.top/gtprwdtdtv.html

================================================================================
来源：http://hz.52xcode.cn/gthepctaie.html

[T01] Kotlin：Hello World
来源：http://hz.cdnleiting.top/gtvqpnvpug.html

println("Hello")
来源：http://hz.snrcjt.cn/gtnmsghssp.html

[T02] Kotlin：变量
来源：http://hz.gaohongyu789.top/gtwdzskisd.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.tanke756.top/gtsokdqkfj.html

[T03] Kotlin：字符串模板
来源：http://hz.cucudq.cn/gtfhlrukzo.html

"值: $b"
来源：http://hz.iojbl.cn/gtwrpkamnj.html

[T04] Kotlin：空安全
来源：http://hz.guowangkeji.top/gtoqjkaoji.html

val n: String? = null;  n?.length
来源：http://hz.cashguo.top/gthgkpeyva.html

[T05] Kotlin：when 表达式
来源：http://hz.xinyue.icu/gtoxnaqhib.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.xuanzx.com/gtjbhmrldx.html

[T06] Kotlin：集合映射
来源：http://hz.svipenyu.cn/gtvfgrtnzd.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.andypj.xyz/gtbhtrsphk.html

[T07] Kotlin：集合过滤
来源：http://hz.jqgfzy.top/gtsyunqish.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.hongshengwenyu.top/gtjnlkgdxr.html

[T08] Kotlin：数据类
来源：http://hz.nwbrower.top/gtlyvkxjbf.html

data class User(val name: String, val age: Int)
来源：http://hz.yuanzhike.top/gtoxdwzowq.html

[T09] Kotlin：扩展函数
来源：http://hz.hnxiangtu.top/gtjjtzuctx.html

fun String.exclaim() = this + "!"
来源：http://hz.jiagoushi.top/gtvwxuilfw.html

[T10] Kotlin：默认参数
来源：http://hz.bjfxy.top/gthhiobvqw.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.gotoacloud.top/gtgxytkonr.html

[T11] Kotlin：协程
来源：http://hz.wangdashe.top/gtnvjopuwd.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.guannengcc.top/gtvnhznfex.html

[T12] Kotlin：解构声明
来源：http://hz.shanyushiyangtech.top/gtqzxhxvvt.html

val (a, b) = Pair(1, 2)
来源：http://hz.dashuyun.cn/gtyvxbonsu.html

[T13] Kotlin：只读 Map
来源：http://hz.yuxming.cn/gtakzosyry.html

val m = mapOf("a" to 1)
来源：http://hz.fengsongda.top/gtnsqgjnae.html

[T14] Kotlin：循环
来源：http://hz.hfpthk.cn/gtltbeyvge.html

for (i in 1..10) println(i)
来源：http://hz.cdnleiting.top/gtubpejhxe.html

[T15] Kotlin：接口
来源：http://hz.gzhubu.top/gtibfdxrmj.html

interface Shape { fun area(): Double }
来源：http://hz.nwbrower.top/gtwimwkjoq.html

[T16] Swift：Hello World
来源：http://hz.0kj1m.cn/gtdiyhfhkh.html

print("Hello")
来源：http://hz.xingfuxueyuan.xyz/gtkxhsyrtn.html

[T17] Swift：变量与常量
来源：http://hz.sufxvd.cn/gthdfrxguu.html

var a = 1;  let b = 2
来源：http://hz.wangshuangyany.cn/gtknhjbhsl.html

[T18] Swift：字符串插值
来源：http://hz.andypj.xyz/gtupxltzve.html

"值: \(b)"
来源：http://hz.daria6918.cn/gtiuynpxme.html

[T19] Swift：可选绑定
来源：http://hz.xziqi.cn/gtgoxmqerp.html

if let n = opt { print(n) }
来源：http://hz.316326.xyz/gtyeddtequ.html

[T20] Swift：数组操作
来源：http://hz.cdnleiting.top/gtjvlrntto.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.tian-w.cn/gtknscrseh.html

[T21] Swift：遍历
来源：http://hz.zhijiandao.cn/gtduhjkqvx.html

for x in a { print(x) }
来源：http://hz.9152youxi.cn/gtcqxmbqre.html

[T22] Swift：字典
来源：http://hz.feifeiyinyue.top/gtmniupysz.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.hammf.cn/gtfalhugit.html

[T23] Swift：函数
来源：http://hz.ehwqpu.com/gtcwxbtxdv.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.hysaishi.cn/gttegwntrf.html

[T24] Swift：闭包
来源：http://hz.jinghuilouyu.cn/gtkfhmmkgh.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.yanxiufei.cn/gtdncosltk.html

[T25] Swift：结构体
来源：http://hz.guannengcc.top/gtfavmygku.html

struct P { var x: Int }
来源：http://hz.sxryk.cn/gtjdvivnzk.html

[T26] Swift：类与重写
来源：http://hz.cqqwz.cn/gtymkmbxxm.html

class A: Base { override func f() {} }
来源：http://hz.wangdashe.top/gtrclrlzpi.html

[T27] Swift：错误处理
来源：http://hz.tanke756.top/gtahrhfkzp.html

do { try f() } catch { print(error) }
来源：http://hz.xuanzx.com/gtwboyimwg.html

[T28] Swift：枚举
来源：http://hz.jqgufenzy.top/gtbbwjgsty.html

enum Color { case red, green }
来源：http://hz.gogol.net.cn/gtntjxpzur.html

[T29] Swift：guard 提前返回
来源：http://hz.sysykeji.top/gtghevhzzg.html

guard let x = opt else { return }
来源：http://hz.c1oappe.top/gtlwxmgeex.html

[T30] Swift：协议
来源：http://hz.wangshuangyany.cn/gtykbrbcnl.html

protocol Shape { func area() -> Double }
来源：http://hz.meibo888.top/gtmhnvcafb.html

[T31] Lua：Hello World
来源：http://hz.yuxming.cn/gteznnjlbf.html

print("Hello")
来源：http://hz.quarkkingdee.top/gtjuuopepp.html

[T32] Lua：局部变量
来源：http://hz.yanxiufei.cn/gthcxqptaq.html

local a = 1
来源：http://hz.c1oappe.top/gtlaxrkdrn.html

[T33] Lua：表（数组）
来源：http://hz.jyoumei.cn/gtqsafkdwc.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.yanxiufei.cn/gtiwnahybh.html

[T34] Lua：遍历表
来源：http://hz.hysaishi.cn/gttfebqijq.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.xingfuxueyuan.xyz/gtjbqubqqb.html

[T35] Lua：字典表
来源：http://hz.sysykeji.top/gtblstrtig.html

local d = { a = 1 };  d.b = 2
来源：http://hz.jianghu66.top/gtwgippphk.html

[T36] Lua：函数
来源：http://hz.guowangkeji.top/gtqmggvple.html

function add(a, b) return a + b end
来源：http://hz.guowangkeji.top/gtwlcnpgwg.html

[T37] Lua：字符串拼接
来源：http://hz.fengsongda.top/gtihwvcjah.html

"a" .. "b"
来源：http://hz.316326.xyz/gtyyqmfohk.html

[T38] Lua：条件
来源：http://hz.hnxiangtu.top/gtpgpjsusq.html

if x > 0 then print("正") end
来源：http://hz.ivvv.top/gtxabzqibk.html

[T39] Lua：模式匹配
来源：http://hz.yanxiufei.cn/gtlqkwrabu.html

string.find(s, "%d+")
来源：http://hz.zhoulong.xyz/gtuqctmocs.html

[T40] Lua：元表
来源：http://hz.yj202588.top/gtynuucftr.html

setmetatable({}, { __index = base })
来源：http://hz.mhx1999.top/gtocdtspur.html

[T41] Perl：Hello World
来源：http://hz.sxryk.cn/gttuggakxz.html

print "Hello\n";
来源：http://hz.jiagoushi.top/gtsbxmbdux.html

[T42] Perl：变量类型
来源：http://hz.havefunace.top/gtjadqxrsv.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.zhixingplan.top/gtjglvkfkm.html

[T43] Perl：字符串插值
来源：http://hz.nanxinkj.top/gtrkvqgnyh.html

"值: $a"
来源：http://hz.zycfv.cn/gtwnfuhbad.html

[T44] Perl：条件
来源：http://hz.jqgfzy.top/gtmbxyyjgl.html

if ($a > 0) { print "正"; }
来源：http://hz.dashuyun.cn/gtluqsmuzl.html

[T45] Perl：数组遍历
来源：http://hz.tian-w.cn/gtnqxmcvyp.html

for my $x (@arr) { print $x; }
来源：http://hz.jinqigfzy.top/gtppfsjvxw.html

[T46] Perl：哈希操作
来源：http://hz.jlsjyb.cn/gtprjnhlrg.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.zhixingplan.top/gtqlclxgpy.html

[T47] Perl：正则捕获
来源：http://hz.zhixingplan.top/gtuxbvvxys.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.meibo888.top/gtsojriqqr.html

[T48] Perl：正则替换
来源：http://hz.yueranfly.top/gtcjncotdk.html

$s =~ s/old/new/g;
来源：http://hz.gogol.net.cn/gttcggcait.html


<!-- 参考信息 -->