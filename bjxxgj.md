代发 wailian999

find . -name "*.log" -type f
来源：http://hz.smart0.xyz/gtivnyccyq.html

[R44] 按修改时间查找
来源：http://hz.shangyingyoupin.top/gtfyglmfzn.html

find . -mtime -7 -type f
来源：http://hz.wangshuangyany.cn/gtrtnymtcm.html

[R45] 批量删除
来源：http://hz.jinqigufen.top/gthgykwooj.html

find . -name "*.tmp" -delete
来源：http://hz.zhongyouzk.top/gtbievnanr.html

[R46] 递归替换文件内容
来源：http://hz.havefunace.top/gttckkdipk.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.quarkkingdee.top/gtlqxwchdx.html

[R47] sed 单行替换
来源：http://hz.yangfankeji.com/gtroemvdre.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.fzhhl.top/gtifezaxdy.html

[R48] awk 取指定列
来源：http://hz.ydjk.org.cn/gttuqgsnro.html

awk '{print $1, $3}' a.txt
来源：http://hz.yongpay.top/gtpootiybf.html

[R49] awk 带条件
来源：http://hz.fzhhl.top/gtfjapfqcy.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.zdqjudy.top/gtpbrqqtgp.html

[R50] awk 求和
来源：http://hz.ybcxt.top/gtfsrziitb.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.hnqzz.top/gtexvmxcrb.html

[R51] 排序去重取前几
来源：http://hz.zhengqikj.top/gtzzxuofis.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.hammf.cn/gtlmczsggh.html

[R52] 统计行数
来源：http://hz.shuidangran.top/gtvhyyvywt.html

wc -l a.txt
来源：http://hz.jiagoushi.top/gtrjufcczn.html

[R53] 查看文件头与实时尾
来源：http://hz.jqgfzy.top/gtpvkkojzt.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.birdmap.top/gtxvjzavjq.html

[R54] 比较两个文件
来源：http://hz.snrcjt.cn/gtmrlrfync.html

diff a.txt b.txt
来源：http://hz.ybcxt.top/gtgmldcxds.html

[R55] 压缩与解压
来源：http://hz.zhijiandao.cn/gtmzjbjlzk.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.jlsjyb.cn/gtstnqncyk.html

[R56] 远程拷贝
来源：http://hz.vqdsnc.cn/gtfgddlisp.html

scp file user@host:/path/
来源：http://hz.zhaomingkeji.xyz/gtinizwqoq.html

[R57] 远程执行命令
来源：http://hz.hywenlv.cn/gtldozjhev.html

ssh user@host 'uptime'
来源：http://hz.wangdashe.top/gtfvvevlvw.html

[R58] 下载文件
来源：http://hz.svipenyu.cn/gtqnlrxjev.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.hywenlv.cn/gthzkvrtrg.html

[R59] 发 POST JSON
来源：http://hz.mhx1999.top/gtfoatvyla.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.ybcxt.top/gtdssiojpa.html

[R60] 只看 HTTP 状态码
来源：http://hz.andypj.xyz/gtdekxjjzv.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.fzhhl.top/gtcwticlbu.html

[R61] 磁盘占用
来源：http://hz.vqdsnc.cn/gtqypzgbmd.html

df -h;  du -sh *
来源：http://hz.chenjidiqi.icu/gtlafbctzn.html

[R62] 找最占空间的文件
来源：http://hz.guowangkeji.top/gtdmvienxo.html

du -ah . | sort -rh | head -10
来源：http://hz.yuxming.cn/gtvyysdkha.html

[R63] 内存与进程
来源：http://hz.ydzc1.top/gtfzexdgti.html

free -h;  ps aux | grep nginx
来源：http://hz.snrcjt.cn/gthulzlmck.html

[R64] 结束进程
来源：http://hz.jinqigufen.top/gtzunedhrf.html

kill -9 $(pgrep -f app.py)
来源：http://hz.jianghu66.top/gtysembaxj.html

[R65] 查看端口占用
来源：http://hz.yuanzhike.top/gtzvrcxmtk.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.guannengcc.top/gtqclipprz.html

[R66] 定时任务
来源：http://hz.shuidangran.top/gthlrumpod.html

crontab -e;  crontab -l
来源：http://hz.vqdsnc.cn/gtcqmbcthz.html

[R67] 生成随机十六进制串
来源：http://hz.shuidangran.top/gtgzkilluy.html

openssl rand -hex 16
来源：http://hz.0kj1m.cn/gtylugxhcp.html

[R68] 计算文件校验值
来源：http://hz.jlsjyb.cn/gtqjrujlis.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.ivvv.top/gtydgjgowz.html

[R69] 生成随机密码
来源：http://hz.birdmap.top/gtvoeyxrlu.html

head -c 16 /dev/urandom | base64
来源：http://hz.fengsongda.top/gtlswkwwvk.html

[R70] 时间戳与互转
来源：http://hz.zycfv.cn/gtacpbhjva.html

date +%s;  date -d @1700000000
来源：http://hz.yueranfly.top/gtzgvjeczo.html

[R71] 日期格式化
来源：http://hz.cashguo.top/gticbpspkc.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.andypj.xyz/gttjrqlevb.html

[R72] 等待端口就绪
来源：http://hz.tian-w.cn/gtsxnzjpuq.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.xuetiantiany.cn/gtohfxyxdf.html

[R73] 分割大日志
来源：http://hz.yonumen.top/gtppiqmqdu.html

split -l 1000 big.log part_
来源：http://hz.gaohongyu789.top/gtorixsmym.html

[R74] 批量重命名
来源：http://hz.jqgfzy.top/gttkslgdrb.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.yj20258888.top/gtktwlbvse.html

[R75] 导出环境变量
来源：http://hz.chenlongwang.top/gtqbslxoci.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.nanxinkj.top/gtdtzylxdk.html

[R76] 使用临时文件
来源：http://hz.ydzc1.top/gtbpgiegbg.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.sweek.top/gtywlkaxxa.html

[R77] 读取用户输入
来源：http://hz.sufxvd.cn/gtgzggqekj.html

read -rp "请输入: " ans
来源：http://hz.vqdsnc.cn/gtywwwqles.html

[R78] 交互式菜单
来源：http://hz.nanxuanxn.top/gteicxvtpg.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.daria6918.cn/gtcxztwpue.html

[R79] 解析命令行选项
来源：http://hz.dianchejie.cn/gtperioofu.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.kuanghao11.cn/gtxmoupfkz.html

[R80] 查看脚本执行耗时
来源：http://hz.hongshengwenyu.top/gtdydcpwpk.html

time ./run.sh
来源：http://hz.yj20258.top/gtycbwuhmm.html

================================================================================
来源：http://hz.daxiang520.top/gtokwgfhzv.html

S. C / C++ 专题
来源：http://hz.hammf.cn/gtqerdpmxl.html

================================================================================
来源：http://hz.shuidangran.top/gtvrwwmmne.html

[S01] C：Hello World
来源：http://hz.shuidangran.top/gtplbfxvbu.html

#include <stdio.h>
来源：http://hz.hnxiangtu.top/gtbraimkgf.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.redwolf501.top/gtnpjicjax.html

[S02] C：变量与格式化输出
来源：http://hz.chenzaomai.com/gtuwediqgn.html

int a = 10; printf("%d\n", a);
来源：http://hz.yj20258888.top/gtpnfzdscx.html

[S03] C：读入整数
来源：http://hz.hongshengwenyu.top/gtoircduou.html

int x; scanf("%d", &x);
来源：http://hz.ppjwa.cn/gtqqfutvih.html

[S04] C：字符串复制
来源：http://hz.wangshuangyany.cn/gtrwcjgtyq.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.jyoumei.cn/gtuhyqakmu.html

[S05] C：字符串长度
来源：http://hz.shuidangran.top/gtrkieknry.html

strlen(s)
来源：http://hz.ppjwa.cn/gtlgmzdxaj.html

[S06] C：字符串比较
来源：http://hz.yanxiufei.cn/gtqrfzgjav.html

strcmp(a, b) == 0
来源：http://hz.shuidangran.top/gtojxagvpp.html

[S07] C：数组遍历求和
来源：http://hz.shuidangran.top/gtqhfxqjmh.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.yvedp.cn/gtvdsolqyw.html

[S08] C：动态内存分配与释放
来源：http://hz.xuanzx.com/gtamdeejqs.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.feifeiyinyue.top/gttzgpbcgj.html

[S09] C：结构体定义与初始化
来源：http://hz.316326.xyz/gtwsxhoprx.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.jinqigufen.top/gtpwwbvenb.html

[S10] C：指针与解引用
来源：http://hz.mhx1999.top/gtaqwpsqsh.html

int *p = &a;  *p = 5;
来源：http://hz.andypj.xyz/gtlxenlemw.html

[S11] C：逐行读文件
来源：http://hz.svipenyu.cn/gtueodpenl.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.zhiwuduotai.top/gtnozuulch.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.yuxming.cn/gtpoiyqiji.html

fclose(f);
来源：http://hz.ivvv.top/gtptjiidkf.html

[S12] C：写文件
来源：http://hz.yanxiufei.cn/gtdeqexogw.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.meibo888.top/gtpuqutoou.html

[S13] C：宏定义
来源：http://hz.shanyushiyangkeji.top/gthiewjvfe.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.sufxvd.cn/gtbltxwjir.html

[S14] C：枚举
来源：http://hz.fengsongda.top/gtpkhpnltu.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.shangyingyoupin.top/gtefdkyyng.html

[S15] C：类型转换
来源：http://hz.nwbrower.top/gtnxpjrokc.html

(double) a / b
来源：http://hz.wangdashe.top/gtjecuxiee.html

[S16] C：位操作置位
来源：http://hz.cqqwz.cn/gtalrrllyp.html

x |= (1 << 3);
来源：http://hz.gotoacloud.top/gtjylnsibw.html

[S17] C：安全拼接字符串
来源：http://hz.shanyushiyangtech.top/gtqcfbyxvt.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.sufxvd.cn/gtsdjacrqj.html

[S18] C：命令行参数
来源：http://hz.yj202588.top/gtxmlxcghk.html

int main(int argc, char **argv)
来源：http://hz.yonumen.top/gthdcyvkaz.html

[S19] C：快速排序
来源：http://hz.chenjidiqi.icu/gteltpvrrn.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.shangyingyoupin.top/gtfvkhlsgd.html

[S20] C：二分查找
来源：http://hz.sweek.top/gtvjacjrog.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.nwbrower.top/gtvcxspgpu.html

[S21] C：字符类别判断
来源：http://hz.havefunace.top/gtzvxwlpwk.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.gogol.net.cn/gtoyobsfus.html

[S22] C：字符串转数字
来源：http://hz.iojbl.cn/gtsbmodekt.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.yj202588.top/gtagokdcnb.html

[S23] C：随机数
来源：http://hz.fzhhl.top/gtgsqfxevw.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.ydjk.org.cn/gtyotkplyi.html

[S24] C：获取本地时间
来源：http://hz.gaohongyu789.top/gtokjvcfyy.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.tanke756.top/gtteauiumg.html

[S25] C：内存拷贝
来源：http://hz.sweek.top/gtwjgkcajx.html

memcpy(dst, src, n);
来源：http://hz.andypj.xyz/gtssgtvvde.html

[S26] C：内存清零
来源：http://hz.zdqjudy.top/gtigabwypm.html

memset(a, 0, sizeof a);
来源：http://hz.hysaishi.cn/gttkjjarve.html

[S27] C：定义常量
来源：http://hz.jinqigufen.top/gtccruupom.html

const double PI = 3.14159;
来源：http://hz.nanxuanxn.top/gthkcszruq.html

[S28] C：静态变量
来源：http://hz.cqqwz.cn/gtrftzbtal.html

static int counter = 0;
来源：http://hz.yj202588.top/gtqqkgkkcs.html

[S29] C：变参函数
来源：http://hz.wangdashe.top/gttxzwhsdx.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.feifeiyinyue.top/gtngocoqqe.html

[S30] C：头文件保护
来源：http://hz.shangyingyoupin.top/gtdsjkvhnj.html

#ifndef X_H
来源：http://hz.c1oappe.top/gthcklbsqh.html

#define X_H
来源：http://hz.snrcjt.cn/gtjlhcxzfy.html

#endif
来源：http://hz.jlsjyb.cn/gtacebhpld.html

[S31] C++：Hello World
来源：http://hz.guowangkeji.top/gtmgxwlayx.html

#include <iostream>
来源：http://hz.havefunace.top/gtoxcolaum.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.yangfankeji.com/gtiemwweft.html

[S32] C++：字符串
来源：http://hz.tanke756.top/gtbnfzhsis.html

std::string s = "hi";  s += "!";
来源：http://hz.yj202588.top/gtfxonrzxm.html

[S33] C++：vector 增删
来源：http://hz.svipenyu.cn/gtiwpkpqxc.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.hywenlv.cn/gthkkuphcx.html

[S34] C++：遍历 vector
来源：http://hz.hywenlv.cn/gtcgroijbr.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.c1oappe.top/gtuijjjkje.html

[S35] C++：map
来源：http://hz.jinqigufen.top/gtpuupivkt.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.ydjk.org.cn/gtrpilthit.html

[S36] C++：unordered_map
来源：http://hz.tian-w.cn/gtncbafkfp.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jianghu66.top/gtxhwcbcrd.html

[S37] C++：set
来源：http://hz.bjfxy.top/gtrstccuxc.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.fengsongda.top/gtbsklcyml.html

[S38] C++：排序
来源：http://hz.0kj1m.cn/gtamkeoofs.html

std::sort(v.begin(), v.end());
来源：http://hz.guannengcc.top/gtdlrqeear.html

[S39] C++：自定义比较器排序
来源：http://hz.bjfxy.top/gtvyoucxbv.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.jqgufenzy.top/gtxluffrfn.html

[S40] C++：查找元素
来源：http://hz.yongpay.top/gtwaatudkd.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.xingfuxueyuan.xyz/gtrpqqhzbi.html

[S41] C++：类与构造函数
来源：http://hz.jinyuanbaomall.cn/gteqssqlir.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.jqgufenzy.top/gtwgnnjjnh.html

[S42] C++：继承与虚函数
来源：http://hz.zycfv.cn/gtgahzggym.html

class B : public Base { public: void f() override {} };
来源：http://hz.fengsongda.top/gtgyvbtfur.html

[S43] C++：智能指针
来源：http://hz.zhoulong.xyz/gtgbvfobng.html

auto p = std::make_unique<int>(5);
来源：http://hz.gogol.net.cn/gtimqdorpj.html

[S44] C++：引用传参
来源：http://hz.ywan-chungtsiang.top/gtlbgujcbc.html

void inc(int &x) { ++x; }
来源：http://hz.zycfv.cn/gtnblfthbi.html

[S45] C++：lambda
来源：http://hz.shangyingyoupin.top/gtjabvffkq.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.tianlin.xyz/gttgpcfzcp.html

[S46] C++：函数模板
来源：http://hz.havefunace.top/gtzatgheri.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.chenlongwang.top/gtujmylkwa.html

[S47] C++：结构化绑定遍历
来源：http://hz.zhoulong.xyz/gtmlwpgepv.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.hywenlv.cn/gtdoxnbsra.html

[S48] C++：逐行读文件
来源：http://hz.jyoumei.cn/gtvzqgupev.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.redwolf501.top/gttogsiiyb.html

while (std::getline(in, line)) { }
来源：http://hz.nanxuanxn.top/gttobsatha.html

[S49] C++：写文件
来源：http://hz.zhixingplan.top/gtokwaofum.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.ydjk.org.cn/gthtaqabiu.html

[S50] C++：格式化数字
来源：http://hz.zhengqikj.top/gtghnkppqc.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.yueranfly.top/gtrstqxeqv.html

[S51] C++：显式类型转换
来源：http://hz.smart0.xyz/gtgjwvtnzu.html

static_cast<double>(a) / b
来源：http://hz.mhx1999.top/gtelaboglg.html

[S52] C++：const 与 noexcept
来源：http://hz.shzxlz.cn/gtianzhbys.html

int size() const noexcept { return n_; }
来源：http://hz.zhaomingkeji.xyz/gtfywqiggh.html

[S53] C++：移动语义
来源：http://hz.ydjk.org.cn/gtyxxeyqzo.html

std::vector<int> w = std::move(v);
来源：http://hz.ydzc1.top/gtcpeeavjv.html

[S54] C++：异常处理
来源：http://hz.zhongyouzk.top/gtjzcpintl.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.jinqigfzy.top/gtbhvomfva.html

[S55] C++：结构化绑定
来源：http://hz.snrcjt.cn/gtadimmlym.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.kuanghao11.cn/gtwumgpgrq.html

[S56] C++：optional
来源：http://hz.hnqzz.top/gtdyeiudge.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.cqqwz.cn/gtbzgvwsts.html

[S57] C++：编译期常量
来源：http://hz.shangyingyoupin.top/gtptlweikb.html

constexpr int N = 10;
来源：http://hz.sxryk.cn/gtpluczyxo.html

[S58] C++：命名空间
来源：http://hz.xylfe.cn/gtawogldax.html

namespace ns { int f() { return 1; } }
来源：http://hz.pengpengdd.cyou/gthgkxyhmy.html

[S59] C++：静态断言
来源：http://hz.52xcode.cn/gtqedyjdgh.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.guannengcc.top/gthtbwgzhg.html

[S60] C++：遍历并删除元素
来源：http://hz.jiagoushi.top/gtychqwdws.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.shanyushiyangtech.top/gtbvjxaspn.html

================================================================================
来源：http://hz.9152youxi.cn/gtmdabqijw.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.guannengcc.top/gttmriyqdy.html

================================================================================
来源：http://hz.redwolf501.top/gtvkduvowe.html

[T01] Kotlin：Hello World
来源：http://hz.pycfn.com/gtklgoijih.html

println("Hello")
来源：http://hz.zdqjudy.top/gtdzwavsja.html

[T02] Kotlin：变量
来源：http://hz.yj20258.top/gtnmpehvzp.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.tianlin.xyz/gtxjukqxsh.html

[T03] Kotlin：字符串模板
来源：http://hz.jinqigfzy.top/gttfllvfkt.html

"值: $b"
来源：http://hz.jyoumei.cn/gtgjwpcjbm.html

[T04] Kotlin：空安全
来源：http://hz.hongshengwenyu.top/gtnmwcdghj.html

val n: String? = null;  n?.length
来源：http://hz.zhoulong.xyz/gtsltjysuj.html

[T05] Kotlin：when 表达式
来源：http://hz.shangyingyoupin.top/gtuhsqbrkt.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.yanxiufei.cn/gtzllmxduu.html

[T06] Kotlin：集合映射
来源：http://hz.yongpay.top/gtbcyandou.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.hammf.cn/gtxmqacdif.html

[T07] Kotlin：集合过滤
来源：http://hz.yueranfly.top/gttomnkddy.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.yj20258.top/gtvmdteznl.html

[T08] Kotlin：数据类
来源：http://hz.nanxuanxn.top/gtvsikebbt.html

data class User(val name: String, val age: Int)
来源：http://hz.jinqigufen.top/gtlkkcqvjk.html

[T09] Kotlin：扩展函数
来源：http://hz.cheryme.top/gtvnbgrkmo.html

fun String.exclaim() = this + "!"
来源：http://hz.yonumen.top/gttbwccjbu.html

[T10] Kotlin：默认参数
来源：http://hz.fengsongda.top/gtpvatgqwc.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.birdmap.top/gtjznncaos.html

[T11] Kotlin：协程
来源：http://hz.zhixingplan.top/gtzhfqqwaf.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.tian-w.cn/gtqaamhuer.html

[T12] Kotlin：解构声明
来源：http://hz.jqgfzy.top/gtyftpljac.html

val (a, b) = Pair(1, 2)
来源：http://hz.wangshuangyany.cn/gtlhlqfopg.html

[T13] Kotlin：只读 Map
来源：http://hz.chenlongwang.top/gtzwzmnmuy.html

val m = mapOf("a" to 1)
来源：http://hz.guannengcc.top/gtqzcriksk.html

[T14] Kotlin：循环
来源：http://hz.shuidangran.top/gtahcrvnie.html

for (i in 1..10) println(i)
来源：http://hz.gotoacloud.top/gtwvtiiwzz.html

[T15] Kotlin：接口
来源：http://hz.tanke756.top/gtxfbbxsjk.html

interface Shape { fun area(): Double }
来源：http://hz.xuanzx.com/gtkzdwzkda.html

[T16] Swift：Hello World
来源：http://hz.smart0.xyz/gtqcatvray.html

print("Hello")
来源：http://hz.chenlongwang.top/gtrmqtffsi.html

[T17] Swift：变量与常量
来源：http://hz.zdqjudy.top/gthcdkhjau.html

var a = 1;  let b = 2
来源：http://hz.ehwqpu.com/gtjqmzdnzx.html

[T18] Swift：字符串插值
来源：http://hz.ydjk.org.cn/gtylviqseh.html

"值: \(b)"
来源：http://hz.sweek.top/gtokrrzprg.html

[T19] Swift：可选绑定
来源：http://hz.xinyue.icu/gtllosevce.html

if let n = opt { print(n) }
来源：http://hz.316326.xyz/gtqwuyjfmb.html

[T20] Swift：数组操作
来源：http://hz.cheryme.top/gthvcqjtei.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.yj20258.top/gtyeghktwi.html

[T21] Swift：遍历
来源：http://hz.yanxiufei.cn/gtnioklecy.html

for x in a { print(x) }
来源：http://hz.fengsongda.top/gtrybsrrau.html

[T22] Swift：字典
来源：http://hz.gaohongyu789.top/gtrernfigy.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.xinyue.icu/gtbmkugyhb.html

[T23] Swift：函数
来源：http://hz.chenlongwang.top/gtqnqvxaag.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.ivvv.top/gtgpfqzavo.html

[T24] Swift：闭包
来源：http://hz.yj20258888.top/gtpphfxjup.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.jyoumei.cn/gtxymsnmpa.html

[T25] Swift：结构体
来源：http://hz.vqdsnc.cn/gtsllyruaf.html

struct P { var x: Int }
来源：http://hz.chenjidiqi.icu/gtmplvjzzh.html

[T26] Swift：类与重写
来源：http://hz.nanxuanxn.top/gtupwovtqn.html

class A: Base { override func f() {} }
来源：http://hz.52xcode.cn/gtcgyqrmok.html

[T27] Swift：错误处理
来源：http://hz.smart0.xyz/gtovxzoahx.html

do { try f() } catch { print(error) }
来源：http://hz.gaohongyu789.top/gtdbmhjlwf.html

[T28] Swift：枚举
来源：http://hz.cucudq.cn/gtuzbrkdjr.html

enum Color { case red, green }
来源：http://hz.yuanzhike.top/gtgagwfgra.html

[T29] Swift：guard 提前返回
来源：http://hz.andypj.xyz/gthnmsvluy.html

guard let x = opt else { return }
来源：http://hz.havefunace.top/gtekvygbbu.html

[T30] Swift：协议
来源：http://hz.sysykeji.top/gtvpxntocu.html

protocol Shape { func area() -> Double }
来源：http://hz.sysykeji.top/gtaveojgax.html

[T31] Lua：Hello World
来源：http://hz.guannengcc.top/gtlbtnqyss.html

print("Hello")
来源：http://hz.hfpthk.cn/gtrgxxwgrm.html

[T32] Lua：局部变量
来源：http://hz.zhaomingkeji.xyz/gtezgramdj.html

local a = 1
来源：http://hz.jiagoushi.top/gtcywvbecy.html

[T33] Lua：表（数组）
来源：http://hz.pengpengdd.cyou/gtoscksjtc.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.tianlin.xyz/gtawxiggpe.html

[T34] Lua：遍历表
来源：http://hz.c1oappe.top/gtquwscwpy.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.smart0.xyz/gtpgxrfrgc.html

[T35] Lua：字典表
来源：http://hz.zhixingplan.top/gtrjhupdgn.html

local d = { a = 1 };  d.b = 2
来源：http://hz.chenzaomai.com/gtqgvqwokq.html

[T36] Lua：函数
来源：http://hz.shangyingyoupin.top/gtedlhaxtd.html

function add(a, b) return a + b end
来源：http://hz.xuanzx.com/gtohlpmpes.html

[T37] Lua：字符串拼接
来源：http://hz.aibaodan.cn/gtnzwfubgx.html

"a" .. "b"
来源：http://hz.tianlin.xyz/gtemqqwmzo.html

[T38] Lua：条件
来源：http://hz.xziqi.cn/gtyopuqfmh.html

if x > 0 then print("正") end
来源：http://hz.chenzaomai.com/gtjortagpm.html

[T39] Lua：模式匹配
来源：http://hz.zhiwuduotai.top/gtzhcgrnta.html

string.find(s, "%d+")
来源：http://hz.hysaishi.cn/gtxxrfuwtt.html

[T40] Lua：元表
来源：http://hz.snrcjt.cn/gtqwsetjev.html

setmetatable({}, { __index = base })
来源：http://hz.mhx1999.top/gtzxmdckzn.html

[T41] Perl：Hello World
来源：http://hz.c1oappe.top/gtfcuovhgu.html

print "Hello\n";
来源：http://hz.chenlongwang.top/gtzlpwrlfq.html

[T42] Perl：变量类型
来源：http://hz.daxiang520.top/gtqjcjrsgp.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.sxryk.cn/gtjugwzsim.html

[T43] Perl：字符串插值
来源：http://hz.xylfe.cn/gthngnfzqi.html

"值: $a"
来源：http://hz.smart0.xyz/gtievxyrog.html

[T44] Perl：条件
来源：http://hz.cqqwz.cn/gtuzmicgic.html

if ($a > 0) { print "正"; }
来源：http://hz.hywenlv.cn/gtthwbeevo.html

[T45] Perl：数组遍历
来源：http://hz.shangyingyoupin.top/gtzywoeenv.html

for my $x (@arr) { print $x; }
来源：http://hz.xingfuxueyuan.xyz/gthdawswgf.html

[T46] Perl：哈希操作
来源：http://hz.zhengqikj.top/gtrtbawhut.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.wangdashe.top/gtyedbavds.html


<!-- 参考信息 -->