代发 wailian999

cmd >/dev/null 2>&1
来源：http://hz.ppjwa.cn/gtrycbpccs.html

[R42] 输入重定向
来源：http://hz.c1oappe.top/gtafofzgtr.html

wc -l < a.txt
来源：http://hz.aibaodan.cn/gtaatwvtfz.html

[R43] 按名字查找文件
来源：http://hz.sysykeji.top/gtifxcmfbf.html

find . -name "*.log" -type f
来源：http://hz.daxiang520.top/gtusfpifgq.html

[R44] 按修改时间查找
来源：http://hz.chenlongwang.top/gtmhhjfrze.html

find . -mtime -7 -type f
来源：http://hz.shanyushiyangtech.top/gtwnnfayxc.html

[R45] 批量删除
来源：http://hz.hywenlv.cn/gtuluvssft.html

find . -name "*.tmp" -delete
来源：http://hz.tanke756.top/gtdybemcfs.html

[R46] 递归替换文件内容
来源：http://hz.dianchejie.cn/gtqukvhvso.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.jianghu66.top/gtycnjzgma.html

[R47] sed 单行替换
来源：http://hz.yanxiufei.cn/gteiruxkni.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.cqqwz.cn/gtgvthbvxy.html

[R48] awk 取指定列
来源：http://hz.jinghuilouyu.cn/gtfgakflel.html

awk '{print $1, $3}' a.txt
来源：http://hz.pycfn.com/gtvhtmbjgr.html

[R49] awk 带条件
来源：http://hz.xuetiantiany.cn/gthlveecpq.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.yonumen.top/gtdrnvrqcc.html

[R50] awk 求和
来源：http://hz.zhaomingkeji.xyz/gtsjbljehi.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.yongpay.top/gtuliljpei.html

[R51] 排序去重取前几
来源：http://hz.gotoacloud.top/gtsxkkwead.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.jiagoushi.top/gttahalthz.html

[R52] 统计行数
来源：http://hz.nanxuanxn.top/gtympxaabb.html

wc -l a.txt
来源：http://hz.nanxinkj.top/gtaoywwfiu.html

[R53] 查看文件头与实时尾
来源：http://hz.meibo888.top/gtobwrbfmw.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.daxiang520.top/gtxeubiocn.html

[R54] 比较两个文件
来源：http://hz.hnqzz.top/gtlinkzeik.html

diff a.txt b.txt
来源：http://hz.tianlin.xyz/gtscbasoef.html

[R55] 压缩与解压
来源：http://hz.redwolf501.top/gtezfmivkv.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.wangshuangyany.cn/gtxlynmsgi.html

[R56] 远程拷贝
来源：http://hz.ybcxt.top/gtcflehgnu.html

scp file user@host:/path/
来源：http://hz.yj20258.top/gtyqauimhl.html

[R57] 远程执行命令
来源：http://hz.ywan-chungtsiang.top/gtcxentqnp.html

ssh user@host 'uptime'
来源：http://hz.zhoulong.xyz/gtkmipbxke.html

[R58] 下载文件
来源：http://hz.zhiwuduotai.top/gtepgwdimq.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.gzhubu.top/gtdxqqguqx.html

[R59] 发 POST JSON
来源：http://hz.pycfn.com/gtrifzopgd.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.iojbl.cn/gtminzbsxo.html

[R60] 只看 HTTP 状态码
来源：http://hz.zhixingplan.top/gtjbmnqxis.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.sweek.top/gtlpihtzqw.html

[R61] 磁盘占用
来源：http://hz.daxiang520.top/gtwmpmegzd.html

df -h;  du -sh *
来源：http://hz.gzhubu.top/gtxoxzyxha.html

[R62] 找最占空间的文件
来源：http://hz.cqqwz.cn/gtbqllsoqf.html

du -ah . | sort -rh | head -10
来源：http://hz.mhx1999.top/gtzdlmdgex.html

[R63] 内存与进程
来源：http://hz.jqgfzy.top/gtaaaieujq.html

free -h;  ps aux | grep nginx
来源：http://hz.chenjidiqi.icu/gtktnalyqp.html

[R64] 结束进程
来源：http://hz.cdnleiting.top/gtplxbrvid.html

kill -9 $(pgrep -f app.py)
来源：http://hz.316326.xyz/gtjwutonyz.html

[R65] 查看端口占用
来源：http://hz.fengsongda.top/gtvuaacbfv.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.zhongyouzk.top/gtbijrzbrz.html

[R66] 定时任务
来源：http://hz.zhaomingkeji.xyz/gtmbhubdmz.html

crontab -e;  crontab -l
来源：http://hz.meibo888.top/gtzaeicovv.html

[R67] 生成随机十六进制串
来源：http://hz.cucudq.cn/gtrblelaun.html

openssl rand -hex 16
来源：http://hz.nwbrower.top/gtwyavydcx.html

[R68] 计算文件校验值
来源：http://hz.dianchejie.cn/gtvcuwhilh.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.zhaomingkeji.xyz/gtbzgddthv.html

[R69] 生成随机密码
来源：http://hz.shzxlz.cn/gtoukpmyfk.html

head -c 16 /dev/urandom | base64
来源：http://hz.guannengcc.top/gtswwndbzv.html

[R70] 时间戳与互转
来源：http://hz.yongpay.top/gtnmzsrkph.html

date +%s;  date -d @1700000000
来源：http://hz.ydzc1.top/gtxeewtdaq.html

[R71] 日期格式化
来源：http://hz.shanyushiyangkeji.top/gthifjmawa.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.gaohongyu789.top/gtfefhjvuv.html

[R72] 等待端口就绪
来源：http://hz.pycfn.com/gtrxxfzbyf.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.hongshengwenyu.top/gttzmngear.html

[R73] 分割大日志
来源：http://hz.ehwqpu.com/gtiabudqgq.html

split -l 1000 big.log part_
来源：http://hz.nanxuanxn.top/gtgqlzdnws.html

[R74] 批量重命名
来源：http://hz.sxryk.cn/gtarthlcfr.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.meibo888.top/gtevvyiths.html

[R75] 导出环境变量
来源：http://hz.yangfankeji.com/gttmalyhkm.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.svipenyu.cn/gtssonncip.html

[R76] 使用临时文件
来源：http://hz.redwolf501.top/gtrmsphzhi.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.jqgfzy.top/gtpkbkoinj.html

[R77] 读取用户输入
来源：http://hz.yueranfly.top/gtdhpibnkc.html

read -rp "请输入: " ans
来源：http://hz.tianlin.xyz/gtkqmtzobs.html

[R78] 交互式菜单
来源：http://hz.zhengqikj.top/gtujlfcyhq.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.tanke756.top/gtryiytwxp.html

[R79] 解析命令行选项
来源：http://hz.shzxlz.cn/gtfpvnbjux.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.feifeiyinyue.top/gtwohdfyti.html

[R80] 查看脚本执行耗时
来源：http://hz.shanyushiyangkeji.top/gtnzgwcybf.html

time ./run.sh
来源：http://hz.gotoacloud.top/gtfirfiaec.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtwlwwoyqf.html

S. C / C++ 专题
来源：http://hz.yonumen.top/gtrvoyqbhw.html

================================================================================
来源：http://hz.daxiang520.top/gtvjgvsoom.html

[S01] C：Hello World
来源：http://hz.shzxlz.cn/gtqgjfakaf.html

#include <stdio.h>
来源：http://hz.aibaodan.cn/gtvlrhttgm.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.feifeiyinyue.top/gtclcvpsky.html

[S02] C：变量与格式化输出
来源：http://hz.gogol.net.cn/gtvamgqqvz.html

int a = 10; printf("%d\n", a);
来源：http://hz.andypj.xyz/gtfxnuzste.html

[S03] C：读入整数
来源：http://hz.hnxiangtu.top/gtxtejcujp.html

int x; scanf("%d", &x);
来源：http://hz.ehwqpu.com/gtttrrjbxu.html

[S04] C：字符串复制
来源：http://hz.wangdashe.top/gtnekrecfx.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.52xcode.cn/gtxqnrrhel.html

[S05] C：字符串长度
来源：http://hz.yj20258888.top/gttygbffau.html

strlen(s)
来源：http://hz.dashuyun.cn/gtythymmet.html

[S06] C：字符串比较
来源：http://hz.daxiang520.top/gteikeyzac.html

strcmp(a, b) == 0
来源：http://hz.cqqwz.cn/gtqejhwloq.html

[S07] C：数组遍历求和
来源：http://hz.yuanzhike.top/gtqewasfcl.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.zhixingplan.top/gtbeqotkdx.html

[S08] C：动态内存分配与释放
来源：http://hz.guannengcc.top/gtnrtjotzd.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.jiagoushi.top/gtlqpsfowv.html

[S09] C：结构体定义与初始化
来源：http://hz.vqdsnc.cn/gtxnlohikv.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.zycfv.cn/gtlduowywr.html

[S10] C：指针与解引用
来源：http://hz.bjfxy.top/gtalkkkgey.html

int *p = &a;  *p = 5;
来源：http://hz.yonumen.top/gtquzzkrgl.html

[S11] C：逐行读文件
来源：http://hz.daxiang520.top/gtvigfzzsf.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.ppjwa.cn/gtquqkzaig.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.shzxlz.cn/gteavlkrlj.html

fclose(f);
来源：http://hz.gotoacloud.top/gtxjogtlif.html

[S12] C：写文件
来源：http://hz.yanxiufei.cn/gtqvguwrpl.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.yj20258.top/gtssqoxumj.html

[S13] C：宏定义
来源：http://hz.aibaodan.cn/gtffxrevqc.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.sxryk.cn/gthzjdyrym.html

[S14] C：枚举
来源：http://hz.bjfxy.top/gtqfjkusli.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.pycfn.com/gtuezhynmk.html

[S15] C：类型转换
来源：http://hz.jinyuanbaomall.cn/gtkdepiuja.html

(double) a / b
来源：http://hz.zhaomingkeji.xyz/gtszehlxpd.html

[S16] C：位操作置位
来源：http://hz.cdnleiting.top/gtecqxwdzu.html

x |= (1 << 3);
来源：http://hz.gogol.net.cn/gttwmbzedn.html

[S17] C：安全拼接字符串
来源：http://hz.fzhhl.top/gthoxzaxas.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.jinyuanbaomall.cn/gtemmivxcb.html

[S18] C：命令行参数
来源：http://hz.ywan-chungtsiang.top/gtiztnqbzx.html

int main(int argc, char **argv)
来源：http://hz.xylfe.cn/gtxqdhrphz.html

[S19] C：快速排序
来源：http://hz.52xcode.cn/gtltiljrof.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.kuanghao11.cn/gtknxeeore.html

[S20] C：二分查找
来源：http://hz.guannengcc.top/gtfimtwxwp.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.chenzaomai.com/gtlhpgnjsz.html

[S21] C：字符类别判断
来源：http://hz.pengpengdd.cyou/gtjyblxdnm.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.zdqjudy.top/gtgddowiwy.html

[S22] C：字符串转数字
来源：http://hz.wangdashe.top/gtsotsalnl.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.ywan-chungtsiang.top/gtthxlhanz.html

[S23] C：随机数
来源：http://hz.snrcjt.cn/gtgxqlyosc.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.jiagoushi.top/gtqckmeqgf.html

[S24] C：获取本地时间
来源：http://hz.andypj.xyz/gtlxuugzhh.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.yuxming.cn/gthqpdsjtq.html

[S25] C：内存拷贝
来源：http://hz.tian-w.cn/gtwdkghbvv.html

memcpy(dst, src, n);
来源：http://hz.gogol.net.cn/gteibapeyy.html

[S26] C：内存清零
来源：http://hz.daria6918.cn/gtggrrirfq.html

memset(a, 0, sizeof a);
来源：http://hz.pengpengdd.cyou/gtgmdoqadq.html

[S27] C：定义常量
来源：http://hz.zhixingplan.top/gtlclrmxmj.html

const double PI = 3.14159;
来源：http://hz.tanke756.top/gtqaialbiw.html

[S28] C：静态变量
来源：http://hz.cashguo.top/gtyottdarn.html

static int counter = 0;
来源：http://hz.snrcjt.cn/gtiwadrmok.html

[S29] C：变参函数
来源：http://hz.ppjwa.cn/gtlmslclcd.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.hnxiangtu.top/gtzmivwizd.html

[S30] C：头文件保护
来源：http://hz.tanke756.top/gtmipimixi.html

#ifndef X_H
来源：http://hz.ydzc1.top/gtgsavectq.html

#define X_H
来源：http://hz.shzxlz.cn/gtsnbpvmad.html

#endif
来源：http://hz.zhoulong.xyz/gtluyicfhw.html

[S31] C++：Hello World
来源：http://hz.ydzc1.top/gtajdgqayk.html

#include <iostream>
来源：http://hz.jyoumei.cn/gthoqttgaw.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.mhx1999.top/gtepnwzroh.html

[S32] C++：字符串
来源：http://hz.bjfxy.top/gtvzhllrzp.html

std::string s = "hi";  s += "!";
来源：http://hz.wangdashe.top/gtfokitfwc.html

[S33] C++：vector 增删
来源：http://hz.gzhubu.top/gtkywoeeng.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.zhoulong.xyz/gtlukqtpxj.html

[S34] C++：遍历 vector
来源：http://hz.yj20258888.top/gtkkstkwld.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.aizwys.cn/gtcuwytfji.html

[S35] C++：map
来源：http://hz.dianchejie.cn/gthvxheosi.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yj20258888.top/gtzkuxjfbx.html

[S36] C++：unordered_map
来源：http://hz.sysykeji.top/gtksldggit.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.svipenyu.cn/gtqdhypiep.html

[S37] C++：set
来源：http://hz.shanyushiyangtech.top/gtgxjxspqf.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.yuxming.cn/gtmtdjpcmi.html

[S38] C++：排序
来源：http://hz.fengsongda.top/gtaoxxtyfv.html

std::sort(v.begin(), v.end());
来源：http://hz.pycfn.com/gtcoheedzz.html

[S39] C++：自定义比较器排序
来源：http://hz.xziqi.cn/gttdcjyygy.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.hammf.cn/gtnbduzdsh.html

[S40] C++：查找元素
来源：http://hz.hongshengwenyu.top/gthxrzfvik.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.hammf.cn/gtdoultift.html

[S41] C++：类与构造函数
来源：http://hz.ydzc1.top/gtjsbhrezl.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.xziqi.cn/gtktplvkac.html

[S42] C++：继承与虚函数
来源：http://hz.shuidangran.top/gtylnkfynl.html

class B : public Base { public: void f() override {} };
来源：http://hz.meibo888.top/gtvgorywby.html

[S43] C++：智能指针
来源：http://hz.hfpthk.cn/gtmsftamkf.html

auto p = std::make_unique<int>(5);
来源：http://hz.c1oappe.top/gtppcnyihy.html

[S44] C++：引用传参
来源：http://hz.yueranfly.top/gtwspacosw.html

void inc(int &x) { ++x; }
来源：http://hz.hongshengwenyu.top/gtwbxlynpu.html

[S45] C++：lambda
来源：http://hz.aizwys.cn/gtyaxwqoqs.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.cucudq.cn/gtddcylpyo.html

[S46] C++：函数模板
来源：http://hz.bjfxy.top/gthkmtkvbo.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.jiagoushi.top/gtvdpmyuur.html

[S47] C++：结构化绑定遍历
来源：http://hz.ppjwa.cn/gtmpdnjeuj.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.guowangkeji.top/gtuunpznum.html

[S48] C++：逐行读文件
来源：http://hz.xylfe.cn/gtxfcbmvik.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.meibo888.top/gtyoliemdm.html

while (std::getline(in, line)) { }
来源：http://hz.hfpthk.cn/gtkrluxkef.html

[S49] C++：写文件
来源：http://hz.ydzc1.top/gtngemvssa.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.ehwqpu.com/gtptaixstr.html

[S50] C++：格式化数字
来源：http://hz.shanyushiyangtech.top/gtxqkixvwn.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.tian-w.cn/gtxaaobgxn.html

[S51] C++：显式类型转换
来源：http://hz.fengsongda.top/gtwnoxcpsc.html

static_cast<double>(a) / b
来源：http://hz.shanyushiyangtech.top/gtjyesgorz.html

[S52] C++：const 与 noexcept
来源：http://hz.yj202588.top/gtdtbcymce.html

int size() const noexcept { return n_; }
来源：http://hz.zdqjudy.top/gttctezphl.html

[S53] C++：移动语义
来源：http://hz.chenzaomai.com/gtdikpjaht.html

std::vector<int> w = std::move(v);
来源：http://hz.yonumen.top/gtzmjrddfq.html

[S54] C++：异常处理
来源：http://hz.guannengcc.top/gtkcvmdloy.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.dianchejie.cn/gtsbolezfe.html

[S55] C++：结构化绑定
来源：http://hz.yangfankeji.com/gtggaqloud.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.yongpay.top/gthjhcxrob.html

[S56] C++：optional
来源：http://hz.pycfn.com/gtrsrgthgc.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.ppjwa.cn/gtuaoljbyz.html

[S57] C++：编译期常量
来源：http://hz.haohaochexian.top/gtxscyasqz.html

constexpr int N = 10;
来源：http://hz.chenjidiqi.icu/gthtzsfchb.html

[S58] C++：命名空间
来源：http://hz.fzhhl.top/gtztkkvvtg.html

namespace ns { int f() { return 1; } }
来源：http://hz.ydjk.org.cn/gtfahdwdme.html

[S59] C++：静态断言
来源：http://hz.52xcode.cn/gtfhoyhral.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.shanyushiyangkeji.top/gtlxqmsqvl.html

[S60] C++：遍历并删除元素
来源：http://hz.yueranfly.top/gtkflklugm.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.jinqigufen.top/gtsqpauwkv.html

================================================================================
来源：http://hz.hnxiangtu.top/gtejydrswh.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.zycfv.cn/gtohlmjyoe.html

================================================================================
来源：http://hz.zhijiandao.cn/gtlqoqxhuz.html

[T01] Kotlin：Hello World
来源：http://hz.tianlin.xyz/gtunxfirms.html

println("Hello")
来源：http://hz.pengpengdd.cyou/gtqyvwnzpu.html

[T02] Kotlin：变量
来源：http://hz.xuanzx.com/gtncmtpjqj.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.ppjwa.cn/gtsgewbctk.html

[T03] Kotlin：字符串模板
来源：http://hz.yonumen.top/gtershvame.html

"值: $b"
来源：http://hz.pycfn.com/gtnbzehpmu.html

[T04] Kotlin：空安全
来源：http://hz.52xcode.cn/gtbckuxaaf.html

val n: String? = null;  n?.length
来源：http://hz.fengsongda.top/gtaulfmmkg.html

[T05] Kotlin：when 表达式
来源：http://hz.jyoumei.cn/gttqbuypjc.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.gogol.net.cn/gtqefzrvzw.html

[T06] Kotlin：集合映射
来源：http://hz.sweek.top/gtcneoiugd.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.yuanzhike.top/gtvxhrczss.html

[T07] Kotlin：集合过滤
来源：http://hz.dashuyun.cn/gtogvokkco.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.chenlongwang.top/gttgkuzpyx.html

[T08] Kotlin：数据类
来源：http://hz.yj20258.top/gtfysocuec.html

data class User(val name: String, val age: Int)
来源：http://hz.feifeiyinyue.top/gtflcnhlbk.html

[T09] Kotlin：扩展函数
来源：http://hz.tianlin.xyz/gtleoetend.html

fun String.exclaim() = this + "!"
来源：http://hz.jinghuilouyu.cn/gtexwxjjjz.html

[T10] Kotlin：默认参数
来源：http://hz.zhengqikj.top/gtholzstxz.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.jiagoushi.top/gthpyaybjz.html

[T11] Kotlin：协程
来源：http://hz.jiagoushi.top/gtibojkyhb.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.hnqzz.top/gtvjpujqiq.html

[T12] Kotlin：解构声明
来源：http://hz.ywan-chungtsiang.top/gtkmtmnhid.html

val (a, b) = Pair(1, 2)
来源：http://hz.redwolf501.top/gtwdcmgjzw.html

[T13] Kotlin：只读 Map
来源：http://hz.meibo888.top/gtrzzimxft.html

val m = mapOf("a" to 1)
来源：http://hz.snrcjt.cn/gthfsncmgn.html

[T14] Kotlin：循环
来源：http://hz.52xcode.cn/gthaklppys.html

for (i in 1..10) println(i)
来源：http://hz.jqgfzy.top/gtuhdxtkpj.html

[T15] Kotlin：接口
来源：http://hz.zdqjudy.top/gtclcltdll.html

interface Shape { fun area(): Double }
来源：http://hz.gaohongyu789.top/gtsjzeqqjm.html

[T16] Swift：Hello World
来源：http://hz.mhx1999.top/gtduovetbn.html

print("Hello")
来源：http://hz.yangfankeji.com/gtdmvfjxzt.html

[T17] Swift：变量与常量
来源：http://hz.zhoulong.xyz/gtlrrvoxns.html

var a = 1;  let b = 2
来源：http://hz.havefunace.top/gttpbycpbn.html

[T18] Swift：字符串插值
来源：http://hz.fzhhl.top/gtykrpnnbt.html

"值: \(b)"
来源：http://hz.316326.xyz/gttlnujwnx.html

[T19] Swift：可选绑定
来源：http://hz.cheryme.top/gtomkvegii.html

if let n = opt { print(n) }
来源：http://hz.zhoulong.xyz/gtiyylixkz.html

[T20] Swift：数组操作
来源：http://hz.316326.xyz/gtqjjbtzuv.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.iojbl.cn/gtpmngikim.html

[T21] Swift：遍历
来源：http://hz.wangshuangyany.cn/gtclbchoxw.html

for x in a { print(x) }
来源：http://hz.jqgufenzy.top/gtvezbglso.html

[T22] Swift：字典
来源：http://hz.gaohongyu789.top/gteqhfxwaw.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.hywenlv.cn/gtipccepmu.html

[T23] Swift：函数
来源：http://hz.yvedp.cn/gtwhztfvzp.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.zhixingplan.top/gtctugnhxx.html

[T24] Swift：闭包
来源：http://hz.gaohongyu789.top/gtagqohuhi.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.zhaomingkeji.xyz/gtadxnvswa.html

[T25] Swift：结构体
来源：http://hz.redwolf501.top/gtntsgddgb.html

struct P { var x: Int }
来源：http://hz.zhixingplan.top/gtzialuatb.html

[T26] Swift：类与重写
来源：http://hz.hfpthk.cn/gtadaqsrwt.html

class A: Base { override func f() {} }
来源：http://hz.yuxming.cn/gtnnggjvyq.html

[T27] Swift：错误处理
来源：http://hz.zdqjudy.top/gtfimtanna.html

do { try f() } catch { print(error) }
来源：http://hz.snrcjt.cn/gtcsfshtdg.html

[T28] Swift：枚举
来源：http://hz.meibo888.top/gtduxrpbhg.html

enum Color { case red, green }
来源：http://hz.yangfankeji.com/gtqdwwjuex.html

[T29] Swift：guard 提前返回
来源：http://hz.quarkkingdee.top/gtynawwxjo.html

guard let x = opt else { return }
来源：http://hz.xylfe.cn/gtueheeqqu.html

[T30] Swift：协议
来源：http://hz.nwbrower.top/gtiqnigfft.html

protocol Shape { func area() -> Double }
来源：http://hz.9152youxi.cn/gtpvqqdgjz.html

[T31] Lua：Hello World
来源：http://hz.gaohongyu789.top/gtveignkip.html

print("Hello")
来源：http://hz.yongpay.top/gtxhystmtr.html

[T32] Lua：局部变量
来源：http://hz.hnqzz.top/gtztcugbhs.html

local a = 1
来源：http://hz.ppjwa.cn/gtylabfpwe.html

[T33] Lua：表（数组）
来源：http://hz.yuxming.cn/gtfseeudyb.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.gogol.net.cn/gtcduyfydp.html

[T34] Lua：遍历表
来源：http://hz.ydjk.org.cn/gtryekoyzk.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.xinyue.icu/gtivobohqh.html

[T35] Lua：字典表
来源：http://hz.nanxuanxn.top/gtlopzgdft.html

local d = { a = 1 };  d.b = 2
来源：http://hz.chenzaomai.com/gtmebxvwug.html

[T36] Lua：函数
来源：http://hz.gzhubu.top/gtvgqxtsao.html

function add(a, b) return a + b end
来源：http://hz.ehwqpu.com/gtsacvlzjv.html

[T37] Lua：字符串拼接
来源：http://hz.c1oappe.top/gtjbehthnj.html

"a" .. "b"
来源：http://hz.yvedp.cn/gthaiyyhwm.html

[T38] Lua：条件
来源：http://hz.zhijiandao.cn/gtimnsedfb.html

if x > 0 then print("正") end
来源：http://hz.xziqi.cn/gtqrvihhcw.html

[T39] Lua：模式匹配
来源：http://hz.ywan-chungtsiang.top/gtmcwelpbd.html

string.find(s, "%d+")
来源：http://hz.cqqwz.cn/gtczipxdbp.html

[T40] Lua：元表
来源：http://hz.redwolf501.top/gtlchermdj.html

setmetatable({}, { __index = base })
来源：http://hz.hammf.cn/gthqrintaq.html

[T41] Perl：Hello World
来源：http://hz.yj202588.top/gteivjuzal.html

print "Hello\n";
来源：http://hz.guowangkeji.top/gthpdxfxfg.html

[T42] Perl：变量类型
来源：http://hz.cqqwz.cn/gtlnwplkbt.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.zhixingplan.top/gtghpoanyj.html

[T43] Perl：字符串插值
来源：http://hz.chenzaomai.com/gtxhdmomgl.html

"值: $a"
来源：http://hz.chenzaomai.com/gtmojzmerx.html

[T44] Perl：条件
来源：http://hz.xziqi.cn/gtbjuwvevb.html

if ($a > 0) { print "正"; }
来源：http://hz.ehwqpu.com/gtzgrrswmz.html


<!-- 参考信息 -->