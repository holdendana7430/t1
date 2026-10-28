代发 wailian999

cmd > out.log 2>&1
来源：http://hz.sxryk.cn/gthrrhjxow.html

[R40] 追加写日志
来源：http://hz.chenlongwang.top/gtqqsiejkm.html

echo "log" >> out.log
来源：http://hz.snrcjt.cn/gtfjdlwnvw.html

[R41] 丢弃输出
来源：http://hz.yongpay.top/gtorchiyqk.html

cmd >/dev/null 2>&1
来源：http://hz.xylfe.cn/gtdrdksane.html

[R42] 输入重定向
来源：http://hz.svipenyu.cn/gtksnogsug.html

wc -l < a.txt
来源：http://hz.wangdashe.top/gtopusthyr.html

[R43] 按名字查找文件
来源：http://hz.jinghuilouyu.cn/gtrlghhzkc.html

find . -name "*.log" -type f
来源：http://hz.316326.xyz/gtbfxxanea.html

[R44] 按修改时间查找
来源：http://hz.chenlongwang.top/gtcsuvzifr.html

find . -mtime -7 -type f
来源：http://hz.gaohongyu789.top/gtbcoehgtt.html

[R45] 批量删除
来源：http://hz.fengsongda.top/gtjsmsxjvk.html

find . -name "*.tmp" -delete
来源：http://hz.yonumen.top/gtqxndewhe.html

[R46] 递归替换文件内容
来源：http://hz.ydzc1.top/gtfpiryzzq.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.zhoulong.xyz/gtaviwvkih.html

[R47] sed 单行替换
来源：http://hz.dianchejie.cn/gtrhutrqsf.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.cdnleiting.top/gteqjeidnb.html

[R48] awk 取指定列
来源：http://hz.ydjk.org.cn/gteawohqrq.html

awk '{print $1, $3}' a.txt
来源：http://hz.zhengqikj.top/gtvyehtxtq.html

[R49] awk 带条件
来源：http://hz.cucudq.cn/gtwyguijox.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.shangyingyoupin.top/gtylmdzstf.html

[R50] awk 求和
来源：http://hz.iojbl.cn/gtpgihludm.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.ehwqpu.com/gtthwieeao.html

[R51] 排序去重取前几
来源：http://hz.hongshengwenyu.top/gtxsrbjouy.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.ydjk.org.cn/gttrkmcokz.html

[R52] 统计行数
来源：http://hz.chenjidiqi.icu/gtcqtxxqpo.html

wc -l a.txt
来源：http://hz.aizwys.cn/gtredjajoc.html

[R53] 查看文件头与实时尾
来源：http://hz.hnxiangtu.top/gtcigiqymj.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.cdnleiting.top/gtztpuxfby.html

[R54] 比较两个文件
来源：http://hz.chenlongwang.top/gterhibkfk.html

diff a.txt b.txt
来源：http://hz.hnxiangtu.top/gtdyovilqo.html

[R55] 压缩与解压
来源：http://hz.snrcjt.cn/gtrycalkgl.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.cucudq.cn/gthovgjivo.html

[R56] 远程拷贝
来源：http://hz.gogol.net.cn/gtwfwfcdsj.html

scp file user@host:/path/
来源：http://hz.hfpthk.cn/gtsnscudhe.html

[R57] 远程执行命令
来源：http://hz.vqdsnc.cn/gtycsgpozg.html

ssh user@host 'uptime'
来源：http://hz.c1oappe.top/gtrdkhzvut.html

[R58] 下载文件
来源：http://hz.jqgfzy.top/gtkkemczmy.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.0kj1m.cn/gtblhyuchr.html

[R59] 发 POST JSON
来源：http://hz.svipenyu.cn/gttoempmns.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.smart0.xyz/gtgyaixtqy.html

[R60] 只看 HTTP 状态码
来源：http://hz.chenlongwang.top/gtqvuipssz.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.ydjk.org.cn/gtclyceipy.html

[R61] 磁盘占用
来源：http://hz.tanke756.top/gtuibkgrpp.html

df -h;  du -sh *
来源：http://hz.yj20258.top/gtoahejcpb.html

[R62] 找最占空间的文件
来源：http://hz.andypj.xyz/gtotmxpdzf.html

du -ah . | sort -rh | head -10
来源：http://hz.ydjk.org.cn/gtwbkgaxfu.html

[R63] 内存与进程
来源：http://hz.cucudq.cn/gtikvaabpx.html

free -h;  ps aux | grep nginx
来源：http://hz.yanxiufei.cn/gtayvtekrd.html

[R64] 结束进程
来源：http://hz.svipenyu.cn/gtnqzvizbm.html

kill -9 $(pgrep -f app.py)
来源：http://hz.shuidangran.top/gtlvkiruuo.html

[R65] 查看端口占用
来源：http://hz.shanyushiyangtech.top/gtxvuqntre.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.cdnleiting.top/gtkhzxxcou.html

[R66] 定时任务
来源：http://hz.xziqi.cn/gtsvakmhdf.html

crontab -e;  crontab -l
来源：http://hz.dianchejie.cn/gtevrckcfk.html

[R67] 生成随机十六进制串
来源：http://hz.sxryk.cn/gttkkbtfos.html

openssl rand -hex 16
来源：http://hz.andypj.xyz/gtvmolgfmb.html

[R68] 计算文件校验值
来源：http://hz.hammf.cn/gtgzvesezv.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.hfpthk.cn/gtrynmlobs.html

[R69] 生成随机密码
来源：http://hz.aizwys.cn/gtfyqpjpqe.html

head -c 16 /dev/urandom | base64
来源：http://hz.gogol.net.cn/gtwklyzjro.html

[R70] 时间戳与互转
来源：http://hz.daria6918.cn/gtlzqssojo.html

date +%s;  date -d @1700000000
来源：http://hz.hnqzz.top/gtjfauvjor.html

[R71] 日期格式化
来源：http://hz.xuetiantiany.cn/gttxcsxybb.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.nanxuanxn.top/gtceiwqlai.html

[R72] 等待端口就绪
来源：http://hz.bjfxy.top/gtmqsluccr.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.daxiang520.top/gtwxdmzhqz.html

[R73] 分割大日志
来源：http://hz.svipenyu.cn/gtbslzefqp.html

split -l 1000 big.log part_
来源：http://hz.daxiang520.top/gtevbzrxmt.html

[R74] 批量重命名
来源：http://hz.cdnleiting.top/gtuwkyesuw.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.yueranfly.top/gtcxgumypc.html

[R75] 导出环境变量
来源：http://hz.jinyuanbaomall.cn/gtiomcaeod.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.xuetiantiany.cn/gtqvxoplvz.html

[R76] 使用临时文件
来源：http://hz.zhiwuduotai.top/gtudomytqg.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.gzhubu.top/gtnzqnsysp.html

[R77] 读取用户输入
来源：http://hz.jinqigufen.top/gtetmgcrfb.html

read -rp "请输入: " ans
来源：http://hz.iojbl.cn/gtkqqkypsv.html

[R78] 交互式菜单
来源：http://hz.ehwqpu.com/gtkktijurx.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.cashguo.top/gtwazpyeyh.html

[R79] 解析命令行选项
来源：http://hz.quarkkingdee.top/gtmusteiab.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.hongshengwenyu.top/gtbtyrfiuo.html

[R80] 查看脚本执行耗时
来源：http://hz.chenlongwang.top/gtnzntsmmo.html

time ./run.sh
来源：http://hz.cdnleiting.top/gtafvhyhcv.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtvhkjhuhx.html

S. C / C++ 专题
来源：http://hz.aibaodan.cn/gteafuxsjv.html

================================================================================
来源：http://hz.xinyue.icu/gteebwulhr.html

[S01] C：Hello World
来源：http://hz.sufxvd.cn/gtqjfqdlde.html

#include <stdio.h>
来源：http://hz.cashguo.top/gtmchocxvm.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.ehwqpu.com/gtwgafhkjx.html

[S02] C：变量与格式化输出
来源：http://hz.zhengqikj.top/gtgimdbrtd.html

int a = 10; printf("%d\n", a);
来源：http://hz.sxryk.cn/gtpxyqdcpd.html

[S03] C：读入整数
来源：http://hz.zhijiandao.cn/gtaxwmierd.html

int x; scanf("%d", &x);
来源：http://hz.snrcjt.cn/gtflrijrmh.html

[S04] C：字符串复制
来源：http://hz.xuanzx.com/gtjwniyoun.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.sweek.top/gtyevguukz.html

[S05] C：字符串长度
来源：http://hz.redwolf501.top/gtmpqzwgls.html

strlen(s)
来源：http://hz.hnxiangtu.top/gtdlfareeb.html

[S06] C：字符串比较
来源：http://hz.cdnleiting.top/gtcucpozuo.html

strcmp(a, b) == 0
来源：http://hz.yuanzhike.top/gtbfsarrrx.html

[S07] C：数组遍历求和
来源：http://hz.yuanzhike.top/gtoqjejfwg.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.jinyuanbaomall.cn/gtatdprnhn.html

[S08] C：动态内存分配与释放
来源：http://hz.zhongyouzk.top/gtpqttveyp.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.kuanghao11.cn/gtnqpwoctx.html

[S09] C：结构体定义与初始化
来源：http://hz.hywenlv.cn/gtvicufxki.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.0kj1m.cn/gtfluhoiau.html

[S10] C：指针与解引用
来源：http://hz.yuanzhike.top/gtdzglfrvj.html

int *p = &a;  *p = 5;
来源：http://hz.fengsongda.top/gthuqjwedj.html

[S11] C：逐行读文件
来源：http://hz.tian-w.cn/gtxzopemfv.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.quarkkingdee.top/gtftrrscnb.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.hnxiangtu.top/gtrxcnyeyr.html

fclose(f);
来源：http://hz.xuetiantiany.cn/gtofzsdoxw.html

[S12] C：写文件
来源：http://hz.xingfuxueyuan.xyz/gtgxqenrdd.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.meibo888.top/gtwhegdnbj.html

[S13] C：宏定义
来源：http://hz.zhaomingkeji.xyz/gtpixfnrlr.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.jqgufenzy.top/gttkskutil.html

[S14] C：枚举
来源：http://hz.guannengcc.top/gtsbklaizc.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.havefunace.top/gtaobfodrq.html

[S15] C：类型转换
来源：http://hz.guannengcc.top/gtayajqjns.html

(double) a / b
来源：http://hz.zhiwuduotai.top/gtrdyomtcm.html

[S16] C：位操作置位
来源：http://hz.xziqi.cn/gtgpwawrma.html

x |= (1 << 3);
来源：http://hz.zycfv.cn/gtujjegbef.html

[S17] C：安全拼接字符串
来源：http://hz.yanxiufei.cn/gthtxvkhdg.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.cashguo.top/gtjdtfdmdh.html

[S18] C：命令行参数
来源：http://hz.wangdashe.top/gtrmizdjbl.html

int main(int argc, char **argv)
来源：http://hz.hongshengwenyu.top/gtfyxybwfi.html

[S19] C：快速排序
来源：http://hz.guowangkeji.top/gtahlsbrzp.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.smart0.xyz/gtcgctfhyx.html

[S20] C：二分查找
来源：http://hz.zhiwuduotai.top/gtlvkvxckb.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.sufxvd.cn/gtldgujbcr.html

[S21] C：字符类别判断
来源：http://hz.redwolf501.top/gtgzbrauvt.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.yanxiufei.cn/gtkpjlehva.html

[S22] C：字符串转数字
来源：http://hz.ivvv.top/gtbscmudwp.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.vqdsnc.cn/gtiyjfgetu.html

[S23] C：随机数
来源：http://hz.zhaomingkeji.xyz/gtmeaglmhf.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.snrcjt.cn/gtcjsjqmam.html

[S24] C：获取本地时间
来源：http://hz.chenzaomai.com/gtddqvvkpl.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.pycfn.com/gtaugoskfq.html

[S25] C：内存拷贝
来源：http://hz.52xcode.cn/gtmrtkakrd.html

memcpy(dst, src, n);
来源：http://hz.bjfxy.top/gtlduuyopt.html

[S26] C：内存清零
来源：http://hz.c1oappe.top/gtfkxrnnof.html

memset(a, 0, sizeof a);
来源：http://hz.redwolf501.top/gtxfzqnklz.html

[S27] C：定义常量
来源：http://hz.iojbl.cn/gtpddmracj.html

const double PI = 3.14159;
来源：http://hz.zhixingplan.top/gtqvoxxuhk.html

[S28] C：静态变量
来源：http://hz.feifeiyinyue.top/gtgmcdsiib.html

static int counter = 0;
来源：http://hz.zhoulong.xyz/gtoqwbdtzw.html

[S29] C：变参函数
来源：http://hz.jqgufenzy.top/gtlsywjsyf.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.zhoulong.xyz/gtgaavpqra.html

[S30] C：头文件保护
来源：http://hz.zhongyouzk.top/gtzdrvtvgp.html

#ifndef X_H
来源：http://hz.shanyushiyangtech.top/gtynllqlrd.html

#define X_H
来源：http://hz.cheryme.top/gtyomwsups.html

#endif
来源：http://hz.xingfuxueyuan.xyz/gtfemqmrna.html

[S31] C++：Hello World
来源：http://hz.iojbl.cn/gtvlvqgxqj.html

#include <iostream>
来源：http://hz.xinyue.icu/gtnxoyidhk.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.hnxiangtu.top/gtwsdwhakv.html

[S32] C++：字符串
来源：http://hz.nanxinkj.top/gtxdxfymfu.html

std::string s = "hi";  s += "!";
来源：http://hz.kuanghao11.cn/gtyoydmhyg.html

[S33] C++：vector 增删
来源：http://hz.xingfuxueyuan.xyz/gtyvifwzuh.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.sxryk.cn/gtkqbizlrd.html

[S34] C++：遍历 vector
来源：http://hz.kuanghao11.cn/gtpnypfwmd.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.pengpengdd.cyou/gtwbzlpysa.html

[S35] C++：map
来源：http://hz.yvedp.cn/gtuktmamej.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.gaohongyu789.top/gtpqakemdf.html

[S36] C++：unordered_map
来源：http://hz.jiagoushi.top/gteixwmlfg.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jinghuilouyu.cn/gtbjlavhco.html

[S37] C++：set
来源：http://hz.sxryk.cn/gtudebcirn.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.zhoulong.xyz/gtelxvvzgt.html

[S38] C++：排序
来源：http://hz.dashuyun.cn/gtwadcsjot.html

std::sort(v.begin(), v.end());
来源：http://hz.ehwqpu.com/gtoaicdufq.html

[S39] C++：自定义比较器排序
来源：http://hz.tianlin.xyz/gtahdqamvd.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.chenjidiqi.icu/gtsbfjwtev.html

[S40] C++：查找元素
来源：http://hz.yj20258888.top/gtjwatijir.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.zhijiandao.cn/gtmjwonffj.html

[S41] C++：类与构造函数
来源：http://hz.cdnleiting.top/gtieebgmkg.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.hongshengwenyu.top/gtlxwigfgf.html

[S42] C++：继承与虚函数
来源：http://hz.ywan-chungtsiang.top/gtqdvsjtub.html

class B : public Base { public: void f() override {} };
来源：http://hz.xuetiantiany.cn/gtyncdzrkt.html

[S43] C++：智能指针
来源：http://hz.xziqi.cn/gtdjlacvip.html

auto p = std::make_unique<int>(5);
来源：http://hz.yueranfly.top/gtabybojpi.html

[S44] C++：引用传参
来源：http://hz.jinqigufen.top/gtpczxudrs.html

void inc(int &x) { ++x; }
来源：http://hz.nanxinkj.top/gtyazvwqac.html

[S45] C++：lambda
来源：http://hz.ywan-chungtsiang.top/gtbvsjrzoj.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.guowangkeji.top/gtsawvulpf.html

[S46] C++：函数模板
来源：http://hz.yongpay.top/gtqgyxapkp.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.yueranfly.top/gtrzbmgnjn.html

[S47] C++：结构化绑定遍历
来源：http://hz.yonumen.top/gtecqmxwvq.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.yanxiufei.cn/gtmscgdfjm.html

[S48] C++：逐行读文件
来源：http://hz.c1oappe.top/gtpcgguxfp.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.quarkkingdee.top/gtorqebjaj.html

while (std::getline(in, line)) { }
来源：http://hz.ydjk.org.cn/gtecgglyly.html

[S49] C++：写文件
来源：http://hz.tanke756.top/gtglrtkrjk.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.tanke756.top/gtkallvtpg.html

[S50] C++：格式化数字
来源：http://hz.xuetiantiany.cn/gtnjwpvzpd.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.snrcjt.cn/gtsiqvvirb.html

[S51] C++：显式类型转换
来源：http://hz.snrcjt.cn/gtzmummuoi.html

static_cast<double>(a) / b
来源：http://hz.zhiwuduotai.top/gtunrrytun.html

[S52] C++：const 与 noexcept
来源：http://hz.chenzaomai.com/gttkavrjtf.html

int size() const noexcept { return n_; }
来源：http://hz.yvedp.cn/gtsnicwsqg.html

[S53] C++：移动语义
来源：http://hz.sxryk.cn/gtmsynaknx.html

std::vector<int> w = std::move(v);
来源：http://hz.ppjwa.cn/gtjvffhhyt.html

[S54] C++：异常处理
来源：http://hz.snrcjt.cn/gtyzbxlssw.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.nanxuanxn.top/gtfjjjvxnp.html

[S55] C++：结构化绑定
来源：http://hz.hammf.cn/gtspvlhpcz.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.chenjidiqi.icu/gtkuqushmb.html

[S56] C++：optional
来源：http://hz.jinqigufen.top/gteaqalodc.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.jqgfzy.top/gtnkdgspbj.html

[S57] C++：编译期常量
来源：http://hz.zhixingplan.top/gtqqdvxaqg.html

constexpr int N = 10;
来源：http://hz.guannengcc.top/gtqeoqjvlb.html

[S58] C++：命名空间
来源：http://hz.cdnleiting.top/gtbopwgrkm.html

namespace ns { int f() { return 1; } }
来源：http://hz.gzhubu.top/gtqzfkhotp.html

[S59] C++：静态断言
来源：http://hz.jianghu66.top/gtnmilnjzu.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.fengsongda.top/gtezjsqaio.html

[S60] C++：遍历并删除元素
来源：http://hz.52xcode.cn/gtlrlxptmr.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.haohaochexian.top/gtrbrprstb.html

================================================================================
来源：http://hz.dashuyun.cn/gttgfwykmv.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.sufxvd.cn/gtkfsnhlwp.html

================================================================================
来源：http://hz.zhixingplan.top/gtnfjdguuy.html

[T01] Kotlin：Hello World
来源：http://hz.shanyushiyangtech.top/gtymhsulvz.html

println("Hello")
来源：http://hz.yj20258888.top/gtfkrorkhe.html

[T02] Kotlin：变量
来源：http://hz.snrcjt.cn/gtaggqxmqs.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.cheryme.top/gtsemuweyc.html

[T03] Kotlin：字符串模板
来源：http://hz.quarkkingdee.top/gtohybpspl.html

"值: $b"
来源：http://hz.gaohongyu789.top/gtuiugbrhw.html

[T04] Kotlin：空安全
来源：http://hz.wangshuangyany.cn/gtrupajdjy.html

val n: String? = null;  n?.length
来源：http://hz.cdnleiting.top/gtutkjnhip.html

[T05] Kotlin：when 表达式
来源：http://hz.cdnleiting.top/gtuilnhhma.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.shanyushiyangkeji.top/gtaqrlhdqf.html

[T06] Kotlin：集合映射
来源：http://hz.yanxiufei.cn/gtrsohvqsp.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.pengpengdd.cyou/gtgggmmvee.html

[T07] Kotlin：集合过滤
来源：http://hz.nanxuanxn.top/gtotdxucid.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.aibaodan.cn/gttvddiavi.html

[T08] Kotlin：数据类
来源：http://hz.ydzc1.top/gtnxluebhe.html

data class User(val name: String, val age: Int)
来源：http://hz.zhoulong.xyz/gtgnflmiew.html

[T09] Kotlin：扩展函数
来源：http://hz.hywenlv.cn/gtwcbtnlox.html

fun String.exclaim() = this + "!"
来源：http://hz.dashuyun.cn/gtfdvrokfn.html

[T10] Kotlin：默认参数
来源：http://hz.yj202588.top/gtstgybrsy.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.hnqzz.top/gtgwrmksrj.html

[T11] Kotlin：协程
来源：http://hz.chenzaomai.com/gtafkjlgbr.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.yj202588.top/gtqscghlnl.html

[T12] Kotlin：解构声明
来源：http://hz.pycfn.com/gthbivuzkv.html

val (a, b) = Pair(1, 2)
来源：http://hz.xinyue.icu/gtsrueowfw.html

[T13] Kotlin：只读 Map
来源：http://hz.xuanzx.com/gtimwngorf.html

val m = mapOf("a" to 1)
来源：http://hz.hnqzz.top/gthkpdchgl.html

[T14] Kotlin：循环
来源：http://hz.sufxvd.cn/gtvzplrugr.html

for (i in 1..10) println(i)
来源：http://hz.c1oappe.top/gtrsdsayka.html

[T15] Kotlin：接口
来源：http://hz.cqqwz.cn/gtkkctjvfc.html

interface Shape { fun area(): Double }
来源：http://hz.0kj1m.cn/gtncawwhjf.html

[T16] Swift：Hello World
来源：http://hz.gaohongyu789.top/gtjqnnanxg.html

print("Hello")
来源：http://hz.yanxiufei.cn/gtsznvfwpb.html

[T17] Swift：变量与常量
来源：http://hz.daria6918.cn/gtfeqohdxm.html

var a = 1;  let b = 2
来源：http://hz.hysaishi.cn/gtivdqliiy.html

[T18] Swift：字符串插值
来源：http://hz.hnqzz.top/gtddcvgmev.html

"值: \(b)"
来源：http://hz.tian-w.cn/gtkcgeqhtw.html

[T19] Swift：可选绑定
来源：http://hz.ywan-chungtsiang.top/gtzehcvspp.html

if let n = opt { print(n) }
来源：http://hz.jiagoushi.top/gtdwcgfbua.html

[T20] Swift：数组操作
来源：http://hz.shuidangran.top/gtzqhrxflv.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.dashuyun.cn/gtpmgkxeoe.html

[T21] Swift：遍历
来源：http://hz.zdqjudy.top/gtdvwiqcoi.html

for x in a { print(x) }
来源：http://hz.shanyushiyangkeji.top/gtojdtsbyj.html

[T22] Swift：字典
来源：http://hz.yongpay.top/gtkyvyavih.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.daxiang520.top/gtknazvfhg.html

[T23] Swift：函数
来源：http://hz.iojbl.cn/gtsslaacli.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.jinghuilouyu.cn/gtciopnryj.html

[T24] Swift：闭包
来源：http://hz.bjfxy.top/gtfovzpjuu.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.jqgufenzy.top/gthtuvphgv.html

[T25] Swift：结构体
来源：http://hz.316326.xyz/gtscvitocu.html

struct P { var x: Int }
来源：http://hz.shzxlz.cn/gtcaujuctu.html

[T26] Swift：类与重写
来源：http://hz.chenlongwang.top/gtmbswdqtn.html

class A: Base { override func f() {} }
来源：http://hz.cdnleiting.top/gtrhfhtjcv.html

[T27] Swift：错误处理
来源：http://hz.zhixingplan.top/gtvjqbdpku.html

do { try f() } catch { print(error) }
来源：http://hz.xziqi.cn/gtgoaplifo.html

[T28] Swift：枚举
来源：http://hz.tian-w.cn/gthfjcvupq.html

enum Color { case red, green }
来源：http://hz.dianchejie.cn/gtuxlsryqd.html

[T29] Swift：guard 提前返回
来源：http://hz.hnqzz.top/gtzqbzfcos.html

guard let x = opt else { return }
来源：http://hz.yongpay.top/gtvkxwkrlh.html

[T30] Swift：协议
来源：http://hz.ydjk.org.cn/gtigrghzkm.html

protocol Shape { func area() -> Double }
来源：http://hz.yonumen.top/gtwrbfabhi.html

[T31] Lua：Hello World
来源：http://hz.smart0.xyz/gtamttlepy.html

print("Hello")
来源：http://hz.guannengcc.top/gtpdambvus.html

[T32] Lua：局部变量
来源：http://hz.pycfn.com/gtbypvfpzx.html

local a = 1
来源：http://hz.ywan-chungtsiang.top/gtpouhupva.html

[T33] Lua：表（数组）
来源：http://hz.snrcjt.cn/gtrryfders.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.meibo888.top/gtiuqxrfge.html

[T34] Lua：遍历表
来源：http://hz.zhoulong.xyz/gtmhpvfaha.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.zhixingplan.top/gttcfmiihp.html

[T35] Lua：字典表
来源：http://hz.fengsongda.top/gtxznadvkd.html

local d = { a = 1 };  d.b = 2
来源：http://hz.zhoulong.xyz/gtpzkepbly.html

[T36] Lua：函数
来源：http://hz.andypj.xyz/gtdzfpaxxi.html

function add(a, b) return a + b end
来源：http://hz.zhoulong.xyz/gturhpabgy.html

[T37] Lua：字符串拼接
来源：http://hz.haohaochexian.top/gtnpeqgkio.html

"a" .. "b"
来源：http://hz.sysykeji.top/gtwrpeapfu.html

[T38] Lua：条件
来源：http://hz.jlsjyb.cn/gtqgoxemgy.html

if x > 0 then print("正") end
来源：http://hz.316326.xyz/gtrbxmebfk.html

[T39] Lua：模式匹配
来源：http://hz.snrcjt.cn/gtfnpgtpeu.html

string.find(s, "%d+")
来源：http://hz.xylfe.cn/gttafukvta.html

[T40] Lua：元表
来源：http://hz.52xcode.cn/gtverpziiv.html

setmetatable({}, { __index = base })
来源：http://hz.gaohongyu789.top/gtwubfrnoq.html

[T41] Perl：Hello World
来源：http://hz.hysaishi.cn/gtjruvnijw.html

print "Hello\n";
来源：http://hz.xinyue.icu/gtqkavnxgr.html

[T42] Perl：变量类型
来源：http://hz.ydjk.org.cn/gtxzjtiryo.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.dashuyun.cn/gtbdwvydae.html


<!-- 参考信息 -->